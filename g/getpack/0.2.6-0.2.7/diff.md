# Comparing `tmp/getpack-0.2.6.tar.gz` & `tmp/getpack-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpack-0.2.6.tar", last modified: Wed May 10 21:47:31 2023, max compression
+gzip compressed data, was "getpack-0.2.7.tar", last modified: Fri May 12 15:05:07 2023, max compression
```

## Comparing `getpack-0.2.6.tar` & `getpack-0.2.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.777969 getpack-0.2.6/
--rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2222 2023-05-10 21:47:31.777969 getpack-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1535 2023-02-17 09:18:11.000000 getpack-0.2.6/README.md
--rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0     1078 2023-05-10 21:47:31.790964 getpack-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.656966 getpack-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.694964 getpack-0.2.6/src/getpack/
--rw-rw-rw-   0        0        0      403 2023-05-10 21:22:58.000000 getpack-0.2.6/src/getpack/__init__.py
--rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.6/src/getpack/executable.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.763965 getpack-0.2.6/src/getpack/library/
--rw-rw-rw-   0        0        0     3024 2023-05-04 17:14:18.000000 getpack-0.2.6/src/getpack/library/__init__.py
--rw-rw-rw-   0        0        0    12295 2023-05-10 21:26:12.000000 getpack-0.2.6/src/getpack/resource.py
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.759968 getpack-0.2.6/src/getpack.egg-info/
--rw-rw-rw-   0        0        0     2222 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 21:47:31.000000 getpack-0.2.6/src/getpack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 21:47:31.775966 getpack-0.2.6/tests/
--rw-rw-rw-   0        0        0     1452 2023-05-10 20:32:48.000000 getpack-0.2.6/tests/test_common.py
--rw-rw-rw-   0        0        0     1071 2023-05-10 21:29:25.000000 getpack-0.2.6/tests/test_concurrency.py
--rw-rw-rw-   0        0        0      444 2023-05-10 21:41:05.000000 getpack-0.2.6/tests/test_executable.py
--rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.6/tests/test_unicode.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.989065 getpack-0.2.7/
+-rw-rw-rw-   0        0        0     1097 2022-11-26 18:28:38.000000 getpack-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     2643 2023-05-12 15:05:06.990063 getpack-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1647 2023-05-12 14:04:44.000000 getpack-0.2.7/README.md
+-rw-rw-rw-   0        0        0       85 2022-11-26 18:28:38.000000 getpack-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1078 2023-05-12 15:05:07.001063 getpack-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0       38 2022-11-26 18:28:38.000000 getpack-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.863949 getpack-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.909949 getpack-0.2.7/src/getpack/
+-rw-rw-rw-   0        0        0      403 2023-05-12 14:09:49.000000 getpack-0.2.7/src/getpack/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-04-27 23:53:20.000000 getpack-0.2.7/src/getpack/executable.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.963959 getpack-0.2.7/src/getpack/library/
+-rw-rw-rw-   0        0        0     3024 2023-05-04 17:14:18.000000 getpack-0.2.7/src/getpack/library/__init__.py
+-rw-rw-rw-   0        0        0    12401 2023-05-12 14:14:32.000000 getpack-0.2.7/src/getpack/resource.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.961948 getpack-0.2.7/src/getpack.egg-info/
+-rw-rw-rw-   0        0        0     2643 2023-05-12 15:05:06.000000 getpack-0.2.7/src/getpack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-05-12 15:05:06.000000 getpack-0.2.7/src/getpack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 15:05:06.000000 getpack-0.2.7/src/getpack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-05-12 15:05:06.000000 getpack-0.2.7/src/getpack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 15:05:06.000000 getpack-0.2.7/src/getpack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 15:05:06.987948 getpack-0.2.7/tests/
+-rw-rw-rw-   0        0        0     1452 2023-05-10 20:32:48.000000 getpack-0.2.7/tests/test_common.py
+-rw-rw-rw-   0        0        0     1071 2023-05-10 21:29:25.000000 getpack-0.2.7/tests/test_concurrency.py
+-rw-rw-rw-   0        0        0      444 2023-05-10 21:41:05.000000 getpack-0.2.7/tests/test_executable.py
+-rw-rw-rw-   0        0        0      496 2023-04-03 00:10:25.000000 getpack-0.2.7/tests/test_unicode.py
```

### Comparing `getpack-0.2.6/LICENSE` & `getpack-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `getpack-0.2.6/PKG-INFO` & `getpack-0.2.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,40 @@
-Metadata-Version: 2.1
-Name: getpack
-Version: 0.2.6
-Summary: Declarative external resources with implicit deployment
-Home-page: https://github.com/kalemas/getpack
-Author: Konstantin Maslyuk
-Author-email: Kostya.Maslyuk@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-### Declarative external resources any with implicit deployment
-
-This package provide classes that allow to setup external resources (utilities,
-python packages etc.) that will be deployed as they are used. In most
-cases data should be on the web and it will be deployed and cached locally on
-only first usage.
-
-There are several examples in `test/` folder and `getpack.library` module
-already defined and useable. But main intention is to provide framework for
-declarative setup of any resource and work with it without care of deployment.
-```python
-from getpack.resource import WebResource
-class Example(WebResource):
-    version = '0.1'
-    archive_url = 'https://example.com/example-0.1.zip'
-```
-then it would be used:
-```python
-import subprocess
-subprocess.call(Example()().path / 'example.exe')
-```
-Second round braces required to actually make an effect from resource
-and first round braces used to initialize resource class, that would produce
-resource descriptions on the fly like follows:
-```python
-Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
-```
-You may experiment with following working snippet and try to change `PySide2`
-version:
-```bash
-python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
-```
-
-### TODO
-
-- Utilize `requirements.txt` to reproduce both development and production
-  environments.
-
-
+### Declarative external resources any with implicit deployment
+
+This package provide classes that allow to setup external resources (utilities,
+python packages etc.) that will be deployed as they are used. In most
+cases data should be on the web and it will be deployed and cached locally on
+only first usage.
+
+There are several examples in `test/` folder and `getpack.library` module
+already defined and useable. But main intention is to provide framework for
+declarative setup of any resource and work with it without care of deployment.
+```python
+from getpack.resource import WebResource
+class Example(WebResource):
+    version = '0.1'
+    archive_url = 'https://example.com/example-0.1.zip'
+```
+then it would be used:
+```python
+import subprocess
+subprocess.call(Example()().path / 'example.exe')
+```
+Second round braces required to actually make an effect from resource
+and first round braces used to initialize resource class, that would produce
+resource descriptions on the fly like follows:
+```python
+Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
+```
+You may experiment with following working snippet and try to change `PySide2`
+version:
+```bash
+python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
+```
+
+### TODO
+
+- Utilize `requirements.txt` to reproduce both development and production
+  environments.
+
+### Testings
+For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
```

