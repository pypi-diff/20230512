# Comparing `tmp/edman_cli-2023.3.15.tar.gz` & `tmp/edman_cli-2023.5.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edman_cli-2023.3.15.tar", last modified: Wed Mar 15 06:40:47 2023, max compression
+gzip compressed data, was "edman_cli-2023.5.12.tar", last modified: Fri May 12 07:10:39 2023, max compression
```

## Comparing `edman_cli-2023.3.15.tar` & `edman_cli-2023.5.12.tar`

### file list

```diff
@@ -1,16 +1,66 @@
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-03-15 06:40:47.762953 edman_cli-2023.3.15/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.3.15/LICENSE.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       19 2022-01-31 01:52:15.000000 edman_cli-2023.3.15/MANIFEST.in
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3772 2023-03-15 06:40:47.762953 edman_cli-2023.3.15/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.3.15/README.rst
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-03-15 06:40:47.762953 edman_cli-2023.3.15/edman_cli.egg-info/
--rw-r--r--   0 ohno      (1000) ohno      (1000)     3772 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/PKG-INFO
--rw-r--r--   0 ohno      (1000) ohno      (1000)      274 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/entry_points.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/requires.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-03-15 06:40:47.000000 edman_cli-2023.3.15/edman_cli.egg-info/top_level.txt
--rw-r--r--   0 ohno      (1000) ohno      (1000)      735 2023-03-15 06:40:47.762953 edman_cli-2023.3.15/setup.cfg
--rw-r--r--   0 ohno      (1000) ohno      (1000)      833 2022-02-03 08:45:05.000000 edman_cli-2023.3.15/setup.py
-drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-03-15 06:40:47.762953 edman_cli-2023.3.15/tests/
--rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2022-11-21 07:40:05.000000 edman_cli-2023.3.15/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1100 2023-03-15 06:38:21.000000 edman_cli-2023.5.12/LICENSE.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3345 2023-01-20 03:57:51.000000 edman_cli-2023.5.12/README.rst
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/edman_cli.egg-info/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     4934 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1495 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        1 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      512 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       71 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/requires.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       36 2023-05-12 07:10:39.000000 edman_cli-2023.5.12/edman_cli.egg-info/top_level.txt
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1468 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/pyproject.toml
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16460 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2229 2022-03-23 07:12:34.000000 edman_cli-2023.5.12/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1573 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2557 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2328 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2947 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2513 2023-05-12 07:08:01.000000 edman_cli-2023.5.12/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2022-04-13 08:48:24.000000 edman_cli-2023.5.12/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2628 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1907 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2403 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2096 2022-02-03 08:34:28.000000 edman_cli-2023.5.12/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)       38 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/setup.cfg
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2022-11-21 07:40:05.000000 edman_cli-2023.5.12/tests/test_action.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/bin/
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1729 2023-04-07 00:41:13.000000 edman_cli-2023.5.12/venv/bin/jp.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      636 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      758 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html4.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     1093 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2html5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      835 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2latex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      658 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2man.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      824 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2odt.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)     2180 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      643 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      679 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2s5.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      915 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      644 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rst2xml.py
+-rwxr-xr-x   0 ohno      (1000) ohno      (1000)      712 2023-05-10 01:28:58.000000 edman_cli-2023.5.12/venv/bin/rstpep2html.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/src/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.193199 edman_cli-2023.5.12/venv/src/edman-cli/
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/venv/src/edman-cli/scripts/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    16618 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/action.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2287 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/assign_bson_type.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3510 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_create.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2722 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/db_destroy.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1618 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2624 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/entry.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2266 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_add.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3027 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     3177 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/file_dl.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2374 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/find.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2702 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/item_delete.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     1960 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/pullout.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2462 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/structure_convert.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)     2156 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/scripts/update.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)      855 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/setup.py
+drwxr-xr-x   0 ohno      (1000) ohno      (1000)        0 2023-05-12 07:10:39.203199 edman_cli-2023.5.12/venv/src/edman-cli/tests/
+-rw-r--r--   0 ohno      (1000) ohno      (1000)        0 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/tests/__init__.py
+-rw-r--r--   0 ohno      (1000) ohno      (1000)    10946 2023-04-07 00:41:06.000000 edman_cli-2023.5.12/venv/src/edman-cli/tests/test_action.py
```

### Comparing `edman_cli-2023.3.15/LICENSE.txt` & `edman_cli-2023.5.12/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.3.15/PKG-INFO` & `edman_cli-2023.5.12/edman_cli.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
-Name: edman_cli
-Version: 2023.3.15
-Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Home-page: https://github.com/ryde/edman_cli
-Author: Masaki Ohno
-Author-email: masakio@post.kek.jp
+Name: edman-cli
+Version: 2023.5.12
+Summary: Sub-package of edman for cli applications and scripts.
+Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Database :: Front-Ends
+        
+        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://github.com/ryde/edman_cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman_cli
 =========
