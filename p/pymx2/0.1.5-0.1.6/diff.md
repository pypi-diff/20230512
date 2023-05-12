# Comparing `tmp/pymx2-0.1.5.tar.gz` & `tmp/pymx2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymx2-0.1.5.tar", last modified: Tue May  9 15:23:08 2023, max compression
+gzip compressed data, was "pymx2-0.1.6.tar", last modified: Fri May 12 17:30:09 2023, max compression
```

## Comparing `pymx2-0.1.5.tar` & `pymx2-0.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.455088 pymx2-0.1.5/
--rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.5/.gitignore
--rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.5/LICENSE
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-09 15:23:08.454703 pymx2-0.1.5/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.5/README.md
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.444067 pymx2-0.1.5/docs/
--rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.5/docs/mx2.enums.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.5/docs/mx2.exceptions.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.5/docs/mx2.html
--rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.5/docs/mx2.types.html
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.447185 pymx2-0.1.5/examples/
--rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.5/examples/01_connect.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.5/examples/02_read_write_coil.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.5/examples/03_read_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.5/examples/04_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.5/examples/05_read_write_registers.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.5/examples/06_data_types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.449444 pymx2-0.1.5/mx2/
--rw-r--r--   0 vpaeder    (501) staff       (20)    31998 2023-05-03 07:51:28.000000 pymx2-0.1.5/mx2/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    48828 2023-05-05 06:34:19.000000 pymx2-0.1.5/mx2/enums.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.5/mx2/exceptions.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.5/mx2/types.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.451351 pymx2-0.1.5/pymx2.egg-info/
--rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/PKG-INFO
--rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/SOURCES.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/dependency_links.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/requires.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-09 15:23:08.000000 pymx2-0.1.5/pymx2.egg-info/top_level.txt
--rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-09 15:23:08.455180 pymx2-0.1.5/setup.cfg
--rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-09 15:22:40.000000 pymx2-0.1.5/setup.py
-drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-09 15:23:08.454121 pymx2-0.1.5/tests/
--rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.5/tests/__init__.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.5/tests/inverter.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.5/tests/modbus.py
--rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.5/tests/ser.py
--rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.5/tests/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.543037 pymx2-0.1.6/
+-rw-r--r--   0 vpaeder    (501) staff       (20)       39 2023-04-27 13:13:03.000000 pymx2-0.1.6/.gitignore
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1071 2023-04-27 13:41:31.000000 pymx2-0.1.6/LICENSE
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-12 17:30:09.542510 pymx2-0.1.6/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2938 2023-04-28 18:35:35.000000 pymx2-0.1.6/README.md
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.530221 pymx2-0.1.6/docs/
+-rw-r--r--   0 vpaeder    (501) staff       (20)   214194 2023-05-02 15:01:56.000000 pymx2-0.1.6/docs/mx2.enums.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    60476 2023-05-02 15:02:06.000000 pymx2-0.1.6/docs/mx2.exceptions.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    22217 2023-05-02 15:01:50.000000 pymx2-0.1.6/docs/mx2.html
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10077 2023-05-02 15:02:00.000000 pymx2-0.1.6/docs/mx2.types.html
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.533520 pymx2-0.1.6/examples/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      431 2023-04-24 11:33:12.000000 pymx2-0.1.6/examples/01_connect.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      978 2023-04-24 11:35:16.000000 pymx2-0.1.6/examples/02_read_write_coil.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      903 2023-04-26 16:47:32.000000 pymx2-0.1.6/examples/03_read_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      841 2023-04-27 12:28:11.000000 pymx2-0.1.6/examples/04_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)      954 2023-04-27 11:31:32.000000 pymx2-0.1.6/examples/05_read_write_registers.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1766 2023-04-27 12:08:57.000000 pymx2-0.1.6/examples/06_data_types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.536140 pymx2-0.1.6/mx2/
+-rw-r--r--   0 vpaeder    (501) staff       (20)    32004 2023-05-12 17:27:05.000000 pymx2-0.1.6/mx2/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    48828 2023-05-05 06:34:19.000000 pymx2-0.1.6/mx2/enums.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     2161 2023-04-21 11:17:50.000000 pymx2-0.1.6/mx2/exceptions.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    11345 2023-05-02 14:57:19.000000 pymx2-0.1.6/mx2/types.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.538869 pymx2-0.1.6/pymx2.egg-info/
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3690 2023-05-12 17:30:09.000000 pymx2-0.1.6/pymx2.egg-info/PKG-INFO
+-rw-r--r--   0 vpaeder    (501) staff       (20)      577 2023-05-12 17:30:09.000000 pymx2-0.1.6/pymx2.egg-info/SOURCES.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        1 2023-05-12 17:30:09.000000 pymx2-0.1.6/pymx2.egg-info/dependency_links.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)        9 2023-05-12 17:30:09.000000 pymx2-0.1.6/pymx2.egg-info/requires.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       10 2023-05-12 17:30:09.000000 pymx2-0.1.6/pymx2.egg-info/top_level.txt
+-rw-r--r--   0 vpaeder    (501) staff       (20)       38 2023-05-12 17:30:09.543174 pymx2-0.1.6/setup.cfg
+-rw-r--r--   0 vpaeder    (501) staff       (20)     1056 2023-05-12 17:28:14.000000 pymx2-0.1.6/setup.py
+drwxr-xr-x   0 vpaeder    (501) staff       (20)        0 2023-05-12 17:30:09.541826 pymx2-0.1.6/tests/
+-rw-r--r--   0 vpaeder    (501) staff       (20)      144 2023-04-27 07:40:09.000000 pymx2-0.1.6/tests/__init__.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    15021 2023-05-02 15:00:57.000000 pymx2-0.1.6/tests/inverter.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     4511 2023-05-02 14:58:17.000000 pymx2-0.1.6/tests/modbus.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)     3616 2023-04-21 10:52:45.000000 pymx2-0.1.6/tests/ser.py
+-rw-r--r--   0 vpaeder    (501) staff       (20)    10281 2023-04-27 12:31:47.000000 pymx2-0.1.6/tests/types.py
```

### Comparing `pymx2-0.1.5/LICENSE` & `pymx2-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/PKG-INFO` & `pymx2-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.5/README.md` & `pymx2-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/docs/mx2.enums.html` & `pymx2-0.1.6/docs/mx2.enums.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/docs/mx2.exceptions.html` & `pymx2-0.1.6/docs/mx2.exceptions.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/docs/mx2.html` & `pymx2-0.1.6/docs/mx2.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/docs/mx2.types.html` & `pymx2-0.1.6/docs/mx2.types.html`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/examples/02_read_write_coil.py` & `pymx2-0.1.6/examples/02_read_write_coil.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/examples/03_read_registers.py` & `pymx2-0.1.6/examples/03_read_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/examples/04_write_registers.py` & `pymx2-0.1.6/examples/04_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/examples/05_read_write_registers.py` & `pymx2-0.1.6/examples/05_read_write_registers.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/examples/06_data_types.py` & `pymx2-0.1.6/examples/06_data_types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/mx2/__init__.py` & `pymx2-0.1.6/mx2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
         if register_count<1 or register_count>16:
             raise BadParameterException("Invalid register count (must be between 1 and 16).")
 
         if isinstance(start_address, Register):
             last_reg = start_address.next(register_count-1)[-1]
             word_count = last_reg.address - start_address.address + last_reg.n_words
             if word_count > 16:
-                BadParameterException("Register count spans a too large address range.")
+                raise BadParameterException("Register count spans a too large address range.")
         else:
             word_count = register_count
         
         self._send(FunctionCode.ReadHoldingRegister, bytes([
             (start_address-1) >> 8,
             (start_address-1) & 0xff,
             0,
```

