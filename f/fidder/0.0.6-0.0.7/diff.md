# Comparing `tmp/fidder-0.0.6.tar.gz` & `tmp/fidder-0.0.7.tar.gz`

## Comparing `fidder-0.0.6.tar` & `fidder-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fidder-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fidder-0.0.6/mkdocs.yml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fidder-0.0.6/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 fidder-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 fidder-0.0.6/docs/index.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fidder-0.0.6/docs/stylesheets/extra.css
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fidder-0.0.6/docs/usage/command_line.md
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fidder-0.0.6/docs/usage/python.md
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 fidder-0.0.6/examples/pretrained_model.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fidder-0.0.6/examples/quickstart.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fidder-0.0.6/examples/quickstart.sh
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/_cli.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/constants.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/train.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/utils.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/_tests/test_utils.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/__init__.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/augmentation.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/download.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/training_datamodule.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/training_dataset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/_tests/__init__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/data/_tests/test_download_data.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/erase/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/erase/cli.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/erase/erase.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/erase/sparse_local_mean.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/erase/_tests/test_erasing.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/_pretrained_weights.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/dice.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/model.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/model_parts.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/_tests/test_dice.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/_tests/test_download_checkpoint.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/model/_tests/test_model.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/predict/__init__.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/predict/cli.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/predict/predict.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 fidder-0.0.6/src/fidder/predict/probabilities_to_mask.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fidder-0.0.6/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fidder-0.0.6/LICENSE
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 fidder-0.0.6/README.md
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 fidder-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 fidder-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fidder-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fidder-0.0.7/mkdocs.yml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fidder-0.0.7/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 fidder-0.0.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/index.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/usage/command_line.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/usage/python.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/pretrained_model.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/quickstart.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/quickstart.sh
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/_cli.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/constants.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/train.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/utils.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/_tests/test_utils.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/__init__.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/augmentation.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/download.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/training_datamodule.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/training_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/_tests/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/_tests/test_download_data.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/cli.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/erase.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/sparse_local_mean.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/_tests/test_erasing.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/__init__.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_pretrained_weights.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/dice.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/model.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/model_parts.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_dice.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_download_checkpoint.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_model.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/__init__.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/cli.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/predict.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/probabilities_to_mask.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fidder-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fidder-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 fidder-0.0.7/README.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 fidder-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fidder-0.0.7/PKG-INFO
```

### Comparing `fidder-0.0.6/.pre-commit-config.yaml` & `fidder-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/mkdocs.yml` & `fidder-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/.github/workflows/build-and-deploy-docs.yml` & `fidder-0.0.7/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/.github/workflows/ci.yml` & `fidder-0.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/docs/index.md` & `fidder-0.0.7/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,21 @@
 
 pip:
 
 ```shell
 pip install fidder
 ```
 
