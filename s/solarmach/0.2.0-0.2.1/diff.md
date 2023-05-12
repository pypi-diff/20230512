# Comparing `tmp/solarmach-0.2.0.tar.gz` & `tmp/solarmach-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solarmach-0.2.0.tar", last modified: Thu May 11 14:29:48 2023, max compression
+gzip compressed data, was "/home/gieseler/uni/serpentine/solarmach/dist/.tmp-lhamsoxp/solarmach-0.2.1.tar", last modified: Fri May 12 08:06:14 2023, max compression
```

## Comparing `solarmach-0.2.0.tar` & `solarmach-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.0/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.0/MANIFEST.in
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-11 14:29:48.427020 solarmach-0.2.0/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.2.0/README.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.0/code_of_conduct.md
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.415020 solarmach-0.2.0/docs/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.0/docs/Makefile
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.0/docs/conf.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.0/docs/index.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.0/docs/make.bat
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.423020 solarmach-0.2.0/examples/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.0/examples/example.ipynb
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.0/examples/solarmach.png
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/licenses/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.0/licenses/LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.0/licenses/TEMPLATE_LICENSE.rst
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.0/pyproject.toml
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       84 2023-05-11 14:24:48.000000 solarmach-0.2.0/requirements.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2103 2023-05-11 14:29:48.431020 solarmach-0.2.0/setup.cfg
--rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.0/setup.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    51602 2023-05-11 14:20:54.000000 solarmach-0.2.0/solarmach/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    23221 2023-05-11 14:20:54.000000 solarmach-0.2.0/solarmach/pfss_utilities.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach/tests/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.0/solarmach/tests/__init__.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.0/solarmach/tests/test.py
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach/version.py
-drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-11 14:29:48.427020 solarmach-0.2.0/solarmach.egg-info/
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/PKG-INFO
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/SOURCES.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/dependency_links.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.0/solarmach.egg-info/not-zip-safe
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      169 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/requires.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-11 14:29:48.000000 solarmach-0.2.0/solarmach.egg-info/top_level.txt
--rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.0/tox.ini
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.629089 solarmach-0.2.1/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.1/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      457 2022-01-10 16:26:49.000000 solarmach-0.2.1/MANIFEST.in
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-12 08:06:14.629089 solarmach-0.2.1/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     5268 2023-04-27 13:45:25.000000 solarmach-0.2.1/README.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     3370 2022-03-30 15:50:45.000000 solarmach-0.2.1/code_of_conduct.md
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.617089 solarmach-0.2.1/docs/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      634 2022-01-10 16:26:49.000000 solarmach-0.2.1/docs/Makefile
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2300 2022-03-14 11:55:52.000000 solarmach-0.2.1/docs/conf.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      300 2022-03-14 11:56:45.000000 solarmach-0.2.1/docs/index.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      760 2022-01-10 16:26:49.000000 solarmach-0.2.1/docs/make.bat
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.621089 solarmach-0.2.1/examples/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)  1915936 2023-04-27 13:41:04.000000 solarmach-0.2.1/examples/example.ipynb
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)   348683 2022-03-14 16:09:27.000000 solarmach-0.2.1/examples/solarmach.png
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/licenses/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1478 2022-03-14 11:21:13.000000 solarmach-0.2.1/licenses/LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1659 2022-01-10 16:26:49.000000 solarmach-0.2.1/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      134 2022-01-10 16:26:49.000000 solarmach-0.2.1/pyproject.toml
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      106 2023-05-12 08:03:40.000000 solarmach-0.2.1/requirements.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     2127 2023-05-12 08:06:14.629089 solarmach-0.2.1/setup.cfg
+-rwxrwxr-x   0 gieseler  (1000) gieseler  (1000)      660 2022-03-14 12:48:51.000000 solarmach-0.2.1/setup.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/solarmach/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    51602 2023-05-11 14:20:54.000000 solarmach-0.2.1/solarmach/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)    23221 2023-05-11 14:20:54.000000 solarmach-0.2.1/solarmach/pfss_utilities.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.629089 solarmach-0.2.1/solarmach/tests/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      108 2022-01-10 16:26:49.000000 solarmach-0.2.1/solarmach/tests/__init__.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1695 2022-11-09 14:33:28.000000 solarmach-0.2.1/solarmach/tests/test.py
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      345 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach/version.py
+drwxrwxr-x   0 gieseler  (1000) gieseler  (1000)        0 2023-05-12 08:06:14.625089 solarmach-0.2.1/solarmach.egg-info/
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     6117 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/PKG-INFO
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      584 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/SOURCES.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/dependency_links.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)        1 2022-03-17 17:20:48.000000 solarmach-0.2.1/solarmach.egg-info/not-zip-safe
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)      191 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/requires.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)       10 2023-05-12 08:06:14.000000 solarmach-0.2.1/solarmach.egg-info/top_level.txt
+-rw-rw-r--   0 gieseler  (1000) gieseler  (1000)     1292 2022-03-14 12:48:29.000000 solarmach-0.2.1/tox.ini
```

### Comparing `solarmach-0.2.0/LICENSE.rst` & `solarmach-0.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/PKG-INFO` & `solarmach-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.0
+Version: 0.2.1
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solarmach-0.2.0/README.rst` & `solarmach-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/code_of_conduct.md` & `solarmach-0.2.1/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/docs/Makefile` & `solarmach-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/docs/conf.py` & `solarmach-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/docs/make.bat` & `solarmach-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/examples/example.ipynb` & `solarmach-0.2.1/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/examples/solarmach.png` & `solarmach-0.2.1/examples/solarmach.png`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/licenses/LICENSE.rst` & `solarmach-0.2.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/licenses/TEMPLATE_LICENSE.rst` & `solarmach-0.2.1/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/setup.cfg` & `solarmach-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
 	astroquery
+	cmasher
 	drms
 	Jinja2
 	lxml
-	matplotlib
+	matplotlib==3.5.3
 	numpy
 	pandas
 	pfsspy
+	plotly
 	scipy
 	sunpy
 	zeep
 
 [options.extras_require]
 all = 
 test =
```

### Comparing `solarmach-0.2.0/setup.py` & `solarmach-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/solarmach/__init__.py` & `solarmach-0.2.1/solarmach/__init__.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/solarmach/pfss_utilities.py` & `solarmach-0.2.1/solarmach/pfss_utilities.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/solarmach/tests/test.py` & `solarmach-0.2.1/solarmach/tests/test.py`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/solarmach.egg-info/PKG-INFO` & `solarmach-0.2.1/solarmach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solarmach
-Version: 0.2.0
+Version: 0.2.1
 Summary: Multi-spacecraft longitudinal configuration plotter
 Home-page: https://github.com/jgieseler/solarmach
 Author: Jan Gieseler
 Author-email: jan.gieseler@utu.fi
 License: BSD 3-clause
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `solarmach-0.2.0/solarmach.egg-info/SOURCES.txt` & `solarmach-0.2.1/solarmach.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `solarmach-0.2.0/tox.ini` & `solarmach-0.2.1/tox.ini`

 * *Files identical despite different names*

