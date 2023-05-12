# Comparing `tmp/cheap_pie-0.9.19.tar.gz` & `tmp/cheap_pie-0.9.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-0.9.19.tar", last modified: Thu May 11 21:56:40 2023, max compression
+gzip compressed data, was "cheap_pie-0.9.20.tar", last modified: Fri May 12 09:57:39 2023, max compression
```

## Comparing `cheap_pie-0.9.19.tar` & `cheap_pie-0.9.20.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.999783 cheap_pie-0.9.19/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.19/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 21:56:40.000027 cheap_pie-0.9.19/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8013 2023-05-11 21:25:50.000000 cheap_pie-0.9.19/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-11 21:56:40.001217 cheap_pie-0.9.19/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-11 21:49:48.000000 cheap_pie-0.9.19/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.922427 cheap_pie-0.9.19/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.934968 cheap_pie-0.9.19/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.965853 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-11 21:49:21.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cheap_pie.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6501 2023-05-11 21:50:54.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     9037 2023-05-11 21:40:13.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.981113 cheap_pie-0.9.19/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/name_subs.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.990652 cheap_pie-0.9.19/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.19/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/rdl2verilog.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/reload_module.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2200 2023-05-11 21:44:55.000000 cheap_pie-0.9.19/src/cheap_pie/tools/search.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/test_rdl.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.998519 cheap_pie-0.9.19/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.944653 cheap_pie-0.9.19/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.901868 cheap_pie-0.9.20/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.20/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-12 09:57:39.902188 cheap_pie-0.9.20/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8013 2023-05-11 21:25:50.000000 cheap_pie-0.9.20/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-12 09:57:39.902963 cheap_pie-0.9.20/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-12 09:20:29.000000 cheap_pie-0.9.20/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.821803 cheap_pie-0.9.20/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.832108 cheap_pie-0.9.20/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.862509 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-11 21:49:21.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cheap_pie.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6501 2023-05-11 21:50:54.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     9037 2023-05-11 21:40:13.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.876745 cheap_pie-0.9.20/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/name_subs.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.888286 cheap_pie-0.9.20/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      156 2023-05-12 09:20:29.000000 cheap_pie-0.9.20/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.20/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/rdl2verilog.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/reload_module.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2200 2023-05-11 21:44:55.000000 cheap_pie-0.9.20/src/cheap_pie/tools/search.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/tools/test_rdl.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.900249 cheap_pie-0.9.20/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-12 09:57:39.842349 cheap_pie-0.9.20/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-12 09:57:39.000000 cheap_pie-0.9.20/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-0.9.19/LICENSE` & `cheap_pie-0.9.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/README.md` & `cheap_pie-0.9.20/README.md`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/setup.py` & `cheap_pie-0.9.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='0.9.19',
+    version='0.9.20',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     url='https://github.com/bat52/cheap_pie',
```

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cheap_pie.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cheap_pie.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-0.9.20/src/cheap_pie/cheap_pie_core/test.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/cp_parsers_wrapper.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/cp_parsers_wrapper.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/rdl_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-0.9.20/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/rdl2verilog.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/rdl2verilog.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/reload_module.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/reload_module.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/search.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/search.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/tools/test_rdl.py` & `cheap_pie-0.9.20/src/cheap_pie/tools/test_rdl.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-0.9.20/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-0.9.20/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-0.9.20/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-0.9.20/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.19/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-0.9.20/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

