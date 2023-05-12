# Comparing `tmp/ykenan_fragments-1.2.6.tar.gz` & `tmp/ykenan_fragments-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.6.tar", last modified: Thu May 11 07:14:38 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.7.tar", last modified: Fri May 12 01:08:45 2023, max compression
```

## Comparing `ykenan_fragments-1.2.6.tar` & `ykenan_fragments-1.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 07:14:38.685279 ykenan_fragments-1.2.6/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.6/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-11 07:14:38.684279 ykenan_fragments-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.6/README.md
--rw-rw-rw-   0        0        0      773 2023-05-11 06:57:59.000000 ykenan_fragments-1.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-05-11 01:21:49.000000 ykenan_fragments-1.2.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 07:14:38.685279 ykenan_fragments-1.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 07:14:38.634279 ykenan_fragments-1.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-11 07:14:38.668281 ykenan_fragments-1.2.6/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     2012 2023-05-10 13:00:59.000000 ykenan_fragments-1.2.6/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     5383 2023-05-11 07:06:55.000000 ykenan_fragments-1.2.6/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    15901 2023-05-11 01:33:09.000000 ykenan_fragments-1.2.6/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    14773 2023-05-11 06:50:37.000000 ykenan_fragments-1.2.6/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-11 07:14:38.683278 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-11 07:14:38.000000 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-11 07:14:38.000000 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 07:14:38.000000 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-11 07:14:38.000000 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-11 07:14:38.000000 ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.864653 ykenan_fragments-1.2.7/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-12 01:08:45.863653 ykenan_fragments-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.7/README.md
+-rw-rw-rw-   0        0        0      775 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       52 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 01:08:45.864653 ykenan_fragments-1.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.830653 ykenan_fragments-1.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.848656 ykenan_fragments-1.2.7/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     2012 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     5383 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    15901 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    14835 2023-05-12 00:45:39.000000 ykenan_fragments-1.2.7/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-12 01:08:45.862652 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 01:08:45.000000 ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.6/LICENSE` & `ykenan_fragments-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.6/PKG-INFO` & `ykenan_fragments-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.6
+Version: 1.2.7
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.6/pyproject.toml` & `ykenan_fragments-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.9", "pandas>=1.5.3"]
+requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.10", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
-dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.9", "pandas>=1.5.3"]
+dependencies = ["ykenan-log>=0.2.0", "ykenan-file>=0.1.10", "pandas>=1.5.3"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 github = "https://github.com/YuZhengM/ykenan_fragments"
```

### Comparing `ykenan_fragments-1.2.6/src/ykenan_fragments/__init__.py` & `ykenan_fragments-1.2.7/src/ykenan_fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.6/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.7/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.6/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.7/src/ykenan_fragments/get_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.6/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.7/src/ykenan_fragments/get_sort_fragments.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,24 @@
         genome_output: str = os.path.join(base_path, self.genome_generate)
 
         if genome == self.genome_generate and self.lift_over_path:
             # 执行信息
             Hg19AndHg38(path=base_path, lift_over_path=self.lift_over_path, is_hg19_to_hg38=self.is_hg19_to_hg38)
 
         files_dict: dict = self.file.entry_files_dict(genome_output)
-        files_name = self.file.entry_files_dict(genome_output)
+        files_name = files_dict["name"]
+        genome_chr_name: list = []
         for filename in files_name:
             chr_: str = "chr" + filename.split("_chr")[1].split(".")[0]
+            genome_chr_name.append(chr_)
             genome_f_path.update({chr_: files_dict[filename]})
         return {
             self.genome_source: chr_file_dict,
             self.genome_generate: {
-                "name": chr_name,
+                "name": genome_chr_name,
                 "path": genome_f_path
             }
         }
 
     def sort_position_files_core(self, param: tuple):
         position: str = param[0]
         file_dict_path: dict = param[1]
```

### Comparing `ykenan_fragments-1.2.6/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.7/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.6
+Version: 1.2.7
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

