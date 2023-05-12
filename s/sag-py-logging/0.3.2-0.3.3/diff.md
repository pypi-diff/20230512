# Comparing `tmp/sag-py-logging-0.3.2.tar.gz` & `tmp/sag-py-logging-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sag-py-logging-0.3.2.tar", last modified: Sat May  6 07:49:28 2023, max compression
+gzip compressed data, was "sag-py-logging-0.3.3.tar", last modified: Fri May 12 12:00:09 2023, max compression
```

## Comparing `sag-py-logging-0.3.2.tar` & `sag-py-logging-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/sag_py_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/log_config_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/sag_py_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/sag_py_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 07:49:28.000000 sag-py-logging-0.3.2/sag_py_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:49:28.469739 sag-py-logging-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_console_extra_field_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-06 07:49:16.000000 sag-py-logging-0.3.2/tests/test_log_config_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/sag_py_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/log_config_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/sag_py_logging/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/sag_py_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 12:00:09.000000 sag-py-logging-0.3.3/sag_py_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:00:09.022979 sag-py-logging-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_console_extra_field_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-12 12:00:00.000000 sag-py-logging-0.3.3/tests/test_log_config_processors.py
```

### Comparing `sag-py-logging-0.3.2/LICENSE.txt` & `sag-py-logging-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/PKG-INFO` & `sag-py-logging-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.2
+Version: 0.3.3
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
```

### Comparing `sag-py-logging-0.3.2/README.md` & `sag-py-logging-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/sag_py_logging/console_extra_field_filter.py` & `sag-py-logging-0.3.3/sag_py_logging/console_extra_field_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             "threadName",
             "logsource",
             "program",
             "type",
             "tags",
             "@metadata",
             "color_message",
+            "stringified_extra",
         }
 
     def filter(self, record: logging.LogRecord) -> bool:
         extra_fields: Dict[str, Any] = self._get_extra_fields(record)
         extra_list: List[str] = self._to_key_value_strings(extra_fields)
         record.stringified_extra = ", ".join(extra_list)
         return True
```

### Comparing `sag-py-logging-0.3.2/sag_py_logging/log_config_initializer.py` & `sag-py-logging-0.3.3/sag_py_logging/log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/sag_py_logging/log_config_loader.py` & `sag-py-logging-0.3.3/sag_py_logging/log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/sag_py_logging/log_config_processors.py` & `sag-py-logging-0.3.3/sag_py_logging/log_config_processors.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/sag_py_logging.egg-info/PKG-INFO` & `sag-py-logging-0.3.3/sag_py_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sag-py-logging
-Version: 0.3.2
+Version: 0.3.3
 Summary: Initialize logging from a configuration json
 Home-page: https://github.com/SamhammerAG/sag_py_logging
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/sag_py_logging
 Project-URL: Bug Reports, https://github.com/SamhammerAG/sag_py_logging/issues
```

### Comparing `sag-py-logging-0.3.2/sag_py_logging.egg-info/SOURCES.txt` & `sag-py-logging-0.3.3/sag_py_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/setup.py` & `sag-py-logging-0.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 JINJA_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require jinia" in item]
 TOMLI_EXTRA = [item.split(" #", 1)[0] for item in REQS_DEV if "# extras_require tomli" in item]
 
 setuptools.setup(
     name="sag-py-logging",
-    version="0.3.2",
+    version="0.3.3",
     description="Initialize logging from a configuration json",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/sag_py_logging",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `sag-py-logging-0.3.2/tests/test_console_extra_field_filter.py` & `sag-py-logging-0.3.3/tests/test_console_extra_field_filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,7 +42,32 @@
         cast(ExtraFieldsLogRecord, log_record).stringified_extra == 'my_extra_string="test", '
         "my_extra_int=1, "
         "my_extra_bool=true, "
         'my_extra_dict_object={"keyOne": "valueOne", "keyTwo": 2}, '
         'my_extra_not_serializable_object={"testtext": "test"}, '
         "my_extra_object_without_dict=ClassWithoutDict(x=123, y=456)"
     )
+
+
+def test_with_extra_fields_when_called_twice(log_record: LogRecord) -> None:
+    # Arrange
+    filter_ = ConsoleExtraFieldFilter()
+    log_record.my_extra_string = "test"
+    log_record.my_extra_int = 1
+    log_record.my_extra_bool = True
+    log_record.my_extra_dict_object = {"keyOne": "valueOne", "keyTwo": 2}
+    log_record.my_extra_not_serializable_object = NotSerializableClass("test")
+    log_record.my_extra_object_without_dict = ClassWithoutDict(x=123, y=456)
+
+    # Act
+    filter_.filter(log_record)
+    filter_.filter(log_record)
+
+    # Assert
+    assert (
+        cast(ExtraFieldsLogRecord, log_record).stringified_extra == 'my_extra_string="test", '
+        "my_extra_int=1, "
+        "my_extra_bool=true, "
+        'my_extra_dict_object={"keyOne": "valueOne", "keyTwo": 2}, '
+        'my_extra_not_serializable_object={"testtext": "test"}, '
+        "my_extra_object_without_dict=ClassWithoutDict(x=123, y=456)"
+    )
```

### Comparing `sag-py-logging-0.3.2/tests/test_log_config_initializer.py` & `sag-py-logging-0.3.3/tests/test_log_config_initializer.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/tests/test_log_config_loader.py` & `sag-py-logging-0.3.3/tests/test_log_config_loader.py`

 * *Files identical despite different names*

### Comparing `sag-py-logging-0.3.2/tests/test_log_config_processors.py` & `sag-py-logging-0.3.3/tests/test_log_config_processors.py`

 * *Files identical despite different names*

