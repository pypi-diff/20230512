# Comparing `tmp/gitlabdata-0.3.8.tar.gz` & `tmp/gitlabdata-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitlabdata-0.3.8.tar", last modified: Fri Nov 26 14:41:50 2021, max compression
+gzip compressed data, was "dist/gitlabdata-0.3.9.tar", last modified: Fri Nov 26 16:45:49 2021, max compression
```

## Comparing `gitlabdata-0.3.8.tar` & `gitlabdata-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/
--rw-r--r--   0 root         (0) root         (0)      764 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      585 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      764 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       58 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      391 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      231 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2786 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/tests/test_orchestration_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 14:41:50.000000 gitlabdata-0.3.8/gitlabdata/
--rw-rw-rw-   0 root         (0) root         (0)     9496 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/gitlabdata/orchestration_utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-26 14:41:48.000000 gitlabdata-0.3.8/gitlabdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/
+-rw-r--r--   0 root         (0) root         (0)      764 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      585 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      764 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)      391 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      231 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/tests/test_orchestration_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-26 16:45:49.000000 gitlabdata-0.3.9/gitlabdata/
+-rw-rw-rw-   0 root         (0) root         (0)     9381 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/gitlabdata/orchestration_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-11-26 16:45:47.000000 gitlabdata-0.3.9/gitlabdata/__init__.py
```

### Comparing `gitlabdata-0.3.8/PKG-INFO` & `gitlabdata-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabdata
-Version: 0.3.8
+Version: 0.3.9
 Summary: GitLab Data Utils
 Home-page: https://gitlab.com/gitlab-data/gitlab-data-utils
 Author: GitLab Data Team
 Author-email: data@gitlab.com
 License: UNKNOWN
 Description: ## Data Team
```

### Comparing `gitlabdata-0.3.8/setup.py` & `gitlabdata-0.3.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 requires = ["snowflake-sqlalchemy>=1.1.10", "pandas>=0.25.3", "pyyaml==5.4.1"]
 
 
 setup(
     name="gitlabdata",
-    version="0.3.8",
+    version="0.3.9",
     author="GitLab Data Team",
     author_email="data@gitlab.com",
     description="GitLab Data Utils",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/gitlab-data/gitlab-data-utils",
     packages=find_packages(),
```

### Comparing `gitlabdata-0.3.8/gitlabdata.egg-info/PKG-INFO` & `gitlabdata-0.3.9/gitlabdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabdata
-Version: 0.3.8
+Version: 0.3.9
 Summary: GitLab Data Utils
 Home-page: https://gitlab.com/gitlab-data/gitlab-data-utils
 Author: GitLab Data Team
 Author-email: data@gitlab.com
 License: UNKNOWN
 Description: ## Data Team
```

### Comparing `gitlabdata-0.3.8/tests/test_orchestration_utils.py` & `gitlabdata-0.3.9/tests/test_orchestration_utils.py`

 * *Files identical despite different names*

### Comparing `gitlabdata-0.3.8/gitlabdata/orchestration_utils.py` & `gitlabdata-0.3.9/gitlabdata/orchestration_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -249,33 +249,33 @@
     logging.basicConfig(stream=sys.stdout, level=20)
 
     try:
         connection = engine.connect()
 
         logging.info(f"Clearing {type} files from stage.")
         remove = connection.execute(remove_query)
-        logging.info(f"Succssfully run query: {remove.context.statement}")
+        logging.info(f"Query successfully run")
 
         logging.info("Writing to Snowflake.")
         results = connection.execute(put_query)
-        logging.info(f"Succssfully run query: {results.context.statement}")
+        logging.info(f"Query successfully run")
     finally:
         connection.close()
         engine.dispose()
 
     try:
         connection = engine.connect()
 
         logging.info(f"Copying to Table {table_path}.")
         copy_results = connection.execute(copy_query)
-        logging.info(f"Succssfully run query: {copy_results.context.statement}")
+        logging.info(f"Query successfully run")
 
         logging.info(f"Removing {file} from stage.")
         remove = connection.execute(remove_query)
-        logging.info(f"Succssfully run query: {remove.context.statement}")
+        logging.info(f"Query successfully run")
     finally:
         connection.close()
         engine.dispose()
 
 
 def push_to_xcom_file(xcom_json: Dict[Any, Any]) -> None:
     """
```

