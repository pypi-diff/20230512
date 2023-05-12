# Comparing `tmp/aws_lambda_mess-0.0.8.tar.gz` & `tmp/aws_lambda_mess-0.0.9.tar.gz`

## Comparing `aws_lambda_mess-0.0.8.tar` & `aws_lambda_mess-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/__about__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/cli.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/framework/Route.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/framework/failures.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/framework/lambda_dispatcher.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/framework/server.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/framework/success.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/init_files/.aws_lambda_mess.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/init_files/.gitignore
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/init_files/app.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/aws_lambda_mess/init_files/requirements.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/.gitignore
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/__about__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/cli.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/framework/Route.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/framework/failures.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/framework/lambda_dispatcher.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/framework/server.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/framework/success.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/init_files/.aws_lambda_mess.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/init_files/.gitignore
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/init_files/app.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/aws_lambda_mess/init_files/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/.gitignore
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/README.md
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.9/PKG-INFO
```

### Comparing `aws_lambda_mess-0.0.8/aws_lambda_mess/cli.py` & `aws_lambda_mess-0.0.9/aws_lambda_mess/cli.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.8/aws_lambda_mess/framework/Route.py` & `aws_lambda_mess-0.0.9/aws_lambda_mess/framework/Route.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.8/aws_lambda_mess/framework/server.py` & `aws_lambda_mess-0.0.9/aws_lambda_mess/framework/server.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.8/aws_lambda_mess/init_files/app.py` & `aws_lambda_mess-0.0.9/aws_lambda_mess/init_files/app.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.8/README.md` & `aws_lambda_mess-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ```
 After a successful installation check that the cli works:
 ```shell
 alm --help
 ```
 
 # Create and run a new project
-Create a new project using th cli:
+Create a new project using the cli:
 ```shell
 alm new demo
 ```
 This will: 
  * create a new directory with the name you specified 
  * populate the directory with some standard boilerplate
 
@@ -73,17 +73,17 @@
 
 
 def default(params, body):
     return bad_request()
 
 
 routes = [
-    Route(method_pattern="GET", path_pattern="/", handler=index),
     Route(method_pattern="GET", path_pattern="/greet/<name>", handler=greet),
     Route(method_pattern=".*", path_pattern=".*", handler=default)
+    Route(method_pattern="GET", path_pattern="/", handler=index),
 ]
 
 from aws_lambda_mess.framework.lambda_dispatcher import get_handler
 lambda_handler = get_handler(routes)
 
 if __name__ == "__main__":
     run(9000, routes)
```

### Comparing `aws_lambda_mess-0.0.8/pyproject.toml` & `aws_lambda_mess-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.8/PKG-INFO` & `aws_lambda_mess-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_mess
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/johanjordaan/aws_lambda_mess#readme
 Project-URL: Issues, https://github.com/johanjordaan/aws_lambda_mess/issues
 Project-URL: Source, https://github.com/johanjordaan/aws_lambda_mess
 Author-email: johan jordaan <djjordaan@gmail.com>
 License-Expression: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -54,15 +54,15 @@
 ```
 After a successful installation check that the cli works:
 ```shell
 alm --help
 ```
 
 # Create and run a new project
-Create a new project using th cli:
+Create a new project using the cli:
 ```shell
 alm new demo
 ```
 This will: 
  * create a new directory with the name you specified 
  * populate the directory with some standard boilerplate
 
@@ -84,17 +84,17 @@
 
 
 def default(params, body):
     return bad_request()
 
 
 routes = [
-    Route(method_pattern="GET", path_pattern="/", handler=index),
     Route(method_pattern="GET", path_pattern="/greet/<name>", handler=greet),
     Route(method_pattern=".*", path_pattern=".*", handler=default)
+    Route(method_pattern="GET", path_pattern="/", handler=index),
 ]
 
 from aws_lambda_mess.framework.lambda_dispatcher import get_handler
 lambda_handler = get_handler(routes)
 
 if __name__ == "__main__":
     run(9000, routes)
```

