# Comparing `tmp/vale-2.25.2.0.tar.gz` & `tmp/vale-2.26.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/.tmp-o0wx8oq6/vale-2.25.2.0.tar", last modified: Fri May 12 21:30:56 2023, max compression
+gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/.tmp-id8up31_/vale-2.26.0.0.tar", last modified: Fri May 12 21:28:23 2023, max compression
```

## Comparing `vale-2.25.2.0.tar` & `vale-2.26.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:30:56.000000 vale-2.25.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 21:30:43.000000 vale-2.25.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 21:30:43.000000 vale-2.25.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-12 21:30:56.000000 vale-2.25.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-12 21:30:43.000000 vale-2.25.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 21:30:43.000000 vale-2.25.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:30:56.000000 vale-2.25.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:30:43.000000 vale-2.25.2.0/vale/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5023 2023-05-12 21:30:43.000000 vale-2.25.2.0/vale/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-12 21:30:43.000000 vale-2.25.2.0/vale/vale_bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 21:30:56.000000 vale-2.25.2.0/vale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:23.000000 vale-2.26.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 21:28:13.000000 vale-2.26.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 21:28:13.000000 vale-2.26.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-12 21:28:23.000000 vale-2.26.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-12 21:28:13.000000 vale-2.26.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 21:28:13.000000 vale-2.26.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:28:23.000000 vale-2.26.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:28:13.000000 vale-2.26.0.0/vale/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5023 2023-05-12 21:28:13.000000 vale-2.26.0.0/vale/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-12 21:28:13.000000 vale-2.26.0.0/vale/vale_bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 21:28:23.000000 vale-2.26.0.0/vale.egg-info/top_level.txt
```

### Comparing `vale-2.25.2.0/LICENSE` & `vale-2.26.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vale-2.25.2.0/PKG-INFO` & `vale-2.26.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 2.25.2.0
+Version: 2.26.0.0
 Summary: Install and use Vale (grammar & style check tool) in python environments.
 Author: Dani Perez
 License: MIT
 Project-URL: Homepage, https://github.com/daniperez/vale-python-package
 Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,18 @@
 
 # Releasing (only for contributors)
 1. Change version in `pyproject.toml`. Changing the version changes the
    version of Vale that gets downloaded. See note below.
 2. Commit & push.
 3. Github's Actions will deal with the new release.
 
+Note: you can create as many commits as versions (one commit by version).
+Every commit will be tested individually and published to PyPi if it's
+not already the case.
+
 Note: Pypi doesn't allow to re-release (even if releases or projects are
 deleted). If you want to release this package for a new version of Vale, just
 update the `version` attribute found in `pyproject.toml` so that it matches the
 version of Vale that you want to release. If something needs to be fixed in
 this package, use or increase the 4th number in the version in
 `pyproject.toml`.  The 4th number will be ignored when it comes to downloading
 Vale but will be used to release the package to PyPi.. For example, if you use
```

### Comparing `vale-2.25.2.0/README.md` & `vale-2.26.0.0/vale.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: vale
+Version: 2.26.0.0
+Summary: Install and use Vale (grammar & style check tool) in python environments.
+Author: Dani Perez
+License: MIT
+Project-URL: Homepage, https://github.com/daniperez/vale-python-package
+Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Package Release](https://github.com/daniperez/vale-python-package/actions/workflows/python-publish.yml/badge.svg)](https://github.com/daniperez/vale-python-package/actions/workflows/python-publish.yml)
 
 # Vale Python Package
 
 > ⚠️  Vale is a software developed by errata.ai and a community of open-source
 > contributors. This repository just makes that software available to Python
 > users. The author is not affiliated nor endorsed by errata.ai.
@@ -28,14 +43,18 @@
 
 # Releasing (only for contributors)
 1. Change version in `pyproject.toml`. Changing the version changes the
    version of Vale that gets downloaded. See note below.
 2. Commit & push.
 3. Github's Actions will deal with the new release.
 
+Note: you can create as many commits as versions (one commit by version).
+Every commit will be tested individually and published to PyPi if it's
+not already the case.
+
 Note: Pypi doesn't allow to re-release (even if releases or projects are
 deleted). If you want to release this package for a new version of Vale, just
 update the `version` attribute found in `pyproject.toml` so that it matches the
 version of Vale that you want to release. If something needs to be fixed in
 this package, use or increase the 4th number in the version in
 `pyproject.toml`.  The 4th number will be ignored when it comes to downloading
 Vale but will be used to release the package to PyPi.. For example, if you use
```

### Comparing `vale-2.25.2.0/pyproject.toml` & `vale-2.26.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [project]
 name="vale"
 # This version corresponds to the original Vale's version, plus a 4th number to
 # account for fixes to this package. That 4th number is needed because PyPi
 # doesn't allow to re-release or upload deleted versions, every uploaded
 # version must be unique.
-version = "2.25.2.0"
+version = "2.26.0.0"
 authors = [
   { name="Dani Perez"},
 ]
 description = "Install and use Vale (grammar & style check tool) in python environments."
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
```

### Comparing `vale-2.25.2.0/vale/main.py` & `vale-2.26.0.0/vale/main.py`

 * *Files identical despite different names*

### Comparing `vale-2.25.2.0/vale.egg-info/PKG-INFO` & `vale-2.26.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: vale
-Version: 2.25.2.0
-Summary: Install and use Vale (grammar & style check tool) in python environments.
-Author: Dani Perez
-License: MIT
-Project-URL: Homepage, https://github.com/daniperez/vale-python-package
-Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Package Release](https://github.com/daniperez/vale-python-package/actions/workflows/python-publish.yml/badge.svg)](https://github.com/daniperez/vale-python-package/actions/workflows/python-publish.yml)
 
 # Vale Python Package
 
 > ⚠️  Vale is a software developed by errata.ai and a community of open-source
 > contributors. This repository just makes that software available to Python
 > users. The author is not affiliated nor endorsed by errata.ai.
@@ -43,14 +28,18 @@
 
 # Releasing (only for contributors)
 1. Change version in `pyproject.toml`. Changing the version changes the
    version of Vale that gets downloaded. See note below.
 2. Commit & push.
 3. Github's Actions will deal with the new release.
 
+Note: you can create as many commits as versions (one commit by version).
+Every commit will be tested individually and published to PyPi if it's
+not already the case.
+
 Note: Pypi doesn't allow to re-release (even if releases or projects are
 deleted). If you want to release this package for a new version of Vale, just
 update the `version` attribute found in `pyproject.toml` so that it matches the
 version of Vale that you want to release. If something needs to be fixed in
 this package, use or increase the 4th number in the version in
 `pyproject.toml`.  The 4th number will be ignored when it comes to downloading
 Vale but will be used to release the package to PyPi.. For example, if you use
```

