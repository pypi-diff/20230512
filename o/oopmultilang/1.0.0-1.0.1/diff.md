# Comparing `tmp/oopmultilang-1.0.0.tar.gz` & `tmp/oopmultilang-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oopmultilang-1.0.0.tar", max compression
+gzip compressed data, was "oopmultilang-1.0.1.tar", max compression
```

## Comparing `oopmultilang-1.0.0.tar` & `oopmultilang-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 oopmultilang-1.0.0/LICENSE
--rw-r--r--   0        0        0      157 2023-05-07 06:50:29.394145 oopmultilang-1.0.0/oopmultilang/__init__.py
--rw-r--r--   0        0        0     2622 2023-05-07 05:07:35.877185 oopmultilang-1.0.0/oopmultilang/_errors.py
--rw-r--r--   0        0        0     1501 2023-05-07 05:07:35.882169 oopmultilang-1.0.0/oopmultilang/_lang_dict_parser.py
--rw-r--r--   0        0        0     7620 2023-05-07 06:50:29.397145 oopmultilang-1.0.0/oopmultilang/lang_switcher.py
--rw-r--r--   0        0        0      572 2023-05-07 05:54:22.364140 oopmultilang-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1398 2023-05-07 05:25:45.827359 oopmultilang-1.0.0/README.md
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 oopmultilang-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 oopmultilang-1.0.1/LICENSE
+-rw-r--r--   0        0        0      157 2023-05-07 06:50:29.394145 oopmultilang-1.0.1/oopmultilang/__init__.py
+-rw-r--r--   0        0        0     2622 2023-05-07 05:07:35.877185 oopmultilang-1.0.1/oopmultilang/_errors.py
+-rw-r--r--   0        0        0     1501 2023-05-07 05:07:35.882169 oopmultilang-1.0.1/oopmultilang/_lang_dict_parser.py
+-rw-r--r--   0        0        0     7594 2023-05-12 14:08:19.489799 oopmultilang-1.0.1/oopmultilang/lang_switcher.py
+-rw-r--r--   0        0        0      572 2023-05-12 14:10:35.605659 oopmultilang-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1398 2023-05-07 05:25:45.827359 oopmultilang-1.0.1/README.md
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 oopmultilang-1.0.1/PKG-INFO
```

### Comparing `oopmultilang-1.0.0/LICENSE` & `oopmultilang-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oopmultilang-1.0.0/oopmultilang/_errors.py` & `oopmultilang-1.0.1/oopmultilang/_errors.py`

 * *Files identical despite different names*

### Comparing `oopmultilang-1.0.0/oopmultilang/_lang_dict_parser.py` & `oopmultilang-1.0.1/oopmultilang/_lang_dict_parser.py`

 * *Files identical despite different names*

### Comparing `oopmultilang-1.0.0/oopmultilang/lang_switcher.py` & `oopmultilang-1.0.1/oopmultilang/lang_switcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,57 +52,63 @@
         self.__m_dict = {}
         self._m_load_mode = load_mode
 
         # None represents the universal word.
         self.__m_default_source_lang = None
         self.__m_default_target_lang = None
 
-        if len(include) != 0:
+        # Avoid parsing a tuple with only one element as a single string.
+        if isinstance(include, tuple):
             for expression in include:
-                """
-                Parses expressions imported into language dictionaries via param<include>.
+                self.__parse_expression(expression)
+        else:
+            self.__parse_expression(include)
+
+        # One-time loading mode.
+        if self._m_load_mode == LoadMode.ONETIME:
+            self.__load_lang_dict()
 
-                There are two forms of this expression, one is full and the other is short.
+    def __parse_expression(self,expression):
+        """
+        Parses expressions imported into language dictionaries via param<include>.
 
-                For example:
+        There are two forms of this expression, one is full and the other is short.
 
-                1. ``full``: './en_us.lang as en_us'
-                2. ``short``: './en_us.lang'
+        For example:
 
-                Note that when using the short form, the name of the associated language will be the name of the file.
+        1. ``full``: './en_us.lang as en_us'
+        2. ``short``: './en_us.lang'
+
+        Note that when using the short form, the name of the associated language will be the name of the file.
+        """
+        if expression.find("as") != -1:
+            if expression.count("as") == 1:
                 """
-                if expression.find("as") != -1:
-                    if expression.count("as") == 1:
-                        """
-                        A list of strings representing the distinct terms of the expression after it is parsed.
-                        
-                        - ``expression_parsing[0]``: The file path of the language dictionary.
-                        - ``expression_parsing[1]``: The associated language of the language dictionary.
-                        """
-                        expression_parsing = [expression_unit.strip() for expression_unit in expression.split("as")]
-                        dictionary_file = File(expression_parsing[0], False, False)
-                        dictionary_associated_lang = expression_parsing[1]
-                    else:
-                        raise ExpressionError(expression)
-                else:
-                    dictionary_file = File(expression, False, False)
-                    dictionary_associated_lang = dictionary_file.info["name"]
-
-                # Store language dictionary file information for different languages into member:private<self.__m_dict>.
-                if not dictionary_file.state["exist"]:
-                    raise FileNotFoundError("Language dictionary not found: " + dictionary_file.info["path"])
-                else:
-                    if dictionary_associated_lang in self.__m_dict.keys():
-                        self.__m_dict[dictionary_associated_lang].append(dictionary_file.info["path"])
-                    else:
-                        self.__m_dict[dictionary_associated_lang] = [dictionary_file.info["path"]]
+                A list of strings representing the distinct terms of the expression after it is parsed.
 
-        # One-time loading mode.
-        if self._m_load_mode == LoadMode.ONETIME:
-            self.__load_lang_dict()
+                - ``expression_parsing[0]``: The file path of the language dictionary.
+                - ``expression_parsing[1]``: The associated language of the language dictionary.
+                """
+                expression_parsing = [expression_unit.strip() for expression_unit in expression.split("as")]
+                dictionary_file = File(expression_parsing[0], False, False)
+                dictionary_associated_lang = expression_parsing[1]
+            else:
+                raise ExpressionError(expression)
+        else:
+            dictionary_file = File(expression, False, False)
+            dictionary_associated_lang = dictionary_file.info["name"]
+
+        # Store language dictionary file information for different languages into member:private<self.__m_dict>.
+        if not dictionary_file.state["exist"]:
+            raise FileNotFoundError("Language dictionary not found: " + dictionary_file.info["path"])
+        else:
+            if dictionary_associated_lang in self.__m_dict.keys():
+                self.__m_dict[dictionary_associated_lang].append(dictionary_file.info["path"])
+            else:
+                self.__m_dict[dictionary_associated_lang] = [dictionary_file.info["path"]]
 
     def __load_lang_dict(self):
         new_dict = self.__m_dict.copy()
         for dictionary_associated_lang, dictionary in self.__m_dict.items():
             if isinstance(dictionary, list):  # Indicates that var<dictionary> is a list of lang dict file path.
                 new_dict[dictionary_associated_lang] = {}
                 for dictionary_file_path in dictionary:
```

### Comparing `oopmultilang-1.0.0/pyproject.toml` & `oopmultilang-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oopmultilang"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python package that supports multi-language conversion of the object-oriented paradigm."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-OOPMultilang"
 classifiers = [
     "Development Status :: 3 - Alpha"
```

### Comparing `oopmultilang-1.0.0/README.md` & `oopmultilang-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oopmultilang-1.0.0/PKG-INFO` & `oopmultilang-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopmultilang
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package that supports multi-language conversion of the object-oriented paradigm.
 Home-page: https://github.com/leoweyr/Python-OOPMultilang
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