### Comparing `getpack-0.2.6/README.md` & `getpack-0.2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,57 @@
-### Declarative external resources any with implicit deployment
-
-This package provide classes that allow to setup external resources (utilities,
-python packages etc.) that will be deployed as they are used. In most
-cases data should be on the web and it will be deployed and cached locally on
-only first usage.
-
-There are several examples in `test/` folder and `getpack.library` module
-already defined and useable. But main intention is to provide framework for
-declarative setup of any resource and work with it without care of deployment.
-```python
-from getpack.resource import WebResource
-class Example(WebResource):
-    version = '0.1'
-    archive_url = 'https://example.com/example-0.1.zip'
-```
-then it would be used:
-```python
-import subprocess
-subprocess.call(Example()().path / 'example.exe')
-```
-Second round braces required to actually make an effect from resource
-and first round braces used to initialize resource class, that would produce
-resource descriptions on the fly like follows:
-```python
-Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
-```
-You may experiment with following working snippet and try to change `PySide2`
-version:
-```bash
-python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
-```
-
-### TODO
-
-- Utilize `requirements.txt` to reproduce both development and production
-  environments.
+Metadata-Version: 2.1
+Name: getpack
+Version: 0.2.7
+Summary: Declarative external resources with implicit deployment
+Home-page: https://github.com/kalemas/getpack
+Author: Konstantin Maslyuk
+Author-email: Kostya.Maslyuk@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/kalemas/getpack/issues
+Description: ### Declarative external resources any with implicit deployment
+        
+        This package provide classes that allow to setup external resources (utilities,
+        python packages etc.) that will be deployed as they are used. In most
+        cases data should be on the web and it will be deployed and cached locally on
+        only first usage.
+        
+        There are several examples in `test/` folder and `getpack.library` module
+        already defined and useable. But main intention is to provide framework for
+        declarative setup of any resource and work with it without care of deployment.
+        ```python
+        from getpack.resource import WebResource
+        class Example(WebResource):
+            version = '0.1'
+            archive_url = 'https://example.com/example-0.1.zip'
+        ```
+        then it would be used:
+        ```python
+        import subprocess
+        subprocess.call(Example()().path / 'example.exe')
+        ```
+        Second round braces required to actually make an effect from resource
+        and first round braces used to initialize resource class, that would produce
+        resource descriptions on the fly like follows:
+        ```python
+        Example(version='0.2', archive_url='https://Example.com/example-0.2.zip')
+        ```
+        You may experiment with following working snippet and try to change `PySide2`
+        version:
+        ```bash
+        python -c "import getpack.library;getpack.library.PySide2(version='5.14.1')(); import PySide2.QtWidgets; app=PySide2.QtWidgets.QApplication(); w=PySide2.QtWidgets.QPushButton(PySide2.__version__); w.clicked.connect(w.close); w.show(); app.exec_()"
+        ```
+        
+        ### TODO
+        
+        - Utilize `requirements.txt` to reproduce both development and production
+          environments.
+        
+        ### Testings
+        For linux testing with Docker, run: `docker build -t test . && docker run -it --rm test pytest .`
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 2
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
```

### Comparing `getpack-0.2.6/setup.cfg` & `getpack-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `getpack-0.2.6/src/getpack/executable.py` & `getpack-0.2.7/src/getpack/executable.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.6/src/getpack/library/__init__.py` & `getpack-0.2.7/src/getpack/library/__init__.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.6/src/getpack/resource.py` & `getpack-0.2.7/src/getpack/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 import typing
 import zipfile
 
 import fasteners
 from six.moves import urllib
 
 
-__FILE_LOCK_TIMEOUT__ = 15 * 60
-
-
 class HybridLock:
     def __init__(self, key):
         self.key = key.as_posix() + '.lock'
         self.folder = os.path.dirname(self.key)
         self.file_lock = fasteners.InterProcessLock(self.key)
         self.lock = threading.RLock()
         self.counter = 0
@@ -140,15 +137,18 @@
 
     def cleanup(self):
         raise NotImplementedError
 
 
 class LocalResource(Resource):
     """Locally cached resource."""
-    local_base = Path(os.getenv('APPDATA')) / 'getpack'
+    if sys.platform == 'win32':
+        local_base = Path(os.getenv('APPDATA')) / 'getpack'
+    elif sys.platform == 'linux':
+        local_base = Path(os.environ['HOME']) / '.config' / 'getpack'
     local_prefix = ''
     _path = None
 
     @property
     def path(self):  # type: () -> Path
         if self._path is None:
             self._path = (
```

### Comparing `getpack-0.2.6/tests/test_common.py` & `getpack-0.2.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `getpack-0.2.6/tests/test_concurrency.py` & `getpack-0.2.7/tests/test_concurrency.py`

 * *Files identical despite different names*

