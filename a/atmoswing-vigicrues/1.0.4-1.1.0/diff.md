# Comparing `tmp/atmoswing-vigicrues-1.0.4.tar.gz` & `tmp/atmoswing-vigicrues-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.0.4.tar", last modified: Wed May 10 12:17:38 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.0.tar", last modified: Fri May 12 15:15:38 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.0.4.tar` & `atmoswing-vigicrues-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.822834 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 12:17:38.000000 atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:17:38.826834 atmoswing-vigicrues-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 12:17:19.000000 atmoswing-vigicrues-1.0.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.492329 atmoswing-vigicrues-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.496329 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 15:15:38.000000 atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:15:38.500329 atmoswing-vigicrues-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 15:15:19.000000 atmoswing-vigicrues-1.1.0/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.0.4/LICENSE` & `atmoswing-vigicrues-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/pyproject.toml` & `atmoswing-vigicrues-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.0.4"
+version = "1.1.0"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,25 @@
     import eccodes
 except ImportError:
     has_eccodes = False
 else:
     has_eccodes = True
 
 from .controller import Controller
-from .options import Options
+from .disseminations.transfer_sftp_out import TransferSftpOut
 from .exceptions import (ConfigError, Error, FilePathError, OptionError,
                          PathError)
+from .options import Options
+from .postactions.export_bdapbp import ExportBdApBp
+from .postactions.export_prv import ExportPrv
 from .preactions.download_gfs import DownloadGfsData
 from .preactions.transfer_sftp_in import TransferSftpIn
-from .preactions.transform_gfs import TransformGfsData
 from .preactions.transform_ecmwf import TransformEcmwfData
-from .postactions.export_bdapbp import ExportBdApBp
-from .postactions.export_prv import ExportPrv
-from .disseminations.transfer_sftp_out import TransferSftpOut
-from .utils import file_exists, check_dir_exists, check_file_exists, \
-    build_date_dir_structure
-
+from .preactions.transform_gfs import TransformGfsData
+from .utils import (build_date_dir_structure, check_dir_exists,
+                    check_file_exists, file_exists)
 
 __all__ = ('Error', 'OptionError', 'ConfigError', 'PathError', 'FilePathError',
            'Controller', 'Options', 'ExportBdApBp', 'ExportPrv', 'TransferSftpOut',
            'DownloadGfsData', 'TransformGfsData', 'TransformEcmwfData', 'file_exists',
            'check_file_exists', 'check_dir_exists', 'build_date_dir_structure',
            'Dataset', 'eccodes', 'TransferSftpIn')
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import argparse
 from datetime import datetime
 
 from atmoswing_vigicrues.controller import Controller
 
 
-def main() -> int:
+def main(args=None) -> int:
     parser = argparse.ArgumentParser(
         description="Traite les prévisions et les exportations d'AtmoSwing pour "
                     "le réseau Vigicrues.")
     parser.add_argument(
-        '--config-file', type=str, required=False,
+        '-c', '--config-file', type=str, required=False,
         help="Fichier de configuration du présent module.")
     parser.add_argument(
-        '--date', type=str, required=False,
+        '-d', '--date', type=str, required=False,
         help="Date pour laquelle émettre une prévision (YYYYMMDDHH).")
 
-    args = parser.parse_args()
+    args = parser.parse_args(args)
 
     controller = Controller(args)
 
     if args.date:
         date = datetime.strptime(args.date, '%Y%m%d%H')
         return controller.run(date)
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Attributes
     ----------
     options : object
         Options de la prévision combinant les arguments passés lors de l'utilisation en
         lignes de commandes et les options du fichier de configuration.
     verbose : bool
         Affichage verbose des messages d'erreurs (pas beaucoup utilisé)
-    date : datetime
+    date : datetime.datetime
         Date de la prévision.
     """
 
     def __init__(self, cli_options):
         """
         Initialisation de l'instance Controller
 
@@ -29,28 +29,29 @@
         ----------
         cli_options : object
             Options passées en lignes de commandes à la fonction main()
         """
         self.options = asv.Options(cli_options)
         self.time_increment = 6
         self.date = datetime.datetime.utcnow()
+        self.existing_files = []
         self.pre_actions = []
         self.post_actions = []
         self.disseminations = []
         self._register_pre_actions()
         self._register_post_actions()
         self._register_disseminations()
 
     def run(self, date=None) -> int:
         """
         Exécution du flux de la prévision et du postprocessing.
 
         Parameters
         ----------
