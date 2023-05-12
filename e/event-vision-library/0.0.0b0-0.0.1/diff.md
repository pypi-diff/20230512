# Comparing `tmp/event_vision_library-0.0.0b0.tar.gz` & `tmp/event_vision_library-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_vision_library-0.0.0b0.tar", max compression
+gzip compressed data, was "event_vision_library-0.0.1.tar", max compression
```

## Comparing `event_vision_library-0.0.0b0.tar` & `event_vision_library-0.0.1.tar`

### file list

```diff
@@ -1,40 +1,48 @@
--rw-r--r--   0        0        0     1070 2023-04-06 15:28:48.708961 event_vision_library-0.0.0b0/LICENSE
--rw-r--r--   0        0        0     3265 2023-04-06 15:28:48.708961 event_vision_library-0.0.0b0/README.md
--rw-r--r--   0        0        0     2802 2023-04-06 15:29:00.281004 event_vision_library-0.0.0b0/pyproject.toml
--rw-r--r--   0        0        0      111 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/__init__.py
--rw-r--r--   0        0        0    23618 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/_version.py
--rw-r--r--   0        0        0       21 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/__init__.py
--rw-r--r--   0        0        0      265 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/block_access.py
--rw-r--r--   0        0        0      552 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/_block_access.py
--rw-r--r--   0        0        0      319 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/_iterator_access.py
--rw-r--r--   0        0        0     2560 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/aedat.py
--rw-r--r--   0        0        0     2712 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/conversion.py
--rw-r--r--   0        0        0      677 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/evk.py
--rw-r--r--   0        0        0     2155 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/hdf5.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/npy.py
--rw-r--r--   0        0        0     3362 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/fileformat/text.py
--rw-r--r--   0        0        0      274 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/codec/iterator_access.py
--rw-r--r--   0        0        0      131 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/constant.py
--rw-r--r--   0        0        0       25 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/__init__.py
--rw-r--r--   0        0        0       90 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/__init__.py
--rw-r--r--   0        0        0     4673 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/__init__.py
--rw-r--r--   0        0        0      821 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/base_model.py
--rw-r--r--   0        0        0     3453 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/__init__.py
--rw-r--r--   0        0        0     2971 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/model.py
--rw-r--r--   0        0        0     8677 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py
--rw-r--r--   0        0        0     7788 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/unet.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/utils/__init__.py
--rw-r--r--   0        0        0     7154 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py
--rw-r--r--   0        0        0      871 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/py.typed
--rw-r--r--   0        0        0      182 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/representation/__init__.py
--rw-r--r--   0        0        0     1787 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/representation/histogram.py
--rw-r--r--   0        0        0     1430 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/representation/time_map.py
--rw-r--r--   0        0        0     2201 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/representation/voxel_grid.py
--rw-r--r--   0        0        0       33 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/utils/__init__.py
--rw-r--r--   0        0        0     1062 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/utils/basics.py
--rw-r--r--   0        0        0      638 2023-04-06 15:28:48.712962 event_vision_library-0.0.0b0/src/evlib/version.py
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 event_vision_library-0.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-12 10:25:25.998453 event_vision_library-0.0.1/LICENSE
+-rw-r--r--   0        0        0     3435 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/README.md
+-rw-r--r--   0        0        0     2800 2023-05-12 10:25:42.646519 event_vision_library-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/__init__.py
+-rw-r--r--   0        0        0    23618 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/_version.py
+-rw-r--r--   0        0        0       21 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/block_access.py
+-rw-r--r--   0        0        0      552 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/_block_access.py
+-rw-r--r--   0        0        0      308 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/_iterator_access.py
+-rw-r--r--   0        0        0     2485 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/aedat.py
+-rw-r--r--   0        0        0     2712 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/conversion.py
+-rw-r--r--   0        0        0      677 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/evk.py
+-rw-r--r--   0        0        0     2307 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/hdf5.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/npy.py
+-rw-r--r--   0        0        0     3283 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/fileformat/text.py
+-rw-r--r--   0        0        0      274 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/codec/iterator_access.py
+-rw-r--r--   0        0        0      131 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/constant.py
+-rw-r--r--   0        0        0       54 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/preproc/__init__.py
+-rw-r--r--   0        0        0     1460 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/preproc/hot_pixel.py
+-rw-r--r--   0        0        0       25 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/__init__.py
+-rw-r--r--   0        0        0     4673 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/base_model.py
+-rw-r--r--   0        0        0     3453 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/__init__.py
+-rw-r--r--   0        0        0     2971 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/model.py
+-rw-r--r--   0        0        0     8677 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py
+-rw-r--r--   0        0        0     7788 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/unet.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/__init__.py
+-rw-r--r--   0        0        0     7154 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py
+-rw-r--r--   0        0        0      873 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/py.typed
+-rw-r--r--   0        0        0      182 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/__init__.py
+-rw-r--r--   0        0        0     1820 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/histogram.py
+-rw-r--r--   0        0        0     1462 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/time_map.py
+-rw-r--r--   0        0        0     2235 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/representation/voxel_grid.py
+-rw-r--r--   0        0        0      246 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/raw_event.py
+-rw-r--r--   0        0        0     2159 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/types/raw_events.py
+-rw-r--r--   0        0        0       33 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/utils/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/utils/basics.py
+-rw-r--r--   0        0        0      638 2023-05-12 10:25:26.002453 event_vision_library-0.0.1/src/evlib/version.py
+-rw-r--r--   0        0        0       28 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/__init__.py
+-rw-r--r--   0        0        0     3660 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/utils.py
+-rw-r--r--   0        0        0     1872 2023-05-12 10:25:26.006453 event_vision_library-0.0.1/src/evlib/vis/view2d.py
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 event_vision_library-0.0.1/PKG-INFO
```

### Comparing `event_vision_library-0.0.0b0/LICENSE` & `event_vision_library-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/README.md` & `event_vision_library-0.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,51 +21,48 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
 - Python 3.7, 3.8, 3.9, 3.10
 - Pure-python library
