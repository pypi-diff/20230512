# Comparing `tmp/dbt-ai-0.2.5.tar.gz` & `tmp/dbt-ai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.2.5.tar", last modified: Fri May 12 00:16:33 2023, max compression
+gzip compressed data, was "dbt-ai-0.2.6.tar", last modified: Fri May 12 00:19:25 2023, max compression
```

## Comparing `dbt-ai-0.2.5.tar` & `dbt-ai-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4217 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4017 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/dbt_ai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/ai.py
--rw-r--r--   0 root         (0) root         (0)     9524 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/dbt.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/helper.py
--rw-r--r--   0 root         (0) root         (0)     2247 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/main.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/py.typed
--rw-r--r--   0 root         (0) root         (0)      811 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/dbt_ai/templates/
--rw-r--r--   0 root         (0) root         (0)     3094 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/dbt_ai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4217 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      181 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:16:33.000000 dbt-ai-0.2.5/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1600 2023-05-12 00:16:25.000000 dbt-ai-0.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:16:33.185914 dbt-ai-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-12 00:15:33.000000 dbt-ai-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:19:25.688171 dbt-ai-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-05-12 00:19:25.684171 dbt-ai-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:19:25.684171 dbt-ai-0.2.6/dbt_ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/ai.py
+-rw-r--r--   0 root         (0) root         (0)     9524 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/dbt.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/helper.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/main.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/py.typed
+-rw-r--r--   0 root         (0) root         (0)      811 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:19:25.684171 dbt-ai-0.2.6/dbt_ai/templates/
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 00:19:25.684171 dbt-ai-0.2.6/dbt_ai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      384 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:19:25.000000 dbt-ai-0.2.6/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-05-12 00:19:17.000000 dbt-ai-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 00:19:25.688171 dbt-ai-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-12 00:18:22.000000 dbt-ai-0.2.6/setup.py
```

### Comparing `dbt-ai-0.2.5/LICENSE` & `dbt-ai-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/PKG-INFO` & `dbt-ai-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.2.5
+Version: 0.2.6
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DBT AI
```

### Comparing `dbt-ai-0.2.5/README.md` & `dbt-ai-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/ai.py` & `dbt-ai-0.2.6/dbt_ai/ai.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/dbt.py` & `dbt-ai-0.2.6/dbt_ai/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/helper.py` & `dbt-ai-0.2.6/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/main.py` & `dbt-ai-0.2.6/dbt_ai/main.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/report.py` & `dbt-ai-0.2.6/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai/templates/report_template.html` & `dbt-ai-0.2.6/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.2.5/dbt_ai.egg-info/PKG-INFO` & `dbt-ai-0.2.6/dbt_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-ai
-Version: 0.2.5
+Version: 0.2.6
 Summary: AI powered DBT helper application
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # DBT AI
```

### Comparing `dbt-ai-0.2.5/pyproject.toml` & `dbt-ai-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.2.5"
+version = "0.2.6"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