-        date : datetime
+        date : datetime.datetime
             La date de la prévision (par défaut, la date actuelle est utilisée).
 
         Returns
         -------
         int
             Le code de retour (0 en cas de succès)
         """
@@ -58,14 +59,15 @@
         if date:
             self.date = date
 
         self._fix_date()
 
         try:
             self._run_pre_actions()
+            self.existing_files = self._list_atmoswing_output_files()
             self._run_atmoswing()
             self._run_post_actions()
             self._run_disseminations()
         except asv.Error as e:
             print("La prévision a échoué.")
             print(f"Erreur: {e}")
             return -1
@@ -143,45 +145,50 @@
             for action in self.pre_actions:
                 print(f"Exécution de : '{action.type_name}' [{action.name}]")
                 if not action.run(self.date):
                     attempts_hours += attempts_step_hours
                     success = False
                     break
             if success:
-                print("  -> Exécution correcte")
+                print("  -> Exécution correcte.")
                 break
             else:
-                print("  -> Recul de l'heure de la prévision")
+                print("  -> Recul de l'heure de la prévision.")
                 self._back_in_time(attempts_step_hours)
         else:
-            print("  -> Échec de l'exécution")
-            raise asv.Error("Nombre maximum de tentatives atteint pour la pré-action.")
+            print("  -> Échec de l'exécution.")
+            print("  -> Nombre maximum de tentatives atteint pour la pré-action.")
 
     def _run_atmoswing(self):
         """
         Exécution d'AtmoSwing.
         """
         run = self.options.get('atmoswing')
+        if 'active' in run and run['active'] is False:
+            print("  -> Prévision par AtmoSwing Forecaster désactivée.")
+            return True
+
         name = run['name']
         options = run['with']
         cmd = self._build_atmoswing_cmd(options)
         print(f"Exécution de : '{name}'")
         print(f"Prévision pour la date : {self.date.strftime('%Y-%m-%d %H')}")
         print("Commande: " + ' '.join(cmd))
 
         try:
             ret = subprocess.run(cmd, capture_output=True, check=True)
 
             if ret.returncode != 0:
-                print("  -> Échec de l'exécution")
+                print("  -> Échec de l'exécution.")
+                raise asv.Error("Erreur de AtmoSwing Forecaster.")
             else:
-                print("  -> Exécution correcte")
+                print("  -> Exécution correcte.")
         except Exception as e:
-            print("  -> Échec de l'exécution")
-            print(f"Exception lors de l'exécution d'AtmoSwing Forecaster: {e}")
+            print("  -> Échec de l'exécution.")
+            raise asv.Error(f"Exception de AtmoSwing Forecaster: {e}")
 
     def _build_atmoswing_cmd(self, options):
         now_str = self.date.strftime("%Y%m%d%H")
         cmd = []
 
         if 'atmoswing_path' not in options or not options['atmoswing_path']:
             cmd.append("atmoswing-forecaster")
@@ -219,22 +226,28 @@
     def _run_post_actions(self):
         """
         Exécute les opérations postérieures à la prévision par AtmoSwing.
         """
         if not self.post_actions or len(self.post_actions) == 0:
             return
 
-        files = self._list_atmoswing_output_files()
+        files = self._get_files_for_post_actions()
+        if len(files) == 0:
+            print("  -> Aucun nouveau fichier à traiter en post-action.")
+            return
+
+        print(f"  -> {len(files)} nouveaux fichier à traiter en post-action.")
+
         for action in self.post_actions:
             print(f"Exécution de : '{action.type_name}' [{action.name}]")
             action.feed(files, {'forecast_date': self.date})
             if action.run():
-                print("  -> Exécution correcte")
+                print("  -> Exécution correcte.")
             else:
-                print("  -> Échec de l'exécution")
+                print("  -> Échec de l'exécution.")
 
     def _run_disseminations(self):
         """
         Exécute les opérations de diffusion.
         """
         if not self.disseminations or len(self.disseminations) == 0:
             return
@@ -242,17 +255,17 @@
         for action in self.disseminations:
             print(f"Exécution de : '{action.type_name}' [{action.name}]")
             local_dir = action.local_dir
             extension = action.extension
             files = self._list_files(local_dir, extension)
             action.feed(files)
             if action.run(self.date):
-                print("  -> Exécution correcte")
+                print("  -> Exécution correcte.")
             else:
-                print("  -> Échec de l'exécution")
+                print("  -> Échec de l'exécution.")
 
     def _fix_date(self):
         date = self.date
         if isinstance(date, str):
             date = datetime.datetime.strptime(date, "%Y-%m-%d %H")
         hour = date.hour
         hour = self.time_increment * (hour // self.time_increment)
@@ -261,12 +274,17 @@
     def _back_in_time(self, time_increment):
         self.date = self.date - datetime.timedelta(hours=time_increment)
 
     def _list_atmoswing_output_files(self):
         output_dir = self.options.get('atmoswing')['with']['output_dir']
         return self._list_files(output_dir, '.nc', '%Y-%m-%d_%H')
 
+    def _get_files_for_post_actions(self):
+        files = self._list_atmoswing_output_files()
+        files = [x for x in files if x not in self.existing_files]
+        return files
+
     def _list_files(self, local_dir, ext, pattern='%Y-%m-%d_%H'):
         local_dir = asv.utils.build_date_dir_structure(local_dir, self.date)
         pattern = f"{str(local_dir)}/{self.date.strftime(pattern)}{f'.*{ext}'}"
         files = glob.glob(pattern)
         return files
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,11 +19,11 @@
 
     def run(self, date) -> bool:
         """
         Exécution de la diffusion.
 
         Parameters
         ----------
