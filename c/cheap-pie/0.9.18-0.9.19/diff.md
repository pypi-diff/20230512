# Comparing `tmp/cheap_pie-0.9.18.tar.gz` & `tmp/cheap_pie-0.9.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheap_pie-0.9.18.tar", last modified: Thu May 11 06:08:09 2023, max compression
+gzip compressed data, was "cheap_pie-0.9.19.tar", last modified: Thu May 11 21:56:40 2023, max compression
```

## Comparing `cheap_pie-0.9.18.tar` & `cheap_pie-0.9.19.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.291383 cheap_pie-0.9.18/
--rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.18/LICENSE
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 06:08:09.291718 cheap_pie-0.9.18/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7746 2023-05-05 18:19:03.000000 cheap_pie-0.9.18/README.md
--rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-11 06:08:09.292769 cheap_pie-0.9.18/setup.cfg
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-11 05:59:04.000000 cheap_pie-0.9.18/setup.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.220646 cheap_pie-0.9.18/src/
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.232795 cheap_pie-0.9.18/src/cheap_pie/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/__init__.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.252300 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cbitfield.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-05 19:38:54.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cheap_pie.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_banner.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_cli.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     6282 2023-05-07 08:06:02.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_hal.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     8909 2023-05-07 08:47:20.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_register.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/test.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.272649 cheap_pie-0.9.18/src/cheap_pie/parsers/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/cp_parsers_wrapper.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/ipxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/ipyxact_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/name_subs.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/rdl_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse_repo.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/parsers/xml_xslt.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.282639 cheap_pie-0.9.18/src/cheap_pie/tools/
--rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/hal2doc.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.18/src/cheap_pie/tools/rdl2any.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/rdl2verilog.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/reload_module.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2275 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/search.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/tools/test_rdl.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.290274 cheap_pie-0.9.18/src/cheap_pie/transport/
--rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/__init__.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_dummy_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_esptool_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_jlink_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyocd_transport.py
--rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyverilator_transport.py
-drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 06:08:09.241993 cheap_pie-0.9.18/src/cheap_pie.egg-info/
--rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/PKG-INFO
--rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/SOURCES.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/dependency_links.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/requires.txt
--rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-11 06:08:09.000000 cheap_pie-0.9.18/src/cheap_pie.egg-info/top_level.txt
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.999783 cheap_pie-0.9.19/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)    11357 2022-12-10 01:01:26.000000 cheap_pie-0.9.19/LICENSE
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 21:56:40.000027 cheap_pie-0.9.19/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     8013 2023-05-11 21:25:50.000000 cheap_pie-0.9.19/README.md
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      103 2023-05-11 21:56:40.001217 cheap_pie-0.9.19/setup.cfg
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1071 2023-05-11 21:49:48.000000 cheap_pie-0.9.19/setup.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.922427 cheap_pie-0.9.19/src/
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.934968 cheap_pie-0.9.19/src/cheap_pie/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/__init__.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.965853 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     7394 2023-05-06 21:35:32.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cbitfield.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2205 2023-05-11 21:49:21.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cheap_pie.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2873 2023-05-05 19:42:59.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_banner.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2092 2023-05-05 19:46:51.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_cli.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     6501 2023-05-11 21:50:54.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_hal.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     9037 2023-05-11 21:40:13.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_register.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2534 2023-05-11 05:47:26.000000 cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/test.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.981113 cheap_pie-0.9.19/src/cheap_pie/parsers/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2088 2023-05-07 09:34:36.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/cp_parsers_wrapper.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3989 2023-05-07 09:06:44.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/ipxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     3294 2023-05-07 08:41:29.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/ipyxact_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      430 2023-05-07 09:09:07.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/name_subs.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1026 2023-05-07 09:10:56.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/rdl_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4091 2023-05-07 09:33:12.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     4134 2023-05-07 09:35:26.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse_repo.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1968 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/parsers/xml_xslt.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.990652 cheap_pie-0.9.19/src/cheap_pie/tools/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       40 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5727 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/hal2doc.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1553 2022-12-12 21:51:02.000000 cheap_pie-0.9.19/src/cheap_pie/tools/rdl2any.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      890 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/rdl2verilog.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      944 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/reload_module.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2200 2023-05-11 21:44:55.000000 cheap_pie-0.9.19/src/cheap_pie/tools/search.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      563 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/tools/test_rdl.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.998519 cheap_pie-0.9.19/src/cheap_pie/transport/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        0 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/__init__.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1775 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_dummy_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2289 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_esptool_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     2027 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_jlink_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1985 2022-12-10 02:06:51.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyocd_transport.py
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     5284 2023-05-06 21:31:25.000000 cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyverilator_transport.py
+drwxrwxrwx   0 marco     (1000) marco     (1000)        0 2023-05-11 21:56:39.944653 cheap_pie-0.9.19/src/cheap_pie.egg-info/
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      309 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/PKG-INFO
+-rwxrwxrwx   0 marco     (1000) marco     (1000)     1408 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/SOURCES.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)        1 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/dependency_links.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)      101 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/requires.txt
+-rwxrwxrwx   0 marco     (1000) marco     (1000)       10 2023-05-11 21:56:39.000000 cheap_pie-0.9.19/src/cheap_pie.egg-info/top_level.txt
```

### Comparing `cheap_pie-0.9.18/LICENSE` & `cheap_pie-0.9.19/LICENSE`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/README.md` & `cheap_pie-0.9.19/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -119,47 +119,60 @@
         ./cheap_pie.sh -dd  ./devices/rdl -rf basic.rdl -fmt rdl -t verilator -topv ./devices/rdl/basic/basic_rf.sv
 
 # Install
 ## From pypi
         pip3 install cheap_pie
 ## From github
         pip3 install git+https://github.com/bat52/cheap_pie.git@master
-# Dependencies for validation:
+
+# Dependencies for core (required):        
+        # for XML parsing (used by legacy svd parser and IP-XACT parser)
+        pip3 install untangle
+        # for exporting XML info into a human-readable document
+        pip3 install python-docx
+        # for dumping registers
+        pip3 install hickle
         # CMSIS-SVD python parser including many svd files https://github.com/posborne/cmsis-svd
         pip3 install cmsis-svd
         # SPIRIT IP-XACT parser through ipyxact https://github.com/olofk/ipyxact
-        pip3 install ipyxact
-        # for XML parsing (used by legacy svd parser and IP-XACT parser)
-        pip3 install untangle
+        pip3 install ipyxact                
+        # SystemRDL to register-file verilog
+        https://github.com/hughjackson/PeakRDL-verilog
+        # SystemRDL to IP-XACT
+        https://github.com/SystemRDL/PeakRDL-ipxact
+# Dependencies for validation/transport layers (optional):        
         # for JLINK
         pip3 install pylink-square
         # pyOCD for CMSIS-DAP and JLINK support (only tested in python-venv)
         pip3 install pyocd
         # esptool for Espressif devices (not yet functional)
-        pip3 install esptool
-        # for exporting XML info into a human-readable document
-        pip3 install python-docx
-        # for dumping registers
-        pip3 install hickle
-        
-# Dependencies for verification:
+        pip3 install esptool        
+# Dependencies for verification (optional AND experimental):
         # verilator
         https://www.veripool.org/verilator/
         # pyverilator (python verilator wrapper)
-        https://github.com/csail-csg/pyverilator
-        # SystemRDL to register-file verilog
-        https://github.com/hughjackson/PeakRDL-verilog
-        # SystemRDL to IP-XACT
-        https://github.com/SystemRDL/PeakRDL-ipxact
+        https://github.com/csail-csg/pyverilator        
         # gtkwave
         http://gtkwave.sourceforge.net/
 
-# python transport wrappers
-- pyOCD sypports JLINK, CMSIS-DAP and GDB https://github.com/pyocd/pyOCD
-- esptool supports espressif targets https://github.com/espressif/esptool
+# Releasing
+
+Releases are published automatically when a tag is pushed to GitHub.
+
+.. code-block:: bash
+
+   # Set next version number
+   export RELEASE=x.x.x
+
+   # Create tags
+   git commit --allow-empty -m "Release $RELEASE"
+   git tag -a $RELEASE -m "Version $RELEASE"
+
+   # Push
+   git push upstream --tags
 
 # Register description formats
 regtool from opentitan project seems similar, using JSON to represent chip/IP structure, and I2C transport
 https://docs.opentitan.org/doc/rm/register_tool/
 
 custom input, output: verilog, VHDL, YAML, JSON, TOML, Spreadsheet (XLSX, XLS, OSD, CSV)
 https://github.com/rggen/rggen
```

