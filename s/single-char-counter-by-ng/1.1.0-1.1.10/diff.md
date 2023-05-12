# Comparing `tmp/single_char_counter_by_ng-1.1.0.tar.gz` & `tmp/single_char_counter_by_ng-1.1.10.tar.gz`

## Comparing `single_char_counter_by_ng-1.1.0.tar` & `single_char_counter_by_ng-1.1.10.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/README.md
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/requirements.txt
--rwxr-xr-x   0        0        0   467401 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/t.txt
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/__init__.py
--rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char.py
--rwxr-xr-x   0        0        0     1460 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char_cli.py
--rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char_in_file.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/__init__.py
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/test_count_single_char/__init__.py
--rwxr-xr-x   0        0        0      962 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/test_count_single_char/data_for_test_count_single_char.py
--rwxr-xr-x   0        0        0     1296 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char.py
--rwxr-xr-x   0        0        0     3176 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char_cli.py
--rwxr-xr-x   0        0        0     1249 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char_in_file.py
--rwxr-xr-x   0        0        0     3091 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/.gitignore
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/LICENSE
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     2149 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/README.md
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/requirements.txt
+-rwxr-xr-x   0        0        0   467401 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/t.txt
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/__init__.py
+-rwxr-xr-x   0        0        0      527 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char.py
+-rwxr-xr-x   0        0        0     1460 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char_cli.py
+-rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char_in_file.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/__init__.py
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/test_count_single_char/__init__.py
+-rwxr-xr-x   0        0        0      962 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/test_count_single_char/data_for_test_count_single_char.py
+-rwxr-xr-x   0        0        0     1296 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char.py
+-rwxr-xr-x   0        0        0     3176 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char_cli.py
+-rwxr-xr-x   0        0        0     1249 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char_in_file.py
+-rwxr-xr-x   0        0        0     3091 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/.gitignore
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/LICENSE
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/pyproject.toml
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 single_char_counter_by_ng-1.1.10/PKG-INFO
```

### Comparing `single_char_counter_by_ng-1.1.0/README.md` & `single_char_counter_by_ng-1.1.10/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: single_char_counter_by_ng
+Version: 1.1.10
+Summary: Application that takes a string or file and returns the number of all characters in the string or file occurring only once.
+Author-email: Nazar Hots <gotsjob@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # Single char counter
 
 ## Installation
 Clone this repository to your local machine:
 
 ```bash
-git clone http://git.foxminded.ua/foxstudent103611/task_5.git
+pip install single-char-counter-by-ng
 ```
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requirements:
 
 ```bash
 pip install -r requirements.txt
 ```
```

### Comparing `single_char_counter_by_ng-1.1.0/t.txt` & `single_char_counter_by_ng-1.1.10/t.txt`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char.py` & `single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char_cli.py` & `single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char_cli.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/single_char_counter_by_ng/count_single_char_in_file.py` & `single_char_counter_by_ng-1.1.10/single_char_counter_by_ng/count_single_char_in_file.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/tests/test_count_single_char/data_for_test_count_single_char.py` & `single_char_counter_by_ng-1.1.10/tests/test_count_single_char/data_for_test_count_single_char.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char.py` & `single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char_cli.py` & `single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char_cli.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/tests/test_count_single_char/test_count_single_char_in_file.py` & `single_char_counter_by_ng-1.1.10/tests/test_count_single_char/test_count_single_char_in_file.py`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/.gitignore` & `single_char_counter_by_ng-1.1.10/.gitignore`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/LICENSE` & `single_char_counter_by_ng-1.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `single_char_counter_by_ng-1.1.0/pyproject.toml` & `single_char_counter_by_ng-1.1.10/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "single_char_counter_by_ng"
-version = "1.1.0"
+version = "1.1.10"
 authors = [
   { name = "Nazar Hots", email = "gotsjob@gmail.com" },
 ]
 description = "Application that takes a string or file and returns the number of all characters in the string or file occurring only once."
 readme = "/mnt/e/Foxminded/task-5-create-the-python-package/README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry]
 name = "single_char_counter_by_ng"
-version = "1.1.0"
+version = "1.1.10"
 description = "Application that takes a string or file and returns the number of all characters in the string or file occurring only once."
 authors = ["Nazar Hots <gotsjob@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pytest = "^7.1"
```

### Comparing `single_char_counter_by_ng-1.1.0/PKG-INFO` & `single_char_counter_by_ng-1.1.10/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: single_char_counter_by_ng
-Version: 1.1.0
-Summary: Application that takes a string or file and returns the number of all characters in the string or file occurring only once.
-Author-email: Nazar Hots <gotsjob@gmail.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Single char counter
 
 ## Installation
 Clone this repository to your local machine:
 
 ```bash
-git clone http://git.foxminded.ua/foxstudent103611/task_5.git
+pip install single-char-counter-by-ng
 ```
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requirements:
 
 ```bash
 pip install -r requirements.txt
 ```
```

