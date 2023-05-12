# Comparing `tmp/pipenv-check-0.0.6.tar.gz` & `tmp/pipenv-check-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipenv-check-0.0.6.tar", last modified: Thu May 11 09:01:05 2023, max compression
+gzip compressed data, was "pipenv-check-0.0.7.tar", last modified: Thu May 11 13:57:54 2023, max compression
```

## Comparing `pipenv-check-0.0.6.tar` & `pipenv-check-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.365694 pipenv-check-0.0.6/
--rw-r--r--   0 ayse       (501) staff       (20)     1061 2023-05-10 13:32:16.000000 pipenv-check-0.0.6/LICENSE
--rw-r--r--   0 ayse       (501) staff       (20)     1117 2023-05-11 09:01:05.365273 pipenv-check-0.0.6/PKG-INFO
--rw-r--r--   0 ayse       (501) staff       (20)      847 2023-05-11 08:04:38.000000 pipenv-check-0.0.6/README.md
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.358666 pipenv-check-0.0.6/pipenv_check/
--rw-r--r--   0 ayse       (501) staff       (20)        0 2023-05-10 13:32:16.000000 pipenv-check-0.0.6/pipenv_check/__init__.py
--rw-r--r--   0 ayse       (501) staff       (20)     5697 2023-05-11 08:58:32.000000 pipenv-check-0.0.6/pipenv_check/check.py
-drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 09:01:05.364695 pipenv-check-0.0.6/pipenv_check.egg-info/
--rw-r--r--   0 ayse       (501) staff       (20)     1117 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/PKG-INFO
--rw-r--r--   0 ayse       (501) staff       (20)      256 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/SOURCES.txt
--rw-r--r--   0 ayse       (501) staff       (20)        1 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/dependency_links.txt
--rw-r--r--   0 ayse       (501) staff       (20)       57 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/entry_points.txt
--rw-r--r--   0 ayse       (501) staff       (20)       13 2023-05-11 09:01:05.000000 pipenv-check-0.0.6/pipenv_check.egg-info/top_level.txt
--rw-r--r--   0 ayse       (501) staff       (20)       38 2023-05-11 09:01:05.365828 pipenv-check-0.0.6/setup.cfg
--rw-r--r--   0 ayse       (501) staff       (20)      692 2023-05-10 13:43:50.000000 pipenv-check-0.0.6/setup.py
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 13:57:54.853838 pipenv-check-0.0.7/
+-rw-r--r--   0 ayse       (501) staff       (20)     1061 2023-05-10 13:32:16.000000 pipenv-check-0.0.7/LICENSE
+-rw-r--r--   0 ayse       (501) staff       (20)     1118 2023-05-11 13:57:54.853116 pipenv-check-0.0.7/PKG-INFO
+-rw-r--r--   0 ayse       (501) staff       (20)      848 2023-05-11 10:22:44.000000 pipenv-check-0.0.7/README.md
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 13:57:54.847461 pipenv-check-0.0.7/pipenv_check/
+-rw-r--r--   0 ayse       (501) staff       (20)        0 2023-05-10 13:32:16.000000 pipenv-check-0.0.7/pipenv_check/__init__.py
+-rw-r--r--   0 ayse       (501) staff       (20)     5828 2023-05-11 13:55:08.000000 pipenv-check-0.0.7/pipenv_check/check.py
+drwxr-xr-x   0 ayse       (501) staff       (20)        0 2023-05-11 13:57:54.851415 pipenv-check-0.0.7/pipenv_check.egg-info/
+-rw-r--r--   0 ayse       (501) staff       (20)     1118 2023-05-11 13:57:54.000000 pipenv-check-0.0.7/pipenv_check.egg-info/PKG-INFO
+-rw-r--r--   0 ayse       (501) staff       (20)      256 2023-05-11 13:57:54.000000 pipenv-check-0.0.7/pipenv_check.egg-info/SOURCES.txt
+-rw-r--r--   0 ayse       (501) staff       (20)        1 2023-05-11 13:57:54.000000 pipenv-check-0.0.7/pipenv_check.egg-info/dependency_links.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       57 2023-05-11 13:57:54.000000 pipenv-check-0.0.7/pipenv_check.egg-info/entry_points.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       13 2023-05-11 13:57:54.000000 pipenv-check-0.0.7/pipenv_check.egg-info/top_level.txt
+-rw-r--r--   0 ayse       (501) staff       (20)       38 2023-05-11 13:57:54.854001 pipenv-check-0.0.7/setup.cfg
+-rw-r--r--   0 ayse       (501) staff       (20)      692 2023-05-11 13:55:00.000000 pipenv-check-0.0.7/setup.py
```

### Comparing `pipenv-check-0.0.6/LICENSE` & `pipenv-check-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pipenv-check-0.0.6/PKG-INFO` & `pipenv-check-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pipenv-check
-Version: 0.0.6
+Version: 0.0.7
 Summary: View installed pip packages and their update status.
 Home-page: https://github.com/3bfab/pipenv-check
 Author: 3bfab
 Author-email: info@3bfab.com
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 # pipenv-check
 