### Comparing `cheap_pie-0.9.18/setup.py` & `cheap_pie-0.9.19/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='cheap_pie',
-    version='0.9.18',
+    version='0.9.19',
     license='Apache 2.0',
     author="Marco Merlin",
     author_email='marcomerli@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     description="A python tool for silicon validation.",
     url='https://github.com/bat52/cheap_pie',
```

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cbitfield.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cbitfield.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cheap_pie.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cheap_pie.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_banner.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_banner.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_cli.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_cli.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_hal.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_hal.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 """
 #
 # -*- coding: utf-8 -*-
 ## this file is part of cheap_pie, a python tool for chip validation
 ## author: Marco Merlin
 ## email: marcomerli@gmail.com
 
-import sys
-import os.path
 import hickle as hkl
 
-sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
+try:
+    # cheap_pie installed with pip 
+    from cheap_pie.transport.cp_dummy_transport import cp_dummy
+    import cheap_pie.tools.search
+    from cheap_pie.tools.hal2doc import hal2doc
 
-from transport.cp_dummy_transport import cp_dummy
-import tools.search
-from tools.hal2doc import hal2doc
+except:
+    import sys
+    import os.path
+    sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
+    from transport.cp_dummy_transport import cp_dummy
+    import tools.search
+    from tools.hal2doc import hal2doc
 
 class cp_hal:
     """
     Cheap Pie Hardware Abstraction Layer
     """
     regs = []
     hif = None
```

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/cp_register.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/cp_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 ## email: marcomerli@gmail.com
 
 import textwrap
 from collections import namedtuple
 from ast import literal_eval
 
 try:
-    from cheap_pie_core.cbitfield import cp_bitfield
+    # cheap_pie installed with pip 
+    from cheap_pie.cheap_pie_core.cbitfield import cp_bitfield
 except:
-    from cbitfield import cp_bitfield
+    try:
+        from cheap_pie_core.cbitfield import cp_bitfield
+    except:
+        from cbitfield import cp_bitfield
 
 class cp_register:
     """
     Register Class for Cheap Pie
     """
     addr = 0
     regname = ''
```

### Comparing `cheap_pie-0.9.18/src/cheap_pie/cheap_pie_core/test.py` & `cheap_pie-0.9.19/src/cheap_pie/cheap_pie_core/test.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/cp_parsers_wrapper.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/cp_parsers_wrapper.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/ipxact_parse.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/ipxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/ipyxact_parse.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/ipyxact_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/rdl_parse.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/rdl_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/svd_parse_repo.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/svd_parse_repo.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/parsers/xml_xslt.py` & `cheap_pie-0.9.19/src/cheap_pie/parsers/xml_xslt.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/hal2doc.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/hal2doc.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/rdl2any.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/rdl2any.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/rdl2verilog.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/rdl2verilog.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/reload_module.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/reload_module.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/search.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/search.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,76 +5,70 @@
 ## email: marcomerli@gmail.com
 
 from ast import literal_eval
 
 def str_in_str(str1,str2,case_sensitive=True):
     if case_sensitive:
         return (str1 in str2)
-    else:
-        return (str1.upper() in str2.upper())
-    pass
+    return (str1.upper() in str2.upper())
 
 def register(hal,regname,case_sensitive=True):
     retval = []    
     for reg in hal: # loop over all registers
         if str_in_str(regname,reg.regname,case_sensitive):
             print( reg.regname )
             retval.append(reg.regname)
-    return retval    
+    return retval
 
 def bitfield(hal,bitfield,case_sensitive=True):
-    retval = []    
+    retval = []
     for reg in hal: # loop over all registers
         # print reg.regname        
         for field in reg.bitfields:
             if str_in_str(bitfield,field.fieldname,case_sensitive):
                 print( reg.regname + " @ " + field.fieldname )
                 retval.append(field)
     return retval
 
-def address(hal, address, mask='0xFFFFFFFF'):     
-    # convert address into integer, if needed    
+def address(hal, address, mask='0xFFFFFFFF'):
+    # convert address into integer, if needed
     if isinstance(mask,str):
         mask    = int( literal_eval(mask) )
     if isinstance(address,str):
         address = int( literal_eval(address) )
-    
+
     retval = []    
     for reg in hal: # loop over all registers
         # print reg.regname
         if (reg.addr & mask) == (address & mask):
             print( reg.regname + " : " + hex(reg.addr) )
             return reg.regname
 
 def test_search():
     print('Testing search...')
     from parsers.svd_parse_repo import svd_parse
     hal = svd_parse(fname="./devices/QN908XC.svd", hif=None)
 
-    print('## ADC registers:')    
-    ret = register(hal,'ADC')    
-    assert(len(ret) > 0)
+    print('## ADC registers:')
+    ret = register(hal,'ADC')
+    assert len(ret) > 0
 
     print('##  ADC_BM bitfields:')
     ret = bitfield(hal,'ADC_BM')
-    assert(len(ret) > 0)
+    assert len(ret) > 0
 
     print('## 0x4000702c register name:')
     ret = address(hal,'0x4000702c')
-    assert(len(ret) > 0)
-    
+    assert len(ret) > 0
+
     print('## 0xF000702c register name:')
     ret = address(hal,'0xF000702c',mask='0x0FFFFFFF')
-    assert(len(ret) > 0)
+    assert len(ret) > 0
 
     ret = address(hal,'0xF000702c')
-    assert( ret is None )
-
+    assert ret is None
 
 if __name__ == '__main__':
     import sys
     import os.path
     sys.path.append( os.path.join(os.path.dirname(__file__), '..') )
     test_search()
-    pass
-
-
```

### Comparing `cheap_pie-0.9.18/src/cheap_pie/tools/test_rdl.py` & `cheap_pie-0.9.19/src/cheap_pie/tools/test_rdl.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/transport/cp_dummy_transport.py` & `cheap_pie-0.9.19/src/cheap_pie/transport/cp_dummy_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/transport/cp_esptool_transport.py` & `cheap_pie-0.9.19/src/cheap_pie/transport/cp_esptool_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/transport/cp_jlink_transport.py` & `cheap_pie-0.9.19/src/cheap_pie/transport/cp_jlink_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyocd_transport.py` & `cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyocd_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie/transport/cp_pyverilator_transport.py` & `cheap_pie-0.9.19/src/cheap_pie/transport/cp_pyverilator_transport.py`

 * *Files identical despite different names*

### Comparing `cheap_pie-0.9.18/src/cheap_pie.egg-info/SOURCES.txt` & `cheap_pie-0.9.19/src/cheap_pie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

