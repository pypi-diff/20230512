# Comparing `tmp/vale-2.24.4.0.tar.gz` & `tmp/vale-2.25.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/.tmp-eoylvro7/vale-2.24.4.0.tar", last modified: Tue Apr 25 12:06:00 2023, max compression
+gzip compressed data, was "/home/runner/work/vale-python-package/vale-python-package/dist/.tmp-q0y3qhft/vale-2.25.0.0.tar", last modified: Fri May 12 21:27:19 2023, max compression
```

## Comparing `vale-2.24.4.0.tar` & `vale-2.25.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:06:00.000000 vale-2.24.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 12:05:48.000000 vale-2.24.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 12:05:48.000000 vale-2.24.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-25 12:06:00.000000 vale-2.24.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-25 12:05:48.000000 vale-2.24.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-25 12:05:48.000000 vale-2.24.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 12:06:00.000000 vale-2.24.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:05:48.000000 vale-2.24.4.0/vale/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4296 2023-04-25 12:05:48.000000 vale-2.24.4.0/vale/main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-04-25 12:05:48.000000 vale-2.24.4.0/vale/vale_bin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 12:06:00.000000 vale-2.24.4.0/vale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:27:19.000000 vale-2.25.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-12 21:27:07.000000 vale-2.25.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 21:27:07.000000 vale-2.25.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-12 21:27:19.000000 vale-2.25.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-12 21:27:07.000000 vale-2.25.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 21:27:07.000000 vale-2.25.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:27:19.000000 vale-2.25.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:27:07.000000 vale-2.25.0.0/vale/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5023 2023-05-12 21:27:07.000000 vale-2.25.0.0/vale/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-12 21:27:07.000000 vale-2.25.0.0/vale/vale_bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 21:27:19.000000 vale-2.25.0.0/vale.egg-info/top_level.txt
```

### Comparing `vale-2.24.4.0/LICENSE` & `vale-2.25.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vale-2.24.4.0/PKG-INFO` & `vale-2.25.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 2.24.4.0
+Version: 2.25.0.0
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

### Comparing `vale-2.24.4.0/README.md` & `vale-2.25.0.0/vale.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: vale
+Version: 2.25.0.0
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

### Comparing `vale-2.24.4.0/pyproject.toml` & `vale-2.25.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [project]
 name="vale"
 # This version corresponds to the original Vale's version, plus a 4th number to
 # account for fixes to this package. That 4th number is needed because PyPi
 # doesn't allow to re-release or upload deleted versions, every uploaded
 # version must be unique.
-version = "2.24.4.0"
+version = "2.25.0.0"
 authors = [
   { name="Dani Perez"},
 ]
 description = "Install and use Vale (grammar & style check tool) in python environments."
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
```

### Comparing `vale-2.24.4.0/vale/main.py` & `vale-2.25.0.0/vale/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 """Downloads Vale if not downloaded yet and executes it."""
 
 import os
+import platform
 import shutil
+import subprocess
 import sys
 import tarfile
 import tempfile
 import zipfile
 from functools import partial
 from pathlib import Path
 from typing import Optional
@@ -17,15 +19,15 @@
 if sys.version_info >= (3, 8):
     import importlib.metadata as importlib_metadata
 else:
     import importlib_metadata
 
 
 def major_minor_patch(version: str) -> str:
-    """E.g.: 2.20.0.1 -> 2.20.0 ."""
+    """E.g.: 2.20.0.1 -> 2.20.0 """
     return ".".join(version.split(".")[0:3])
 
 
 # We download the Vale version corresponding to this Python package's version
 # (see pyproject.toml) up to major, minor and patch (3 numbers). This Python
 # package uses a 4th number to account for fixes to this package, which will be
 # ignored here. That 4th number is needed because PyPi doesn't allow to
@@ -41,15 +43,18 @@
     if sys.platform.startswith("linux"):
         operating_system = "Linux"
     elif sys.platform.startswith("darwin"):
         operating_system = "macOS"
     elif sys.platform.startswith("win32"):
         operating_system = "Windows"
 
