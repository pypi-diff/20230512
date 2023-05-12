# Comparing `tmp/mmcb-avt-0.0.88.tar.gz` & `tmp/mmcb-avt-0.0.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.88.tar", last modified: Fri May 12 09:55:16 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.89.tar", last modified: Fri May 12 10:50:20 2023, max compression
```

## Comparing `mmcb-avt-0.0.88.tar` & `mmcb-avt-0.0.89.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:55:16.694043 mmcb-avt-0.0.88/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.88/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 09:55:16.692481 mmcb-avt-0.0.88/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     8165 2023-05-11 21:03:57.000000 mmcb-avt-0.0.88/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.88/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-12 09:55:16.694377 mmcb-avt-0.0.88/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-12 09:54:30.000000 mmcb-avt-0.0.88/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:55:16.649498 mmcb-avt-0.0.88/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:55:16.683769 mmcb-avt-0.0.88/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.88/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.88/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.88/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.88/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.88/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.88/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.88/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4545 2023-05-12 09:54:32.000000 mmcb-avt-0.0.88/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.88/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.88/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.88/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.88/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.88/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.88/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.88/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.88/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.88/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.88/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.88/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.88/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:55:16.691324 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-12 09:55:16.000000 mmcb-avt-0.0.88/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.393566 mmcb-avt-0.0.89/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.89/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-12 10:50:20.392777 mmcb-avt-0.0.89/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.89/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.89/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-12 10:50:20.393788 mmcb-avt-0.0.89/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-12 10:49:59.000000 mmcb-avt-0.0.89/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.346208 mmcb-avt-0.0.89/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.385772 mmcb-avt-0.0.89/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.89/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.89/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.89/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.89/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.89/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.89/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.89/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4545 2023-05-12 10:00:32.000000 mmcb-avt-0.0.89/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.89/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.89/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.89/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.89/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.89/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.89/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.89/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.89/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.89/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.89/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.89/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.89/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.391787 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.88/LICENSE` & `mmcb-avt-0.0.89/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/PKG-INFO` & `mmcb-avt-0.0.89/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.88
+Version: 0.0.89
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
@@ -174,29 +174,27 @@
 Python 3.9.2 (default, Feb 28 2021, 17:03:44)
 [GCC 10.2.1 20210110] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> from mmcb import dmm_interface
 cache: keithley instruments dmm6500 serial number 04592428 on /dev/ttyUSB0
 >>> dmm = dmm_interface.Dmm6500()
 >>> dmm.