-        date : datetime
+        date : datetime.datetime
             Date de la prévision.
         """
         raise NotImplementedError
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 import paramiko
-import socks
 
 import atmoswing_vigicrues as asv
 
 from .dissemination import Dissemination
 
 
 class TransferSftpOut(Dissemination):
@@ -44,76 +43,76 @@
         Initialisation de l'instance TransferSftp
         """
         self.type_name = "Transfert SFTP"
         self.name = name
         self.local_dir = options['local_dir']
         self.extension = options['extension']
         self.hostname = options['hostname']
-        self.port = options['port']
+        self.port = int(options['port'])
         self.username = options['username']
         self.password = options['password']
         self.remote_dir = options['remote_dir']
 
-        if 'proxy_host' in options:
+        if 'proxy_host' in options and len(options['proxy_host']) > 0:
             self.proxy_host = options['proxy_host']
-            if 'proxy_port' in options:
-                self.proxy_port = options['proxy_port']
+            if 'proxy_port' in options and len(options['proxy_port']) > 0:
+                self.proxy_port = int(options['proxy_port'])
             else:
                 self.proxy_port = 1080
         else:
             self.proxy_host = None
 
         super().__init__()
 
     def run(self, date) -> bool:
         """
         Exécution de la diffusion par SFTP.
 
         Parameters
         ----------
-        date : datetime
+        date : datetime.datetime
             Date de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
-            print("Aucun fichier à traiter")
+            print("  -> Aucun fichier à traiter")
             return False
 
         try:
+            # Create a transport object for the SFTP connection
+            transport = paramiko.Transport((self.hostname, self.port))
+
             if self.proxy_host:
-                sock = socks.socksocket()
-                sock.set_proxy(
-                    proxy_type=socks.SOCKS5,
-                    addr=self.proxy_host,
-                    port=self.proxy_port
-                )
-                sock.connect((self.hostname, self.port))
-                transport = paramiko.Transport(sock)
-            else:
-                transport = paramiko.Transport((self.hostname, self.port))
+                transport.start_client()
+                transport.open_channel('direct-tcpip',
+                                       (self.hostname, self.port),
+                                       (self.proxy_host, self.proxy_port))
+
+            # Authenticate with the SFTP server
+            transport.connect(username=self.username, password=self.password)
+
+            # Create an SFTP client object
+            sftp = transport.open_sftp_client()
 
-            transport.connect(None, self.username, self.password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
             self._chdir_or_mkdir(self.remote_dir, sftp)
             self._chdir_or_mkdir(date.strftime('%Y'), sftp)
             self._chdir_or_mkdir(date.strftime('%m'), sftp)
             self._chdir_or_mkdir(date.strftime('%d'), sftp)
 
             for file in self._file_paths:
                 filename = os.path.basename(file)
                 asv.check_file_exists(file)
                 sftp.put(file, filename)
 
-            if sftp:
-                sftp.close()
-            if transport:
-                transport.close()
+            # Close the SFTP client and transport objects
+            sftp.close()
+            transport.close()
 
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
             return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
             return False
@@ -138,10 +137,10 @@
 
         return True
 
     @staticmethod
     def _chdir_or_mkdir(dir_path, sftp):
         try:
             sftp.chdir(dir_path)
-        except IOError:
+        except OSError:
             sftp.mkdir(dir_path)
             sftp.chdir(dir_path)
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import json
 import datetime
-import numpy as np
+import json
 from pathlib import Path
 
+import numpy as np
+
 import atmoswing_vigicrues as asv
 
 from .postaction import PostAction
 
 
 class ExportBdApBp(PostAction):
     """
@@ -72,37 +73,37 @@
         * 200 : Erreur lors du traitement fichier netcdf.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
