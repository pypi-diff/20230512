# Comparing `tmp/moku-2.6.2.tar.gz` & `tmp/moku-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moku-2.6.2.tar", last modified: Mon Feb 20 05:27:20 2023, max compression
+gzip compressed data, was "moku-3.0.0.tar", last modified: Fri May 12 04:51:08 2023, max compression
```

## Comparing `moku-2.6.2.tar` & `moku-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-02-20 05:27:20.142430 moku-2.6.2/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1158 2023-02-20 05:27:20.142430 moku-2.6.2/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-2.6.2/README.md
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-02-20 05:27:20.142430 moku-2.6.2/moku/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    10709 2023-02-20 03:41:30.000000 moku-2.6.2/moku/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     3758 2023-02-20 03:40:59.000000 moku-2.6.2/moku/cli.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-2.6.2/moku/exceptions.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-2.6.2/moku/finder.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-02-20 05:27:20.142430 moku-2.6.2/moku/instruments/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      618 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/__init__.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    11989 2023-02-20 03:40:52.000000 moku-2.6.2/moku/instruments/_awg.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     5563 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_cloudcompile.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    13107 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_datalogger.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    29029 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_digitalfilterbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    34115 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_firfilter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    13814 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_fra.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    35183 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_laserlockbox.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    27944 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_lockinamp.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    14999 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_logicanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     6148 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_mim.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    24035 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_oscilloscope.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    16699 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_phasemeter.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    28679 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_pidcontroller.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    12184 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_spectrumanalyzer.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     4394 2023-02-20 03:40:59.000000 moku-2.6.2/moku/instruments/_stream.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)    15254 2023-01-27 07:08:13.000000 moku-2.6.2/moku/instruments/_waveformgenerator.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     5819 2023-01-27 07:08:13.000000 moku-2.6.2/moku/session.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      502 2023-02-09 22:36:03.000000 moku-2.6.2/moku/utilities.py
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      311 2023-02-20 03:40:59.000000 moku-2.6.2/moku/version.py
-drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-02-20 05:27:20.142430 moku-2.6.2/moku.egg-info/
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1158 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/PKG-INFO
--rw-rw-r--   0 sashi     (1001) sashi     (1001)      883 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/SOURCES.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/dependency_links.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/entry_points.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-01-27 05:59:57.000000 moku-2.6.2/moku.egg-info/not-zip-safe
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/requires.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2023-02-20 05:27:20.000000 moku-2.6.2/moku.egg-info/top_level.txt
--rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2023-02-20 05:27:20.142430 moku-2.6.2/setup.cfg
--rw-rw-r--   0 sashi     (1001) sashi     (1001)     1610 2023-02-20 04:30:01.000000 moku-2.6.2/setup.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-05-12 04:51:08.929612 moku-3.0.0/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     2674 2022-12-12 03:43:28.000000 moku-3.0.0/README.md
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    11336 2023-05-05 05:13:11.000000 moku-3.0.0/moku/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     3758 2023-02-20 03:40:59.000000 moku-3.0.0/moku/cli.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1672 2023-01-27 07:08:13.000000 moku-3.0.0/moku/exceptions.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     4353 2022-12-12 03:43:28.000000 moku-3.0.0/moku/finder.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku/instruments/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      618 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/__init__.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    11544 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_awg.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     5563 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_cloudcompile.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    13107 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_datalogger.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    29487 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_digitalfilterbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    34552 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_firfilter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    14902 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_fra.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    35211 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_laserlockbox.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    27944 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_lockinamp.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    14999 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_logicanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6148 2023-04-10 23:20:50.000000 moku-3.0.0/moku/instruments/_mim.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    24210 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_oscilloscope.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    17079 2023-05-05 05:13:01.000000 moku-3.0.0/moku/instruments/_phasemeter.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    28679 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_pidcontroller.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    12184 2023-01-27 07:08:13.000000 moku-3.0.0/moku/instruments/_spectrumanalyzer.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     4394 2023-02-20 03:40:59.000000 moku-3.0.0/moku/instruments/_stream.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)    15462 2023-04-30 23:41:00.000000 moku-3.0.0/moku/instruments/_waveformgenerator.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     6189 2023-04-30 23:41:00.000000 moku-3.0.0/moku/session.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      502 2023-02-09 22:36:03.000000 moku-3.0.0/moku/utilities.py
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      311 2023-05-12 01:14:23.000000 moku-3.0.0/moku/version.py
+drwxrwxr-x   0 sashi     (1001) sashi     (1001)        0 2023-05-12 04:51:08.925612 moku-3.0.0/moku.egg-info/
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1146 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/PKG-INFO
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)      883 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/SOURCES.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/dependency_links.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       40 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/entry_points.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        1 2023-01-27 05:59:57.000000 moku-3.0.0/moku.egg-info/not-zip-safe
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       26 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/requires.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)        5 2023-05-12 04:51:08.000000 moku-3.0.0/moku.egg-info/top_level.txt
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)       38 2023-05-12 04:51:08.929612 moku-3.0.0/setup.cfg
+-rw-rw-r--   0 sashi     (1001) sashi     (1001)     1598 2023-05-12 04:50:47.000000 moku-3.0.0/setup.py
```

### Comparing `moku-2.6.2/PKG-INFO` & `moku-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 2.6.2
+Version: 3.0.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
-Description:  # noqa
+Description: 
                 # Moku
                 A Python library for the command, control and monitoring of