-I moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
+Moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
 
-An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. I accomplished this with decode('utf-8') .
+An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. This was accomplished with decode('utf-8') .
 
 At the same time, this operation may result in any errors (for example, if pip is not found or returns an error). Therefore, I enclosed this code in a try-except block and informed the user when the error occurred and terminated the program.
 
-After calling the ThreadPool's close method, I also called the join method. This waits for all threads to complete and provides more predictable program behavior.
+After calling the ThreadPool's close method, we also called the join method. This waits for all threads to complete and provides more predictable program behavior.
```

### Comparing `pipenv-check-0.0.6/README.md` & `pipenv-check-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pipenv-check
 
-I moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
+Moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
 
-An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. I accomplished this with decode('utf-8') .
+An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. This was accomplished with decode('utf-8') .
 
 At the same time, this operation may result in any errors (for example, if pip is not found or returns an error). Therefore, I enclosed this code in a try-except block and informed the user when the error occurred and terminated the program.
 
-After calling the ThreadPool's close method, I also called the join method. This waits for all threads to complete and provides more predictable program behavior.
+After calling the ThreadPool's close method, we also called the join method. This waits for all threads to complete and provides more predictable program behavior.
```

### Comparing `pipenv-check-0.0.6/pipenv_check/check.py` & `pipenv-check-0.0.7/pipenv_check/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,19 @@
     try:
         installed_packages = json.loads(subprocess.check_output(["pip", "list", "--format=json"]).decode('utf-8').lower())
     except Exception as e:
         print("Error occurred while fetching installed packages:", e)
         exit(1)
 
     # installed_packages_in_pipfile with current version
+    # pip list --format=json command sometimes gives different naming formats of the libraries.
     installed_packages_in_pipfile = {
-        package["name"]: {"current": package["version"]}
+        package["name"].replace('_', '-'): {"current": package["version"]}
         for package in installed_packages
-        if package["name"] in pipfile_packages
+        if package["name"].replace('_', '-') in pipfile_packages
     }
 
     # uninstalled packages
     for package in pipfile_packages:
         if package not in installed_packages_in_pipfile:
             installed_packages_in_pipfile[package] = {"current": "not installed"}
 
@@ -151,8 +152,8 @@
                 print()
 
 
 if __name__ == "__main__":
     try:
         main()
     except KeyboardInterrupt:
-        pass
+        pass
```

### Comparing `pipenv-check-0.0.6/pipenv_check.egg-info/PKG-INFO` & `pipenv-check-0.0.7/pipenv_check.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pipenv-check
-Version: 0.0.6
+Version: 0.0.7
 Summary: View installed pip packages and their update status.
 Home-page: https://github.com/3bfab/pipenv-check
 Author: 3bfab
 Author-email: info@3bfab.com
 License: MIT
 Requires-Python: >=3.6
 License-File: LICENSE
 
 # pipenv-check
 
-I moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
+Moved the color_print and BColors class, which were defined inside the main function, outside the main function to increase the readability of the code.
 
-An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. I accomplished this with decode('utf-8') .
+An error occurred when you tried to directly convert the result of subprocess.check_output(["pip", "list", "--format=json"]) to JSON. Since this output is a byte array, you must first convert this output to a character array. This was accomplished with decode('utf-8') .
 
 At the same time, this operation may result in any errors (for example, if pip is not found or returns an error). Therefore, I enclosed this code in a try-except block and informed the user when the error occurred and terminated the program.
 
-After calling the ThreadPool's close method, I also called the join method. This waits for all threads to complete and provides more predictable program behavior.
+After calling the ThreadPool's close method, we also called the join method. This waits for all threads to complete and provides more predictable program behavior.
```

### Comparing `pipenv-check-0.0.6/setup.py` & `pipenv-check-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 long_description = u"\n\n".join((open("README.md").read(),))
 
 setup(
     name="pipenv-check",
-    version="0.0.6",
+    version="0.0.7",
     description="View installed pip packages and their update status.",
     long_description=long_description,
     author="3bfab",
     author_email="info@3bfab.com",
     license="MIT",
     url="https://github.com/3bfab/pipenv-check",
     classifiers=[],
```

