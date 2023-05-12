# Comparing `tmp/acids-msprior-1.0.2.tar.gz` & `tmp/acids-msprior-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.2.tar", last modified: Wed May 10 14:21:34 2023, max compression
+gzip compressed data, was "acids-msprior-1.0.3.tar", last modified: Fri May 12 09:25:42 2023, max compression
```

## Comparing `acids-msprior-1.0.2.tar` & `acids-msprior-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.066957 acids-msprior-1.0.2/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.148608 acids-msprior-1.0.3/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 09:25:42.000000 acids-msprior-1.0.3/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.148608 acids-msprior-1.0.3/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19774 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:25:42.152608 acids-msprior-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 09:22:29.000000 acids-msprior-1.0.3/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.2/PKG-INFO` & `acids-msprior-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.2
+Version: 1.0.3
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.2 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.3 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.2/README.md` & `acids-msprior-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.0.3/acids_msprior.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.2
+Version: 1.0.3
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.2 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.3 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.2/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.0.3/acids_msprior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/attention.py` & `acids-msprior-1.0.3/msprior/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,42 +50,42 @@
         m = torch.cumprod(m, -1)[:, None, None]
         bias = bias * m
         self.register_buffer('_cached_attention_bias', bias)
 
     @torch.jit.unused
     def init_kv_cache(self, k: torch.Tensor, v: torch.Tensor):
         self._keys_cache = torch.zeros(
-            k.shape[0],
+            cc.MAX_BATCH_SIZE,
             k.shape[1],
             self._max_seq_len,
             k.shape[-1],
         ).type_as(k)
         self._values_cache = torch.zeros(
-            v.shape[0],
+            cc.MAX_BATCH_SIZE,
             v.shape[1],
             self._max_seq_len,
             v.shape[-1],
         ).type_as(v)
 
     def update_cache(self, k: torch.Tensor, v: torch.Tensor):
         if not len(self._keys_cache) or not len(self._values_cache):
             self.init_kv_cache(k, v)
 
         input_length = k.shape[2]
 
         if input_length > self._max_seq_len:
-            k = k[:, :, -self._max_seq_len:]
+            k = k[:k.shape[0], :, -self._max_seq_len:]
             v = v[:, :, -self._max_seq_len:]
             input_length = self._max_seq_len
 
         self._keys_cache = self._keys_cache.roll(-input_length, dims=2)
-        self._keys_cache[:, :, -input_length:] = k
+        self._keys_cache[:k.shape[0], :, -input_length:] = k
 
         self._values_cache = self._values_cache.roll(-input_length, dims=2)
-        self._values_cache[:, :, -input_length:] = v
+        self._values_cache[:k.shape[0], :, -input_length:] = v
 
         if self._cache_length < self._max_seq_len:
             self._cache_length += input_length
 
     def split_heads(self, x: torch.Tensor) -> torch.Tensor:
         x = x.reshape(x.shape[0], x.shape[1], self._n_head, -1)
         x = x.permute(0, 2, 1, 3)
@@ -120,16 +120,16 @@
 
         if self._cached:
             if kv_available:
                 assert k is not None
                 assert v is not None
                 self.update_cache(k, v)
 
-            k = self._keys_cache
-            v = self._values_cache
+            k = self._keys_cache[:q.shape[0]]
+            v = self._values_cache[:q.shape[0]]
 
         assert q is not None
         assert k is not None
         assert v is not None
 
         content_score = torch.einsum('bhtd,bhsd->bhts', q, k)
         attention = content_score / math.sqrt(q.shape[-1])