-                the [Liquid Instruments Moku:Pro & Moku:Go]
+                the [Liquid Instruments Moku hardware]
                 (http://www.liquidinstruments.com).
         
                 ## Installation
         
                     pip install moku
         
                 ## Useful links:
```

### Comparing `moku-2.6.2/README.md` & `moku-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/__init__.py` & `moku-3.0.0/moku/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import tarfile
 from hashlib import sha256
 from os import environ
 from pathlib import Path
 from shutil import which
 from subprocess import Popen, PIPE
 
@@ -65,17 +64,20 @@
         bs_path = MOKU_DATA_PATH.joinpath(bs_name)
         if bs_path.exists():
             bs_data = bs_path.read_bytes()
             if not (chksum and sha256(bs_data).hexdigest() == chksum):
                 self.upload("bitstreams", bs_name, bs_data)
         else:
             data_file = self._get_data_file(self.firmware_version)
+            hw_dir = {"mokupro": "mokupro",
+                      "mokugo": "mokugo", 
+                      "mokulab": "moku20"}
             with tarfile.open(data_file) as _ts:
                 bs_tarinfo = _ts.getmember(
-                    f"{self.hardware}/{bs_name}")
+                    f"{hw_dir[self.hardware]}/{bs_name}")
                 bs_file = _ts.extractfile(bs_tarinfo)
                 bs_data = bs_file.read()
                 if not (chksum and sha256(
                         bs_data).hexdigest() == chksum):
                     self.upload("bitstreams", bs_name, bs_data)
                 bs_file.close()
 
