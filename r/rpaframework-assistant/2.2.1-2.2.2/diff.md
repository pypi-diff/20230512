# Comparing `tmp/rpaframework_assistant-2.2.1.tar.gz` & `tmp/rpaframework_assistant-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_assistant-2.2.1.tar", max compression
+gzip compressed data, was "rpaframework_assistant-2.2.2.tar", max compression
```

## Comparing `rpaframework_assistant-2.2.1.tar` & `rpaframework_assistant-2.2.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-02-09 07:27:59.020329 rpaframework_assistant-2.2.1/LICENSE
--rw-r--r--   0        0        0      288 2023-02-09 07:27:59.020477 rpaframework_assistant-2.2.1/README.rst
--rw-r--r--   0        0        0    60522 2023-04-05 08:31:12.892324 rpaframework_assistant-2.2.1/RPA_Assistant.libspec
--rw-r--r--   0        0        0     2456 2023-04-05 08:25:25.430515 rpaframework_assistant-2.2.1/pyproject.toml
--rw-r--r--   0        0        0       94 2023-03-08 07:24:21.287143 rpaframework_assistant-2.2.1/src/RPA/Assistant/__init__.py
--rw-r--r--   0        0        0     3387 2023-04-05 07:04:25.280100 rpaframework_assistant-2.2.1/src/RPA/Assistant/background_flet.py
--rw-r--r--   0        0        0     5168 2023-04-05 07:04:25.280288 rpaframework_assistant-2.2.1/src/RPA/Assistant/callback_runner.py
--rw-r--r--   0        0        0    11936 2023-04-05 07:04:25.280562 rpaframework_assistant-2.2.1/src/RPA/Assistant/flet_client.py
--rw-r--r--   0        0        0    52976 2023-04-05 07:04:25.281059 rpaframework_assistant-2.2.1/src/RPA/Assistant/library.py
--rw-r--r--   0        0        0     1530 2023-03-10 06:28:54.269842 rpaframework_assistant-2.2.1/src/RPA/Assistant/types.py
--rw-r--r--   0        0        0     3646 2023-03-10 06:28:54.270004 rpaframework_assistant-2.2.1/src/RPA/Assistant/utils.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 rpaframework_assistant-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-02-08 14:04:37.406505 rpaframework_assistant-2.2.2/LICENSE
+-rw-r--r--   0        0        0      288 2023-02-08 14:04:37.406609 rpaframework_assistant-2.2.2/README.rst
+-rw-r--r--   0        0        0     2456 2023-05-12 07:53:19.051682 rpaframework_assistant-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-03-02 10:36:58.328764 rpaframework_assistant-2.2.2/src/RPA/Assistant/__init__.py
+-rw-r--r--   0        0        0     3387 2023-04-04 10:42:49.583449 rpaframework_assistant-2.2.2/src/RPA/Assistant/background_flet.py
+-rw-r--r--   0        0        0     5168 2023-04-04 10:42:49.583708 rpaframework_assistant-2.2.2/src/RPA/Assistant/callback_runner.py
+-rw-r--r--   0        0        0    11936 2023-04-04 10:42:49.584044 rpaframework_assistant-2.2.2/src/RPA/Assistant/flet_client.py
+-rw-r--r--   0        0        0    52984 2023-05-12 07:53:48.535675 rpaframework_assistant-2.2.2/src/RPA/Assistant/library.py
+-rw-r--r--   0        0        0     1530 2023-03-14 14:53:39.551068 rpaframework_assistant-2.2.2/src/RPA/Assistant/types.py
+-rw-r--r--   0        0        0     3646 2023-03-14 09:01:07.895769 rpaframework_assistant-2.2.2/src/RPA/Assistant/utils.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 rpaframework_assistant-2.2.2/PKG-INFO
```

### Comparing `rpaframework_assistant-2.2.1/LICENSE` & `rpaframework_assistant-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/pyproject.toml` & `rpaframework_assistant-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-assistant"
-version = "2.2.1"
+version = "2.2.2"
 description = "Interactive UI library for RPA Framework"
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
```

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/background_flet.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/background_flet.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/callback_runner.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/callback_runner.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/flet_client.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/flet_client.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/library.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
         Input form dialog
             Add heading       Send feedback
             Add text input    email    label=E-mail address
             Add text input    message
             ...    label=Feedback
             ...    placeholder=Enter feedback here
-            ...    rows=5
+            ...    maximum_rows=5
             ${result}=    Run dialog
             Send feedback message    ${result.email}  ${result.message}
     """
 
     def __init__(self) -> None:
         self.logger = logging.getLogger(__name__)
         os.environ["FLET_LOG_LEVEL"] = "warning"
```

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/types.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/types.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/src/RPA/Assistant/utils.py` & `rpaframework_assistant-2.2.2/src/RPA/Assistant/utils.py`

 * *Files identical despite different names*

### Comparing `rpaframework_assistant-2.2.1/PKG-INFO` & `rpaframework_assistant-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-assistant
-Version: 2.2.1
+Version: 2.2.2
 Summary: Interactive UI library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,dialogs,assistant
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.7,<4.0
```

