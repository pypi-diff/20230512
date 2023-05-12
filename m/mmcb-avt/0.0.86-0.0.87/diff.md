# Comparing `tmp/mmcb-avt-0.0.86.tar.gz` & `tmp/mmcb-avt-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.86.tar", last modified: Fri May 12 08:27:24 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.87.tar", last modified: Fri May 12 09:50:06 2023, max compression
```

## Comparing `mmcb-avt-0.0.86.tar` & `mmcb-avt-0.0.87.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 08:27:24.577027 mmcb-avt-0.0.86/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.86/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 08:27:24.575656 mmcb-avt-0.0.86/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     8165 2023-05-11 21:03:57.000000 mmcb-avt-0.0.86/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.86/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-12 08:27:24.577341 mmcb-avt-0.0.86/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-12 08:27:07.000000 mmcb-avt-0.0.86/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 08:27:24.548792 mmcb-avt-0.0.86/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 08:27:24.569680 mmcb-avt-0.0.86/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.86/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.86/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.86/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.86/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.86/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.86/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.86/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4529 2023-05-12 08:25:40.000000 mmcb-avt-0.0.86/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.86/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.86/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.86/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.86/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.86/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.86/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.86/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.86/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.86/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.86/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.86/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.86/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 08:27:24.574679 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-12 08:27:24.000000 mmcb-avt-0.0.86/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:50:06.352105 mmcb-avt-0.0.87/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.87/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 09:50:06.350372 mmcb-avt-0.0.87/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     8165 2023-05-11 21:03:57.000000 mmcb-avt-0.0.87/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.87/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-12 09:50:06.353815 mmcb-avt-0.0.87/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-12 09:49:42.000000 mmcb-avt-0.0.87/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:50:06.296098 mmcb-avt-0.0.87/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:50:06.341562 mmcb-avt-0.0.87/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.87/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.87/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.87/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.87/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.87/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.87/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.87/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4533 2023-05-12 09:48:23.000000 mmcb-avt-0.0.87/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.87/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.87/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.87/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.87/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.87/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.87/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.87/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.87/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.87/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.87/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.87/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.87/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 09:50:06.348284 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9388 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-12 09:50:06.000000 mmcb-avt-0.0.87/src/mmcb_avt.egg-info/top_level.txt
```

### Comparing `mmcb-avt-0.0.86/LICENSE` & `mmcb-avt-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/PKG-INFO` & `mmcb-avt-0.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.86
+Version: 0.0.87
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.86/README.md` & `mmcb-avt-0.0.87/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/setup.py` & `mmcb-avt-0.0.87/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.86",
+    version="0.0.87",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.86/src/mmcb/common.py` & `mmcb-avt-0.0.87/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.87/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.87/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/dat2root.py` & `mmcb-avt-0.0.87/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/detect.py` & `mmcb-avt-0.0.87/src/mmcb/detect.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/dmm.py` & `mmcb-avt-0.0.87/src/mmcb/dmm.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.87/src/mmcb/dmm_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
     """
 
     _cached_instruments = common.cache_read({'instrument'})
 
     _channels = []
     for _port, _details in _cached_instruments.items():
         (
-            config,
+            _config,
             device_type,
             serial_number,
             model,
             manufacturer,
             device_channels,
             release_delay,
         ) = _details
 
         for _device_channel in device_channels:
             _channels.append(
                 common.Channel(
                     _port,
-                    config,
+                    _config,
                     serial_number,
                     model,
                     manufacturer,
                     _device_channel,
                     device_type,
                     release_delay,
                     None,
@@ -103,15 +103,15 @@
         returns : none
         -----------------------------------------------------------------------
         """
         common.send_command(
             self._pipeline,
             self._ser,
             self._channel,
-            lexicon.instrument(self.channel.model, command),
+            lexicon.instrument(self._channel.model, command),
         )
 
     def configure_read_capacitance(self):
         self._send_command('configure to read capacitance')
 
     def configure_read_ac_current(self):
         self._send_command('configure to read ac current')
@@ -143,15 +143,15 @@
             value : float or None
         -----------------------------------------------------------------------
         """
         response = common.atomic_send_command_read_response(
             self._pipeline,
             self._ser,
             self._channel,
-            lexicon.instrument(self.channel.model, 'read value'),
+            lexicon.instrument(self._channel.model, 'read value'),
         )
 
         try:
             value = float(response)
         except ValueError:
             value = None
```

### Comparing `mmcb-avt-0.0.86/src/mmcb/iv.py` & `mmcb-avt-0.0.87/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/lexicon.py` & `mmcb-avt-0.0.87/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/liveplot.py` & `mmcb-avt-0.0.87/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/log2dat.py` & `mmcb-avt-0.0.87/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/peltier.py` & `mmcb-avt-0.0.87/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/psuset.py` & `mmcb-avt-0.0.87/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/psustat.py` & `mmcb-avt-0.0.87/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/sense.py` & `mmcb-avt-0.0.87/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/sensors.py` & `mmcb-avt-0.0.87/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.87/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/sequence.py` & `mmcb-avt-0.0.87/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb/ult80.py` & `mmcb-avt-0.0.87/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.86/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.87/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.86
+Version: 0.0.87
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.86/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.87/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