-## Notes
+## Compatibility
+
+If trying to use an `10.X` CUDA runtime you may have to install older versions of 
+`torch` and `pytorch-lightning`, see 
+[teamtomo/fidder#17](https://github.com/teamtomo/fidder/issues/17) for details.
+
+# Notes
 
 This package provides similar functionality to 
 [BoxNet](http://www.warpem.com/warp/?page_id=135) from Warp
 when 
 [retrained for gold fiducial segmentation](http://www.warpem.com/warp/?page_id=137).
 
 This package was developed to make this functionality available in a standalone,
```

#### html2text {}

```diff
@@ -20,14 +20,17 @@
 load your image image = torch.tensor(mrcfile.read('my_image_file.mrc')) # use a
 pretrained model to predict a mask mask, probabilities = predict_fiducial_mask
 ( image, pixel_spacing=1.35, probability_threshold=0.5 ) # erase fiducials
 erased_image = erase_masked_region(image=image, mask=mask) ``` ## Command Line
 ```bash # predict fiducial mask fidder predict \ --input-image example.mrc \ --
 probability-threshold 0.5 \ --output-mask mask.mrc # erase masked region fidder
 erase \ --input-image example.mrc \ --input-mask mask.mrc \ --output-image
-erased.mrc ``` --- # Installation pip: ```shell pip install fidder ``` ## Notes
-This package provides similar functionality to [BoxNet](http://www.warpem.com/
-warp/?page_id=135) from Warp when [retrained for gold fiducial segmentation]
-(http://www.warpem.com/warp/?page_id=137). This package was developed to make
-this functionality available in a standalone, easy to install Python package.
-The architecture and training data preprocessing are based on the description
-in the [Warp paper](https://doi.org/10.1038/s41592-019-0580-y).
+erased.mrc ``` --- # Installation pip: ```shell pip install fidder ``` ##
+Compatibility If trying to use an `10.X` CUDA runtime you may have to install
+older versions of `torch` and `pytorch-lightning`, see [teamtomo/fidder#17]
+(https://github.com/teamtomo/fidder/issues/17) for details. # Notes This
+package provides similar functionality to [BoxNet](http://www.warpem.com/warp/
+?page_id=135) from Warp when [retrained for gold fiducial segmentation](http://
+www.warpem.com/warp/?page_id=137). This package was developed to make this
+functionality available in a standalone, easy to install Python package. The
+architecture and training data preprocessing are based on the description in
+the [Warp paper](https://doi.org/10.1038/s41592-019-0580-y).
```

### Comparing `fidder-0.0.6/src/fidder/__init__.py` & `fidder-0.0.7/src/fidder/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,12 +8,19 @@
 
 __author__ = "Alister Burt"
 __email__ = "alisterburt@gmail.com"
 
 __all__ = ["__version__", "cli", "Fidder", "train_fidder", "download_training_data"]
 
 from ._cli import cli
-from .model import Fidder
-from .data import download_training_data
+# cli tools
 from .train import train_fidder
 from .predict.cli import predict_fiducial_mask
-from .erase.cli import erase_segmented_fiducials
+from .erase.cli import erase_masked_region
+
+# python things
+from .model import Fidder
+from .data import download_training_data
+from .predict import predict_fiducial_mask
+from .erase import erase_masked_region
+
+
```

### Comparing `fidder-0.0.6/src/fidder/train.py` & `fidder-0.0.7/src/fidder/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 ) -> None:
     """Train a semantic segmentation model for fiducial detection."""
     model = Fidder(batch_size=batch_size, learning_rate=learning_rate)
     data_module = FidderDataModule(dataset_directory)
 
     trainer = Trainer(
         accelerator="auto",
-        devices=1,
-        auto_select_gpus=True,
+        devices="auto",
         default_root_dir=output_directory,
         max_steps=gradient_steps,
         log_every_n_steps=10,
         check_val_every_n_epoch=None,
         val_check_interval=20,
         num_sanity_val_steps=0,
         enable_checkpointing=True,
```

### Comparing `fidder-0.0.6/src/fidder/utils.py` & `fidder-0.0.7/src/fidder/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,29 +121,36 @@
 
 
 def get_pixel_spacing_from_header(image: Path) -> float:
     with mrcfile.open(image, header_only=True, permissive=True) as mrc:
         return float(mrc.voxel_size.x)
 
 
-def connected_component_transform_2d(mask: torch.Tensor):
-    """Perform a connected component transform on a binary 2D image.
+def pixel_count_map_2d(mask: torch.Tensor):
+    """Calculate a pixel count map from a binary 2D image.
 
-    A connected component transform replaces every pixel in a binary image with
-    the number of connected components in the region around that pixel.
+    https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/60_data_visualization/parametric_maps.html
 
     Parameters
     ----------
     mask: torch.Tensor
         `(h, w)` binary array
 
     Returns
     -------
 
     """
     labels, n = ndi.label(mask.cpu().numpy())
     labels = torch.tensor(labels, dtype=torch.long)
-    labels_one_hot = F.one_hot(labels, num_classes=(n + 1))
-    counts = reduce(labels_one_hot, "h w c -> c", reduction="sum")
-    counts = {label_index: count.item() for label_index, count in enumerate(counts)}
-    connected_component_image = np.vectorize(counts.__getitem__)(labels)
-    return torch.tensor(connected_component_image)
+    if n < 100:  # vectorised, not memory efficient
+        labels_one_hot = F.one_hot(labels, num_classes=(n + 1))
+        counts = reduce(labels_one_hot, "h w c -> c", reduction="sum")
+        counts = {label_index: count.item() for label_index, count in enumerate(counts)}
+        connected_component_image = np.vectorize(counts.__getitem__)(labels)
+        connected_component_image = torch.tensor(connected_component_image)
+    else:
+        connected_component_image = torch.zeros_like(labels)
+        for label_id in range(n + 1):
+            conected_component_mask = labels == label_id
+            n_connected_components = torch.sum(conected_component_mask)
+            connected_component_image[conected_component_mask] = n_connected_components
+    return connected_component_image
```

### Comparing `fidder-0.0.6/src/fidder/_tests/test_utils.py` & `fidder-0.0.7/src/fidder/_tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import torch
 
-from fidder.utils import connected_component_transform_2d
+from fidder.utils import pixel_count_map_2d
 
 
 def test_connected_component_transform_2d():
     mask = torch.zeros((10, 10))
     mask[::2, ::2] = 1
     mask[1::2, 1::2] = 1
-    connected_component_image = connected_component_transform_2d(mask).long()
+    connected_component_image = pixel_count_map_2d(mask).long()
     assert torch.allclose(
         connected_component_image[::2, ::2], torch.tensor(1).long())
     assert torch.allclose(
         connected_component_image[1::2, 1::2], torch.tensor(1).long()
     )
     assert torch.allclose(
         connected_component_image[1::2, ::2], torch.tensor(50).long()
```

### Comparing `fidder-0.0.6/src/fidder/data/augmentation.py` & `fidder-0.0.7/src/fidder/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/data/download.py` & `fidder-0.0.7/src/fidder/data/download.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/data/training_datamodule.py` & `fidder-0.0.7/src/fidder/data/training_datamodule.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/data/training_dataset.py` & `fidder-0.0.7/src/fidder/data/training_dataset.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/erase/cli.py` & `fidder-0.0.7/src/fidder/erase/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .erase import erase_masked_region
 from ..utils import get_pixel_spacing_from_header
 from .._cli import cli, OPTION_PROMPT_KWARGS as PKWARGS
 
 
 @cli.command(name="erase", no_args_is_help=True)
-def erase_segmented_fiducials(
+def erase_masked_region(
     input_image: Path = Option(
         default=...,
         help="Image file in MRC format.",
         **PKWARGS
     ),
     input_mask: Path = Option(
         default=...,
```

### Comparing `fidder-0.0.6/src/fidder/erase/erase.py` & `fidder-0.0.7/src/fidder/erase/erase.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/erase/sparse_local_mean.py` & `fidder-0.0.7/src/fidder/erase/sparse_local_mean.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/erase/_tests/test_erasing.py` & `fidder-0.0.7/src/fidder/erase/_tests/test_erasing.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/model/dice.py` & `fidder-0.0.7/src/fidder/model/dice.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/model/model.py` & `fidder-0.0.7/src/fidder/model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def __init__(self, batch_size: int = 4, learning_rate: float = 1e-05):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.save_hyperparameters()
 
         self.validation_dice_score = 0
+        self.validation_step_outputs = []
 
         self.base_layer = nn.Sequential(
             nn.Conv2d(
                 in_channels=self.in_channels,
                 out_channels=32,
                 kernel_size=7,
                 stride=1,
@@ -93,14 +94,15 @@
         batch: Tuple[torch.Tensor, torch.Tensor],
         batch_idx: int,
     ):
         images, labels = batch
         logits = self(images)  # (b, c, h, w)
         dice = dice_score(ground_truth=labels, logits=logits)
         self.log("validation dice score", dice)
+        self.validation_step_outputs.append(dice)
         return dice
 
     def predict_step(
         self,
         image: torch.Tensor,  # (h, w)
         batch_idx: int = 0,
         dataloader_idx: int = 0,
@@ -122,18 +124,19 @@
             probabilities = F.softmax(prediction, dim=1)[:, 1, ...]
             probabilities = probabilities.detach().cpu().numpy()
             merger.add_batch(
                 batch_id=idx, batch_size=self.batch_size, data=probabilities
             )
         return torch.tensor(merger.merge(unpad=True))
 
-    def validation_epoch_end(self, batch_dice_scores):
-        mean_dice_score = torch.mean(torch.as_tensor(batch_dice_scores))
+    def on_validation_epoch_end(self):
+        mean_dice_score = torch.mean(torch.as_tensor(self.validation_step_outputs))
         self.validation_dice_score = mean_dice_score
         self.log(name="validation dice score", value=mean_dice_score)
+        self.validation_step_outputs.clear()
 
     def configure_optimizers(self):
         optimizer = optim.RMSprop(
             params=self.parameters(),
             lr=self.learning_rate,
             weight_decay=1e-8,
             momentum=0.9,
@@ -142,24 +145,23 @@
         return optimizer
 
     def optimizer_step(
         self,
         epoch_idx: int,
         batch_idx: int,
         optimizer: torch.optim.Optimizer,
-        optimizer_idx: int,
         optimizer_closure: Optional[Callable[[], Any]] = None,
         **kwargs,
     ) -> None:
         self.log("learning rate", optimizer.param_groups[0]["lr"])
         if batch_idx == 0:  # call the scheduler after each validation
             self.scheduler.step(self.validation_dice_score)
             print(
                 "\n"
                 f"validation dice: {self.validation_dice_score}, "
                 f"best: {self.scheduler.best}, "
                 f"num_bad_epochs: {self.scheduler.num_bad_epochs}"
                 "\n"
             )  # for debugging
         super().optimizer_step(
-            epoch_idx, batch_idx, optimizer, optimizer_idx, optimizer_closure, **kwargs
+            epoch_idx, batch_idx, optimizer, optimizer_closure, **kwargs
         )
```

### Comparing `fidder-0.0.6/src/fidder/model/model_parts.py` & `fidder-0.0.7/src/fidder/model/model_parts.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/model/_tests/test_dice.py` & `fidder-0.0.7/src/fidder/model/_tests/test_dice.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/model/_tests/test_model.py` & `fidder-0.0.7/src/fidder/model/_tests/test_model.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/predict/cli.py` & `fidder-0.0.7/src/fidder/predict/cli.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/src/fidder/predict/predict.py` & `fidder-0.0.7/src/fidder/predict/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     )
     image = rescale_2d_bicubic(image, factor=downscale_factor)
     image = rearrange(image, "1 1 h w -> 1 h w")
 
     # prepare model
     if model_checkpoint_file is None:
         model_checkpoint_file = get_latest_checkpoint()
-    model = Fidder.load_from_checkpoint(model_checkpoint_file)
+    model = Fidder.load_from_checkpoint(model_checkpoint_file, map_location="cpu")
     model.eval()
 
     # predict
     [probabilities] = Trainer(accelerator="auto").predict(model, image)
     mask = probabilities_to_mask(
         probabilities=probabilities,
         threshold=probability_threshold,
```

### Comparing `fidder-0.0.6/src/fidder/predict/probabilities_to_mask.py` & `fidder-0.0.7/src/fidder/predict/probabilities_to_mask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from ..utils import connected_component_transform_2d
+from ..utils import pixel_count_map_2d
 
 
 def probabilities_to_mask(
     probabilities: torch.Tensor,
     threshold: float = 0.5,
     connected_pixel_count_threshold: int = 20,
 ) -> torch.Tensor:
@@ -23,10 +23,10 @@
 
     Returns
     -------
     mask: torch.Tensor
         `(h, w)` boolean array.
     """
     mask = probabilities > threshold
-    pixel_count_map = connected_component_transform_2d(mask)
+    pixel_count_map = pixel_count_map_2d(mask)
     mask[pixel_count_map < connected_pixel_count_threshold] = 0
     return mask
```

### Comparing `fidder-0.0.6/.gitignore` & `fidder-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/LICENSE` & `fidder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/README.md` & `fidder-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 
 pip:
 
 ```shell
 pip install fidder
 ```
 
+### Compatibility
+
+If trying to use an `10.X` CUDA runtime you may have to install older versions of 
+`torch` and `pytorch-lightning`, see 
+[teamtomo/fidder#17](https://github.com/teamtomo/fidder/issues/17) for details.
+
 ## Notes
 
 This package provides similar functionality to 
 [BoxNet](http://www.warpem.com/warp/?page_id=135) from Warp
 when 
 [retrained for gold fiducial segmentation](http://www.warpem.com/warp/?page_id=137).
```

### Comparing `fidder-0.0.6/pyproject.toml` & `fidder-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.6/PKG-INFO` & `fidder-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidder
-Version: 0.0.6
+Version: 0.0.7
 Summary: U-Net for 2D fiducial segmentation in cryo-EM
 Project-URL: homepage, https://github.com/teamtomo/fidder
 Project-URL: repository, https://github.com/teamtomo/fidder
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
@@ -114,14 +114,20 @@
 
 pip:
 
 ```shell
 pip install fidder
 ```
 
+### Compatibility
+
+If trying to use an `10.X` CUDA runtime you may have to install older versions of 
+`torch` and `pytorch-lightning`, see 
+[teamtomo/fidder#17](https://github.com/teamtomo/fidder/issues/17) for details.
+
 ## Notes
 
 This package provides similar functionality to 
 [BoxNet](http://www.warpem.com/warp/?page_id=135) from Warp
 when 
 [retrained for gold fiducial segmentation](http://www.warpem.com/warp/?page_id=137).
```

