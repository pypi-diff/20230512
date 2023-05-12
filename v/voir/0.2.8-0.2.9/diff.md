# Comparing `tmp/voir-0.2.8.tar.gz` & `tmp/voir-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voir-0.2.8.tar", max compression
+gzip compressed data, was "voir-0.2.9.tar", max compression
```

## Comparing `voir-0.2.8.tar` & `voir-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      803 2023-05-04 19:45:04.353603 voir-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.8/voir/__init__.py
--rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.8/voir/__main__.py
--rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.8/voir/argparse_ext.py
--rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.8/voir/cli.py
--rw-r--r--   0        0        0      107 2023-05-02 17:55:30.856401 voir-0.2.8/voir/errors.py
--rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.8/voir/helpers.py
--rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.8/voir/instruments/__init__.py
--rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.8/voir/instruments/dash.py
--rw-r--r--   0        0        0     3408 2023-05-04 17:50:09.395001 voir-0.2.8/voir/instruments/gpu/__init__.py
--rw-r--r--   0        0        0      257 2023-05-04 19:44:56.525148 voir-0.2.8/voir/instruments/gpu/cpu.py
--rw-r--r--   0        0        0     2286 2023-05-04 19:44:56.525362 voir-0.2.8/voir/instruments/gpu/cuda.py
--rw-r--r--   0        0        0     5896 2023-05-04 17:50:09.395420 voir-0.2.8/voir/instruments/gpu/rocm.py
--rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.8/voir/instruments/log.py
--rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.8/voir/instruments/manage.py
--rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.8/voir/instruments/metric.py
--rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.8/voir/instruments/utils.py
--rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.8/voir/overseer.py
--rw-r--r--   0        0        0     9968 2023-05-02 17:55:30.857303 voir-0.2.8/voir/phase.py
--rw-r--r--   0        0        0     6183 2023-05-02 17:53:58.153830 voir-0.2.8/voir/proc.py
--rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.8/voir/run.py
--rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.8/voir/scriptutils.py
--rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.8/voir/smuggle.py
--rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.8/voir/tools.py
--rw-r--r--   0        0        0       18 2023-05-04 19:45:04.378428 voir-0.2.8/voir/version.py
--rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 voir-0.2.8/setup.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      803 2023-05-12 19:35:14.811010 voir-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-03-23 16:47:14.434366 voir-0.2.9/voir/__init__.py
+-rw-r--r--   0        0        0       61 2023-03-20 20:01:11.843872 voir-0.2.9/voir/__main__.py
+-rw-r--r--   0        0        0     7819 2023-03-23 16:47:14.434629 voir-0.2.9/voir/argparse_ext.py
+-rw-r--r--   0        0        0      759 2023-03-23 16:47:14.434905 voir-0.2.9/voir/cli.py
+-rw-r--r--   0        0        0      107 2023-05-02 17:55:30.856401 voir-0.2.9/voir/errors.py
+-rw-r--r--   0        0        0     1809 2023-03-25 15:52:21.103341 voir-0.2.9/voir/helpers.py
+-rw-r--r--   0        0        0      399 2023-03-23 16:47:14.435425 voir-0.2.9/voir/instruments/__init__.py
+-rw-r--r--   0        0        0     3292 2023-03-23 16:47:14.435688 voir-0.2.9/voir/instruments/dash.py
+-rw-r--r--   0        0        0     3584 2023-05-12 19:35:07.579889 voir-0.2.9/voir/instruments/gpu/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-12 19:35:07.580243 voir-0.2.9/voir/instruments/gpu/cpu.py
+-rw-r--r--   0        0        0     2914 2023-05-12 19:35:07.580424 voir-0.2.9/voir/instruments/gpu/cuda.py
+-rw-r--r--   0        0        0     5992 2023-05-12 19:35:07.580593 voir-0.2.9/voir/instruments/gpu/rocm.py
+-rw-r--r--   0        0        0      884 2023-03-23 16:47:14.436583 voir-0.2.9/voir/instruments/log.py
+-rw-r--r--   0        0        0      818 2023-04-01 02:22:45.030632 voir-0.2.9/voir/instruments/manage.py
+-rw-r--r--   0        0        0     5981 2023-03-25 16:19:36.879569 voir-0.2.9/voir/instruments/metric.py
+-rw-r--r--   0        0        0      382 2023-03-28 03:32:37.110995 voir-0.2.9/voir/instruments/utils.py
+-rw-r--r--   0        0        0     6334 2023-03-23 16:47:14.437785 voir-0.2.9/voir/overseer.py
+-rw-r--r--   0        0        0     9968 2023-05-02 17:55:30.857303 voir-0.2.9/voir/phase.py
+-rw-r--r--   0        0        0     6183 2023-05-02 17:53:58.153830 voir-0.2.9/voir/proc.py
+-rw-r--r--   0        0        0     1667 2023-03-23 16:47:14.438784 voir-0.2.9/voir/run.py
+-rw-r--r--   0        0        0     1306 2023-03-23 16:47:14.439124 voir-0.2.9/voir/scriptutils.py
+-rw-r--r--   0        0        0     3060 2023-03-23 16:47:14.439374 voir-0.2.9/voir/smuggle.py
+-rw-r--r--   0        0        0     1720 2023-03-23 16:47:14.439677 voir-0.2.9/voir/tools.py
+-rw-r--r--   0        0        0       18 2023-05-12 19:35:14.835265 voir-0.2.9/voir/version.py
+-rw-r--r--   0        0        0      903 1970-01-01 00:00:00.000000 voir-0.2.9/setup.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 voir-0.2.9/PKG-INFO
```

### Comparing `voir-0.2.8/pyproject.toml` & `voir-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voir"
-version = "0.2.8"
+version = "0.2.9"
 description = "Instrument, extend and visualize your programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 ptera = "^1.4.1"