-            print("Aucun fichier à traiter")
+            print("  -> Aucun fichier à traiter")
             return False
 
         for file in self._file_paths:
             file = Path(file)
             self._reset_status()
             nc_file = None
 
             if not asv.file_exists(file):
                 self.status = 100
                 self.message = "Absence du fichier netcdf."
             else:
                 try:
                     nc_file = asv.Dataset(file, 'r', format='NETCDF4')
-                except:
+                except Exception:
                     self.status = 110
                     self.message = "Fichier netcdf corrompu."
 
             try:
                 metadata = self._create_metadata_block(nc_file)
                 data = self._create_data_block(nc_file)
                 statistics = self._create_statistics_block(nc_file)
-            except:
+            except Exception:
                 metadata = None
                 data = None
                 statistics = None
                 self.status = 200
                 self.message = "Erreur lors du traitement fichier netcdf."
 
             exported_analogs = "full"
@@ -111,15 +112,16 @@
 
             data = {
                 'status': self.status,
                 'report': {
                     'file': file.name,
                     'date': self._get_now_formatted(),
                     'message': self.message,
-                    'exported_analogs': exported_analogs
+                    'exported_analogs': exported_analogs,
+                    'only_relevant_stations': self.only_relevant_stations
                 },
                 'metadata': metadata,
                 'data': data,
                 'statistics': statistics,
             }
 
             # Nom du fichier
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
-import numpy as np
 from pathlib import Path
 
+import numpy as np
+
 import atmoswing_vigicrues as asv
 
 from .postaction import PostAction
 
 
 class ExportPrv(PostAction):
     """
@@ -16,14 +17,16 @@
     name: str
         Le nom de l'action
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * output_dir : str
             Chemin cible pour l'enregistrement des fichiers.
+        * date_format : str
+            Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
         * frequencies : list
             Les fréquences à extraire.
             Par défaut : [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
         * combine_stations_in_one_file : bool
             Combinaison des différentes stations (entités) dans un seul fichier.
     """
 
@@ -32,14 +35,19 @@
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
 
         self.type_name = "Export PRV"
         self.name = name
         self.output_dir = options['output_dir']
         asv.check_dir_exists(self.output_dir, True)
 
+        if 'date_format' in options:
+            self.date_format = options['date_format']
+        else:
+            self.date_format = "%d-%m-%Y"
+
         if 'frequencies' in options:
             self.frequencies = options['frequencies']
         else:
             self.frequencies = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.95]
 
         if 'combine_stations_in_one_file' in options:
             self.combine_stations_in_one_file = options['combine_stations_in_one_file']
@@ -53,15 +61,15 @@
         Exécution de la post-action.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         if not self._file_paths:
-            print("Aucun fichier à traiter")
+            print("  -> Aucun fichier à traiter")
             return False
 
         for file in self._file_paths:
             nc_file = asv.Dataset(file, 'r', format='NETCDF4')
             station_ids = self._extract_station_ids(nc_file)
             header_comments = self._create_header_comments(nc_file)
             if self.combine_stations_in_one_file:
@@ -197,15 +205,14 @@
 
     def _build_id_series(self, nc_file):
         ids = ""
         for freq in self.frequencies:
             ids += f"{nc_file.method_id}.{nc_file.specific_tag}.{int(100 * freq):03d};"
         return ids
 
-    @staticmethod
-    def _get_time_format(target_dates):
+    def _get_time_format(self, target_dates):
         time_step = target_dates[1] - target_dates[0]
         show_hour = time_step < 24 * 3600
-        time_format_target = "%Y-%m-%d"
+        time_format_target = self.date_format
         if show_hour:
-            time_format_target = "%Y-%m-%d %H:%M"
+            time_format_target = self.date_format + " %H:%M"
         return time_format_target
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class PostAction:
     """
     Classe de base pour les opérations de traitement des résultats d'AtmoSwing.
     """
 
     def __init__(self):
         self._file_paths = []
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-import atmoswing_vigicrues as asv
 import datetime
+import re
+
 import requests
 
+import atmoswing_vigicrues as asv
+
 from .preaction import PreAction
 
