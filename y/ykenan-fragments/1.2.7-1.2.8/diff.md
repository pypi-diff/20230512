# Comparing `tmp/ykenan_fragments-1.2.7.tar.gz` & `tmp/ykenan_fragments-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.7.tar", last modified: Fri May 12 01:08:45 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.8.tar", last modified: Fri May 12 02:30:31 2023, max compression
```

## Comparing `ykenan_fragments-1.2.7.tar` & `ykenan_fragments-1.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.864653 ykenan_fragments-1.2.7/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.7/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-12 01:08:45.863653 ykenan_fragments-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.7/README.md
--rw-rw-rw-   0        0        0      775 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       52 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 01:08:45.864653 ykenan_fragments-1.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.830653 ykenan_fragments-1.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.848656 ykenan_fragments-1.2.7/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     2012 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     5383 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    15901 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    14835 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.862652 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.8/README.md
+-rw-rw-rw-   0        0        0      775 2023-05-12 02:21:10.000000 ykenan_fragments-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       52 2023-05-12 02:21:10.000000 ykenan_fragments-1.2.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 02:30:31.559351 ykenan_fragments-1.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.497350 ykenan_fragments-1.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.531352 ykenan_fragments-1.2.8/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     2012 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     5383 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    15901 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    14835 2023-05-12 02:02:30.000000 ykenan_fragments-1.2.8/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-12 02:30:31.558353 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 02:30:31.000000 ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.7/LICENSE` & `ykenan_fragments-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.7/PKG-INFO` & `ykenan_fragments-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.7
+Version: 1.2.8
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.7/pyproject.toml` & `ykenan_fragments-1.2.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.10", "pandas>=1.5.3"]
+requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.11", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.7"
+version = "1.2.8"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
-dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.10", "pandas>=1.5.3"]
+dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.11", "pandas>=1.5.3"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 github = "https://github.com/YuZhengM/ykenan_fragments"
```

### Comparing `ykenan_fragments-1.2.7/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.2.8/src/ykenan_fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.7/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.8/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.7/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.8/src/ykenan_fragments/get_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.7/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.8/src/ykenan_fragments/get_sort_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.8/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.7
+Version: 1.2.8
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