+- 🚧 This library is under construction and currently alpha version. The APIs may change significantly. Contributions and discussions are welcomed! 🚧
+
+### Data
+
+- [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
+- [ ] ROS bag files (optional, based on ROS installation)
+- [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
+- [ ] Support iterator-based loading and also block-based (random access) loading.
 
 ### Algorithms
 
 - Have different off-the-shelf methods, ready to use:
   - [ ] Optical Flow estimation
   - [ ] Image reconstruction
   - [ ] Ego-motion estimation
   - more to come.
 - [ ] C++ implementation and extension for faster execution (TODO)
 
-### Data
-
-- [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
-- [ ] ROS bag files (optional, based on ROS installation)
-- [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
-- [ ] Support iterator-based loading and also block-based (random access) loading.
-
 ### Log and Vsualization
 
 - [ ] Various visualization for 2D/3D representation of events
 - [ ] Useful logging
 
-## Requirements
-
-- TODO
-
 ## Installation
 
 You can install _Event Vision Library_ via [pip] from [PyPI]:
 
 ```console
 $ pip install event-vision-library
 ```
 
 ## Usage
 
-TBD
+Please see our examples and documentations.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `event_vision_library-0.0.0b0/pyproject.toml` & `event_vision_library-0.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-vision-library"
-version = "0.0.0b"
+version = "0.0.1"
 description = "Event Vision Library"
 authors = ["Shintaro Shiba <shiba.shintaro@gmail.com>", "Friedhelm Hamann <friedhelmha2@gmail.com>"]
 maintainers = [
     "Shintaro Shiba <shiba.shintaro@gmail.com>",
     "Friedhelm Hamann <friedhelmha2@gmail.com>",
 ]
 license = "MIT"
@@ -36,14 +36,16 @@
     {version = "<=1.9.1", python = "==3.7"}
 ]  # TODO check newer version of scipy
 torch = [
     {version = ">=2.0.0", python = ">=3.8,<3.11"},
     {version = "<=2.0.0", python = "==3.7"}
 ]  # TODO check newer version of torch
 # check https://github.com/python-poetry/poetry/issues/6409 and https://github.com/pytorch/pytorch/issues/76557
+pillow = ">=9.5.0"
+matplotlib = ">=3.5.3"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -55,19 +57,17 @@
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
-safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
-typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 myst-parser = {version = ">=0.16.1"}
 
 [tool.poetry.scripts]
 event-vision-library = "evlib.__main__:main"
 
 [tool.coverage.paths]
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/_version.py` & `event_vision_library-0.0.1/src/evlib/_version.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/__init__.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/__init__.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/aedat.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/aedat.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,44 +7,42 @@
 import dv
 import numpy as np
 from dv import AedatFile
 
 
 logger = logging.getLogger(__name__)
 
+from ...types import RawEvents
 from ._iterator_access import IteratorAccess
 
 
 # TODO make parser abstract and merge these classes.
 
 
 class IteratorAedat4(IteratorAccess):
     FORMAT = "aedat4"
 
     def __init__(self, aedat4file: str) -> None:
         super().__init__(aedat4file)
         self.file = dv.AedatFile(self.file_name)
         self.count = 0
 
-    def __next__(self) -> Dict[str, Any]:
-        raise NotImplementedError
-
 
 class IteratorAedat4Event(IteratorAedat4):
     def __init__(self, aedat4file: str) -> None:
         super().__init__(aedat4file)
         self.file_iter = self.file["events"].numpy()
 
-    def __next__(self) -> Dict[str, Any]:
+    def __next__(self) -> RawEvents:
         """
         Returns:
-            dict: {"x", "y", "t", "p": all np.ndarray (N)}
+            RawEvents:
         """
         ev = self.file_iter.__next__()
-        return {"x": ev["x"], "y": ev["y"], "t": ev["timestamp"], "p": ev["polarity"]}
+        return RawEvents(x=ev["x"], y=ev["y"], timestamp=ev["timestamp"], polarity=ev["polarity"])
 
 
 class IteratorAedat4Trigger(IteratorAedat4):
     def __init__(self, aedat4file: str) -> None:
         super().__init__(aedat4file)
         self.file_iter = self.file["triggers"]
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/conversion.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/conversion.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/evk.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/evk.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/hdf5.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/hdf5.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,60 +16,69 @@
 logger = logging.getLogger(__name__)
 
 
 def load_hdf5(
     path: str, key_dtype_pairs: Union[List[H5_SET], H5_SET]
 ) -> Dict[str, np.ndarray]:
     """Load all the contents of .hdf5 file at once.
+    
     Args:
-        path (str) ... Path to the .hdf5 file.
-        key_dtype_pairs (list of tuple) ... A triplet, or list of triplets of
-            (key of the return dictionary, key of the hdf5 file data, data type for numpy).
+        path (str): Path to the .hdf5 file.
+        key_dtype_pairs (list of tuple): A triplet, or list of triplets of \\
+            (key of the return dictionary, key of the hdf5 file data, data type for numpy).\\
             For example,
             [("ts", "raw_events/ts", np.int32), ("x", "raw_events/x", np.int16), ...]
 
     Returns:
-        dict ... {key of the return dictionary: np.ndarray}
+        dict: {key of the return dictionary: np.ndarray}
     """
     if isinstance(key_dtype_pairs, tuple):
         key_dtype_pairs = [key_dtype_pairs]  # make it list.
     f = h5py.File(path, "r")
     data = {k: np.array(f[v], dtype=t) for (k, v, t) in key_dtype_pairs}
     f.close()
     return data
 
 
 def open_hdf5(path: str) -> Any:
     """Open .hdf5 file, not to load them at once.
+    
     Args:
-        path (str) ... Path to the .hdf5 file.
+        path (str): Path to the .hdf5 file.
 
     Returns:
         (Any) opened hdf5 object.
     """
     return h5py.File(path, "r")
 
 
 def load_event_timestamp_hdf5(
     path: str, key_pairs: Tuple[str, str], dtype: type = np.int32
 ) -> Dict[str, np.ndarray]:
     """For utility: load only timestamps from the hdf5 data.
+    
     Args:
-        path (str) ... Path to the .hdf5 file.
-        key_pairs  ... The tuple of
+        path (str): Path to the .hdf5 file.
+        key_pairs : The tuple of \\
             (key of the return dictionary, key of the hdf5 file data)
     
     Returns:
         dict
     """
     data = load_hdf5(path, list(key_pairs + (dtype,)))  # type: ignore
     if np.max(data[key_pairs[0]]) == np.iinfo(dtype):
         w = f"Please check the size of the data and data type. {dtype} may not be enough."
         logger.warning(w)
     return data
 
 
 def hdf5append(data: Any, new_arr: np.ndarray) -> None:
+    """For utility: append an array to hdf5 data.
+
+    Args:
+        data (Any): _description_
+        new_arr (np.ndarray): _description_
+    """
     n_old = data.shape[0]
     n_new = n_old + len(new_arr)
     data.resize(n_new, axis=0)
     data[n_old:] = new_arr
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/codec/fileformat/text.py` & `event_vision_library-0.0.1/src/evlib/codec/fileformat/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import cv2
 import numpy as np
 
 
 logger = logging.getLogger(__name__)
 
+from ...types import RawEvents
 from ._iterator_access import IteratorAccess
 
 
 # TODO make parser abstract and merge these classes.
 
 
 class IteratorText(IteratorAccess):
@@ -32,38 +33,35 @@
 
     def read_next_lines(self) -> List[str]:
         lines = self.file.readlines()
         if not lines:
             raise StopIteration
         return lines
 
-    def __next__(self) -> Dict[str, Any]:
-        raise NotImplementedError
-
 
 class IteratorTextEvent(IteratorText):
-    def __next__(self) -> Dict[str, Any]:
+    def __next__(self) -> RawEvents:
         """
         Returns:
-            dict: {"x", "y", "t", "p": all np.ndarray (N)}
+            RawEvents: events
         """
         lines = self.read_next_lines()
         _l = len(lines)
         x = np.zeros((_l,), dtype=np.int32)
         y = np.zeros((_l,), dtype=np.int32)
         t = np.zeros((_l,), dtype=np.float64)
         p = np.zeros((_l,), dtype=bool)
         for _i, line in enumerate(lines):
             val = line.split()
             t[_i] = np.float64(val[0])
             x[_i] = int(val[1])
             y[_i] = int(val[2])
             p[_i] = int(val[3])
         self.count += _l
-        return {"x": x, "y": y, "t": t, "p": p, "num": _l}
+        return RawEvents(x=x, y=y, timestamp=t, polarity=p)
 
 
 class IteratorTextPose(IteratorText):
     def __next__(self) -> Dict[str, Any]:
         """
         Returns:
             dict: {"pose": np.ndarray (N, 7)}
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/base_model.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/base_model.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/image_reconstructor.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/model.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/model.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/submodules.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/model/unet.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/model/unet.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/inference_utils.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py` & `event_vision_library-0.0.1/src/evlib/processing/reconstruction/e2vid_module/utils/loading_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
 
 def get_device(use_gpu: bool) -> torch.device:
     if use_gpu and torch.cuda.is_available():
         device = torch.device('cuda:0')
     else:
         device = torch.device('cpu')
-    logger.info('Device:', device)
+    logger.info(f'Device: {device}')
 
     return device
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/representation/histogram.py` & `event_vision_library-0.0.1/src/evlib/representation/histogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Histogram representation.
+"""
 from typing import Any
 from typing import Tuple
 
 import numpy as np
 
 
 class Histogram:
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/representation/time_map.py` & `event_vision_library-0.0.1/src/evlib/representation/time_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Time-map representation.
+"""
 from typing import Any
 from typing import Tuple
 
 import numpy as np
 
 
 class TimeMap:
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/representation/voxel_grid.py` & `event_vision_library-0.0.1/src/evlib/representation/voxel_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Voxel-grid representation.
+"""
 from typing import Any
 from typing import Tuple
 
 import numpy as np
 
 
 class VoxelGrid:
```

### Comparing `event_vision_library-0.0.0b0/src/evlib/version.py` & `event_vision_library-0.0.1/src/evlib/version.py`

 * *Files identical despite different names*

### Comparing `event_vision_library-0.0.0b0/PKG-INFO` & `event_vision_library-0.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-vision-library
-Version: 0.0.0b0
+Version: 0.0.1
 Summary: Event Vision Library
 Home-page: https://github.com/shiba24/event-vision-library
 License: MIT
 Author: Shintaro Shiba
 Author-email: shiba.shintaro@gmail.com
 Maintainer: Shintaro Shiba
 Maintainer-email: shiba.shintaro@gmail.com
@@ -16,16 +16,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: dv (>=1.0.11)
 Requires-Dist: expelliarmus (>=1.1.12)
 Requires-Dist: h5py (>=3.2)
+Requires-Dist: matplotlib (>=3.5.3)
 Requires-Dist: numpy (>=1.21.2)
 Requires-Dist: opencv-python (>=4.6)
+Requires-Dist: pillow (>=9.5.0)
 Requires-Dist: scipy (<=1.9.1) ; python_version == "3.7"
 Requires-Dist: scipy (==1.9.1) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: torch (<=2.0.0) ; python_version == "3.7"
 Requires-Dist: torch (>=2.0.0) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: wheel (>=0.38.4)
 Project-URL: Changelog, https://github.com/shiba24/event-vision-library/releases
 Project-URL: Documentation, https://event-vision-library.readthedocs.io
@@ -55,51 +57,48 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Features
 
 - Python 3.7, 3.8, 3.9, 3.10
 - Pure-python library
+- 🚧 This library is under construction and currently alpha version. The APIs may change significantly. Contributions and discussions are welcomed! 🚧
+
+### Data
+
+- [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
+- [ ] ROS bag files (optional, based on ROS installation)
+- [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
+- [ ] Support iterator-based loading and also block-based (random access) loading.
 
 ### Algorithms
 
 - Have different off-the-shelf methods, ready to use:
   - [ ] Optical Flow estimation
   - [ ] Image reconstruction
   - [ ] Ego-motion estimation
   - more to come.
 - [ ] C++ implementation and extension for faster execution (TODO)
 
-### Data
-
-- [ ] Support different data types (.text, .raw, .hdf5, .npy, .aedat) for various file encoding of event data
-- [ ] ROS bag files (optional, based on ROS installation)
-- [ ] Support multiple existing dataset (e.g., ECD, MVSEC, DSEC, etc.)
-- [ ] Support iterator-based loading and also block-based (random access) loading.
-
 ### Log and Vsualization
 
 - [ ] Various visualization for 2D/3D representation of events
 - [ ] Useful logging
 
-## Requirements
-
-- TODO
-
 ## Installation
 
 You can install _Event Vision Library_ via [pip] from [PyPI]:
 
 ```console
 $ pip install event-vision-library
 ```
 
 ## Usage
 
-TBD
+Please see our examples and documentations.
 
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