+CLEAN_HTML = re.compile('<.*?>')
+
 
 class DownloadGfsData(PreAction):
     """
     Téléchargement des prévisions émises par GFS.
 
     Parameters
     ----------
@@ -105,43 +110,44 @@
 
     def run(self, date) -> bool:
         """
         Exécute l'action.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.download(date)
 
     def download(self, date) -> bool:
         """
         Télécharge les prévisions de GFS pour une date d'émission de la prévision.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         subregion = self._build_subregion_request()
         levels = self._build_levels_request()
         resol = self.resolution
         sub_product = 'pgrb2'
         if resol == '0p50':
             sub_product = 'pgrb2full'
 
+        files_count = 0
         for time_step_back in range(0, self.time_step_back):
             date_ref = date - datetime.timedelta(
                 hours=self.time_increment * time_step_back
             )
             for lead_time in range(0, self.lead_time_max + 1, 6):
                 lead_time_str = f'{lead_time:03d}'
 
@@ -166,29 +172,31 @@
 
                     try:
                         if self.proxies:
                             r = requests.get(url, proxies=self.proxies)
                         else:
                             r = requests.get(url)
                     except requests.exceptions.RequestException as e:
-                        print(e)
-                        print("Le téléchargement de GFS a échoué.")
+                        print(f"  -> {e}")
+                        print("  -> Le téléchargement de GFS a échoué.")
                         return False
                     except Exception:
-                        print("Le téléchargement de GFS a échoué.")
+                        print("  -> Le téléchargement de GFS a échoué.")
                         return False
 
                     if r.status_code == 200:
                         open(file_path, 'wb').write(r.content)
-                        break
+                        files_count += 1
                     else:
-                        # print(r.status_code)
-                        # print(r.text)
+                        clean_text = re.sub(CLEAN_HTML, '', r.text)
+                        print(f"  -> {clean_text}")
                         return False
 
+        print(f"  -> Nombre de fichiers téléchargés : {files_count}.")
+
         return True
 
     def _get_local_path(self, date):
         local_path = asv.build_date_dir_structure(self.output_dir, date)
         local_path.mkdir(parents=True, exist_ok=True)
         return local_path
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
 import fnmatch
-from pathlib import Path
+import os
 import tarfile
+from pathlib import Path
 
 import paramiko
-import socks
 
 import atmoswing_vigicrues as asv
 
 from .preaction import PreAction
 
 
 class TransferSftpIn(PreAction):
@@ -22,14 +21,16 @@
     options: objet
         L'instance contenant les options de l'action. Les champs possibles sont:
 
         * local_dir : str
             Répertoire cible pour l'enregistrement des fichiers.
         * prefix : str
             Prefix des fichiers à importer.
+        * variables : list (optionnel)
+            Liste des variables météorologiques à importer.
         * hostname : str
             Adresse du serveur distant.
         * port : int
             Port du serveur distant.
         * username : str
             Utilisateur ayant un accès au serveur.
         * password : str
@@ -51,73 +52,94 @@
         Initialisation de l'instance TransferSftp
         """
         self.type_name = "Transfert SFTP"
         self.name = name
         self.local_dir = options['local_dir']
         self.prefix = options['prefix']
         self.hostname = options['hostname']
-        self.port = options['port']
+        self.port = int(options['port'])
         self.username = options['username']
         self.password = options['password']
         self.remote_dir = options['remote_dir']
 
         self._set_attempts_attributes(options)
 
-        if 'proxy_host' in options:
+        if 'variables' in options and len(options['variables']) > 0:
+            self.variables = options['variables']
+        else:
+            self.variables = None
+
+        if 'proxy_host' in options and len(options['proxy_host']) > 0:
             self.proxy_host = options['proxy_host']
-            if 'proxy_port' in options:
-                self.proxy_port = options['proxy_port']
+            if 'proxy_port' in options and len(options['proxy_port']) > 0:
+                self.proxy_port = int(options['proxy_port'])
             else:
                 self.proxy_port = 1080
         else:
             self.proxy_host = None
 
         super().__init__()
 
     def run(self, date) -> bool:
         """
         Exécution de la récupération par SFTP.
 
         Parameters
         ----------
-        date : datetime
+        date : datetime.datetime
             Date de la prévision.
         """
         try:
+
+            # Check if files already in the local folder (only with defined variables)
+            if self.variables is not None:
+                if self._files_already_present(date):
+                    print("  -> Fichiers déjà présents localement.")
+                    return True
+
+            # Create a transport object for the SFTP connection
+            transport = paramiko.Transport((self.hostname, self.port))
+
             if self.proxy_host:
-                sock = socks.socksocket()
-                sock.set_proxy(
-                    proxy_type=socks.SOCKS5,
-                    addr=self.proxy_host,
-                    port=self.proxy_port
-                )
-                sock.connect((self.hostname, self.port))
-                transport = paramiko.Transport(sock)
-            else:
-                transport = paramiko.Transport((self.hostname, self.port))
+                transport.start_client()
+                transport.open_channel('direct-tcpip',
+                                       (self.hostname, self.port),
+                                       (self.proxy_host, self.proxy_port))
+
+            # Authenticate with the SFTP server
+            transport.connect(username=self.username, password=self.password)
 
-            transport.connect(None, self.username, self.password)
-            sftp = paramiko.SFTPClient.from_transport(transport)
+            # Create an SFTP client object
+            sftp = transport.open_sftp_client()
+
+            # Change the directory to the desired remote directory
             sftp.chdir(self.remote_dir)
 
