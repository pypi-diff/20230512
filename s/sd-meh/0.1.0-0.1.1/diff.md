# Comparing `tmp/sd_meh-0.1.0.tar.gz` & `tmp/sd_meh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.1.0.tar", max compression
+gzip compressed data, was "sd_meh-0.1.1.tar", max compression
```

## Comparing `sd_meh-0.1.0.tar` & `sd_meh-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      525 2023-05-10 15:02:24.885526 sd_meh-0.1.0/README.md
--rw-r--r--   0        0        0      346 2023-05-10 15:03:10.474812 sd_meh-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 13:19:22.947635 sd_meh-0.1.0/sd_meh/__init__.py
--rw-r--r--   0        0        0     7166 2023-05-10 14:34:25.938414 sd_meh-0.1.0/sd_meh/merge.py
--rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.1.0/sd_meh/model.py
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 sd_meh-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 14:42:40.197057 sd_meh-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1359 2023-05-12 08:39:24.814256 sd_meh-0.1.1/README.md
+-rw-r--r--   0        0        0      390 2023-05-12 08:38:00.548569 sd_meh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-10 13:19:22.947635 sd_meh-0.1.1/sd_meh/__init__.py
+-rw-r--r--   0        0        0     5804 2023-05-12 08:32:12.808921 sd_meh-0.1.1/sd_meh/merge.py
+-rw-r--r--   0        0        0     1465 2023-05-10 13:19:22.948414 sd_meh-0.1.1/sd_meh/model.py
+-rw-r--r--   0        0        0     1883 1970-01-01 00:00:00.000000 sd_meh-0.1.1/PKG-INFO
```

### Comparing `sd_meh-0.1.0/LICENSE.txt` & `sd_meh-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.1.0/sd_meh/merge.py` & `sd_meh-0.1.1/sd_meh/merge.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Dict, Tuple
 
 import safetensors.torch
 import torch
 from tqdm import tqdm
 
-from meh.model import SDModel
+from sd_meh.model import SDModel
 
 MAX_TOKENS = 77
 NUM_INPUT_BLOCKS = 12
 NUM_MID_BLOCK = 1
 NUM_OUTPUT_BLOCKS = 12
 NUM_TOTAL_BLOCKS = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + NUM_OUTPUT_BLOCKS
 EPSILON = 1e-10  # Define a small constant EPSILON to prevent division by zero
@@ -22,22 +22,14 @@
         "transformer",
         "text_model",
         "embeddings",
         "position_ids",
     ]
 )
 
-NUM_MODELS_NEEDED = {
-    "add_difference": 3,
-    "weighted_sum": 2,
-    "weighted_subtraction": 2,
-    "sum_twice": 3,
-    "triple_sum": 3,
-    "tensor_sum": 2,
-}
 
 NAI_KEYS = {
     "cond_stage_model.transformer.embeddings.": "cond_stage_model.transformer.text_model.embeddings.",
     "cond_stage_model.transformer.encoder.": "cond_stage_model.transformer.text_model.encoder.",
     "cond_stage_model.transformer.final_layer_norm.": "cond_stage_model.transformer.text_model.final_layer_norm.",
 }
 
@@ -56,152 +48,107 @@
         if key.startswith(nk):
             model[key.replace(nk, NAI_KEYS[nk])] = model[key]
             del model[key]
 
     return model
 
 
-def fix_nai_keys(model: Dict) -> Dict:
-    for k in model:
-        model = fix_key(model, k)
-
-    return model
-
-
 # https://github.com/j4ded/sdweb-merge-block-weighted-gui/blob/master/scripts/mbw/merge_block_weighted.py#L115
 def fix_model(model: Dict) -> Dict:
-    model = fix_nai_keys(model)
+    for k in model:
+        model = fix_key(model, k)
     return fix_clip(model)
 
 
 def load_sd_model(model_path: os.PathLike, device: str = "cpu") -> SDModel:
     return SDModel(model_path, device).load_model()
 
 