### Comparing `pymx2-0.1.5/mx2/enums.py` & `pymx2-0.1.6/mx2/enums.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/mx2/exceptions.py` & `pymx2-0.1.6/mx2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/mx2/types.py` & `pymx2-0.1.6/mx2/types.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/pymx2.egg-info/PKG-INFO` & `pymx2-0.1.6/pymx2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymx2
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python driver to communicate with an Omron MX2 inverter through Modbus
 Home-page: https://github.com/vpaeder/pymx2
 Author: Vincent Paeder
 Author-email: python@paeder.fi
 Project-URL: Bug Tracker, https://github.com/vpaeder/pymx2/issues
 Keywords: omron,mx2,inverter
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pymx2-0.1.5/pymx2.egg-info/SOURCES.txt` & `pymx2-0.1.6/pymx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/setup.py` & `pymx2-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymx2",
-    version="0.1.5",
+    version="0.1.6",
     author="Vincent Paeder",
     author_email="python@paeder.fi",
     description="A Python driver to communicate with an Omron MX2 inverter through Modbus",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['omron', 'mx2', 'inverter'],
     url="https://github.com/vpaeder/pymx2",
```

### Comparing `pymx2-0.1.5/tests/inverter.py` & `pymx2-0.1.6/tests/inverter.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/tests/modbus.py` & `pymx2-0.1.6/tests/modbus.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/tests/ser.py` & `pymx2-0.1.6/tests/ser.py`

 * *Files identical despite different names*

### Comparing `pymx2-0.1.5/tests/types.py` & `pymx2-0.1.6/tests/types.py`

 * *Files identical despite different names*

