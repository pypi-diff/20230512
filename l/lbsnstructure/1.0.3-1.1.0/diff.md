# Comparing `tmp/lbsnstructure-1.0.3.tar.gz` & `tmp/lbsnstructure-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbsnstructure-1.0.3.tar", last modified: Thu May  4 09:03:13 2023, max compression
+gzip compressed data, was "lbsnstructure-1.1.0.tar", last modified: Fri May 12 10:28:26 2023, max compression
```

## Comparing `lbsnstructure-1.0.3.tar` & `lbsnstructure-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.703335 lbsnstructure-1.0.3/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/.gitignore
--rwxrwxrwx   0 alex      (1000) alex      (1000)     1553 2020-02-28 07:54:54.000000 lbsnstructure-1.0.3/.gitlab-ci.yml
--rw-r--r--   0 alex      (1000) alex      (1000)      954 2023-05-04 09:03:09.000000 lbsnstructure-1.0.3/CHANGELOG.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.0.3/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2993 2023-05-04 09:03:13.703335 lbsnstructure-1.0.3/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)     2655 2019-10-21 11:34:47.000000 lbsnstructure-1.0.3/README.md
--rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/StructureTest.ipynb
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.583050 lbsnstructure-1.0.3/google/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.617210 lbsnstructure-1.0.3/google/protobuf/
--rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/google/protobuf/duration_pb2.py
--rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/google/protobuf/timestamp_pb2.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.689664 lbsnstructure-1.0.3/lbsnstructure/
--rw-rw-rw-   0 alex      (1000) alex      (1000)      425 2023-05-04 09:00:50.000000 lbsnstructure-1.0.3/lbsnstructure/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/interlinkage_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/social_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/spatial_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/temporal_pb2.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5006 2023-05-04 08:22:28.000000 lbsnstructure-1.0.3/lbsnstructure/topical_pb2.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)       67 2023-05-04 09:03:09.000000 lbsnstructure-1.0.3/lbsnstructure/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 09:03:13.700144 lbsnstructure-1.0.3/lbsnstructure.egg-info/
--rw-rw-rw-   0 alex      (1000) alex      (1000)     2993 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/PKG-INFO
--rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/SOURCES.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/dependency_links.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/not-zip-safe
--rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/requires.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-04 09:03:13.000000 lbsnstructure-1.0.3/lbsnstructure.egg-info/top_level.txt
--rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-04 09:03:13.705952 lbsnstructure-1.0.3/setup.cfg
--rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.0.3/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.895713 lbsnstructure-1.1.0/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1227 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/.gitignore
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      807 2023-05-04 10:44:19.000000 lbsnstructure-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 alex      (1000) alex      (1000)     1655 2023-05-12 10:28:17.000000 lbsnstructure-1.1.0/CHANGELOG.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1121 2019-07-11 10:53:20.000000 lbsnstructure-1.1.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     3115 2023-05-12 10:28:26.896134 lbsnstructure-1.1.0/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     2778 2023-05-10 06:12:09.000000 lbsnstructure-1.1.0/README.md
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     4124 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/StructureTest.ipynb
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.644081 lbsnstructure-1.1.0/google/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.744611 lbsnstructure-1.1.0/google/protobuf/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1625 2023-05-12 09:14:33.000000 lbsnstructure-1.1.0/google/protobuf/duration_pb2.py
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     1641 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/google/protobuf/timestamp_pb2.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.870633 lbsnstructure-1.1.0/lbsnstructure/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      425 2023-05-04 09:00:50.000000 lbsnstructure-1.1.0/lbsnstructure/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2703 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/interlinkage_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5527 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/social_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4172 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/spatial_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2693 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/temporal_pb2.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5116 2023-05-12 09:14:32.000000 lbsnstructure-1.1.0/lbsnstructure/topical_pb2.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       22 2023-05-12 10:28:17.000000 lbsnstructure-1.1.0/lbsnstructure/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-12 10:28:26.893125 lbsnstructure-1.1.0/lbsnstructure.egg-info/
+-rw-rw-rw-   0 alex      (1000) alex      (1000)     3115 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/PKG-INFO
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      584 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        1 2019-07-11 11:04:14.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/not-zip-safe
+-rw-rw-rw-   0 alex      (1000) alex      (1000)        9 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/requires.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)       14 2023-05-12 10:28:25.000000 lbsnstructure-1.1.0/lbsnstructure.egg-info/top_level.txt
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      114 2023-05-12 10:28:26.898553 lbsnstructure-1.1.0/setup.cfg
+-rw-rw-rw-   0 alex      (1000) alex      (1000)      909 2019-07-11 09:18:07.000000 lbsnstructure-1.1.0/setup.py
```

### Comparing `lbsnstructure-1.0.3/.gitignore` & `lbsnstructure-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/CHANGELOG.md` & `lbsnstructure-1.1.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.1.0 (2023-05-12)
+### Documentation
+* Fix pipeline badge url ([`0d4656e`](https://github.com/Sieboldianus/lbsnstructure-python/commit/0d4656e30ea3daaddd633348a2cfb169948f18b4))
+* Clarify difference between python compiled and protobuf upstream version ([`c8ce5f5`](https://github.com/Sieboldianus/lbsnstructure-python/commit/c8ce5f5b4e997f2b224790585d71b7dac32c4a97))
+* Clarify difference between python compiled and protobuf upstream version ([`ee76ba8`](https://github.com/Sieboldianus/lbsnstructure-python/commit/ee76ba83ad8b2dd589bb166e103d0dd6a6197db7))
+* Update references ([`1b6e8a0`](https://github.com/Sieboldianus/lbsnstructure-python/commit/1b6e8a0e3f0e61f9c547bb07177e8a747a56ebb7))
+
 ## v1.0.3 (2023-05-04)
 ### Fix
 * Make objects available in top-level namespace ([`9acb38b`](https://github.com/Sieboldianus/lbsnstructure-python/commit/9acb38b31544958daafc67ab358acd0e1cb1d4b1))
 
 ## v1.0.2 (2023-05-04)
 ### Fix
 * Version import path ([`4a11a9a`](https://github.com/Sieboldianus/lbsnstructure-python/commit/4a11a9a1a2bd498c8b2c9b2654752b1f6ffadb90))
```

### Comparing `lbsnstructure-1.0.3/LICENSE.md` & `lbsnstructure-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/PKG-INFO` & `lbsnstructure-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.3
+Version: 1.1.0
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
+![pypi version](https://lbsn.vgiscience.org/structure/python/version.svg) ![pipeline status](https://gitlab.vgiscience.de/lbsn/structure/python/badges/master/pipeline.svg) from protobuf: ![version](https://lbsn.vgiscience.org/structure/protobuf/version.svg) 
 
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
@@ -24,36 +24,37 @@
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
 Import to python projecty with:  
 ```python
-import lbsnstructure
-from lbsnstructure.lbsnstructure_pb2 import lbsnPost
+import lbsnstructure as lbsn
+post = lbsn.Post()
+place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
 
 1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
 2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
 3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
 4. Install with `pip install .` in examples/python
 
 ## Developers
 
 For development & testing, make a local clone of this repository  
 ```shell
-git clone git@gitlab.vgiscience.de:lbsn/concept.git
+git clone git@gitlab.vgiscience.de:lbsn/structure/python.git
 ```
 
 Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
 Python's site-packages folder with:  
 ```shell
-python setup.py develop
+pip install --editable .
 ```
 
 Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
 
 ## Versioning
 
 For the releases available, see the [tags on this repository](/../tags).
```

### Comparing `lbsnstructure-1.0.3/README.md` & `lbsnstructure-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
+![pypi version](https://lbsn.vgiscience.org/structure/python/version.svg) ![pipeline status](https://gitlab.vgiscience.de/lbsn/structure/python/badges/master/pipeline.svg) from protobuf: ![version](https://lbsn.vgiscience.org/structure/protobuf/version.svg) 
 
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
@@ -12,36 +12,37 @@
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
 Import to python projecty with:  
 ```python
-import lbsnstructure
-from lbsnstructure.lbsnstructure_pb2 import lbsnPost
+import lbsnstructure as lbsn
+post = lbsn.Post()
+place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
 
 1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
 2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
 3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
 4. Install with `pip install .` in examples/python
 
 ## Developers
 
 For development & testing, make a local clone of this repository  
 ```shell
-git clone git@gitlab.vgiscience.de:lbsn/concept.git
+git clone git@gitlab.vgiscience.de:lbsn/structure/python.git
 ```
 
 Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
 Python's site-packages folder with:  
 ```shell
-python setup.py develop
+pip install --editable .
 ```
 
 Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
 
 ## Versioning
 
 For the releases available, see the [tags on this repository](/../tags).
```

### Comparing `lbsnstructure-1.0.3/StructureTest.ipynb` & `lbsnstructure-1.1.0/StructureTest.ipynb`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/google/protobuf/duration_pb2.py` & `lbsnstructure-1.1.0/google/protobuf/duration_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/google/protobuf/timestamp_pb2.py` & `lbsnstructure-1.1.0/google/protobuf/timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/lbsnstructure/interlinkage_pb2.py` & `lbsnstructure-1.1.0/lbsnstructure/interlinkage_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/lbsnstructure/social_pb2.py` & `lbsnstructure-1.1.0/lbsnstructure/social_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/lbsnstructure/spatial_pb2.py` & `lbsnstructure-1.1.0/lbsnstructure/spatial_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/lbsnstructure/temporal_pb2.py` & `lbsnstructure-1.1.0/lbsnstructure/temporal_pb2.py`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/lbsnstructure/topical_pb2.py` & `lbsnstructure-1.1.0/lbsnstructure/topical_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from lbsnstructure import social_pb2 as lbsnstructure_dot_social__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1blbsnstructure/topical.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1albsnstructure/social.proto\"\xa0\x08\n\x04Post\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x13\n\x0bpost_latlng\x18\x02 \x01(\t\x12\x30\n\nplace_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tcity_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x32\n\x0c\x63ountry_pkey\x18\x05 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x35\n\x11post_publish_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tpost_body\x18\x08 \x01(\t\x12>\n\x10post_geoaccuracy\x18\t \x01(\x0e\x32$.lbsn.structure.Post.PostGeoaccuracy\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x10\n\x08hashtags\x18\x0b \x03(\t\x12\r\n\x05\x65moji\x18\x0c \x03(\t\x12\x17\n\x0fpost_like_count\x18\r \x01(\x03\x12\x1a\n\x12post_comment_count\x18\x0e \x01(\x03\x12\x18\n\x10post_views_count\x18\x0f \x01(\x03\x12\x12\n\npost_title\x18\x10 \x01(\t\x12\x34\n\x10post_create_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12post_thumbnail_url\x18\x12 \x01(\t\x12\x10\n\x08post_url\x18\x13 \x01(\t\x12\x30\n\tpost_type\x18\x14 \x01(\x0e\x32\x1d.lbsn.structure.Post.PostType\x12\x13\n\x0bpost_filter\x18\x15 \x01(\t\x12\x18\n\x10post_quote_count\x18\x16 \x01(\x03\x12\x18\n\x10post_share_count\x18\x17 \x01(\x03\x12\x14\n\x0cinput_source\x18\x18 \x01(\t\x12/\n\rpost_language\x18\x19 \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x1c\n\x14post_content_license\x18\x1a \x01(\x05\"L\n\x0fPostGeoaccuracy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LATLNG\x10\x01\x12\t\n\x05PLACE\x10\x02\x12\x08\n\x04\x43ITY\x10\x03\x12\x0b\n\x07\x43OUNTRY\x10\x04\"5\n\x08PostType\x12\x08\n\x04TEXT\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\t\n\x05VIDEO\x10\x02\x12\t\n\x05OTHER\x10\x03\"\xc8\x04\n\x0cPostReaction\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x02 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x39\n\x13referencedPost_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x41\n\x1breferencedPostreaction_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x17\n\x0freaction_latlng\x18\x05 \x01(\t\x12@\n\rreaction_type\x18\x06 \x01(\x0e\x32).lbsn.structure.PostReaction.ReactionType\x12\x31\n\rreaction_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10reaction_content\x18\x08 \x01(\t\x12\x1b\n\x13reaction_like_count\x18\t \x01(\x03\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\"^\n\x0cReactionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05SHARE\x10\x01\x12\x0b\n\x07\x43OMMENT\x10\x02\x12\t\n\x05QUOTE\x10\x03\x12\x08\n\x04LIKE\x10\x04\x12\t\n\x05\x45MOJI\x10\x05\x12\t\n\x05OTHER\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1blbsnstructure/topical.proto\x12\x0elbsn.structure\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1albsnstructure/social.proto\"\xd6\x08\n\x04Post\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x13\n\x0bpost_latlng\x18\x02 \x01(\t\x12\x30\n\nplace_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tcity_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x32\n\x0c\x63ountry_pkey\x18\x05 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x06 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x35\n\x11post_publish_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\tpost_body\x18\x08 \x01(\t\x12>\n\x10post_geoaccuracy\x18\t \x01(\x0e\x32$.lbsn.structure.Post.PostGeoaccuracy\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x10\n\x08hashtags\x18\x0b \x03(\t\x12\r\n\x05\x65moji\x18\x0c \x03(\t\x12\x17\n\x0fpost_like_count\x18\r \x01(\x03\x12\x1a\n\x12post_comment_count\x18\x0e \x01(\x03\x12\x18\n\x10post_views_count\x18\x0f \x01(\x03\x12\x12\n\npost_title\x18\x10 \x01(\t\x12\x34\n\x10post_create_date\x18\x11 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1a\n\x12post_thumbnail_url\x18\x12 \x01(\t\x12\x10\n\x08post_url\x18\x13 \x01(\t\x12\x30\n\tpost_type\x18\x14 \x01(\x0e\x32\x1d.lbsn.structure.Post.PostType\x12\x13\n\x0bpost_filter\x18\x15 \x01(\t\x12\x18\n\x10post_quote_count\x18\x16 \x01(\x03\x12\x18\n\x10post_share_count\x18\x17 \x01(\x03\x12\x14\n\x0cinput_source\x18\x18 \x01(\t\x12/\n\rpost_language\x18\x19 \x01(\x0b\x32\x18.lbsn.structure.Language\x12\x1c\n\x14post_content_license\x18\x1a \x01(\x05\x12\x12\n\npost_topic\x18\x1b \x03(\t\x12\x16\n\x0epost_downvotes\x18\x1c \x01(\x03\"L\n\x0fPostGeoaccuracy\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LATLNG\x10\x01\x12\t\n\x05PLACE\x10\x02\x12\x08\n\x04\x43ITY\x10\x03\x12\x0b\n\x07\x43OUNTRY\x10\x04\"?\n\x08PostType\x12\x08\n\x04TEXT\x10\x00\x12\t\n\x05IMAGE\x10\x01\x12\t\n\x05VIDEO\x10\x02\x12\x08\n\x04LINK\x10\x03\x12\t\n\x05OTHER\x10\x04\"\xc8\x04\n\x0cPostReaction\x12*\n\x04pkey\x18\x01 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12/\n\tuser_pkey\x18\x02 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x39\n\x13referencedPost_pkey\x18\x03 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x41\n\x1breferencedPostreaction_pkey\x18\x04 \x01(\x0b\x32\x1c.lbsn.structure.CompositeKey\x12\x17\n\x0freaction_latlng\x18\x05 \x01(\t\x12@\n\rreaction_type\x18\x06 \x01(\x0e\x32).lbsn.structure.PostReaction.ReactionType\x12\x31\n\rreaction_date\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10reaction_content\x18\x08 \x01(\t\x12\x1b\n\x13reaction_like_count\x18\t \x01(\x03\x12\x38\n\x12user_mentions_pkey\x18\n \x03(\x0b\x32\x1c.lbsn.structure.CompositeKey\"^\n\x0cReactionType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05SHARE\x10\x01\x12\x0b\n\x07\x43OMMENT\x10\x02\x12\t\n\x05QUOTE\x10\x03\x12\x08\n\x04LIKE\x10\x04\x12\t\n\x05\x45MOJI\x10\x05\x12\t\n\x05OTHER\x10\x06\x62\x06proto3')
 
 
 
 _POST = DESCRIPTOR.message_types_by_name['Post']
 _POSTREACTION = DESCRIPTOR.message_types_by_name['PostReaction']
 _POST_POSTGEOACCURACY = _POST.enum_types_by_name['PostGeoaccuracy']
 _POST_POSTTYPE = _POST.enum_types_by_name['PostType']
@@ -39,17 +39,17 @@
   })
 _sym_db.RegisterMessage(PostReaction)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _POST._serialized_start=109
-  _POST._serialized_end=1165
-  _POST_POSTGEOACCURACY._serialized_start=1034
-  _POST_POSTGEOACCURACY._serialized_end=1110
-  _POST_POSTTYPE._serialized_start=1112
-  _POST_POSTTYPE._serialized_end=1165
-  _POSTREACTION._serialized_start=1168
-  _POSTREACTION._serialized_end=1752
-  _POSTREACTION_REACTIONTYPE._serialized_start=1658
-  _POSTREACTION_REACTIONTYPE._serialized_end=1752
+  _POST._serialized_end=1219
+  _POST_POSTGEOACCURACY._serialized_start=1078
+  _POST_POSTGEOACCURACY._serialized_end=1154
+  _POST_POSTTYPE._serialized_start=1156
+  _POST_POSTTYPE._serialized_end=1219
+  _POSTREACTION._serialized_start=1222
+  _POSTREACTION._serialized_end=1806
+  _POSTREACTION_REACTIONTYPE._serialized_start=1712
+  _POSTREACTION_REACTIONTYPE._serialized_end=1806
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lbsnstructure-1.0.3/lbsnstructure.egg-info/PKG-INFO` & `lbsnstructure-1.1.0/lbsnstructure.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lbsnstructure
-Version: 1.0.3
+Version: 1.1.0
 Summary: A common language independent and cross-network social-media data scheme.
 Home-page: https://gitlab.vgiscience.de/lbsn/concept
 Author: Filip Krumpe; Alexander Dunkel; Marc Löchner
 Author-email: alexander.dunkel@tu-dresden.de
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-![pypi version](https://lbsn.vgiscience.org/structure/python/pypi.svg) ![pipeline](https://lbsn.vgiscience.org/structure/python/pipeline.svg)
+![pypi version](https://lbsn.vgiscience.org/structure/python/version.svg) ![pipeline status](https://gitlab.vgiscience.de/lbsn/structure/python/badges/master/pipeline.svg) from protobuf: ![version](https://lbsn.vgiscience.org/structure/protobuf/version.svg) 
 
 # LBSNSTRUCTURE
 
 A python compiled version of the [common location based social network (LBSN) data structure concept](https://gitlab.vgiscience.de/lbsn/concept) (ProtoBuf) to handle cross network Social Media data in Python.
 There are several motivations for prividing a common LBSN interchange data structure. Firstly, the [GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) directly requests Social Media Network operators to allow users to transfer accounts and data inbetween services. 
 While there are attempts by Google, Facebook etc. (see [data-transfer-project](https://github.com/google/data-transfer-project)), it is not currently possible. With this structure concept, we follow an independent road.
 A primary goal is to systematically characterize LBSN data aspects in a common scheme that enables privacy-by-design for connected software, transfer scripts and database design.
@@ -24,36 +24,37 @@
 Install with:  
 ```shell
 pip install --upgrade lbsnstructure
 ```
 
 Import to python projecty with:  
 ```python
-import lbsnstructure
-from lbsnstructure.lbsnstructure_pb2 import lbsnPost
+import lbsnstructure as lbsn
+post = lbsn.Post()
+place = lbsn.Place()
 ```
 
 .. or compile newest version from [Protofiles](https://gitlab.vgiscience.de/lbsn/concept)
 
 1. Clone git Repository `git clone git@gitlab.vgiscience.de/lbsn/concept`
 2. Install [Protocoll Buffers](https://github.com/google/protobuf/releases)
 3. Compile structure to python package `protoc --python_out=examples/python lbsnstructure/structure.proto`  
 4. Install with `pip install .` in examples/python
 
 ## Developers
 
 For development & testing, make a local clone of this repository  
 ```shell
-git clone git@gitlab.vgiscience.de:lbsn/concept.git
+git clone git@gitlab.vgiscience.de:lbsn/structure/python.git
 ```
 
 Go to subfolder `examples\python` and (e.g.) symlink the folder to your  
 Python's site-packages folder with:  
 ```shell
-python setup.py develop
+pip install --editable .
 ```
 
 Now, lbsnstructure should be available through your python path and directly link to the local git clone directory.
 
 ## Versioning
 
 For the releases available, see the [tags on this repository](/../tags).
```

### Comparing `lbsnstructure-1.0.3/lbsnstructure.egg-info/SOURCES.txt` & `lbsnstructure-1.1.0/lbsnstructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbsnstructure-1.0.3/setup.py` & `lbsnstructure-1.1.0/setup.py`

 * *Files identical despite different names*

