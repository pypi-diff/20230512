# Comparing `tmp/livesolid-0.0.7.tar.gz` & `tmp/livesolid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livesolid-0.0.7.tar", last modified: Thu May 11 13:11:30 2023, max compression
+gzip compressed data, was "livesolid-0.0.8.tar", last modified: Fri May 12 13:38:17 2023, max compression
```

## Comparing `livesolid-0.0.7.tar` & `livesolid-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.943922 livesolid-0.0.7/
--rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.7/.coveragerc
--rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.7/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.7/.isort.cfg
--rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.7/.readthedocs.yml
--rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.7/AUTHORS.rst
--rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.7/CHANGELOG.rst
--rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.7/CONTRIBUTING.rst
--rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.7/LICENSE.txt
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-11 13:11:30.944165 livesolid-0.0.7/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.7/README.rst
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.934850 livesolid-0.0.7/docs/
--rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/Makefile
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.935512 livesolid-0.0.7/docs/_static/
--rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/_static/.gitignore
--rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/authors.rst
--rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/changelog.rst
--rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.7/docs/conf.py
--rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/contributing.rst
--rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/index.rst
--rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/license.rst
--rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/readme.rst
--rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.7/docs/requirements.txt
--rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.7/pyproject.toml
--rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-11 13:11:30.945670 livesolid-0.0.7/setup.cfg
--rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.7/setup.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.921148 livesolid-0.0.7/src/
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.937565 livesolid-0.0.7/src/livesolid/
--rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.7/src/livesolid/__init__.py
--rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.7/src/livesolid/lib.py
--rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.7/src/livesolid/main.py
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.942160 livesolid-0.0.7/src/livesolid/templates/
--rw-r--r--   0 mtm        (501) staff       (20)      420 2023-05-11 13:10:29.000000 livesolid-0.0.7/src/livesolid/templates/Makefile.j2
--rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.7/src/livesolid/templates/goreleaser.yaml.j2
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.941101 livesolid-0.0.7/src/livesolid.egg-info/
--rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/PKG-INFO
--rw-r--r--   0 mtm        (501) staff       (20)      810 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/SOURCES.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/dependency_links.txt
--rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/entry_points.txt
--rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/not-zip-safe
--rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/requires.txt
--rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-11 13:11:30.000000 livesolid-0.0.7/src/livesolid.egg-info/top_level.txt
-drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-11 13:11:30.943406 livesolid-0.0.7/tests/
--rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.7/tests/conftest.py
--rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.7/tests/test_skeleton.py
--rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.7/tox.ini
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.198697 livesolid-0.0.8/
+-rw-r--r--   0 mtm        (501) staff       (20)      592 2023-04-28 13:28:55.000000 livesolid-0.0.8/.coveragerc
+-rw-r--r--   0 mtm        (501) staff       (20)      566 2023-04-28 13:28:55.000000 livesolid-0.0.8/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       57 2023-04-28 13:28:55.000000 livesolid-0.0.8/.isort.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)     1670 2023-04-28 14:23:15.000000 livesolid-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 mtm        (501) staff       (20)      530 2023-04-28 13:28:55.000000 livesolid-0.0.8/.readthedocs.yml
+-rw-r--r--   0 mtm        (501) staff       (20)       87 2023-04-28 13:28:55.000000 livesolid-0.0.8/AUTHORS.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      128 2023-04-28 13:28:55.000000 livesolid-0.0.8/CHANGELOG.rst
+-rw-r--r--   0 mtm        (501) staff       (20)    13840 2023-04-28 13:28:55.000000 livesolid-0.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     1083 2023-04-28 13:28:55.000000 livesolid-0.0.8/LICENSE.txt
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 13:38:17.198942 livesolid-0.0.8/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)     2084 2023-04-28 13:28:55.000000 livesolid-0.0.8/README.rst
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.185542 livesolid-0.0.8/docs/
+-rw-r--r--   0 mtm        (501) staff       (20)     1154 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/Makefile
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.186579 livesolid-0.0.8/docs/_static/
+-rw-r--r--   0 mtm        (501) staff       (20)       18 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/_static/.gitignore
+-rw-r--r--   0 mtm        (501) staff       (20)       41 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/authors.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       43 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/changelog.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     9742 2023-04-28 13:36:58.000000 livesolid-0.0.8/docs/conf.py
+-rw-r--r--   0 mtm        (501) staff       (20)       33 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/contributing.rst
+-rw-r--r--   0 mtm        (501) staff       (20)     2321 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/index.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       67 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/license.rst
+-rw-r--r--   0 mtm        (501) staff       (20)       39 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/readme.rst
+-rw-r--r--   0 mtm        (501) staff       (20)      233 2023-04-28 13:28:55.000000 livesolid-0.0.8/docs/requirements.txt
+-rw-r--r--   0 mtm        (501) staff       (20)      346 2023-04-28 13:28:55.000000 livesolid-0.0.8/pyproject.toml
+-rw-r--r--   0 mtm        (501) staff       (20)     1253 2023-05-12 13:38:17.200198 livesolid-0.0.8/setup.cfg
+-rw-r--r--   0 mtm        (501) staff       (20)      704 2023-04-28 13:28:55.000000 livesolid-0.0.8/setup.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.168704 livesolid-0.0.8/src/
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.191314 livesolid-0.0.8/src/livesolid/
+-rw-r--r--   0 mtm        (501) staff       (20)      577 2023-04-28 13:28:55.000000 livesolid-0.0.8/src/livesolid/__init__.py
+-rw-r--r--   0 mtm        (501) staff       (20)      779 2023-04-28 14:23:22.000000 livesolid-0.0.8/src/livesolid/lib.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2881 2023-04-28 14:28:31.000000 livesolid-0.0.8/src/livesolid/main.py
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.197016 livesolid-0.0.8/src/livesolid/templates/
+-rw-r--r--   0 mtm        (501) staff       (20)      735 2023-05-12 13:36:34.000000 livesolid-0.0.8/src/livesolid/templates/Makefile.j2
+-rw-r--r--   0 mtm        (501) staff       (20)     1184 2023-04-28 14:17:25.000000 livesolid-0.0.8/src/livesolid/templates/goreleaser.yaml.j2
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.195719 livesolid-0.0.8/src/livesolid.egg-info/
+-rw-r--r--   0 mtm        (501) staff       (20)     2562 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/PKG-INFO
+-rw-r--r--   0 mtm        (501) staff       (20)      810 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/SOURCES.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/dependency_links.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       49 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/entry_points.txt
+-rw-r--r--   0 mtm        (501) staff       (20)        1 2023-05-12 13:38:16.000000 livesolid-0.0.8/src/livesolid.egg-info/not-zip-safe
+-rw-r--r--   0 mtm        (501) staff       (20)       93 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/requires.txt
+-rw-r--r--   0 mtm        (501) staff       (20)       10 2023-05-12 13:38:17.000000 livesolid-0.0.8/src/livesolid.egg-info/top_level.txt
+drwxr-xr-x   0 mtm        (501) staff       (20)        0 2023-05-12 13:38:17.198091 livesolid-0.0.8/tests/
+-rw-r--r--   0 mtm        (501) staff       (20)      277 2023-04-28 13:28:55.000000 livesolid-0.0.8/tests/conftest.py
+-rw-r--r--   0 mtm        (501) staff       (20)      594 2023-04-28 13:28:55.000000 livesolid-0.0.8/tests/test_skeleton.py
+-rw-r--r--   0 mtm        (501) staff       (20)     2851 2023-04-28 13:28:55.000000 livesolid-0.0.8/tox.ini
```

### Comparing `livesolid-0.0.7/.coveragerc` & `livesolid-0.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/.gitignore` & `livesolid-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/.pre-commit-config.yaml` & `livesolid-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/.readthedocs.yml` & `livesolid-0.0.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/CONTRIBUTING.rst` & `livesolid-0.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/LICENSE.txt` & `livesolid-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/PKG-INFO` & `livesolid-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.7/README.rst` & `livesolid-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/docs/Makefile` & `livesolid-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/docs/conf.py` & `livesolid-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/docs/index.rst` & `livesolid-0.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/setup.cfg` & `livesolid-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/setup.py` & `livesolid-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/src/livesolid/__init__.py` & `livesolid-0.0.8/src/livesolid/__init__.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/src/livesolid/lib.py` & `livesolid-0.0.8/src/livesolid/lib.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/src/livesolid/main.py` & `livesolid-0.0.8/src/livesolid/main.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/src/livesolid/templates/goreleaser.yaml.j2` & `livesolid-0.0.8/src/livesolid/templates/goreleaser.yaml.j2`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/src/livesolid.egg-info/PKG-INFO` & `livesolid-0.0.8/src/livesolid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livesolid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Taylor Monacelli
 Author-email: taylormonacelli@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `livesolid-0.0.7/src/livesolid.egg-info/SOURCES.txt` & `livesolid-0.0.8/src/livesolid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/tests/test_skeleton.py` & `livesolid-0.0.8/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `livesolid-0.0.7/tox.ini` & `livesolid-0.0.8/tox.ini`

 * *Files identical despite different names*