```

### Comparing `acids-msprior-1.0.2/msprior/configs/decoder_only.gin` & `acids-msprior-1.0.3/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.0.3/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.0.3/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/dataset.py` & `acids-msprior-1.0.3/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/preprocessor.py` & `acids-msprior-1.0.3/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/scripted.py` & `acids-msprior-1.0.3/msprior/scripted.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,40 +161,40 @@
             self.set_reset(False)
 
         if self.has_encoder:
             assert hasattr(self, "encoder_ratio")
             if self.encoder_input_type == "discrete":
                 semantic_tokens = x[:, self.num_rave_quantizers:]
                 semantic_tokens = semantic_tokens.reshape(
-                    semantic_tokens.shape[0],
+                    batch_size,
                     semantic_tokens.shape[1],
                     -1,
                     self.encoder_ratio,
                 )[..., -1]
                 semantic_tokens = torch.clamp(
                     semantic_tokens,
                     0,
                     self.encoder_num_tokens,
                 ).long()[:, 0]
                 encoder_out = self.encoder(semantic_tokens)
             elif self.encoder_input_type == "vae":
                 assert self.feature_vae is not None
                 latents = x[:, self.num_rave_quantizers:]
                 latents = latents.reshape(
-                    latents.shape[0],
+                    batch_size,
                     latents.shape[1],
                     -1,
                     self.encoder_ratio,
                 )[..., -1]
                 features = self.feature_vae(latents).permute(0, 2, 1)
                 encoder_out = self.encoder(features)
             elif self.encoder_input_type == "full":
                 features = x[:, self.num_rave_quantizers:]
                 features = features.reshape(
-                    features.shape[0],
+                    batch_size,
                     features.shape[1],
                     -1,
                     self.encoder_ratio,
                 )[..., -1]
                 encoder_out = self.encoder(features.permute(0, 2, 1))
             else:
                 raise ValueError(
```

### Comparing `acids-msprior-1.0.2/msprior/task.py` & `acids-msprior-1.0.3/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior/utils.py` & `acids-msprior-1.0.3/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior_scripts/compact.py` & `acids-msprior-1.0.3/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior_scripts/export.py` & `acids-msprior-1.0.3/msprior_scripts/export.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 
 torch.set_grad_enabled(False)
 
 
 def main(argv):
     cc.use_cached_conv(True)
 
-    model = ScriptedPrior(FLAGS.run, FLAGS.temporal_ratio)
+    model = ScriptedPrior(FLAGS.run, FLAGS.temporal_ratio, FLAGS.continuous)
     model_name = os.path.basename(os.path.normpath(FLAGS.run)) + '.ts'
     export_path = os.path.join(FLAGS.run, model_name)
     model.export_to_ts(export_path)
     print(f'model exported to {export_path}')
 
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string('run', default=None, required=True, help='Run to export')
 flags.DEFINE_integer(
     'temporal_ratio',
     default=1024,
     help='Sequence temporal ratio',
 )
+flags.DEFINE_bool(
+    'continuous',
+    default=False,
+    help=
+    'dequantize predictions if rave model is continuous rather than discrete',
+)
```

### Comparing `acids-msprior-1.0.2/msprior_scripts/main_cli.py` & `acids-msprior-1.0.3/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior_scripts/preprocess.py` & `acids-msprior-1.0.3/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/msprior_scripts/train.py` & `acids-msprior-1.0.3/msprior_scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/setup.py` & `acids-msprior-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/tests/test_attention.py` & `acids-msprior-1.0.3/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/tests/test_cache.py` & `acids-msprior-1.0.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.2/tests/test_configs.py` & `acids-msprior-1.0.3/tests/test_configs.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,9 +29,18 @@
 @pytest.mark.parametrize("config,continuous,listen", configs, ids=names)
 def test_config(config, continuous, listen):
     gin.clear_config()
     gin.parse_config_file(config)
 
     model = ScriptedPrior(from_continuous=continuous, initial_listen=listen)
 
+    if listen and not continuous:
+        x = torch.randint(0, 16, (1, model.forward_params[0], 8)).float()
+        y = model(x)
+        assert torch.allclose(y[:, :-1].float(), x[:, :y.shape[1] - 1].float())
+
+        x = torch.randint(0, 16, (4, model.forward_params[0], 8)).float()
+        y = model(x)
+        assert torch.allclose(y[:, :-1].float(), x[:, :y.shape[1] - 1].float())
+
     with tempfile.TemporaryDirectory() as tmp:
         model.export_to_ts(os.path.join(tmp, "model.ts"))
```