@@ -255,69 +257,84 @@
         params = dict(enable=enable, )
         return self.session.post("moku", operation, params)
 
     def upload(self, target, file_name, data):
         """
         Upload files to bitstreams, ssd, logs, persist.
 
-        :type target: `string`, (bitstreams, ssd, logs, persist)
+        :type target: `string`, (bitstreams, ssd, logs, persist, media)
         :param target: Destination where the file should be uploaded to.
 
         :type file_name: `string`
         :param file_name: Name of the file to be uploaded
 
         :type data: `bytes`
         :param data: File content
 
         """
         target = validate_range(target, list(
-            ['bitstreams', 'ssd', 'logs', 'persist']))
+            ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = f"upload/{file_name}"
         return self.session.post_file(target, operation, data)
 
     def delete(self, target, file_name):
         """
         Delete files from bitstreams, ssd, logs, persist.
 
-        :type target: `string`, (bitstreams, ssd, logs, persist)
+        :type target: `string`, (bitstreams, ssd, logs, persist, media)
         :param target: Destination where the file should be uploaded to.
 
         :type file_name: `string`
         :param file_name: Name of the file to be deleted
 
         """
         target = validate_range(target, list(
-            ['bitstreams', 'ssd', 'logs', 'persist']))
+            ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = f"delete/{file_name}"
         return self.session.delete_file(target, operation)
 
     def list(self, target):
         """
         List files at bitstreams, ssd, logs, persist.
 
-        :type target: `string`, (bitstreams, ssd, logs, persist)
+        :type target: `string`, (bitstreams, ssd, logs, persist, media)
         :param target: Target directory to list files for
 
         """
         target = validate_range(target, list(
-            ['bitstreams', 'ssd', 'logs', 'persist']))
+            ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = "list"
         return self.session.get(target, operation)
 
     def download(self, target, file_name, local_path):
         """
         Download files from bitstreams, ssd, logs, persist.
 
-        :type target: `string`, (bitstreams, ssd, logs, persist)
+        :type target: `string`, (bitstreams, ssd, logs, persist, media)
         :param target: Destination where the file should be downloaded from.
 
         :type file_name: `string`
         :param file_name: Name of the file to be downloaded
 
         :type local_path: `string`
         :param local_path: Local path to download the file
 
         """
         target = validate_range(target, list(
-            ['bitstreams', 'ssd', 'logs', 'persist']))
+            ['bitstreams', 'ssd', 'logs', 'persist', 'media']))
         operation = f"download/{file_name}"
         return self.session.get_file(target, operation, local_path)
+
+    def _modify_config(self, data=None):
+        if data is None:
+            data = {}
+        return self.session.post_to_v2("config", data)
+
+    def _modify_hardware(self, data=None):
+        if data is None:
+            data = {}
+        return self.session.post_to_v2("hwstate", data)
+
+    def _calibrate(self, data=None):
+        if data is None:
+            data = {}
+        return self.session.post_to_v2("calibration", data)
```

### Comparing `moku-2.6.2/moku/cli.py` & `moku-3.0.0/moku/cli.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/exceptions.py` & `moku-3.0.0/moku/exceptions.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/finder.py` & `moku-3.0.0/moku/finder.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/__init__.py` & `moku-3.0.0/moku/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_awg.py` & `moku-3.0.0/moku/instruments/_awg.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     def burst_modulate(
             self,
             channel,
             trigger_source,
             trigger_mode,
             burst_cycles=1,
             trigger_level=0,
-            input_range="4Vpp",
+            input_range=None,
             strict=True):
         """
         burst_modulate.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
@@ -311,15 +311,15 @@
 
         :type burst_cycles: `number` [1, 1e6]  (defaults to 1)
         :param burst_cycles: Number of cycles to generate when triggered
 
         :type trigger_level: `number` [-5V, 5V]  (defaults to 0)
         :param trigger_level: Trigger level
 
-        :type input_range: `string` ['Default', '400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']
+        :type input_range: `string` ['400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']
         :param input_range: Input Range
 
         """
         operation = "burst_modulate"
         params = dict(strict=strict,
                       channel=channel,
                       trigger_source=validate_range(trigger_source,
@@ -333,20 +333,13 @@
                                                      'InputD',
                                                      'External']),
                       trigger_mode=validate_range(trigger_mode,
                                                   ['Start',
                                                    'NCycle']),
                       burst_cycles=burst_cycles,
                       trigger_level=trigger_level,
-                      input_range=validate_range(input_range,
-                                                 ['Default',
-                                                  '400mVpp',
-                                                  '1Vpp',
-                                                  '4Vpp',
-                                                  '10Vpp',
-                                                  '40Vpp',
-                                                  '50Vpp']),
+                      input_range=input_range,
                       )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
```

### Comparing `moku-2.6.2/moku/instruments/_cloudcompile.py` & `moku-3.0.0/moku/instruments/_cloudcompile.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_datalogger.py` & `moku-3.0.0/moku/instruments/_datalogger.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_digitalfilterbox.py` & `moku-3.0.0/moku/instruments/_digitalfilterbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type channel: `integer`
         :param channel: Target channel
 
