# Comparing `tmp/lctutil-0.5.0.tar.gz` & `tmp/lctutil-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctutil-0.5.0.tar", last modified: Mon Apr 17 06:02:10 2023, max compression
+gzip compressed data, was "lctutil-0.6.0.tar", last modified: Fri May 12 09:30:11 2023, max compression
```

## Comparing `lctutil-0.5.0.tar` & `lctutil-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.372366 lctutil-0.5.0/
--rw-rw-rw-   0        0        0      328 2023-04-17 06:02:10.371365 lctutil-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.366364 lctutil-0.5.0/lctutil/
--rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.5.0/lctutil/__init__.py
--rw-rw-rw-   0        0        0     3321 2023-04-16 07:45:57.000000 lctutil-0.5.0/lctutil/ac_matcher.py
--rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.5.0/lctutil/extract_base_info.py
--rw-rw-rw-   0        0        0     1526 2023-04-17 06:01:22.000000 lctutil-0.5.0/lctutil/openai.py
--rw-rw-rw-   0        0        0     1147 2023-04-15 06:04:07.000000 lctutil-0.5.0/lctutil/stock_infos.py
-drwxrwxrwx   0        0        0        0 2023-04-17 06:02:10.370365 lctutil-0.5.0/lctutil.egg-info/
--rw-rw-rw-   0        0        0      328 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-17 06:02:10.000000 lctutil-0.5.0/lctutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 06:02:10.372366 lctutil-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      592 2023-04-17 06:01:22.000000 lctutil-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.700879 lctutil-0.6.0/
+-rw-rw-rw-   0        0        0      328 2023-05-12 09:30:11.699878 lctutil-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-16 12:32:34.000000 lctutil-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.694878 lctutil-0.6.0/lctutil/
+-rw-rw-rw-   0        0        0        0 2023-04-16 06:06:37.000000 lctutil-0.6.0/lctutil/__init__.py
+-rw-rw-rw-   0        0        0     3419 2023-05-12 07:23:14.000000 lctutil-0.6.0/lctutil/ac_matcher.py
+-rw-rw-rw-   0        0        0     5766 2023-04-15 13:05:08.000000 lctutil-0.6.0/lctutil/extract_base_info.py
+-rw-rw-rw-   0        0        0     1526 2023-05-12 07:23:51.000000 lctutil-0.6.0/lctutil/openai.py
+-rw-rw-rw-   0        0        0     1217 2023-05-12 07:50:18.000000 lctutil-0.6.0/lctutil/stock_infos.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:30:11.698878 lctutil-0.6.0/lctutil.egg-info/
+-rw-rw-rw-   0        0        0      328 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 09:30:11.000000 lctutil-0.6.0/lctutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 09:30:11.700879 lctutil-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      592 2023-05-12 09:27:44.000000 lctutil-0.6.0/setup.py
```

### Comparing `lctutil-0.5.0/lctutil/ac_matcher.py` & `lctutil-0.6.0/lctutil/ac_matcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,17 +84,19 @@
             start_index = end_index - key_length + 1
             mt = query[start_index: end_index + 1]
             if mt not in has_seen:
                 has_seen.append(mt)
                 ans.append((mt, tags))
         return ans
 
-from .stock_infos import info_stock_names, all_gainian, all_bankuai_2, all_bankuai_3
+from .stock_infos import info_stock_names, info_stock_codes, all_gainian, all_bankuai_2, all_bankuai_3
 
 S_NAME_TAG = "STOCK"
+S_CODE_TAG = "SCODE"
 S_BK_TAG = "BK"
 S_GAINIAN_TAG = "GAINIAN"
 
 stock_ac = AC()
 stock_ac.init_slot_list_ac(info_stock_names, S_NAME_TAG)
+stock_ac.init_slot_list_ac(info_stock_codes, S_CODE_TAG)
 stock_ac.init_slot_list_ac(all_gainian, S_GAINIAN_TAG)
 stock_ac.make_from_list(set(list(all_bankuai_2) + list(all_bankuai_3)), S_BK_TAG)
```

### Comparing `lctutil-0.5.0/lctutil/extract_base_info.py` & `lctutil-0.6.0/lctutil/extract_base_info.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.5.0/lctutil/openai.py` & `lctutil-0.6.0/lctutil/openai.py`

 * *Files identical despite different names*

### Comparing `lctutil-0.5.0/lctutil/stock_infos.py` & `lctutil-0.6.0/lctutil/stock_infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,8 +39,12 @@
             all_bankuai_2.add(eles[4])
             all_bankuai_3.add(eles[5])
 
             info_tables[name] = (eles[2], eles[3], eles[4], eles[5])
 
 
 _filename = os.getenv("STOCK_INFO_FILE")
-loadcodes(_filename)
+loadcodes(_filename)
+
+
+def get_code_or_name(ele):
+    return code_name_kv.get(ele, "")
```

### Comparing `lctutil-0.5.0/setup.py` & `lctutil-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lctutil',
-    version='0.5.0',
+    version='0.6.0',
     packages=find_packages(),
     install_requires=[
         "pyahocorasick",
         "openai",
         "tenacity"
     ],
     py_modules=["lctutil"],
```

