# Comparing `tmp/single_char_counter_by_ng-1.0.3.tar.gz` & `tmp/single_char_counter_by_ng-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "single_char_counter_by_ng-1.0.3.tar", max compression
+gzip compressed data, was "single_char_counter_by_ng-1.0.4.tar", max compression
```

## Comparing `single_char_counter_by_ng-1.0.3.tar` & `single_char_counter_by_ng-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2023-05-12 07:50:23.409145 single_char_counter_by_ng-1.0.3/LICENSE
--rwxr-xr-x   0        0        0      869 2023-05-12 09:33:32.526858 single_char_counter_by_ng-1.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      188 2023-05-11 14:33:46.323025 single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/__init__.py
--rwxr-xr-x   0        0        0      527 2023-05-11 10:48:54.681602 single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char.py
--rwxr-xr-x   0        0        0     1460 2023-05-11 14:19:47.871831 single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char_cli.py
--rwxr-xr-x   0        0        0      868 2023-05-11 14:21:36.027831 single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char_in_file.py
--rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 single_char_counter_by_ng-1.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-05-12 07:50:23.409145 single_char_counter_by_ng-1.0.4/LICENSE
+-rwxr-xr-x   0        0        0      871 2023-05-12 09:36:11.348467 single_char_counter_by_ng-1.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0      188 2023-05-11 14:33:46.323025 single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/__init__.py
+-rwxr-xr-x   0        0        0      527 2023-05-11 10:48:54.681602 single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char.py
+-rwxr-xr-x   0        0        0     1460 2023-05-11 14:19:47.871831 single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char_cli.py
+-rwxr-xr-x   0        0        0      868 2023-05-11 14:21:36.027831 single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char_in_file.py
+-rw-r--r--   0        0        0      467 1970-01-01 00:00:00.000000 single_char_counter_by_ng-1.0.4/PKG-INFO
```

### Comparing `single_char_counter_by_ng-1.0.3/LICENSE` & `single_char_counter_by_ng-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.0.3/pyproject.toml` & `single_char_counter_by_ng-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "single_char_counter_by_ng"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name = "Nazar Hots", email = "gotsjob@gmail.com" },
 ]
 description = "Application that takes a string or file and returns the number of all characters in the string or file occurring only once."
-readme = "README.md"
+readme = "./README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry]
 name = "single_char_counter_by_ng"
-version = "1.0.3"
+version = "1.0.4"
 description = "Application that takes a string or file and returns the number of all characters in the string or file occurring only once."
 authors = ["Nazar Hots <gotsjob@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.1"
```

### Comparing `single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char.py` & `single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char_cli.py` & `single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char_cli.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.0.3/single_char_counter_by_ng/count_single_char_in_file.py` & `single_char_counter_by_ng-1.0.4/single_char_counter_by_ng/count_single_char_in_file.py`

 * *Files identical despite different names*

