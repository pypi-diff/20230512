# Comparing `tmp/picocosmo-0.9.0.tar.gz` & `tmp/picocosmo-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picocosmo-0.9.0.tar", last modified: Fri May 12 18:11:25 2023, max compression
+gzip compressed data, was "picocosmo-0.9.0rc1.tar", last modified: Sun Oct  9 14:16:48 2022, max compression
```

## Comparing `picocosmo-0.9.0.tar` & `picocosmo-0.9.0rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:11:25.659909 picocosmo-0.9.0/
--rwxrwxr-x   0 root         (0) root         (0)      468 2023-05-06 17:42:42.000000 picocosmo-0.9.0/CosmoGui.py
--rw-rw-r--   0 root         (0) root         (0)     1352 2023-05-06 17:42:42.000000 picocosmo-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2411 2023-05-12 18:11:25.659909 picocosmo-0.9.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1883 2023-05-06 17:42:42.000000 picocosmo-0.9.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:11:25.655909 picocosmo-0.9.0/picocosmo/
--rw-rw-r--   0 root         (0) root         (0)    15737 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/CosmoGuiUi.py
--rw-rw-r--   0 root         (0) root         (0)    29862 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/PulseFilter.py
--rw-rw-r--   0 root         (0) root         (0)      920 2023-05-12 18:07:44.000000 picocosmo-0.9.0/picocosmo/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      416 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/_version_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:11:25.655909 picocosmo-0.9.0/picocosmo/doc/
--rw-rw-r--   0 root         (0) root         (0)     4480 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/doc/Hilfe.html
--rw-rw-r--   0 root         (0) root         (0)     4505 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/doc/help.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:11:25.655909 picocosmo-0.9.0/picocosmo/images/
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/CosmoKanne_icon.png
--rw-rw-r--   0 root         (0) root         (0)      726 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/CosmoPanels_icon.png
--rw-rw-r--   0 root         (0) root         (0)      632 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/application-exit.jpg
--rw-rw-r--   0 root         (0) root         (0)      226 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/flagDE.png
--rw-rw-r--   0 root         (0) root         (0)      950 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/flagUK.png
--rw-rw-r--   0 root         (0) root         (0)      577 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/open-folder.jpg
--rw-rw-r--   0 root         (0) root         (0)    19684 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/picoCosmo_iconic.jpg
--rw-rw-r--   0 root         (0) root         (0)      351 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/images/start.jpg
--rw-rw-r--   0 root         (0) root         (0)     7802 2023-05-12 18:07:44.000000 picocosmo-0.9.0/picocosmo/runCosmoDAQ.py
--rw-rw-r--   0 root         (0) root         (0)    18276 2023-05-06 17:42:42.000000 picocosmo-0.9.0/picocosmo/runCosmoUi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:11:25.655909 picocosmo-0.9.0/picocosmo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2411 2023-05-12 18:11:25.000000 picocosmo-0.9.0/picocosmo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-12 18:11:25.000000 picocosmo-0.9.0/picocosmo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:11:25.000000 picocosmo-0.9.0/picocosmo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-12 18:11:25.000000 picocosmo-0.9.0/picocosmo.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)     1439 2023-05-06 17:42:42.000000 picocosmo-0.9.0/runCosmo.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:11:25.659909 picocosmo-0.9.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1664 2023-05-10 21:07:36.000000 picocosmo-0.9.0/setup.py
+drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/
+-rwxrwxr-x   0 quast     (1000) quast     (1000)      468 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/CosmoGui.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)     2523 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/PKG-INFO
+-rw-rw-r--   0 quast     (1000) quast     (1000)     1883 2022-10-09 14:16:17.000000 picocosmo-0.9.0rc1/README
+-rw-rw-r--   0 quast     (1000) quast     (1000)    14044 2022-10-09 14:14:36.000000 picocosmo-0.9.0rc1/README.md
+drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:16:48.781080 picocosmo-0.9.0rc1/picocosmo/
+-rw-rw-r--   0 quast     (1000) quast     (1000)    15737 2020-08-02 08:16:16.000000 picocosmo-0.9.0rc1/picocosmo/CosmoGuiUi.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)    29862 2021-09-21 15:21:22.000000 picocosmo-0.9.0rc1/picocosmo/PulseFilter.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)      923 2022-10-09 13:08:04.000000 picocosmo-0.9.0rc1/picocosmo/__init__.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)      416 2020-08-02 08:16:16.000000 picocosmo-0.9.0rc1/picocosmo/_version_info.py
+drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/picocosmo/doc/
+-rw-rw-r--   0 quast     (1000) quast     (1000)     4480 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/doc/Hilfe.html
+-rw-rw-r--   0 quast     (1000) quast     (1000)     4505 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/doc/help.html
+drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/picocosmo/images/
+-rw-rw-r--   0 quast     (1000) quast     (1000)     1125 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/CosmoKanne_icon.png
+-rw-rw-r--   0 quast     (1000) quast     (1000)      726 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/CosmoPanels_icon.png
+-rw-rw-r--   0 quast     (1000) quast     (1000)      632 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/application-exit.jpg
+-rw-rw-r--   0 quast     (1000) quast     (1000)      226 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/flagDE.png
+-rw-rw-r--   0 quast     (1000) quast     (1000)      950 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/flagUK.png
+-rw-rw-r--   0 quast     (1000) quast     (1000)      577 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/open-folder.jpg
+-rw-rw-r--   0 quast     (1000) quast     (1000)    19684 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/picoCosmo_iconic.jpg
+-rw-rw-r--   0 quast     (1000) quast     (1000)      351 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/images/start.jpg
+-rw-rw-r--   0 quast     (1000) quast     (1000)     7792 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/picocosmo/runCosmoDAQ.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)    17159 2022-05-15 16:22:07.000000 picocosmo-0.9.0rc1/picocosmo/runCosmoUi.py
+drwxrwxr-x   0 quast     (1000) quast     (1000)        0 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/picocosmo.egg-info/
+-rw-rw-r--   0 quast     (1000) quast     (1000)     2523 2022-10-09 14:16:48.000000 picocosmo-0.9.0rc1/picocosmo.egg-info/PKG-INFO
+-rw-rw-r--   0 quast     (1000) quast     (1000)      644 2022-10-09 14:16:48.000000 picocosmo-0.9.0rc1/picocosmo.egg-info/SOURCES.txt
+-rw-rw-r--   0 quast     (1000) quast     (1000)        1 2022-10-09 14:16:48.000000 picocosmo-0.9.0rc1/picocosmo.egg-info/dependency_links.txt
+-rw-rw-r--   0 quast     (1000) quast     (1000)       10 2022-10-09 14:16:48.000000 picocosmo-0.9.0rc1/picocosmo.egg-info/top_level.txt
+-rwxrwxr-x   0 quast     (1000) quast     (1000)     1439 2022-02-20 09:15:07.000000 picocosmo-0.9.0rc1/runCosmo.py
+-rw-rw-r--   0 quast     (1000) quast     (1000)       38 2022-10-09 14:16:48.785080 picocosmo-0.9.0rc1/setup.cfg
+-rw-rw-r--   0 quast     (1000) quast     (1000)     1664 2022-10-09 14:16:37.000000 picocosmo-0.9.0rc1/setup.py
```

### Comparing `picocosmo-0.9.0/PKG-INFO` & `picocosmo-0.9.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: picocosmo
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary:  Analysis of waveforms from cosmic ray detectors
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
+Description: # picoCosmo
+        
+        *python* script to analyze data from CosMO detectors and Kamiokanne 
+        by Netzwerk Teilchenwelt with picoScope USB device.
+        
+        The software is tailored to identify short pulses from muon detectors (the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt", <http://www.teilchenwelt.de>, or the *Kamiokanne*-Experiment (a water-Cherenkov detector with photomultiplier readout) with a PicoScope USB oscilloscope with two or four channels.
+        
+        Reading out Geiger Counters or detectors for gamma rays, e. g. the GDK 101 PIN diode counter, is also
+        possible with the this software. 
+        
+        Data is read from the PicoScope device via a Buffer Manager, see project *picoDAQ* (<https://github.com/GuenterQuast/picoDAQ>), which records waveforms and distributes them to consumer processes. The consumers either provide real-time displays of a sub-set of the data or perform data analysis. *PiocoCosmo* is a specialised and extended version of the script *runDAQ.py* from project *picoDAQ*.
+        
+        The analysis proceeds in three steps. First, the trigger is validated by cross-correlation with a signal template located around the trigger time. Next, coincidences near a validated triggering pulse are searched for in all connected channels. The optional third step performs a search for additional pulses after the triggering event, indicating the decay of a stopped muon in or near the detector.
+        
+        The software provides real-time displays of waveforms, detector signals and rates. Optionally, parameters of identified pulses or of double-pulses are written to files in CSV format. In addition, raw waveforms or pictures in *.png* format of identified double pulses can optionally be stored for off-line analysis or for an instructive analysis "by hand" based on the waveform pictures. From this information, the mean muon lifetime in the muon rest frame (2.2 µs) can be derived. 
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
-
-# picoCosmo
-
-*python* script to analyze data from CosMO detectors and Kamiokanne 
-by Netzwerk Teilchenwelt with picoScope USB device.
-
-The software is tailored to identify short pulses from muon detectors (the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt", <http://www.teilchenwelt.de>, or the *Kamiokanne*-Experiment (a water-Cherenkov detector with photomultiplier readout) with a PicoScope USB oscilloscope with two or four channels.
-
-Reading out Geiger Counters or detectors for gamma rays, e. g. the GDK 101 PIN diode counter, is also
-possible with the this software. 
-
-Data is read from the PicoScope device via a Buffer Manager, see project *picoDAQ* (<https://github.com/GuenterQuast/picoDAQ>), which records waveforms and distributes them to consumer processes. The consumers either provide real-time displays of a sub-set of the data or perform data analysis. *PiocoCosmo* is a specialised and extended version of the script *runDAQ.py* from project *picoDAQ*.
-
-The analysis proceeds in three steps. First, the trigger is validated by cross-correlation with a signal template located around the trigger time. Next, coincidences near a validated triggering pulse are searched for in all connected channels. The optional third step performs a search for additional pulses after the triggering event, indicating the decay of a stopped muon in or near the detector.
-
-The software provides real-time displays of waveforms, detector signals and rates. Optionally, parameters of identified pulses or of double-pulses are written to files in CSV format. In addition, raw waveforms or pictures in *.png* format of identified double pulses can optionally be stored for off-line analysis or for an instructive analysis "by hand" based on the waveform pictures. From this information, the mean muon lifetime in the muon rest frame (2.2 µs) can be derived. 
-
-
```

### Comparing `picocosmo-0.9.0/README` & `picocosmo-0.9.0rc1/README`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/CosmoGuiUi.py` & `picocosmo-0.9.0rc1/picocosmo/CosmoGuiUi.py`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/PulseFilter.py` & `picocosmo-0.9.0rc1/picocosmo/PulseFilter.py`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/__init__.py` & `picocosmo-0.9.0rc1/picocosmo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     rates and store raw data, wave-form pictures or
     pulse features in files
 """
 
 # Import version info
 from ._version_info import *
 # and set version 
-_version_suffix = ''  # for suffixes such as 'rc' or 'beta' or 'alpha'
+_version_suffix = 'rc1'  # for suffixes such as 'rc' or 'beta' or 'alpha'
 __version__ = _version_info._get_version_string()
 __version__ += _version_suffix
 
 # Import components to be callabel at package level
 __all__ = ["runCosmoDAQ", "PulseFilter", "runCosmoUi"]
```

### Comparing `picocosmo-0.9.0/picocosmo/doc/Hilfe.html` & `picocosmo-0.9.0rc1/picocosmo/doc/Hilfe.html`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/doc/help.html` & `picocosmo-0.9.0rc1/picocosmo/doc/help.html`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/CosmoKanne_icon.png` & `picocosmo-0.9.0rc1/picocosmo/images/CosmoKanne_icon.png`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/CosmoPanels_icon.png` & `picocosmo-0.9.0rc1/picocosmo/images/CosmoPanels_icon.png`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/application-exit.jpg` & `picocosmo-0.9.0rc1/picocosmo/images/application-exit.jpg`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/flagUK.png` & `picocosmo-0.9.0rc1/picocosmo/images/flagUK.png`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/open-folder.jpg` & `picocosmo-0.9.0rc1/picocosmo/images/open-folder.jpg`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/images/picoCosmo_iconic.jpg` & `picocosmo-0.9.0rc1/picocosmo/images/picoCosmo_iconic.jpg`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/picocosmo/runCosmoDAQ.py` & `picocosmo-0.9.0rc1/picocosmo/runCosmoDAQ.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,17 +206,17 @@
     if 'modules' in self.PFconfdict:
       self.PFmodules = self.PFconfdict['modules']
     else:
       self.PFmodules = ['RMeter', 'Hists', 'Display' ]
 
   # run PulseFilter: signal filtering and analysis
     print(' -> initializing PulseFilter')
-    self.PF = PulseFilter( self.BM, self.PFconfdict, self.verbose)
+    PF = PulseFilter( self.BM, self.PFconfdict, self.verbose)
     #                 BM   config   verbose    
-    self.PF.run()
+    PF.run()
     time.sleep(1.)
 
   def run(self):
     """Data acquition loop
     """
 
     # start Buffer Manager
```

### Comparing `picocosmo-0.9.0/picocosmo/runCosmoUi.py` & `picocosmo-0.9.0rc1/picocosmo/runCosmoUi.py`

 * *Files 4% similar despite different names*

```diff
@@ -304,93 +304,65 @@
         if(DAQfile)==None:
           DAQfile= str(self.lE_RunTag.text() ).replace(' ','') + '.daq'
         fullDAQfile = confdir + '/' + DAQfile
         if verbose:
           if self.MB_Question('Question', 
             'saving Config to file ' + fullDAQfile) == QMessageBox.Cancel:
             return 1
-        try:
-          fDAQ = open(fullDAQfile, 'w')
-          print(DAQconf, file = fDAQ )
-          self.DAQfile = DAQfile
-          fDAQ.close()     
-        except Exception as e:
-          self.MB_Warning('Warning', 
-            'Failed to save '+ fullDAQfile + '\n' + str(e) )       
-          return 1
+        fDAQ = open(fullDAQfile, 'w')
+        print(DAQconf, file = fDAQ )
+        self.DAQfile = DAQfile
+        fDAQ.close()     
 
         # store all other configuration files   
 
         fnam = DAQconfDict['DeviceFile']
         dir, fn = os.path.split(fnam)
         if dir != '': 
           if not os.path.exists(confdir + '/' + dir):
-            os.makedirs(confdir + '/' + dir)
-        try: 
-          fPS = open(confdir + '/' + fnam, 'w')
-          print(PSconf, file = fPS )
-          fPS.close()
-        except Exception as e:
-          self.MB_Warning('Warning', 
-            'Failed to store ' + fnam + ' in directory ' + confdir + '\n' + str(e) )       
-          return 1
+            os.makedirs(confdir + '/' + dir) 
+        fPS = open(confdir + '/' + fnam, 'w')
+        print(PSconf, file = fPS )
+        fPS.close()
 
         fnam = DAQconfDict['BMfile']
         dir, fn = os.path.split(fnam)
         if dir != '': 
           if not os.path.exists(confdir + '/' + dir):
             os.makedirs(confdir + '/' + dir) 
-        try:
-          fBM = open(confdir + '/' + fnam, 'w')
-          print(BMconf, file = fBM )
-          fBM.close()
-        except Exception as e:
-          self.MB_Warning('Warning', 
-            'Failed to store ' + fnam + ' in directory ' + confdir + '\n' + str(e) )       
-          return 1
+        fBM = open(confdir + '/' + fnam, 'w')
+        print(BMconf, file = fBM )
+        fBM.close()
 
         fnam = DAQconfDict['PFfile']
         dir, fn = os.path.split(fnam)
         if dir != '': 
           if not os.path.exists(confdir + '/' + dir):
-            os.makedirs(confdir + '/' + dir)
-        try: 
-          fPF = open(confdir + '/' + fnam, 'w')
-          print(PFconf, file = fPF )
-          fPF.close()
-        except Exception as e:
-          self.MB_Warning('Warning', 
-            'Failed to store ' + fnam + ' in directory ' + confdir + '\n' + str(e) )       
-          return 1
-
-        return 0
+            os.makedirs(confdir + '/' + dir) 
+        fPF = open(confdir + '/' + fnam, 'w')
+        print(PFconf, file = fPF )
+        fPF.close()
 
     def saveDefaultConfig(self):
     # save configuration
       # propose name for DAQ configuration file from RunTag 
       _file = self.ConfDir + '/' + str(self.lE_RunTag.text() ).replace(' ','') + '.daq'
       # select file and direcotory 
       path2File = QtWidgets.QFileDialog.getSaveFileName(None,
          'save configuration as', _file, 'daq(*.daq)')
       fullDAQfile = str(path2File[0]).strip()
       if  fullDAQfile != '' :
       # remember new config directory
         self.ConfDir = os.path.dirname(fullDAQfile)
         DAQfile = os.path.basename(fullDAQfile)
       else:
-        print("   abort - no file name given") 
         return 1
      # set name and save all configs
       self.lE_DAQConfFile.setText(fullDAQfile)
-      if self.saveConfigs(self.ConfDir, DAQfile=DAQfile, verbose=0):
-        print("   !!! failed to save configuration files")
-        return 1
-      else:
-        print("   - configuration files stored in directory " + self.ConfDir)
-        return 0 
+      return self.saveConfigs(self.ConfDir, DAQfile=DAQfile, verbose=0)
 
     def saveEnvironment(self):
       '''
         Save picoCosmo configuration to file ~/CONFIG_ENVIRONMENT_file
       '''
       hd = os.getenv('HOME')
   # ... and find name of work directory
@@ -409,19 +381,16 @@
 
       # generate config files for new run in dedicated subdirectory
       self.runDir = (RunTag + '_' + datetime)
       self.path_to_WD = self.WDname + '/' + self.runDir
       if not os.path.exists(self.path_to_WD): 
         os.makedirs(self.path_to_WD)
       # store config in working directory 
-      if self.saveConfigs(self.path_to_WD):
-          print("   !!! failed to save Config files for this run") 
-          return 
-      else: 
-          print("   - files for this run stored in directory " + self.path_to_WD) 
+      if self.saveConfigs(self.path_to_WD): return
+      print("   - files for this run stored in directory " + self.path_to_WD) 
 
       # save changes to picocosmo environment
       self.saveEnvironment()
 
     # close GUI window and start runCosmo 
       print('\n*==* CosmoGui: closing window and starting runCosmo.py')
 #      self.Window.close()
```

### Comparing `picocosmo-0.9.0/picocosmo.egg-info/PKG-INFO` & `picocosmo-0.9.0rc1/picocosmo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: picocosmo
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary:  Analysis of waveforms from cosmic ray detectors
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
+Description: # picoCosmo
+        
+        *python* script to analyze data from CosMO detectors and Kamiokanne 
+        by Netzwerk Teilchenwelt with picoScope USB device.
+        
+        The software is tailored to identify short pulses from muon detectors (the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt", <http://www.teilchenwelt.de>, or the *Kamiokanne*-Experiment (a water-Cherenkov detector with photomultiplier readout) with a PicoScope USB oscilloscope with two or four channels.
+        
+        Reading out Geiger Counters or detectors for gamma rays, e. g. the GDK 101 PIN diode counter, is also
+        possible with the this software. 
+        
+        Data is read from the PicoScope device via a Buffer Manager, see project *picoDAQ* (<https://github.com/GuenterQuast/picoDAQ>), which records waveforms and distributes them to consumer processes. The consumers either provide real-time displays of a sub-set of the data or perform data analysis. *PiocoCosmo* is a specialised and extended version of the script *runDAQ.py* from project *picoDAQ*.
+        
+        The analysis proceeds in three steps. First, the trigger is validated by cross-correlation with a signal template located around the trigger time. Next, coincidences near a validated triggering pulse are searched for in all connected channels. The optional third step performs a search for additional pulses after the triggering event, indicating the decay of a stopped muon in or near the detector.
+        
+        The software provides real-time displays of waveforms, detector signals and rates. Optionally, parameters of identified pulses or of double-pulses are written to files in CSV format. In addition, raw waveforms or pictures in *.png* format of identified double pulses can optionally be stored for off-line analysis or for an instructive analysis "by hand" based on the waveform pictures. From this information, the mean muon lifetime in the muon rest frame (2.2 µs) can be derived. 
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-License-File: LICENSE
-
-# picoCosmo
-
-*python* script to analyze data from CosMO detectors and Kamiokanne 
-by Netzwerk Teilchenwelt with picoScope USB device.
-
-The software is tailored to identify short pulses from muon detectors (the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt", <http://www.teilchenwelt.de>, or the *Kamiokanne*-Experiment (a water-Cherenkov detector with photomultiplier readout) with a PicoScope USB oscilloscope with two or four channels.
-
-Reading out Geiger Counters or detectors for gamma rays, e. g. the GDK 101 PIN diode counter, is also
-possible with the this software. 
-
-Data is read from the PicoScope device via a Buffer Manager, see project *picoDAQ* (<https://github.com/GuenterQuast/picoDAQ>), which records waveforms and distributes them to consumer processes. The consumers either provide real-time displays of a sub-set of the data or perform data analysis. *PiocoCosmo* is a specialised and extended version of the script *runDAQ.py* from project *picoDAQ*.
-
-The analysis proceeds in three steps. First, the trigger is validated by cross-correlation with a signal template located around the trigger time. Next, coincidences near a validated triggering pulse are searched for in all connected channels. The optional third step performs a search for additional pulses after the triggering event, indicating the decay of a stopped muon in or near the detector.
-
-The software provides real-time displays of waveforms, detector signals and rates. Optionally, parameters of identified pulses or of double-pulses are written to files in CSV format. In addition, raw waveforms or pictures in *.png* format of identified double pulses can optionally be stored for off-line analysis or for an instructive analysis "by hand" based on the waveform pictures. From this information, the mean muon lifetime in the muon rest frame (2.2 µs) can be derived. 
-
-
```

### Comparing `picocosmo-0.9.0/picocosmo.egg-info/SOURCES.txt` & `picocosmo-0.9.0rc1/picocosmo.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 CosmoGui.py
-LICENSE
 README
+README.md
 runCosmo.py
 setup.py
 picocosmo/CosmoGuiUi.py
 picocosmo/PulseFilter.py
 picocosmo/__init__.py
 picocosmo/_version_info.py
 picocosmo/runCosmoDAQ.py
```

### Comparing `picocosmo-0.9.0/runCosmo.py` & `picocosmo-0.9.0rc1/runCosmo.py`

 * *Files identical despite different names*

### Comparing `picocosmo-0.9.0/setup.py` & `picocosmo-0.9.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,11 +45,11 @@
     ],
     url='https://www.etp.kit.edu/~quast/',
     license='GNU Public Licence',
     description=' Analysis of waveforms from cosmic ray detectors',
     long_description=open('README').read(),
     setup_requires=[\
         "picodaqa",
-        "NumPy >= 1.17.0",
+        "NumPy >= 1.16.2",
         "SciPy >= 1.1.0",
-        "matplotlib >= 3.4.0",]
+        "matplotlib >= 3.0.0",]
 )
```