-    if os.uname().machine.startswith("x86_64"):
+    if operating_system == "Windows":
+        convert_arch = {"32bit": "32-bit", "64bit": "64-bit"}
+        architecture = convert_arch.get(platform.architecture()[0], None)
+    elif os.uname().machine.startswith("x86_64"):
         architecture = "64-bit"
     elif os.uname().machine.startswith("arm"):
         # This is a loose match. Theoretical valid values:
         # aarch64_be, aarch64, armv8b, armv8, larm64.
         # I need confirmation.
         architecture = "arm64"
 
@@ -65,69 +70,83 @@
         extension = "zip"
     else:
         extension = "tar.gz"
 
     return operating_system, architecture, extension
 
 
-def extract_vale(archive: str, archive_type: str, destination: str) -> str:
+def extract_vale(
+    archive: str, archive_type: str, destination: str, bin_name: str = "vale"
+) -> str:
     """Extract `vale` binary from the given archive."""
     if archive_type == "zip":
-        archiver = zipfile.ZipFile(archive)
+        archiver = zipfile.ZipFile
     elif archive_type == "tar.gz":
         archiver = partial(tarfile.open, mode="r:gz")
     else:
         raise ValueError(f"Archive type '{archive_type}' is not supported. "
                          "Only 'zip' and 'tar.gz' supported.")
 
     with archiver(archive) as archive_volume:
         archive_volume.extractall(destination)
 
-    vale_tmp_path = Path(destination) / "vale"
+    vale_tmp_path = Path(destination) / bin_name
 
     assert (vale_tmp_path.exists())
 
     return f"{vale_tmp_path}"
 
 
 def download_vale_if_missing() -> str:
     """Download vale only if missing."""
     vale_bin_path = Path(vale.__file__).parent / "vale_bin"
 
-    # See vale/vale_bin (in repo, not in its installed form) for an explanation
-    # of this magic number of bytes.
+    # We have a dummy vale placeholder that is overwritten by the downloaded vale version.
+    # See `vale/vale_bin` (in this repo, not in its installed form) for more details about
+    # this magic number of bytes.
     if vale_bin_path.stat().st_size < 1000:
 
         print("* vale not found. Downloading it...")
 
         operating_system, architecture, extension = get_target()
 
-        url = ("https://github.com/errata-ai/vale/releases/download"
-               f"/v{vale_bin_version}/"
-               f"vale_{vale_bin_version}_{operating_system}_{architecture}"
-               f".{extension}")
+        url_str = (
+            "https://github.com/errata-ai/vale/releases/download"
+            f"/v{vale_bin_version}/"
+            f"vale_{vale_bin_version}_{operating_system}_{architecture}"
+            f".{extension}"
+        )
 
-        url = urlopen(url)
+        url = urlopen(url_str)
 
-        with tempfile.NamedTemporaryFile(mode="w+b") as tp:
+        # delete=False is required to avoid permissions errors on windows
+        with tempfile.NamedTemporaryFile(mode="w+b", delete=False) as tp:
 
             tp.write(url.read())
 
-            print(f"* {url} downloaded to {tp.name}")
+            print(f"* {url_str} downloaded to {tp.name}")
 
             with tempfile.TemporaryDirectory() as td:
 
-                vale_tmp_path = extract_vale(tp.name, extension, td)
+                archive_bin_name = "vale.exe" if operating_system == "Windows" else "vale"
+                vale_tmp_path = extract_vale(tp.name, extension, td, archive_bin_name)
 
                 print(f"* Copying {vale_tmp_path} to {vale_bin_path}")
                 shutil.copy(f"{vale_tmp_path}", f"{vale_bin_path}")
 
+        # clean up the temp file if it still exists
+        try:
+            os.unlink(tp.name)
+        except Exception:
+            pass
+
         print("* vale extracted and copied to module path.")
 
     return f"{vale_bin_path}"
 
 
 def main():
     """Download vale if not downloaded and executes it."""
     vale_bin_path = download_vale_if_missing()
 
-    os.execvp(f"{vale_bin_path}", ["vale"] + sys.argv[1:])
+    proc = subprocess.run([f"{vale_bin_path}"] + sys.argv[1:])
+    sys.exit(proc.returncode)
```

### Comparing `vale-2.24.4.0/vale.egg-info/PKG-INFO` & `vale-2.25.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: vale
-Version: 2.24.4.0
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

