# Comparing `tmp/umbridge-1.2.1.tar.gz` & `tmp/umbridge-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umbridge-1.2.1.tar", last modified: Wed Nov  2 08:20:05 2022, max compression
+gzip compressed data, was "umbridge-1.2.2.tar", last modified: Fri May 12 10:38:04 2023, max compression
```

## Comparing `umbridge-1.2.1.tar` & `umbridge-1.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 08:20:05.921150 umbridge-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-11-02 08:19:54.000000 umbridge-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-11-02 08:20:05.921150 umbridge-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2022-11-02 08:19:54.000000 umbridge-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-02 08:20:05.921150 umbridge-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-11-02 08:19:54.000000 umbridge-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 08:20:05.917149 umbridge-1.2.1/umbridge/
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-11-02 08:19:54.000000 umbridge-1.2.1/umbridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-11-02 08:19:54.000000 umbridge-1.2.1/umbridge/pymc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19913 2022-11-02 08:19:54.000000 umbridge-1.2.1/umbridge/um.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 08:20:05.921150 umbridge-1.2.1/umbridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-11-02 08:20:05.000000 umbridge-1.2.1/umbridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-11-02 08:20:05.000000 umbridge-1.2.1/umbridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 08:20:05.000000 umbridge-1.2.1/umbridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-02 08:20:05.000000 umbridge-1.2.1/umbridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-02 08:20:05.000000 umbridge-1.2.1/umbridge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.993322 umbridge-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 10:37:52.000000 umbridge-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-12 10:38:04.993322 umbridge-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-12 10:37:52.000000 umbridge-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:38:04.993322 umbridge-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-12 10:37:52.000000 umbridge-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.989321 umbridge-1.2.2/umbridge/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/pymc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19958 2023-05-12 10:37:52.000000 umbridge-1.2.2/umbridge/um.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:38:04.993322 umbridge-1.2.2/umbridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-12 10:38:04.000000 umbridge-1.2.2/umbridge.egg-info/top_level.txt
```

### Comparing `umbridge-1.2.1/LICENSE` & `umbridge-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.1/PKG-INFO` & `umbridge-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: umbridge
-Version: 1.2.1
+Version: 1.2.2
 Summary: UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 Home-page: https://github.com/UM-Bridge/umbridge
 Author: UM-Bridge
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: pymc
 License-File: LICENSE
 
 # UM-Bridge
 
 UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 
 In many statistical / uncertainty quantification or optimization methods, the model only appears as a function mapping vectors onto vectors with some of the following:
```

### Comparing `umbridge-1.2.1/README.md` & `umbridge-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `umbridge-1.2.1/setup.py` & `umbridge-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="umbridge",
-    version="1.2.1",
+    version="1.2.2",
     author="UM-Bridge",
     author_email="",
     description="UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["aiohttp", "requests", "asyncio"],
-    extras_require = {
-        'pymc':  ["aesara"]
-    },
     url="https://github.com/UM-Bridge/umbridge",
     packages=setuptools.find_packages(),
     classifiers=(                                 # Classifiers help people find your
         "Programming Language :: Python :: 3",    # projects. See all possible classifiers
         "License :: OSI Approved :: MIT License", # in https://pypi.org/classifiers/
         "Operating System :: OS Independent",
     ),
```

### Comparing `umbridge-1.2.1/umbridge/pymc.py` & `umbridge-1.2.2/umbridge/pymc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import aesara.tensor as at
+from pytensor import tensor as pt
 import umbridge
 import numpy as np
 
 
-class UmbridgeGradOp(at.Op):
+class UmbridgeGradOp(pt.Op):
 
-    itypes = [at.dvector, at.dvector]
-    otypes = [at.dvector]
+    itypes = [pt.dvector, pt.dvector]
+    otypes = [pt.dvector]
 
     def __init__(self, umbridge_model, config):
         self.umbridge_model = umbridge_model
         self.config = config
 
     def perform(self, node, inputs_var, output_storage):
         grad = self.umbridge_model.gradient(0, 0, [inputs_var[0].tolist()], inputs_var[1].tolist(), self.config)
         output_storage[0][0] = np.asarray(grad).astype('float64')
 
-class UmbridgeOp(at.Op):
+class UmbridgeOp(pt.Op):
 
-    itypes = [at.dvector]
-    otypes = [at.dvector]
+    itypes = [pt.dvector]
+    otypes = [pt.dvector]
 
     # Take model URL in constructor
     def __init__(self, url, name, config = {}):
         self.umbridge_model = umbridge.HTTPModel(url, name)
         self.config = config
         # For now, make sure model takes a single input vector and returns a single output vector.
-        # More could be supported, but needs improved aesara op.
+        # More could be supported, but needs improved pytensor op.
         # (i.e. adjust input/output types according to UM-Bridge model, pass through multiple vectors etc.)
         assert len(self.umbridge_model.get_input_sizes(config)) == 1
         assert len(self.umbridge_model.get_output_sizes(config)) == 1
 
         self.grad_op = UmbridgeGradOp(self.umbridge_model, config)
 
     def perform(self, node, inputs, output_storage):
```

### Comparing `umbridge-1.2.1/umbridge/um.py` & `umbridge-1.2.2/umbridge/um.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,17 +151,17 @@
         inputParams["config"] = config
         response = requests.post(f"{self.url}/ApplyHessian", json=inputParams).json()
 
         if "error" in response:
             raise Exception(f'Model returned error of type {response["error"]["type"]}: {response["error"]["message"]}')
         return response["output"]
 
-def serve_models(models, port=4242):
+def serve_models(models, port=4242, max_workers=1):
 
-    model_executor = ThreadPoolExecutor(max_workers=1)
+    model_executor = ThreadPoolExecutor(max_workers=max_workers)
 
     def error_response(type, message, status):
         response_body = {
             "error": {
                 "type": type,
                 "message": message
             }
@@ -412,10 +412,10 @@
     async def info(request):
         response_body = {}
         response_body["protocolVersion"] = 1.0;
         response_body["models"] = [model.name for model in models]
         return web.json_response(response_body)
 
 
-    app = web.Application()
+    app = web.Application(client_max_size=None)
     app.add_routes(routes)
     web.run_app(app, port=port)
```

### Comparing `umbridge-1.2.1/umbridge.egg-info/PKG-INFO` & `umbridge-1.2.2/umbridge.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: umbridge
-Version: 1.2.1
+Version: 1.2.2
 Summary: UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 Home-page: https://github.com/UM-Bridge/umbridge
 Author: UM-Bridge
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: pymc
 License-File: LICENSE
 
 # UM-Bridge
 
 UM-Bridge (the UQ and Model Bridge) provides a unified interface for numerical models that is accessible from virtually any programming language or framework. It is primarily intended for coupling advanced models (e.g. simulations of complex physical processes) to advanced statistical or optimization methods.
 
 In many statistical / uncertainty quantification or optimization methods, the model only appears as a function mapping vectors onto vectors with some of the following:
```