+            # Download files
             local_path = Path(self._get_local_path(date))
             forecast_date = date.strftime("%Y%m%d")
-
             for remote_file in sftp.listdir('.'):
-                if fnmatch.fnmatch(remote_file, f'{self.prefix}*_{forecast_date}*.*'):
+                pattern = f'{self.prefix.lower()}*_{forecast_date}*.*'
+                if self.variables is not None:
+                    for variable in self.variables:
+                        pattern = f'{self.prefix.lower()}_{variable.lower()}' \
+                                  f'_{forecast_date}*.*'
+                        if fnmatch.fnmatch(remote_file.lower(), pattern):
+                            break
+
+                if fnmatch.fnmatch(remote_file.lower(), pattern):
                     local_file = local_path / remote_file
                     if local_file.exists():
                         continue
-                    sftp.get(remote_file, str(local_file))
+                    sftp.get(remote_file, str(local_file), prefetch=False)
                     self._unpack_if_needed(local_file, local_path)
 
-            if sftp:
-                sftp.close()
-            if transport:
-                transport.close()
+            # Close the SFTP client and transport objects
+            sftp.close()
+            transport.close()
 
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
             return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
             return False
@@ -142,23 +164,41 @@
 
         return True
 
     @staticmethod
     def _chdir_or_mkdir(dir_path, sftp):
         try:
             sftp.chdir(dir_path)
-        except IOError:
+        except OSError:
             sftp.mkdir(dir_path)
             sftp.chdir(dir_path)
 
     def _get_local_path(self, date):
         local_path = asv.build_date_dir_structure(self.local_dir, date)
         local_path.mkdir(parents=True, exist_ok=True)
         return local_path
 
+    def _files_already_present(self, date):
+        local_path = Path(self._get_local_path(date))
+        forecast_datetime = date.strftime("%Y%m%d%H")
+
+        for variable in self.variables:
+            pattern = f'{self.prefix.lower()}_{variable.lower()}' \
+                      f'_{forecast_datetime}*.*'
+            local_files = local_path.glob(pattern)
+            file_found = False
+            for local_file in local_files:
+                if fnmatch.fnmatch(str(local_file.name).lower(), pattern):
+                    file_found = True
+                    break
+            if not file_found:
+                return False
+
+        return True
+
     @staticmethod
     def _unpack_if_needed(local_file, local_path):
         if local_file.suffix in ['.gz', '.tgz', '.xz', '.txz', '.bz2',
                                  '.tbz', '.tbz2', '.tb2']:
             file = tarfile.open(local_file)
             for member in file.getmembers():
                 if member.isreg():
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,107 @@
 import atmoswing_vigicrues as asv
-from datetime import datetime
-#if asv.has_eccodes and asv.has_netcdf:
-#    from atmoswing_toolbox.datasets import generic, grib_dataset
-
 
 from .preaction import PreAction
 
+if asv.has_eccodes and asv.has_netcdf:
+    from atmoswing_toolbox.datasets import generic_dataset, grib_dataset
+
 
 class TransformEcmwfData(PreAction):
     """
-    Transforme les prévisions émises par l'ECMWF en fichier netcdf.
+    Transforme les prévisions émises par le CEP en fichier netcdf.
+
+    Parameters
+    ----------
+    name: str
+        Le nom de l'action
+    options: objet
+        L'instance contenant les options de l'action. Les champs possibles sont:
+
+        * output_dir : str
+            Chemin cible pour l'enregistrement des fichiers.
+        * date_format : str
+            Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
+        * variables : list
+            Les variables météorologiques à convertir.
     """
 
     def __init__(self, name, options):
-        """
-        Initialisation de l'instance TransformEcmwfData
-
-        Parameters
-        ----------
-        name: str
-            Le nom de l'action
-        options
-            L'instance contenant les options de l'action. Les champs possibles sont:
-            * transform_ecmwf_input_dir: str
-                Répertoire contenant les fichiers originaux (grib2).
-            * transform_ecmwf_output_dir: str
-                Répertoire cible pour l'enregistrement des fichiers.
-            * ecmwf_variables: list
-                Variables à télécharger.
-                Valeur par défaut: ['hgt']
-        """
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
 
-        self.type_name = "Transformation données ECMWF"
+        self.type_name = "Transformation données GFS"
         self.name = name
-        self.input_dir = options.get('transform_ecmwf_input_dir')
-        self.output_dir = options.get('transform_ecmwf_output_dir')
+        self.input_dir = options['input_dir']
+        self.output_dir = options['output_dir']
+        self.variables = options['variables']
+
         asv.check_dir_exists(self.output_dir, True)
 
         self._set_attempts_attributes(options)
 