-def merge(
+def merge_models(
     models: Dict[str, os.PathLike],
     weights: Dict,
     bases: Dict,
     merge_mode: str,
-    skip_position_ids: int = 0,
     precision: int = 16,
 ) -> None:
     thetas = {k: load_sd_model(Path(m)) for k, m in models.items()}
 
     for key in tqdm(thetas["model_a"].keys(), desc="stage 1"):
         if result := merge_key(
             key,
             thetas,
             weights,
             bases,
             merge_mode,
-            skip_position_ids,
             precision,
         ):
             thetas["model_a"][key] = result[1]
 
     for key in tqdm(thetas["model_b"].keys(), desc="stage 2"):
+        if KEY_POSITION_IDS in key:
+            continue
         if "model" in key and key not in thetas["model_a"]:
-            if KEY_POSITION_IDS in key:
-                if skip_position_ids == 1:
-                    continue
-                elif skip_position_ids == 2:
-                    thetas["model_a"][key] = torch.tensor(
-                        [list(range(MAX_TOKENS))], dtype=torch.int64
-                    )
-                    if precision == 16:
-                        thetas["model_a"][key] = thetas["model_a"][key].half()
-                    continue
             thetas["model_a"].update({key: thetas["model_b"][key]})
             if precision == 16:
                 thetas["model_a"][key] = thetas["model_a"][key].half()
 
-    thetas["model_a"] = fix_model(thetas["model_a"])
-
-    return thetas["model_a"]
-
-
-def save_model(model, output_file, file_format) -> None:
-    if file_format == "safetensors":
-        safetensors.torch.save_file(
-            model,
-            output_file,
-            metadata={"format": "pt"},
-        )
-    else:
-        torch.save({"state_dict": model}, output_file)
+    return fix_model(thetas["model_a"])
 
 
 def merge_key(
     key: str,
     thetas: Dict,
     weights: Dict,
     bases: Dict,
     merge_mode: str,
-    skip_position_ids: int = 0,
     precision: int = 16,
 ) -> Tuple[str, Dict]:
-    if skip_position_ids == 1:
-        if KEY_POSITION_IDS in key:
-            return (
-                (key, thetas["model_a"][key].half())
-                if precision == "16"
-                else (key, thetas["model_a"][key])
-            )
-
-    elif skip_position_ids == 2:
-        if KEY_POSITION_IDS in key:
-            thetas["model_a"][key] = torch.tensor(
-                [list(range(MAX_TOKENS))], dtype=torch.int64
-            )
-            return (
-                (key, thetas["model_a"][key].half())
-                if precision == "16"
-                else (key, thetas["model_a"][key])
-            )
+    if KEY_POSITION_IDS in key:
+        return
 
     for theta in thetas.values():
         if key not in theta:
             return
-    current_bases = bases
-    if "model.diffusion_model." in key:
-        weight_index = -1
-
-        re_inp = re.compile(r"\.input_blocks\.(\d+)\.")  # 12
-        re_mid = re.compile(r"\.middle_block\.(\d+)\.")  # 1
-        re_out = re.compile(r"\.output_blocks\.(\d+)\.")  # 12
-
-        if "time_embed" in key:
-            weight_index = 0  # before input blocks
-        elif ".out." in key:
-            weight_index = NUM_TOTAL_BLOCKS - 1  # after output blocks
-        elif m := re_inp.search(key):
-            weight_index = int(m.groups()[0])
-        elif re_mid.search(key):
-            weight_index = NUM_INPUT_BLOCKS
-        elif m := re_out.search(key):
-            weight_index = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + int(m.groups()[0])
-
-        if weight_index >= NUM_TOTAL_BLOCKS:
-            raise ValueError(f"illegal block index {key}")
-
-        if weight_index >= 0 and weight_index < NUM_TOTAL_BLOCKS - 1:
-            current_bases = {k: w[weight_index] for k, w in weights.items()}
-        elif weight_index == NUM_TOTAL_BLOCKS - 1:
-            current_bases = dict(bases.items())
-
-    merged = merge_block(current_bases, thetas, key, merge_mode)
 
-    if precision == 16:
-        merged = merged.half()
+    if "model" in key:
+        current_bases = bases
+
+        if "model.diffusion_model." in key:
+            weight_index = -1
+
+            re_inp = re.compile(r"\.input_blocks\.(\d+)\.")  # 12
+            re_mid = re.compile(r"\.middle_block\.(\d+)\.")  # 1
+            re_out = re.compile(r"\.output_blocks\.(\d+)\.")  # 12
+
+            if "time_embed" in key:
+                weight_index = 0  # before input blocks
+            elif ".out." in key:
+                weight_index = NUM_TOTAL_BLOCKS - 1  # after output blocks
+            elif m := re_inp.search(key):
+                weight_index = int(m.groups()[0])
+            elif re_mid.search(key):
+                weight_index = NUM_INPUT_BLOCKS
+            elif m := re_out.search(key):
+                weight_index = NUM_INPUT_BLOCKS + NUM_MID_BLOCK + int(m.groups()[0])
+
+            if weight_index >= NUM_TOTAL_BLOCKS:
+                raise ValueError(f"illegal block index {key}")
+
+            if weight_index >= 0:
+                current_bases = {k: w[weight_index] for k, w in weights.items()}
+
+        merged_key = merge(current_bases, thetas, key, merge_mode)
 
-    return (key, merged)
+        if precision == 16:
+            merged_key = merged_key.half()
 
+        return (key, merged_key)
 
-def merge_block(current_bases: Dict, thetas: Dict, key: str, merge_mode: str) -> Dict:
+
+def merge(current_bases: Dict, thetas: Dict, key: str, merge_mode: str) -> Dict:
     t0 = thetas["model_a"][key]
     t1 = thetas["model_b"][key]
     alpha = current_bases["alpha"]
     if merge_mode == "weighted_sum":
         return (1 - alpha) * t0 + alpha * t1
     elif merge_mode == "weighted_subtraction":
         beta = current_bases["beta"]
@@ -226,7 +173,16 @@
     if merge_mode == "add_difference":
         return t0 + alpha * (t1 - t2)
     beta = current_bases["beta"]
     if merge_mode == "sum_twice":
         return (1 - beta) * ((1 - alpha) * t0 + alpha * t1) + beta * t2
     elif merge_mode == "triple_sum":
         return (1 - alpha - beta) * t0 + alpha * t1 + beta * t2
+
+
+def save_model(model, output_file, file_format) -> None:
+    if file_format == "safetensors":
+        safetensors.torch.save_file(
+            model, f"{output_file}.safetensors", metadata={"format": "pt"}
+        )
+    else:
+        torch.save({"state_dict": model}, f"{output_file}.ckpt")
```

### Comparing `sd_meh-0.1.0/sd_meh/model.py` & `sd_meh-0.1.1/sd_meh/model.py`

 * *Files identical despite different names*

