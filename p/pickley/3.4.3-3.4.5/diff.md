# Comparing `tmp/pickley-3.4.3.tar.gz` & `tmp/pickley-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickley-3.4.3.tar", last modified: Wed May  3 18:49:49 2023, max compression
+gzip compressed data, was "pickley-3.4.5.tar", last modified: Thu May 11 23:00:46 2023, max compression
```

## Comparing `pickley-3.4.3.tar` & `pickley-3.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 18:48:04.000000 pickley-3.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 18:48:04.000000 pickley-3.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:49:49.117702 pickley-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-03 18:48:04.000000 pickley-3.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-03 18:48:04.000000 pickley-3.4.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:48:04.000000 pickley-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:49:49.117702 pickley-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-03 18:48:04.000000 pickley-3.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.113702 pickley-3.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.113702 pickley-3.4.3/src/pickley/
--rw-r--r--   0 runner    (1001) docker     (123)    36403 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/bstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30237 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-03 18:48:04.000000 pickley-3.4.3/src/pickley/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/src/pickley.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 18:49:49.000000 pickley-3.4.3/src/pickley.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:49:49.117702 pickley-3.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-03 18:48:04.000000 pickley-3.4.3/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.485475 pickley-3.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-11 22:58:55.000000 pickley-3.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 22:58:55.000000 pickley-3.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-11 23:00:46.485475 pickley-3.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-11 22:58:55.000000 pickley-3.4.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-11 22:58:55.000000 pickley-3.4.5/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 22:58:55.000000 pickley-3.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 23:00:46.485475 pickley-3.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-11 22:58:55.000000 pickley-3.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/pickley/
+-rw-r--r--   0 runner    (1001) docker     (123)    36403 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/bstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30237 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-11 22:58:55.000000 pickley-3.4.5/src/pickley/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.481475 pickley-3.4.5/src/pickley.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 23:00:46.000000 pickley-3.4.5/src/pickley.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 23:00:46.485475 pickley-3.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-11 22:58:55.000000 pickley-3.4.5/tests/test_venv.py
```

### Comparing `pickley-3.4.3/LICENSE` & `pickley-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/PKG-INFO` & `pickley-3.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.3
+Version: 3.4.5
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.4.3/README.rst` & `pickley-3.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/setup.py` & `pickley-3.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/src/pickley/__init__.py` & `pickley-3.4.5/src/pickley/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 from datetime import datetime
 
 import runez
 from runez.pyenv import PypiStd, PythonDepot, PythonInstallationScanner, Version
 
 
-__version__ = "3.4.3"
+__version__ = "3.4.5"
 LOG = logging.getLogger(__name__)
 PICKLEY = "pickley"
 DOT_META = ".pickley"
 K_CLI = {"delivery", "index", "python"}
 K_DIRECTIVES = {"include"}
 K_GROUPS = {"bundle", "pinned"}
 K_LEAVES = {
```

### Comparing `pickley-3.4.3/src/pickley/bstrap.py` & `pickley-3.4.5/src/pickley/bstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,16 @@
 
     Returns:
         (str | None): Pinned pip version to use, if applicable
     """
     if python_version and python_version < (3, 7):
         return "21.3.1"
 
+    return "22.2.2"  # TODO: pip started looking for <whl>.metadata all of the sudden... what the heck?
+
 
 def create_virtualenv(tmp_folder, python_version, python_exe, venv_folder, virtualenv_version="20.10.0", runner=None, dryrun=None):
     """
     Args:
         tmp_folder (str): Temp folder to use, virtualenv.pyz is downloaded there
         python_version (tuple): Target python version
         python_exe (str): Target python executable
```

### Comparing `pickley-3.4.3/src/pickley/cli.py` & `pickley-3.4.5/src/pickley/cli.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/src/pickley/delivery.py` & `pickley-3.4.5/src/pickley/delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/src/pickley/package.py` & `pickley-3.4.5/src/pickley/package.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/src/pickley.egg-info/PKG-INFO` & `pickley-3.4.5/src/pickley.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickley
-Version: 3.4.3
+Version: 3.4.5
 Summary: Automate installation of standalone python CLIs
 Home-page: https://github.com/codrsquad/pickley
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/pickley/wiki
 Project-URL: Release notes, https://github.com/codrsquad/pickley/wiki/Release-notes
```

### Comparing `pickley-3.4.3/src/pickley.egg-info/SOURCES.txt` & `pickley-3.4.5/src/pickley.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/tests/test_bootstrap.py` & `pickley-3.4.5/tests/test_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             with patch("pickley.bstrap.built_in_download"):
                 with patch("pickley.bstrap.get_python_version", return_value=(3, 10)):
                     with patch("pickley.bstrap.run_program", side_effect=mocked_logged_run):
                         # Verify that a python without ensurepip still works (via virtualenv)
                         cli.run("1.0", main=bstrap.main)
                         assert cli.succeeded
                         assert " -mvenv --clear " in cli.logged
-                        assert "virtualenv-20.10.0.pyz -q --clear --download -p " in cli.logged
+                        assert "virtualenv-20.10.0.pyz -q --clear --pip 22.2.2 -p " in cli.logged
 
                         # When pip available, don't use virtualenv
                         pip = ".local/bin/.pickley/pickley/pickley-1.0/bin/pip3"
                         runez.touch(pip)
                         runez.make_executable(pip)
                         cli.run("1.0", main=bstrap.main)
                         assert cli.succeeded
@@ -103,15 +103,15 @@
 
 
 def test_edge_cases(temp_folder, monkeypatch, logged):
     monkeypatch.setattr(bstrap, "DRYRUN", True)
     cmd = bstrap.virtualenv_cmd("vv", (3, 6), "pyexe", "venv")
     assert cmd == [sys.executable, "vv", "-q", "--clear", "--pip", "21.3.1", "-p", "pyexe", "venv"]
     cmd = bstrap.virtualenv_cmd("vv", (3, 7), "pyexe", "venv")
-    assert cmd == [sys.executable, "vv", "-q", "--clear", "--download", "-p", "pyexe", "venv"]
+    assert cmd == [sys.executable, "vv", "-q", "--clear", "--pip", "22.2.2", "-p", "pyexe", "venv"]
 
     monkeypatch.setattr(bstrap, "DRYRUN", False)
     assert bstrap.which("python3")  # Check that which() works
 
     monkeypatch.setattr(bstrap, "RUNNING_FROM_VENV", False)
     assert bstrap.find_python3() == sys.executable
```

### Comparing `pickley-3.4.3/tests/test_config.py` & `pickley-3.4.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/tests/test_delivery.py` & `pickley-3.4.5/tests/test_delivery.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/tests/test_ops.py` & `pickley-3.4.5/tests/test_ops.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/tests/test_run.py` & `pickley-3.4.5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pickley-3.4.3/tests/test_venv.py` & `pickley-3.4.5/tests/test_venv.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     runez.touch(".pickley/.cache/virtualenv-20.13.0.pyz")
     with patch("runez.run", return_value=runez.program.RunResult(code=0)):
         cmd = venv._create_virtualenv(runner=lambda *x: x)
         if temp_cfg.available_pythons.invoker.version < "3.7":
             assert cmd[4] == "--pip"
 
         else:
-            assert cmd[4] == "--download"
+            assert cmd[4] == "--pip"
 
 
 def simulated_run(*args, **_):
     if "ansible-core" in args:
         return runez.program.RunResult(PIP_SHOW_OUTPUT, code=0)
 
     if "no-location" in args:
```

