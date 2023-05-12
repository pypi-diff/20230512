# Comparing `tmp/puffy-0.3.0.tar.gz` & `tmp/puffy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puffy-0.3.0.tar", last modified: Mon May  1 04:30:16 2023, max compression
+gzip compressed data, was "puffy-0.3.4.tar", last modified: Fri May 12 10:28:14 2023, max compression
```

## Comparing `puffy-0.3.0.tar` & `puffy-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427446 puffy-0.3.0/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.3.0/LICENSE
--rw-r--r--   0 nicolasdao   (501) staff       (20)    18912 2023-05-01 04:30:16.427537 puffy-0.3.0/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)    18419 2023-05-01 04:27:50.000000 puffy-0.3.0/README.md
--rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.3.0/pyproject.toml
--rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-05-01 04:30:16.427903 puffy-0.3.0/setup.cfg
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.425390 puffy-0.3.0/src/
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.426322 puffy-0.3.0/src/puffy/
--rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.3.0/src/puffy/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427068 puffy-0.3.0/src/puffy/error/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.3.0/src/puffy/error/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427191 puffy-0.3.0/src/puffy/log/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     4341 2023-05-01 04:07:48.000000 puffy-0.3.0/src/puffy/log/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.427318 puffy-0.3.0/src/puffy/object/
--rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.3.0/src/puffy/object/__init__.py
-drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-01 04:30:16.426943 puffy-0.3.0/src/puffy.egg-info/
--rw-r--r--   0 nicolasdao   (501) staff       (20)    18912 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/PKG-INFO
--rw-r--r--   0 nicolasdao   (501) staff       (20)      311 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/SOURCES.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/dependency_links.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/requires.txt
--rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-05-01 04:30:16.000000 puffy-0.3.0/src/puffy.egg-info/top_level.txt
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.926266 puffy-0.3.4/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1541 2023-02-14 15:36:17.000000 puffy-0.3.4/LICENSE
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    19052 2023-05-12 10:28:14.926360 puffy-0.3.4/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    18559 2023-05-01 04:40:26.000000 puffy-0.3.4/README.md
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      251 2023-02-24 11:28:17.000000 puffy-0.3.4/pyproject.toml
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      825 2023-05-12 10:28:14.926783 puffy-0.3.4/setup.cfg
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.923500 puffy-0.3.4/src/
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.924716 puffy-0.3.4/src/puffy/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        0 2023-02-27 02:26:12.000000 puffy-0.3.4/src/puffy/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925542 puffy-0.3.4/src/puffy/error/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     6106 2023-04-28 06:03:30.000000 puffy-0.3.4/src/puffy/error/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925799 puffy-0.3.4/src/puffy/log/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     4384 2023-05-12 10:26:42.000000 puffy-0.3.4/src/puffy/log/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.926048 puffy-0.3.4/src/puffy/object/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)     1278 2023-02-26 16:22:15.000000 puffy-0.3.4/src/puffy/object/__init__.py
+drwxr-xr-x   0 nicolasdao   (501) staff       (20)        0 2023-05-12 10:28:14.925413 puffy-0.3.4/src/puffy.egg-info/
+-rw-r--r--   0 nicolasdao   (501) staff       (20)    19052 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/PKG-INFO
+-rw-r--r--   0 nicolasdao   (501) staff       (20)      311 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        1 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)       54 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/requires.txt
+-rw-r--r--   0 nicolasdao   (501) staff       (20)        6 2023-05-12 10:28:14.000000 puffy-0.3.4/src/puffy.egg-info/top_level.txt
```

### Comparing `puffy-0.3.0/LICENSE` & `puffy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `puffy-0.3.0/PKG-INFO` & `puffy-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.3.0
+Version: 0.3.4
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -442,25 +442,29 @@
 
 ## Building and distributing this package
 
 1. Make sure the test and lint operations have not produced errors:
 ```shell
 make t
 ```
-2. Build this package:
-```shell
-make b
-```
-> This command is a wrapper around `python3 -m build`.
-3. Version and tag this package using one of the following command (1):
+2. Version and tag this package using one of the following commands (1):
     - `easyv bump`: Use this to bump the patch version.
     - `easyv bump minor`: Use this to bump the minor version.
     - `easyv bump major`: Use this to bump the major version.
     - `easyv bump x.x.x`: Use this to bump the version to a specific value.
-4 . Publish this package to https://pypi.org:
+3. Push those latest changes to your source control repository (incl. tags). For example:
+```shell
+git push origin master --follow-tags
+```
+4. Build this package:
+```shell
+make b
+```
+> This command is a wrapper around `python3 -m build`.
+5. Publish this package to https://pypi.org:
 ```shell
 make p
 ```
 > This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
```