-        if options.has('ecmwf_variables'):
-            self.variables = options.get('ecmwf_variables')
-        else:
-            self.variables = ['z']
-
         super().__init__()
 
     def run(self, date) -> bool:
         """
         Exécute l'action.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.transform(date)
 
     def transform(self, date) -> bool:
         """
         Transforme les prévisions de l'ECMWF pour une date d'émission de la prévision.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
             file_name_pattern = f'{forecast_date}{forecast_hour}.ECMWF_IFS.' \
                                 f'{variable.lower()}.*.grib2'
+            new_file_name = f'{forecast_date}{forecast_hour}.ECMWF_IFS.' \
+                            f'{variable.lower()}.nc'
 
             input_files = sorted(input_dir.glob(file_name_pattern))
 
             if len(input_files) == 0:
                 return False
 
-            #data = grib_dataset.Grib(directory=input_dir,
-            #                         file_pattern=file_name_pattern)
-            #data.load()
-
-            #new_file = generic.Generic(directory=self.output_dir,
-            #                           var_name=variable,
-            #                           ref_data=data)
-            #new_file.generate(format=generic.NETCDF_4)
+            data = grib_dataset.GribDataset(
+                directory=input_dir,
+                file_pattern=file_name_pattern)
+            data.load()
+
+            new_file = generic_dataset.GenericDataset(
+                directory=self.output_dir,
+                var_name=variable,
+                ref_data=data)
+            new_file.generate(
+                format=generic_dataset.NETCDF_4,
+                file_name=new_file_name)
 
         return True
 
     def _get_input_dir(self, date):
         return asv.build_date_dir_structure(self.input_dir, date)
 
     def _get_output_dir(self, date):
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 import atmoswing_vigicrues as asv
-#if asv.has_eccodes and asv.has_netcdf:
-#    from atmoswing_toolbox.datasets import generic, grib_dataset
-
 
 from .preaction import PreAction
 
+if asv.has_eccodes and asv.has_netcdf:
+    from atmoswing_toolbox.datasets import generic_dataset, grib_dataset
+
 
 class TransformGfsData(PreAction):
     """
     Transforme les prévisions émises par GFS en fichier netcdf.
+
+    Parameters
+    ----------
+    name: str
+        Le nom de l'action
+    options: objet
+        L'instance contenant les options de l'action. Les champs possibles sont:
+
+        * output_dir : str
+            Chemin cible pour l'enregistrement des fichiers.
+        * date_format : str
+            Format pour l'écriture des dates cibles. Défaut: "%d-%m-%Y"
+        * variables : list
+            Les variables météorologiques à convertir.
     """
 
     def __init__(self, name, options):
-        """
-        Initialisation de l'instance TransformGfsData
-
-        Parameters
-        ----------
-        name: str
-            Le nom de l'action
-        options
-            L'instance contenant les options de l'action. Les champs possibles sont:
-            * transform_gfs_input_dir: str
-                Répertoire contenant les fichiers originaux (grib2).
-            * transform_gfs_output_dir: str
-                Répertoire cible pour l'enregistrement des fichiers.
-            * gfs_variables: list
-                Variables à télécharger.
-                Valeur par défaut: ['hgt']
-        """
         if not asv.has_netcdf:
             raise ImportError("Le paquet netCDF4 est requis pour cette action.")
         if not asv.has_eccodes:
             raise ImportError("Le paquet eccodes est requis pour cette action.")
 
         self.type_name = "Transformation données GFS"
         self.name = name
-        self.input_dir = options.get('transform_gfs_input_dir')
-        self.output_dir = options.get('transform_gfs_output_dir')
+        self.input_dir = options['input_dir']
+        self.output_dir = options['output_dir']
+        self.variables = options['variables']
+
         asv.check_dir_exists(self.output_dir, True)
 
         self._set_attempts_attributes(options)
 
-        if options.has('gfs_variables'):
-            self.variables = options.get('gfs_variables')
-        else:
-            self.variables = ['hgt']
-
         super().__init__()
 
     def run(self, date) -> bool:
         """
         Exécute l'action.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
         return self.transform(date)
 
     def transform(self, date) -> bool:
         """
         Transforme les prévisions de GFS pour une date d'émission de la prévision.
 
         Parameters
         ----------