```

### Comparing `edman_cli-2023.3.15/README.rst` & `edman_cli-2023.5.12/README.rst`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.3.15/edman_cli.egg-info/PKG-INFO` & `edman_cli-2023.5.12/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 Metadata-Version: 2.1
-Name: edman-cli
-Version: 2023.3.15
-Summary: KEK IMSS SBRC/PF Experimental Data Management System
-Home-page: https://github.com/ryde/edman_cli
-Author: Masaki Ohno
-Author-email: masakio@post.kek.jp
+Name: edman_cli
+Version: 2023.5.12
+Summary: Sub-package of edman for cli applications and scripts.
+Author-email: Masaki Ohno <masakio@post.kek.jp>
 License: MIT License
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Database :: Front-Ends
+        
+        Copyright (c) 2019-2023 KEK IMSS SBRC/PF, Masaki Ohno
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: repository, https://github.com/ryde/edman_cli
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 edman_cli
 =========
```

### Comparing `edman_cli-2023.3.15/edman_cli.egg-info/entry_points.txt` & `edman_cli-2023.5.12/edman_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edman_cli-2023.3.15/setup.py` & `edman_cli-2023.5.12/venv/src/edman-cli/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from setuptools import setup
-
-setup(
-    entry_points={
-            'console_scripts': [
-                'ed_assign_bson_type=scripts.assign_bson_type:main',
-                'ed_db_create=scripts.db_create:main',
-                'ed_db_destroy=scripts.db_destroy:main',
-                'ed_delete=scripts.delete:main',
-                'ed_entry=scripts.entry:main',
-                'ed_file_add=scripts.file_add:main',
-                'ed_file_delete=scripts.file_delete:main',
-                'ed_file_dl=scripts.file_dl:main',
-                'ed_find=scripts.find:main',
-                'ed_item_delete=scripts.item_delete:main',
-                'ed_pullout=scripts.pullout:main',
-                'ed_structure_convert=scripts.structure_convert:main',
-                'ed_update=scripts.update:main',
-            ],
-        },
-
-)
+from setuptools import setup
+
+setup(
+    entry_points={
+            'console_scripts': [
+                'ed_assign_bson_type=scripts.assign_bson_type:main',
+                'ed_db_create=scripts.db_create:main',
+                'ed_db_destroy=scripts.db_destroy:main',
+                'ed_delete=scripts.delete:main',
+                'ed_entry=scripts.entry:main',
+                'ed_file_add=scripts.file_add:main',
+                'ed_file_delete=scripts.file_delete:main',
+                'ed_file_dl=scripts.file_dl:main',
+                'ed_find=scripts.find:main',
+                'ed_item_delete=scripts.item_delete:main',
+                'ed_pullout=scripts.pullout:main',
+                'ed_structure_convert=scripts.structure_convert:main',
+                'ed_update=scripts.update:main',
+            ],
+        },
+
+)
```

### Comparing `edman_cli-2023.3.15/tests/test_action.py` & `edman_cli-2023.5.12/tests/test_action.py`

 * *Files identical despite different names*