-dmm.channel                      dmm.configure_read_resistance(   dmm.pipeline
-dmm.channels                     dmm.configure_read_temperature(  dmm.port
-dmm.config                       dmm.details                      dmm.read_value(
-dmm.configure_read_ac_current(   dmm.device_channels              dmm.release_delay
-dmm.configure_read_ac_voltage(   dmm.device_type                  dmm.remove(
-dmm.configure_read_capacitance(  dmm.instruments                  dmm.removed
-dmm.configure_read_dc_current(   dmm.manufacturer                 dmm.ser
-dmm.configure_read_dc_voltage(   dmm.model                        dmm.serial_number
+dmm.configure_read_ac_current(   dmm.configure_read_dc_voltage(   dmm.remove(
+dmm.configure_read_ac_voltage(   dmm.configure_read_resistance(   dmm.removed
+dmm.configure_read_capacitance(  dmm.configure_read_temperature(
+dmm.configure_read_dc_current(   dmm.read_value(
 
 >>> dmm.configure_read_capacitance()
->>> dmm.read_value()
-1.0177340937e-07
+>>> c = dmm.read_value()
+>>> c
+1.0465248938e-07
+
 >>> from mmcb import common
->>> common.si_prefix(dmm.read_value())
-'101.641n'
+>>> common.si_prefix(v)
+'104.652n'
 ```
 
 ## Check the installed version:
 
 ```console
 (pve) avt@raspberrypi:~ $ python3 -m pip show mmcb-avt
 Name: mmcb-avt
```

### Comparing `mmcb-avt-0.0.88/README.md` & `mmcb-avt-0.0.89/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -145,29 +145,27 @@
 Python 3.9.2 (default, Feb 28 2021, 17:03:44)
 [GCC 10.2.1 20210110] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> from mmcb import dmm_interface
 cache: keithley instruments dmm6500 serial number 04592428 on /dev/ttyUSB0
 >>> dmm = dmm_interface.Dmm6500()
 >>> dmm.
-dmm.channel                      dmm.configure_read_resistance(   dmm.pipeline
-dmm.channels                     dmm.configure_read_temperature(  dmm.port
-dmm.config                       dmm.details                      dmm.read_value(
-dmm.configure_read_ac_current(   dmm.device_channels              dmm.release_delay
-dmm.configure_read_ac_voltage(   dmm.device_type                  dmm.remove(
-dmm.configure_read_capacitance(  dmm.instruments                  dmm.removed
-dmm.configure_read_dc_current(   dmm.manufacturer                 dmm.ser
-dmm.configure_read_dc_voltage(   dmm.model                        dmm.serial_number
+dmm.configure_read_ac_current(   dmm.configure_read_dc_voltage(   dmm.remove(
+dmm.configure_read_ac_voltage(   dmm.configure_read_resistance(   dmm.removed
+dmm.configure_read_capacitance(  dmm.configure_read_temperature(
+dmm.configure_read_dc_current(   dmm.read_value(
 
 >>> dmm.configure_read_capacitance()
->>> dmm.read_value()
-1.0177340937e-07
+>>> c = dmm.read_value()
+>>> c
+1.0465248938e-07
+
 >>> from mmcb import common
->>> common.si_prefix(dmm.read_value())
-'101.641n'
+>>> common.si_prefix(v)
+'104.652n'
 ```
 
 ## Check the installed version:
 
 ```console
 (pve) avt@raspberrypi:~ $ python3 -m pip show mmcb-avt
 Name: mmcb-avt
```

### Comparing `mmcb-avt-0.0.88/setup.py` & `mmcb-avt-0.0.89/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.88",
+    version="0.0.89",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.88/src/mmcb/common.py` & `mmcb-avt-0.0.89/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.89/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.89/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/dat2root.py` & `mmcb-avt-0.0.89/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/detect.py` & `mmcb-avt-0.0.89/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/dmm.py` & `mmcb-avt-0.0.89/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.89/src/mmcb/dmm_interface.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/iv.py` & `mmcb-avt-0.0.89/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/lexicon.py` & `mmcb-avt-0.0.89/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/liveplot.py` & `mmcb-avt-0.0.89/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/log2dat.py` & `mmcb-avt-0.0.89/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/peltier.py` & `mmcb-avt-0.0.89/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/psuset.py` & `mmcb-avt-0.0.89/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/psustat.py` & `mmcb-avt-0.0.89/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/sense.py` & `mmcb-avt-0.0.89/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/sensors.py` & `mmcb-avt-0.0.89/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.89/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/sequence.py` & `mmcb-avt-0.0.89/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb/ult80.py` & `mmcb-avt-0.0.89/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.88/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.89/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.88
+Version: 0.0.89
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
@@ -174,29 +174,27 @@
 Python 3.9.2 (default, Feb 28 2021, 17:03:44)
 [GCC 10.2.1 20210110] on linux
 Type "help", "copyright", "credits" or "license" for more information.
 >>> from mmcb import dmm_interface
 cache: keithley instruments dmm6500 serial number 04592428 on /dev/ttyUSB0
 >>> dmm = dmm_interface.Dmm6500()
 >>> dmm.
-dmm.channel                      dmm.configure_read_resistance(   dmm.pipeline
-dmm.channels                     dmm.configure_read_temperature(  dmm.port
-dmm.config                       dmm.details                      dmm.read_value(
-dmm.configure_read_ac_current(   dmm.device_channels              dmm.release_delay
-dmm.configure_read_ac_voltage(   dmm.device_type                  dmm.remove(
-dmm.configure_read_capacitance(  dmm.instruments                  dmm.removed
-dmm.configure_read_dc_current(   dmm.manufacturer                 dmm.ser
-dmm.configure_read_dc_voltage(   dmm.model                        dmm.serial_number
+dmm.configure_read_ac_current(   dmm.configure_read_dc_voltage(   dmm.remove(
+dmm.configure_read_ac_voltage(   dmm.configure_read_resistance(   dmm.removed
+dmm.configure_read_capacitance(  dmm.configure_read_temperature(
+dmm.configure_read_dc_current(   dmm.read_value(
 
 >>> dmm.configure_read_capacitance()
->>> dmm.read_value()
-1.0177340937e-07
+>>> c = dmm.read_value()
+>>> c
+1.0465248938e-07
+
 >>> from mmcb import common
->>> common.si_prefix(dmm.read_value())
-'101.641n'
+>>> common.si_prefix(v)
+'104.652n'
 ```
 
 ## Check the installed version:
 
 ```console
 (pve) avt@raspberrypi:~ $ python3 -m pip show mmcb-avt
 Name: mmcb-avt
```

### Comparing `mmcb-avt-0.0.88/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.89/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

