# Comparing `tmp/carefree-creator-0.2.3.tar.gz` & `tmp/carefree-creator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-creator-0.2.3.tar", last modified: Fri May 12 11:21:00 2023, max compression
+gzip compressed data, was "carefree-creator-0.2.4.tar", last modified: Fri May 12 11:23:59 2023, max compression
```

## Comparing `carefree-creator-0.2.3.tar` & `carefree-creator-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.200718 carefree-creator-0.2.3/
--rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4419 2023-05-12 11:21:00.200718 carefree-creator-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.182714 carefree-creator-0.2.3/carefree_creator.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      138 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 11:21:00.000000 carefree-creator-0.2.3/carefree_creator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.190719 carefree-creator-0.2.3/cfcreator/
--rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.3/cfcreator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.194720 carefree-creator-0.2.3/cfcreator/apis/
--rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.3/cfcreator/apis/config.yml
--rw-rw-rw-   0        0        0     9036 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/apis/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.196718 carefree-creator-0.2.3/cfcreator/apis/kafka/
--rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.3/cfcreator/apis/kafka/config.yml
--rw-rw-rw-   0        0        0    13717 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/apis/kafka/consumer.py
--rw-rw-rw-   0        0        0    12109 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/apis/kafka/producer.py
--rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/cli.py
--rw-rw-rw-   0        0        0    22741 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/common.py
--rw-rw-rw-   0        0        0    15062 2023-05-09 06:40:22.000000 carefree-creator-0.2.3/cfcreator/control.py
--rw-rw-rw-   0        0        0     2226 2023-05-09 07:17:42.000000 carefree-creator-0.2.3/cfcreator/control_multi.py
--rw-rw-rw-   0        0        0     8444 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/cos.py
--rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.3/cfcreator/cv.py
--rw-rw-rw-   0        0        0     2458 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/endpoints.py
--rw-rw-rw-   0        0        0    20523 2023-05-09 04:37:43.000000 carefree-creator-0.2.3/cfcreator/img2img.py
--rw-rw-rw-   0        0        0     1657 2023-05-09 04:37:43.000000 carefree-creator-0.2.3/cfcreator/img2txt.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.198718 carefree-creator-0.2.3/cfcreator/legacy/
--rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.3/cfcreator/legacy/__init__.py
--rw-rw-rw-   0        0        0     2102 2023-05-06 03:00:57.000000 carefree-creator-0.2.3/cfcreator/legacy/common.py
--rw-rw-rw-   0        0        0    13724 2023-05-06 03:00:57.000000 carefree-creator-0.2.3/cfcreator/legacy/control.py
--rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.3/cfcreator/legacy/control_multi.py
--rw-rw-rw-   0        0        0     3298 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/parameters.py
--rw-rw-rw-   0        0        0     3431 2023-05-09 07:27:06.000000 carefree-creator-0.2.3/cfcreator/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:21:00.200718 carefree-creator-0.2.3/cfcreator/sdks/
--rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.3/cfcreator/sdks/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/sdks/direct.py
--rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/sdks/kafka.py
--rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/sdks/utils.py
--rw-rw-rw-   0        0        0     7054 2023-05-09 04:37:43.000000 carefree-creator-0.2.3/cfcreator/txt2img.py
--rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/txt2txt.py
--rw-rw-rw-   0        0        0     4631 2023-04-23 02:27:17.000000 carefree-creator-0.2.3/cfcreator/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-12 11:21:00.200718 carefree-creator-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-05-12 11:18:23.000000 carefree-creator-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.014854 carefree-creator-0.2.4/
+-rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4419 2023-05-12 11:23:59.013854 carefree-creator-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:58.990343 carefree-creator-0.2.4/carefree_creator.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      138 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 11:23:58.000000 carefree-creator-0.2.4/carefree_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.002855 carefree-creator-0.2.4/cfcreator/
+-rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.003855 carefree-creator-0.2.4/cfcreator/apis/
+-rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.4/cfcreator/apis/config.yml
+-rw-rw-rw-   0        0        0     9036 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/apis/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.006855 carefree-creator-0.2.4/cfcreator/apis/kafka/
+-rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/config.yml
+-rw-rw-rw-   0        0        0    13717 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/consumer.py
+-rw-rw-rw-   0        0        0    12109 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/apis/kafka/producer.py
+-rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/cli.py
+-rw-rw-rw-   0        0        0    22741 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/common.py
+-rw-rw-rw-   0        0        0    15062 2023-05-09 06:40:22.000000 carefree-creator-0.2.4/cfcreator/control.py
+-rw-rw-rw-   0        0        0     2226 2023-05-09 07:17:42.000000 carefree-creator-0.2.4/cfcreator/control_multi.py
+-rw-rw-rw-   0        0        0     8444 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/cos.py
+-rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/cv.py
+-rw-rw-rw-   0        0        0     2458 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/endpoints.py
+-rw-rw-rw-   0        0        0    20523 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/img2img.py
+-rw-rw-rw-   0        0        0     1657 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/img2txt.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.009854 carefree-creator-0.2.4/cfcreator/legacy/
+-rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/__init__.py
+-rw-rw-rw-   0        0        0     2102 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/common.py
+-rw-rw-rw-   0        0        0    13724 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/control.py
+-rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.4/cfcreator/legacy/control_multi.py
+-rw-rw-rw-   0        0        0     3298 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/parameters.py
+-rw-rw-rw-   0        0        0     3431 2023-05-09 07:27:06.000000 carefree-creator-0.2.4/cfcreator/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:23:59.012854 carefree-creator-0.2.4/cfcreator/sdks/
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.4/cfcreator/sdks/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/direct.py
+-rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/kafka.py
+-rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/sdks/utils.py
+-rw-rw-rw-   0        0        0     7054 2023-05-09 04:37:43.000000 carefree-creator-0.2.4/cfcreator/txt2img.py
+-rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/txt2txt.py
+-rw-rw-rw-   0        0        0     4631 2023-04-23 02:27:17.000000 carefree-creator-0.2.4/cfcreator/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 11:23:59.014854 carefree-creator-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2023-05-12 11:22:40.000000 carefree-creator-0.2.4/setup.py
```

### Comparing `carefree-creator-0.2.3/LICENSE` & `carefree-creator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/PKG-INFO` & `carefree-creator-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.3
+Version: 0.2.4
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.3/README.md` & `carefree-creator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/carefree_creator.egg-info/PKG-INFO` & `carefree-creator-0.2.4/carefree_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.3
+Version: 0.2.4
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.3/carefree_creator.egg-info/SOURCES.txt` & `carefree-creator-0.2.4/carefree_creator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/apis/config.yml` & `carefree-creator-0.2.4/cfcreator/apis/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/apis/interface.py` & `carefree-creator-0.2.4/cfcreator/apis/interface.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/apis/kafka/config.yml` & `carefree-creator-0.2.4/cfcreator/apis/kafka/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/apis/kafka/consumer.py` & `carefree-creator-0.2.4/cfcreator/apis/kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/apis/kafka/producer.py` & `carefree-creator-0.2.4/cfcreator/apis/kafka/producer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/cli.py` & `carefree-creator-0.2.4/cfcreator/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/common.py` & `carefree-creator-0.2.4/cfcreator/common.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/control.py` & `carefree-creator-0.2.4/cfcreator/control.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/control_multi.py` & `carefree-creator-0.2.4/cfcreator/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/cos.py` & `carefree-creator-0.2.4/cfcreator/cos.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/cv.py` & `carefree-creator-0.2.4/cfcreator/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/endpoints.py` & `carefree-creator-0.2.4/cfcreator/endpoints.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/img2img.py` & `carefree-creator-0.2.4/cfcreator/img2img.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/img2txt.py` & `carefree-creator-0.2.4/cfcreator/img2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/legacy/common.py` & `carefree-creator-0.2.4/cfcreator/legacy/common.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/legacy/control.py` & `carefree-creator-0.2.4/cfcreator/legacy/control.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/legacy/control_multi.py` & `carefree-creator-0.2.4/cfcreator/legacy/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/parameters.py` & `carefree-creator-0.2.4/cfcreator/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/pipeline.py` & `carefree-creator-0.2.4/cfcreator/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/sdks/direct.py` & `carefree-creator-0.2.4/cfcreator/sdks/direct.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/sdks/kafka.py` & `carefree-creator-0.2.4/cfcreator/sdks/kafka.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/sdks/utils.py` & `carefree-creator-0.2.4/cfcreator/sdks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/txt2img.py` & `carefree-creator-0.2.4/cfcreator/txt2img.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/txt2txt.py` & `carefree-creator-0.2.4/cfcreator/txt2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/cfcreator/utils.py` & `carefree-creator-0.2.4/cfcreator/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.3/setup.py` & `carefree-creator-0.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.3"
+VERSION = "0.2.4"
 PACKAGE_NAME = "carefree-creator"
 
 DESCRIPTION = "An AI-powered creator for everyone."
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