### Comparing `puffy-0.3.0/README.md` & `puffy-0.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -426,25 +426,29 @@
 
 ## Building and distributing this package
 
 1. Make sure the test and lint operations have not produced errors:
 ```shell
 make t
 ```
-2. Build this package:
-```shell
-make b
-```
-> This command is a wrapper around `python3 -m build`.
-3. Version and tag this package using one of the following command (1):
+2. Version and tag this package using one of the following commands (1):
     - `easyv bump`: Use this to bump the patch version.
     - `easyv bump minor`: Use this to bump the minor version.
     - `easyv bump major`: Use this to bump the major version.
     - `easyv bump x.x.x`: Use this to bump the version to a specific value.
-4 . Publish this package to https://pypi.org:
+3. Push those latest changes to your source control repository (incl. tags). For example:
+```shell
+git push origin master --follow-tags
+```
+4. Build this package:
+```shell
+make b
+```
+> This command is a wrapper around `python3 -m build`.
+5. Publish this package to https://pypi.org:
 ```shell
 make p
 ```
 > This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
```

### Comparing `puffy-0.3.0/setup.cfg` & `puffy-0.3.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = puffy
-version = 0.3.0
+version = 0.3.4
 author = Nicolas Dao
 author_email = nicolas.dao@gmail.com
 description = A collection of modules with zero-dependencies to help manage common programming tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicolasdao/pypuffy
 readme = README.md
```

### Comparing `puffy-0.3.0/src/puffy/error/__init__.py` & `puffy-0.3.4/src/puffy/error/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.3.0/src/puffy/log/__init__.py` & `puffy-0.3.4/src/puffy/log/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                             [_stringify_error(x) for x in errors]
                         )
                 else:
                     log_data["errors"] = str(errors)
             except:
                 pass
 
-        log_str = json.dumps(log_data)
+        log_str = json.dumps(log_data, default=str)
 
         if print_mock and print_mock is not None:
             print_mock(log_str)
         else:
             print(log_str)
     except Exception as e:
         try:
@@ -147,15 +147,16 @@
                     "data": {
                         "message": f"{message}",
                         "message_type": str(type(message)),
                         "code": f"{code}",
                         "code_type": str(type(code)),
                     },
                     "errors": str(e),
-                }
+                },
+                default=str,
             )
             if print_mock and print_mock is not None:
                 print_mock(log_str)
             else:
                 print(log_str)
         except:
             pass
```

### Comparing `puffy-0.3.0/src/puffy/object/__init__.py` & `puffy-0.3.4/src/puffy/object/__init__.py`

 * *Files identical despite different names*

### Comparing `puffy-0.3.0/src/puffy.egg-info/PKG-INFO` & `puffy-0.3.4/src/puffy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puffy
-Version: 0.3.0
+Version: 0.3.4
 Summary: A collection of modules with zero-dependencies to help manage common programming tasks.
 Home-page: https://github.com/nicolasdao/pypuffy
 Author: Nicolas Dao
 Author-email: nicolas.dao@gmail.com
 License: BSD-3-Clause
 Keywords: util
 Classifier: Programming Language :: Python :: 3
@@ -442,25 +442,29 @@
 
 ## Building and distributing this package
 
 1. Make sure the test and lint operations have not produced errors:
 ```shell
 make t
 ```
-2. Build this package:
-```shell
-make b
-```
-> This command is a wrapper around `python3 -m build`.
-3. Version and tag this package using one of the following command (1):
+2. Version and tag this package using one of the following commands (1):
     - `easyv bump`: Use this to bump the patch version.
     - `easyv bump minor`: Use this to bump the minor version.
     - `easyv bump major`: Use this to bump the major version.
     - `easyv bump x.x.x`: Use this to bump the version to a specific value.
-4 . Publish this package to https://pypi.org:
+3. Push those latest changes to your source control repository (incl. tags). For example:
+```shell
+git push origin master --follow-tags
+```
+4. Build this package:
+```shell
+make b
+```
+> This command is a wrapper around `python3 -m build`.
+5. Publish this package to https://pypi.org:
 ```shell
 make p
 ```
 > This command is a wrapper around the following commands: `python3 -m build; twine upload dist/*`
 
 
 To test your package locally before deploying it to https://pypi.org, you can run build and install it locally with this command:
```

