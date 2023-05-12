# Comparing `tmp/apidevtools-3.2.6.tar.gz` & `tmp/apidevtools-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.2.6.tar", last modified: Fri May 12 15:47:05 2023, max compression
+gzip compressed data, was "apidevtools-3.2.7.tar", last modified: Fri May 12 16:02:39 2023, max compression
```

## Comparing `apidevtools-3.2.6.tar` & `apidevtools-3.2.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.315754 apidevtools-3.2.6/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-05-12 15:47:05.314754 apidevtools-3.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.6/README.md
--rw-rw-rw-   0        0        0     1772 2023-05-12 15:46:50.000000 apidevtools-3.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 15:47:05.315754 apidevtools-3.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.279750 apidevtools-3.2.6/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.282782 apidevtools-3.2.6/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.6/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0     1718 2023-05-12 15:46:30.000000 apidevtools-3.2.6/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.299751 apidevtools-3.2.6/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.2.6/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.6/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-05-12 15:12:51.000000 apidevtools-3.2.6/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.6/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.301750 apidevtools-3.2.6/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.6/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.6/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.6/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.305751 apidevtools-3.2.6/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.310750 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.313754 apidevtools-3.2.6/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.6/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.2.6/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:47:05.295751 apidevtools-3.2.6/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-05-12 15:47:05.000000 apidevtools-3.2.6/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1012 2023-05-12 15:47:05.000000 apidevtools-3.2.6/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 15:47:05.000000 apidevtools-3.2.6/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-12 15:47:05.000000 apidevtools-3.2.6/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.309715 apidevtools-3.2.7/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-05-12 16:02:39.309715 apidevtools-3.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.7/README.md
+-rw-rw-rw-   0        0        0     1772 2023-05-12 16:02:05.000000 apidevtools-3.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 16:02:39.309715 apidevtools-3.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.277714 apidevtools-3.2.7/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.280714 apidevtools-3.2.7/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.7/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0     1718 2023-05-12 15:46:30.000000 apidevtools-3.2.7/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.295714 apidevtools-3.2.7/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.2.7/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.7/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.2.7/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.7/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.298715 apidevtools-3.2.7/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.7/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.7/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.7/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.301714 apidevtools-3.2.7/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.305714 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.307744 apidevtools-3.2.7/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.7/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.2.7/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 16:02:39.291714 apidevtools-3.2.7/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-05-12 16:02:39.000000 apidevtools-3.2.7/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1012 2023-05-12 16:02:39.000000 apidevtools-3.2.7/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 16:02:39.000000 apidevtools-3.2.7/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-12 16:02:39.000000 apidevtools-3.2.7/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.2.6/LICENSE.txt` & `apidevtools-3.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/PKG-INFO` & `apidevtools-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.6
+Version: 3.2.7
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.6/README.md` & `apidevtools-3.2.7/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/pyproject.toml` & `apidevtools-3.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.2.6"
+version = "3.2.7"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
```

### Comparing `apidevtools-3.2.6/src/apidevtools/logman.py` & `apidevtools-3.2.7/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.2.7/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/media/imgproc.py` & `apidevtools-3.2.7/src/apidevtools/media/imgproc.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     :param bg_color:
     :param font_color:
     :return:
     """
     if not fonttf:
         from os import path
 
-        fonttf = path.join(path.basename(__file__), 'ARIALNB.TTF')
+        fonttf = path.join(path.dirname(__file__), 'ARIALNB.TTF')
 
     font = _ImageFont.truetype(font=fonttf, size=int(size * 0.6))
     img = PIL.Image.new(mode='RGB', size=(size, size), color=bg_color)
     draw = _ImageDraw.Draw(img)
     _, _, width, height = draw.textbbox((0, 0), text, font=font)
     draw.text(xy=((size - width) / 2, (size - height) / 3), text=text, font=font, fill=font_color)
     return Image(img, text)
```

### Comparing `apidevtools-3.2.6/src/apidevtools/media/telegraph.py` & `apidevtools-3.2.7/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/security/encryptor.py` & `apidevtools-3.2.7/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/security/hasher.py` & `apidevtools-3.2.7/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.2.7/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools/utils.py` & `apidevtools-3.2.7/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.6/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.2.7/src/apidevtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.6
+Version: 3.2.7
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.6/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.2.7/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