-        :type sample_rate: `string` ['3.906MHz', '488.3kHz', '61.04kHz', '39.06MHz', '4.883MHz', '305.2kHz']
+        :type sample_rate: `string` ['3.906MHz', '488.3kHz', '61.04kHz', '39.06MHz', '4.883MHz', '305.2kHz', '15.625MHz', '1.9531MHz', '122.07kHz']
         :param sample_rate: Sample rate
 
         :type shape: `string` ['Lowpass', 'Highpass', 'Bandpass', 'Bandstop']
         :param shape: Filter shape
 
         :type type: `string` ['Butterworth', 'ChebyshevI', 'ChebyshevII', 'Elliptic', 'Cascaded', 'Bessel', 'Gaussian', 'Legendre']
         :param type: Filter type
@@ -464,15 +464,18 @@
                       channel=channel,
                       sample_rate=validate_range(sample_rate,
                                                  ['3.906MHz',
                                                   '488.3kHz',
                                                   '61.04kHz',
                                                   '39.06MHz',
                                                   '4.883MHz',
-                                                  '305.2kHz']),
+                                                  '305.2kHz',
+                                                  '15.625MHz',
+                                                  '1.9531MHz', 
+                                                  '122.07kHz']),
                       shape=validate_range(shape,
                                            ['Lowpass',
                                             'Highpass',
                                             'Bandpass',
                                             'Bandstop']),
                       type=validate_range(type,
                                           ['Butterworth',
@@ -506,15 +509,15 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type channel: `integer`
         :param channel: Target channel
 
-        :type sample_rate: `string` ['3.906MHz', '488.3kHz', '61.04kHz', '39.06MHz', '4.883MHz', '305.2kHz']
+        :type sample_rate: `string` ['3.906MHz', '488.3kHz', '61.04kHz', '39.06MHz', '4.883MHz', '305.2kHz', '15.625MHz', '1.9531MHz', '122.07kHz']
         :param sample_rate: Sample rate
 
         :type scaling: `number`
         :param scaling: Output scaling
 
         :type coefficients: `list`
         :param coefficients: List of filter stages, where each stage should have six coefficients and each coefficient must be in the range [-4.0, 4.0]
@@ -525,15 +528,18 @@
                       channel=channel,
                       sample_rate=validate_range(sample_rate,
                                                  ['3.906MHz',
                                                   '488.3kHz',
                                                   '61.04kHz',
                                                   '39.06MHz',
                                                   '4.883MHz',
-                                                  '305.2kHz']),
+                                                  '305.2kHz',
+                                                  '15.625MHz',
+                                                  '1.9531MHz', 
+                                                  '122.07kHz']),
                       scaling=scaling,
                       coefficients=coefficients,
                       )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
@@ -920,18 +926,18 @@
         try:
             error = json.loads(result.content)
             raise StreamException(error.get('error', error))
         except StreamException as e:
             raise e
         except Exception:
             return result.content
+
     def get_stream_status(self):
         """
         get_stream_status.
 
         """
         operation = "get_stream_status"
 
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation)
-
```

### Comparing `moku-2.6.2/moku/instruments/_firfilter.py` & `moku-3.0.0/moku/instruments/_firfilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,15 +430,15 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type channel: `integer`
         :param channel: Target channel
 
