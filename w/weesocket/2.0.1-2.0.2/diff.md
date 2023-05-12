# Comparing `tmp/weesocket-2.0.1.tar.gz` & `tmp/weesocket-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weesocket-2.0.1.tar", last modified: Fri May 12 16:26:59 2023, max compression
+gzip compressed data, was "weesocket-2.0.2.tar", last modified: Fri May 12 16:36:52 2023, max compression
```

## Comparing `weesocket-2.0.1.tar` & `weesocket-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:26:59.660063 weesocket-2.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    34701 2023-05-07 19:09:58.000000 weesocket-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5687 2023-05-12 16:26:59.660063 weesocket-2.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5179 2023-05-08 12:49:59.000000 weesocket-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 16:26:59.660063 weesocket-2.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-05-07 19:09:58.000000 weesocket-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:26:59.660063 weesocket-2.0.1/src/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-12 16:26:57.000000 weesocket-2.0.1/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-05-07 22:25:35.000000 weesocket-2.0.1/src/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2824 2023-05-07 23:29:30.000000 weesocket-2.0.1/src/client.py
--rw-rw-rw-   0 root         (0) root         (0)     5303 2023-05-08 09:44:03.000000 weesocket-2.0.1/src/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:26:59.660063 weesocket-2.0.1/weesocket.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5687 2023-05-12 16:26:59.000000 weesocket-2.0.1/weesocket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-12 16:26:59.000000 weesocket-2.0.1/weesocket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:26:59.000000 weesocket-2.0.1/weesocket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-12 16:26:59.000000 weesocket-2.0.1/weesocket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-12 16:26:59.000000 weesocket-2.0.1/weesocket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:36:52.635157 weesocket-2.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)    34701 2023-05-07 19:09:58.000000 weesocket-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-05-12 16:36:52.635157 weesocket-2.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5179 2023-05-08 12:49:59.000000 weesocket-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 16:36:52.635157 weesocket-2.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-05-12 16:36:08.000000 weesocket-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:36:52.631157 weesocket-2.0.2/src/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-05-12 16:36:50.000000 weesocket-2.0.2/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-05-07 22:25:35.000000 weesocket-2.0.2/src/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2023-05-07 23:29:30.000000 weesocket-2.0.2/src/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5303 2023-05-08 09:44:03.000000 weesocket-2.0.2/src/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 16:36:52.635157 weesocket-2.0.2/weesocket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-05-12 16:36:52.000000 weesocket-2.0.2/weesocket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-12 16:36:52.000000 weesocket-2.0.2/weesocket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 16:36:52.000000 weesocket-2.0.2/weesocket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-12 16:36:52.000000 weesocket-2.0.2/weesocket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-12 16:36:52.000000 weesocket-2.0.2/weesocket.egg-info/top_level.txt
```

### Comparing `weesocket-2.0.1/LICENSE` & `weesocket-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `weesocket-2.0.1/PKG-INFO` & `weesocket-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weesocket
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tiny socket wrapper
 Home-page: https://gitlab.com/katry/weesocket
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `weesocket-2.0.1/README.md` & `weesocket-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `weesocket-2.0.1/setup.py` & `weesocket-2.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,33 +7,37 @@
 	class bdist_wheel(_bdist_wheel):
 		def finalize_options(self):
 			_bdist_wheel.finalize_options(self)
 			self.root_is_pure = False
 except ImportError:
 	bdist_wheel = None  # type: ignore
 
-with open("README.md", "r") as fh:
-	long_description = fh.read()
+try:
+	with open("README.md", "r") as fh:
+		long_description = fh.read()
+except Exception:
+	long_description = ""
 
-with open("requirements.txt") as rq:
-	required = rq.read().splitlines()
 
 setuptools.setup(
 	name="weesocket",
 	version=__version__,
 	author="Patrik Katrenak",
 	author_email="patrik@katryapps.com",
 	description="Tiny socket wrapper",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://gitlab.com/katry/weesocket",
 
 	package_dir={"weesocket": "src"},
 	include_package_data=True,
-	install_requires=required,
+	install_requires=[
+		"rsa==4.9",
+		"orjson==3.8.11"
+	],
 
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 		"Operating System :: OS Independent",
 		"Natural Language :: English",
 	],
```

### Comparing `weesocket-2.0.1/src/abstract.py` & `weesocket-2.0.2/src/abstract.py`

 * *Files identical despite different names*

### Comparing `weesocket-2.0.1/src/client.py` & `weesocket-2.0.2/src/client.py`

 * *Files identical despite different names*

### Comparing `weesocket-2.0.1/src/server.py` & `weesocket-2.0.2/src/server.py`

 * *Files identical despite different names*

### Comparing `weesocket-2.0.1/weesocket.egg-info/PKG-INFO` & `weesocket-2.0.2/weesocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weesocket
-Version: 2.0.1
+Version: 2.0.2
 Summary: Tiny socket wrapper
 Home-page: https://gitlab.com/katry/weesocket
 Author: Patrik Katrenak
 Author-email: patrik@katryapps.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