```

### Comparing `voir-0.2.8/voir/argparse_ext.py` & `voir-0.2.9/voir/argparse_ext.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/cli.py` & `voir-0.2.9/voir/cli.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/helpers.py` & `voir-0.2.9/voir/helpers.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/instruments/dash.py` & `voir-0.2.9/voir/instruments/dash.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/instruments/gpu/__init__.py` & `voir-0.2.9/voir/instruments/gpu/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,23 +91,29 @@
         DEVICESMI = backend.DeviceSMI()
     else:
         raise NotAvailable(f"{arch} is not installed")
 
     return DEVICESMI
 
 
-def gpu_info(smi):
+def gpu_info(smi, visible=True):
+    selection = None
+
+    # Make sure to only show the visible devices
+    if visible:
+        selection = _visible_devices(smi)
+
     return {
         "arch": smi.arch,
-        "gpus": smi.get_gpus_info(),
+        "gpus": smi.get_gpus_info(selection),
     }
 
 
-def get_gpu_info(arch=None):
-    return gpu_info(select_backend(arch))
+def get_gpu_info(arch=None, visible=True):
+    return gpu_info(select_backend(arch), visible)
 
 
 def _visible_devices(smi):
     visible = smi.visible_devices
 
     if visible:
         ours = visible.split(",")
```

### Comparing `voir-0.2.8/voir/instruments/gpu/cuda.py` & `voir-0.2.9/voir/instruments/gpu/cuda.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,32 +52,33 @@
     def __init__(self) -> None:
         if IMPORT_ERROR is not None:
             raise IMPORT_ERROR
 
         try:
             nvmlInit()
             self.nvsmi = nvidia_smi.getInstance()
-
         except NVMLError_LibraryNotFound as err:
             raise NotAvailable() from err
 
         except NVMLError_DriverNotLoaded as err:
             raise NotAvailable() from err
 
     @property
     def arch(self):
         return "cuda"
 
     @property
     def visible_devices(self):
         return os.environ.get("CUDA_VISIBLE_DEVICES", None)
 
-    def get_gpus_info(self):
+    def get_gpus_info(self, selection=None):
         to_query = [
-            "gpu_name",
+            "uuid",  # Globally unique immutable alphanumeric identifier of the GPU
+            "index",  # Zero based index of the GPU. Can change at each boot.
+            "gpu_name",  # Official Product name
             "memory.free",
             "memory.used",
             "memory.total",
             "temperature.gpu",
             "utilization.gpu",
             "utilization.memory",
             "power.draw",
@@ -87,11 +88,24 @@
         if not results or "gpu" not in results:
             return {}
 
         gpus = results["gpu"]
         if not isinstance(gpus, list):
             gpus = [gpus]
 
-        return {str(i): parse_gpu(g, i) for i, g in enumerate(gpus)}
+        # To support MIG we start using UUID instead of indexes
+        # Nevertheless indexes are useful to quickly select specific GPUs
+        # so we support selecting GPUs using both
+        results = dict()
+        for g in gpus:
+            i = g["minor_number"]
+            uuid = g["uuid"]
+
+            if (selection is None) or (
+                selection and (i in selection or uuid in selection)
+            ):
+                results[uuid] = parse_gpu(g, i)
+
+        return results
 
     def close(self):
         pass
```

### Comparing `voir-0.2.8/voir/instruments/gpu/rocm.py` & `voir-0.2.9/voir/instruments/gpu/rocm.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,17 @@
     def arch(self):
         return "rocm"
 
     @property
     def visible_devices(self):
         return os.environ.get("ROCR_VISIBLE_DEVICES", None)
 
-    def get_gpus_info(self):
+    def get_gpus_info(self, selection=None):
         gpus = dict()
         for device in self.devices:
-            gpus[device] = self.get_gpu_info(device)
+            if (selection is None) or (selection and device in selection):
+                gpus[device] = self.get_gpu_info(device)
+
         return gpus
 
     def close(self):
         pass
```

### Comparing `voir-0.2.8/voir/instruments/log.py` & `voir-0.2.9/voir/instruments/log.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/instruments/manage.py` & `voir-0.2.9/voir/instruments/manage.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/instruments/metric.py` & `voir-0.2.9/voir/instruments/metric.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/overseer.py` & `voir-0.2.9/voir/overseer.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/phase.py` & `voir-0.2.9/voir/phase.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/proc.py` & `voir-0.2.9/voir/proc.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/run.py` & `voir-0.2.9/voir/run.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/scriptutils.py` & `voir-0.2.9/voir/scriptutils.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/smuggle.py` & `voir-0.2.9/voir/smuggle.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/voir/tools.py` & `voir-0.2.9/voir/tools.py`

 * *Files identical despite different names*

### Comparing `voir-0.2.8/setup.py` & `voir-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'rich>=13.3.2,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['voir = voir.cli:main']}
 
 setup_kwargs = {
     'name': 'voir',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Instrument, extend and visualize your programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `voir-0.2.8/PKG-INFO` & `voir-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voir
-Version: 0.2.8
+Version: 0.2.9
 Summary: Instrument, extend and visualize your programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