-        :type sample_rate: `string` ['3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
+        :type sample_rate: `string` ['15.63MHz','7.813MHz','3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
         :param sample_rate: Sample rate
 
         :type coefficient_count: `integer`
         :param coefficient_count: Coefficient count
 
         :type shape: `string` ['Lowpass', 'Highpass', 'Bandpass', 'Bandstop']
         :param shape: Filter shape
@@ -459,15 +459,17 @@
         :param kaiser_order: Beta/Order for kaiser window
 
         """
         operation = "set_by_frequency"
         params = dict(strict=strict,
                       channel=channel,
                       sample_rate=validate_range(sample_rate,
-                                                 ['3.906MHz',
+                                                 ['15.63MHz',
+                                                  '7.813MHz',
+                                                  '3.906MHz',
                                                   '1.953MHz',
                                                   '976.6kHz',
                                                   '488.3kHz',
                                                   '244.1kHz',
                                                   '122.1kHz',
                                                   '61.04kHz',
                                                   '30.52kHz',
@@ -520,15 +522,15 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type channel: `integer`
         :param channel: Target channel
 
-        :type sample_rate: `string` ['3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
+        :type sample_rate: `string` ['15.63MHz','7.813MHz','3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
         :param sample_rate: Sample rate
 
         :type coefficient_count: `integer`
         :param coefficient_count: Coefficient count
 
         :type response: `string` ['Rectangular', 'Sinc', 'Triangular', 'Gaussian']
         :param response: Impulse response shape
@@ -546,15 +548,17 @@
         :param kaiser_order: Beta/Order for kaiser window
 
         """
         operation = "set_by_time"
         params = dict(strict=strict,
                       channel=channel,
                       sample_rate=validate_range(sample_rate,
-                                                 ['3.906MHz',
+                                                 ['15.63MHz',
+                                                  '7.813MHz',
+                                                  '3.906MHz',
                                                   '1.953MHz',
                                                   '976.6kHz',
                                                   '488.3kHz',
                                                   '244.1kHz',
                                                   '122.1kHz',
                                                   '61.04kHz',
                                                   '30.52kHz',
@@ -601,26 +605,28 @@
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type channel: `integer`
         :param channel: Target channel
 
-        :type sample_rate: `string` ['3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
+        :type sample_rate: `string` ['15.63MHz','7.813MHz','3.906MHz', '1.953MHz', '976.6kHz', '488.3kHz', '244.1kHz', '122.1kHz', '61.04kHz', '30.52kHz', '39.06MHz', '19.53MHz', '9.766MHz', '4.883MHz', '2.441MHz', '1.221MHz', '610.4kHz', '305.2kHz']
         :param sample_rate: Sample rate
 
         :type coefficients: `list`
         :param coefficients: Coefficients normalized to range [-1.0, 1.0]
 
         """
         operation = "set_custom_kernel_coefficients"
         params = dict(strict=strict,
                       channel=channel,
                       sample_rate=validate_range(sample_rate,
-                                                 ['3.906MHz',
+                                                 ['15.63MHz',
+                                                  '7.813MHz',
+                                                  '3.906MHz',
                                                   '1.953MHz',
                                                   '976.6kHz',
                                                   '488.3kHz',
                                                   '244.1kHz',
                                                   '122.1kHz',
                                                   '61.04kHz',
                                                   '30.52kHz',
@@ -1032,8 +1038,7 @@
 
         """
         operation = "get_stream_status"
 
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation)
-
```

### Comparing `moku-2.6.2/moku/instruments/_fra.py` & `moku-3.0.0/moku/instruments/_fra.py`

 * *Files 3% similar despite different names*

```diff
@@ -410,14 +410,57 @@
         """
         get_harmonic_multiplier.
         """
         operation = "get_harmonic_multiplier"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
+    
+    def set_output_load(self, channel, load, strict=True):
+        """
+        set_output_load.
+
+        :type strict: `boolean`
+        :param strict: Disable all implicit conversions and coercions.
+
+        :type channel: `integer`
+        :param channel: Target channel
+
+        :type load: `string` ['1MOhm', '50Ohm']
+        :param load: Output load
+
+        """
+        operation = "set_output_load"
+        params = dict(
+            strict=strict,
+            channel=channel,
+            load=validate_range(load, ['1MOhm', '50Ohm']),
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
+    def get_output_load(self, channel):
+        """
+        get_output_load.
+
+        :type channel: `integer`
+        :param channel: Target channel
+
+        """
+        operation = "get_output_load"
+        params = dict(
+            channel=channel,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
     def get_data(self, timeout=60, wait_reacquire=False):
         """
         get_data.
 
         :type timeout: `number` Seconds (defaults to 60)
         :param timeout: Wait for n seconds to receive a data frame
```

### Comparing `moku-2.6.2/moku/instruments/_laserlockbox.py` & `moku-3.0.0/moku/instruments/_laserlockbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,29 +446,29 @@
     def set_demodulation(self, mode, frequency=1000000, phase=0, strict=True):
         """
         set_demodulation.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
-        :type mode: `string` ['Internal', 'External', 'ExternalPLL', 'None']
+        :type mode: `string` ['Modulation', 'Internal', 'External', 'ExternalPLL', 'None']
         :param mode: Demodulation mode
 
         :type frequency: `number`
         :param frequency: Demodulation signal frequency
 
         :type phase: `number`
         :param phase: Demodulation signal phase
 
         """
         operation = "set_demodulation"
         params = dict(
             strict=strict,
             mode=validate_range(
-                mode, ['Internal', 'External', 'ExternalPLL', 'None']),
+                mode, ['Modulation', 'Internal', 'External', 'ExternalPLL', 'None']),
             frequency=frequency,
             phase=phase,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
```

### Comparing `moku-2.6.2/moku/instruments/_lockinamp.py` & `moku-3.0.0/moku/instruments/_lockinamp.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_logicanalyzer.py` & `moku-3.0.0/moku/instruments/_logicanalyzer.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_mim.py` & `moku-3.0.0/moku/instruments/_mim.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_oscilloscope.py` & `moku-3.0.0/moku/instruments/_oscilloscope.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,33 +431,37 @@
         """
         summary.
         """
         operation = "summary"
         return self.session.get(
             f"slot{self.slot}/{self.operation_group}", operation)
 
-    def set_timebase(self, t1, t2, strict=True):
+    def set_timebase(self, t1, t2, frame_length=1024, strict=True):
         """
         set_timebase.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
         :type t1: `number`
         :param t1: Time from the trigger point to the left of screen. This may be negative (trigger on-screen) or positive (trigger off the left of screen).
 
         :type t2: `number`
         :param t2: Time from the trigger point to the right of screen. (Must be a positive number, i.e. after the trigger event)
 
+        :type frame_length: `number`
+        :param frame_length: Length of the frame to retrieve through get_data()
+
         """
         operation = "set_timebase"
         params = dict(
             strict=strict,
             t1=t1,
             t2=t2,
+            frame_length=frame_length
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_hysteresis(self, hysteresis_mode, value=0, strict=True):
```

### Comparing `moku-2.6.2/moku/instruments/_phasemeter.py` & `moku-3.0.0/moku/instruments/_phasemeter.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             operation,
             params)
 
     def set_pm_loop(
             self,
             channel,
             auto_acquire=False,
-            frequency=30000000,
+            frequency=1e6,
             bandwidth="1kHz",
             strict=True):
         """
         set_pm_loop.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
@@ -238,15 +238,15 @@
             params)
 
     def generate_output(
             self,
             channel,
             signal,
             amplitude=0.5,
-            frequency=30000000,
+            frequency=1e6,
             frequency_multplier=1,
             phase=0,
             phase_locked=False,
             scaling=0.001,
             strict=True):
         """
         generate_output.
@@ -314,14 +314,31 @@
             channel=channel,
         )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
+    def disable_input(self, channel):
+        """
+        disable_input.
+
+        :type channel: `integer`
+        :param channel: Target channel
+
+        """
+        operation = "disable_input"
+        params = dict(
+            channel=channel,
+        )
+        return self.session.post(
+            f"slot{self.slot}/{self.operation_group}",
+            operation,
+            params)
+
     def enable_freewheeling(self, enable=True, strict=True):
         """
         enable_freewheeling.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
```

### Comparing `moku-2.6.2/moku/instruments/_pidcontroller.py` & `moku-3.0.0/moku/instruments/_pidcontroller.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_spectrumanalyzer.py` & `moku-3.0.0/moku/instruments/_spectrumanalyzer.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_stream.py` & `moku-3.0.0/moku/instruments/_stream.py`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/moku/instruments/_waveformgenerator.py` & `moku-3.0.0/moku/instruments/_waveformgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,15 @@
             channel,
             source,
             mode,
             trigger_level=0,
             burst_cycles=3,
             burst_duration=0.1,
             burst_period=1,
+            input_range=None,
             strict=True):
         """
         set_burst_mode.
 
         :type strict: `boolean`
         :param strict: Disable all implicit conversions and coercions.
 
@@ -323,14 +324,17 @@
 
         :type burst_duration: `number` [1 cycle periodSec, 1e3Sec]  (defaults to 0.1)
         :param burst_duration: Burst duration
 
         :type burst_period: `number`
         :param burst_period: Burst Period
 
+        :type input_range: `string` ['400mVpp', '1Vpp', '4Vpp', '10Vpp', '40Vpp', '50Vpp']
+        :param input_range: Input Range
+
         """
         operation = "set_burst_mode"
         params = dict(strict=strict,
                       channel=channel,
                       source=validate_range(source,
                                             ['Input1',
                                              'Input2',
@@ -352,14 +356,15 @@
                                           ['Gated',
                                            'Start',
                                            'NCycle']),
                       trigger_level=trigger_level,
                       burst_cycles=burst_cycles,
                       burst_duration=burst_duration,
                       burst_period=burst_period,
+                      input_range=input_range
                       )
         return self.session.post(
             f"slot{self.slot}/{self.operation_group}",
             operation,
             params)
 
     def set_sweep_mode(
```

### Comparing `moku-2.6.2/moku/session.py` & `moku-3.0.0/moku/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,26 @@
         return self.rs.post(self.url_for(group, operation),
                             json=params,
                             timeout=self.timeout_headers(_to_inc),
                             headers=self.json_headers)
 
     def post_to_v2_raw(self, location, params=None):
         response = self.rs.post(self.url_for_v2(location),
-                            json=params)
+                                json=params)
         return response
 
+    def post_to_v2(self, location, params=None):
+        response = self.rs.post(self.url_for_v2(location),
+                                json=params)
+        if response.status_code != 200:
+            raise exceptions.MokuException(
+                f"Cannot fulfil request, error code "
+                f"{response.status_code}")
+        return response.json()
+
     def get_file(self, group, operation, local_path):
         with self.rs.get(self.url_for(group, operation),
                          stream=True) as r:
             with open(local_path, 'wb') as f:
                 for chunk in r.iter_content(chunk_size=8192):
                     f.write(chunk)
```

### Comparing `moku-2.6.2/moku.egg-info/PKG-INFO` & `moku-3.0.0/moku.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: moku
-Version: 2.6.2
+Version: 3.0.0
 Summary: Python scripting interface to the Liquid Instruments Moku hardware
 Home-page: https://liquidinstruments.com
 Author: Liquid Instruments
 Author-email: info@liquidinstruments.com
 License: MIT
-Description:  # noqa
+Description: 
                 # Moku
                 A Python library for the command, control and monitoring of
-                the [Liquid Instruments Moku:Pro & Moku:Go]
+                the [Liquid Instruments Moku hardware]
                 (http://www.liquidinstruments.com).
         
                 ## Installation
         
                     pip install moku
         
                 ## Useful links:
```

### Comparing `moku-2.6.2/moku.egg-info/SOURCES.txt` & `moku-3.0.0/moku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moku-2.6.2/setup.py` & `moku-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import os.path
 
 setup(
     name="moku",
-    version="2.6.2",
+    version="3.0.0",
     author='Liquid Instruments',
     author_email='info@liquidinstruments.com',
     packages=['moku'],
     package_dir={'moku': 'moku'},
     package_data={
         'moku': [
             os.path.join('instruments', '*'),
@@ -17,18 +17,18 @@
         'console_scripts': [
             'moku=moku.cli:main',
         ]
     },
     license='MIT',
     description=("Python scripting interface to the "
                  "Liquid Instruments Moku hardware"),
-    long_description=""" # noqa
+    long_description="""
         # Moku
         A Python library for the command, control and monitoring of
-        the [Liquid Instruments Moku:Pro & Moku:Go]
+        the [Liquid Instruments Moku hardware]
         (http://www.liquidinstruments.com).
 
         ## Installation
 
             pip install moku
 
         ## Useful links:
```