-        date: datetime
+        date: datetime.datetime
             Date d'émission de la prévision.
 
         Returns
         -------
         Vrai (True) en cas de succès, faux (False) autrement.
         """
 
         input_dir = self._get_input_dir(date)
         forecast_date, forecast_hour = self._format_forecast_date(date)
 
         for variable in self.variables:
             file_name_pattern = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
                                 f'{variable.lower()}.*.grib2'
+            new_file_name = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
+                            f'{variable.lower()}.nc'
 
             input_files = sorted(input_dir.glob(file_name_pattern))
 
             if len(input_files) == 0:
                 return False
 
-            #data = grib_dataset.Grib(directory=input_dir,
-            #                         file_pattern=file_name_pattern)
-            #data.load()
-
-            #new_file = generic.Generic(directory=self.output_dir,
-            #                           var_name=variable,
-            #                           ref_data=data)
-            #new_file.generate(format=generic.NETCDF_4)
+            data = grib_dataset.GribDataset(
+                directory=input_dir,
+                file_pattern=file_name_pattern)
+            data.load()
+
+            new_file = generic_dataset.GenericDataset(
+                directory=self.output_dir,
+                var_name=variable,
+                ref_data=data)
+            new_file.generate(
+                format=generic_dataset.NETCDF_4,
+                file_name=new_file_name)
 
         return True
 
     def _get_input_dir(self, date):
         return asv.build_date_dir_structure(self.input_dir, date)
 
     def _get_output_dir(self, date):
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from pathlib import Path
 import datetime
+from pathlib import Path
+
 import numpy as np
 
 import atmoswing_vigicrues as asv
 
 
 def file_exists(path):
     """ Contrôle du chemin vers un fichier. """
```

### Comparing `atmoswing-vigicrues-1.0.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.0/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -28,9 +28,13 @@
 src/atmoswing_vigicrues/preactions/transform_ecmwf.py
 src/atmoswing_vigicrues/preactions/transform_gfs.py
 tests/test_controller.py
 tests/test_download_gfs.py
 tests/test_exceptions.py
 tests/test_export_bdapbp.py
 tests/test_export_prv.py
+tests/test_main.py
 tests/test_options.py
+tests/test_transfer_sftp_in.py
+tests/test_transfer_sftp_out.py
+tests/test_transform_gfs.py
 tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.0/tests/test_download_gfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,50 +39,50 @@
 
 
 def test_download_gfs_025_succeeds(options):
     options['resolution'] = 0.25
     action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
-    assert count_files_recursively(options) == 3 * 4
+    assert count_files_recursively(options) == 3 * 4 * 2
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_050_succeeds(options):
     options['resolution'] = 0.50
     action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
-    assert count_files_recursively(options) == 3 * 4
+    assert count_files_recursively(options) == 3 * 4 * 2
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_100_succeeds(options):
     options['resolution'] = 1
     action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
-    assert count_files_recursively(options) == 3 * 4
+    assert count_files_recursively(options) == 3 * 4 * 2
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_default_succeeds(options):
     action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.download(date)
-    assert count_files_recursively(options) == 3 * 4
+    assert count_files_recursively(options) == 3 * 4 * 2
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_with_surface_var(options):
     options['levels'] = [500, 1000, 'surface']
     action = asv.DownloadGfsData('Download GFS data', options)
     date = datetime.utcnow() - timedelta(days=1)
     assert action.run(date)
-    assert count_files_recursively(options) == 3 * 4
+    assert count_files_recursively(options) == 3 * 4 * 2
     shutil.rmtree(options['output_dir'])
 
 
 def test_download_gfs_entire_atmosphere_var(options):
     options['levels'] = ['entire_atmosphere']
     options['variables'] = ['pwat']
     action = asv.DownloadGfsData('Download GFS data', options)
```

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.0/tests/test_export_bdapbp.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         '2022-10-01_00.PC-AZ4o.Cretes_sud.json'
     ]
     for created_file in created_files:
         file_path = options['output_dir'] + '/2022/10/01/' + created_file
         with open(file_path) as f:
             data = json.load(f)
             assert data['status'] == 0
+            assert data['report']['only_relevant_stations'] is True
     shutil.rmtree(options['output_dir'])
 
 
 def test_export_bdapbp_with_no_limit(options, forecast_files, metadata):
     forecast_files.sort()
     forecast_files = [forecast_files[0]]
     options['number_analogs'] = -1
```

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.0/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_options.py` & `atmoswing-vigicrues-1.1.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.0.4/tests/test_utils.py` & `atmoswing-vigicrues-1.1.0/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,7 +17,12 @@
         tmp_file = tmp_dir + '/file.txt'
         Path(tmp_file).touch()
         asv.check_file_exists(tmp_file)
 
 
 def test_build_cumulative_frequency():
     f = asv.utils.build_cumulative_frequency(100)
+    assert len(f) == 100
+    assert f[0] > 0
+    assert f[0] < 1/100
+    assert f[99] < 1
+    assert f[99] > 99/100
```

