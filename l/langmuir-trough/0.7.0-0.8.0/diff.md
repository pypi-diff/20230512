# Comparing `tmp/langmuir_trough-0.7.0.tar.gz` & `tmp/langmuir_trough-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langmuir_trough-0.7.0.tar", last modified: Fri Apr 28 18:23:38 2023, max compression
+gzip compressed data, was "langmuir_trough-0.8.0.tar", last modified: Fri May 12 20:43:09 2023, max compression
```

## Comparing `langmuir_trough-0.7.0.tar` & `langmuir_trough-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.389111 langmuir_trough-0.7.0/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.385300 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/
--rw-r--r--   0 gutow    (60685682) staff       (20)     9734 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/SOURCES.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/dependency_links.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/requires.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-04-28 18:23:38.000000 langmuir_trough-0.7.0/Langmuir_Trough.egg-info/top_level.txt
--rw-r--r--   0 gutow    (60685682) staff       (20)     9734 2023-04-28 18:23:38.388951 langmuir_trough-0.7.0/PKG-INFO
--rw-r--r--   0 gutow    (60685682) staff       (20)     9080 2023-04-28 18:13:03.000000 langmuir_trough-0.7.0/README.md
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.385434 langmuir_trough-0.7.0/Trough/
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.386422 langmuir_trough-0.7.0/Trough/Trough_Control/
--rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/message_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_Control/simulation.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    35561 2023-04-28 17:11:38.000000 langmuir_trough-0.7.0/Trough/Trough_Control/trough_util.py
-drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-04-28 18:23:38.388455 langmuir_trough-0.7.0/Trough/Trough_GUI/
--rw-r--r--   0 gutow    (60685682) staff       (20)    29903 2023-04-28 17:39:19.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/Collect_data.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    28732 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/Monitor_Calibrate.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     3017 2023-04-28 14:28:17.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/calibration_utils.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    16304 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/command_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/conversions.py
--rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/Trough_GUI/status_widgets.py
--rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.7.0/Trough/__init__.py
--rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-04-28 18:23:38.389159 langmuir_trough-0.7.0/setup.cfg
--rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-04-28 18:13:03.000000 langmuir_trough-0.7.0/setup.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.703785 langmuir_trough-0.8.0/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.699881 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10405 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)      819 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/SOURCES.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        1 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/dependency_links.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)      348 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/requires.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)        7 2023-05-12 20:43:09.000000 langmuir_trough-0.8.0/Langmuir_Trough.egg-info/top_level.txt
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10405 2023-05-12 20:43:09.703604 langmuir_trough-0.8.0/PKG-INFO
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9751 2023-05-12 20:07:19.000000 langmuir_trough-0.8.0/README.md
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.700005 langmuir_trough-0.8.0/Trough/
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.700886 langmuir_trough-0.8.0/Trough/Trough_Control/
+-rw-r--r--   0 gutow    (60685682) staff       (20)      153 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      313 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/message_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     9991 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_Control/simulation.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    37129 2023-05-12 20:07:19.000000 langmuir_trough-0.8.0/Trough/Trough_Control/trough_util.py
+drwxr-xr-x   0 gutow    (60685682) staff       (20)        0 2023-05-12 20:43:09.703163 langmuir_trough-0.8.0/Trough/Trough_GUI/
+-rw-r--r--   0 gutow    (60685682) staff       (20)    30280 2023-05-12 19:37:48.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/Collect_data.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    28605 2023-05-12 14:45:53.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/Monitor_Calibrate.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     3017 2023-04-28 14:28:17.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    24079 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/calibration_utils.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    15590 2023-05-12 18:11:19.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/command_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)     2614 2023-05-10 20:38:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/conversions.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)    10038 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/Trough_GUI/status_widgets.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)      103 2023-03-29 22:32:39.000000 langmuir_trough-0.8.0/Trough/__init__.py
+-rw-r--r--   0 gutow    (60685682) staff       (20)       38 2023-05-12 20:43:09.703823 langmuir_trough-0.8.0/setup.cfg
+-rw-r--r--   0 gutow    (60685682) staff       (20)     1597 2023-05-12 20:14:13.000000 langmuir_trough-0.8.0/setup.py
```

### Comparing `langmuir_trough-0.7.0/Langmuir_Trough.egg-info/PKG-INFO` & `langmuir_trough-0.8.0/Langmuir_Trough.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langmuir-trough
-Version: 0.7.0
+Version: 0.8.0
 Summary: Controls and collects data from Gutow Lab Langmuir Trough.
 Home-page: https://github.com/gutow/Langmuir_Trough.git
 Author: Jonathan Gutow
 Author-email: gutow@uwosh.edu
 License: GPL-3.0+
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -125,14 +125,25 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.0 (May 12, 2023)
+  * Added capability to do very slow compressions (< 1 cm/min) by moving the 
+    barriers intermittently at near their lowest continuous speed.
+  * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
+    This avoids round off errors in the html based data storage file.
+  * BUG_FIXES:
+    * Errors in conversion of speeds between units.
+    * Make start boost voltage direction dependent.
+    * Fix inconsistent sign on skimmer corrections.
+    * Correct hanging of GUI updates during barrier calibrations.
+    * Fix wrong target value when units were cm**2.
 * 0.7.0 (Apr. 28, 2023)
   * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
     tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
     `Trough_GUI.newCalculatedColumn()`.
   * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
     clobbers an already running notebook that is talking to the trough 
     A-to-D hardware.
@@ -148,19 +159,20 @@
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.8.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
-* Runs don't label graph axes reliably for x-axis units other than cm.
+* Runs don't label graph axes reliably for x-axis units other than cm. This 
+  appears to be associated with Latex in ipywidgets as well.
 
 ## Development
 
 ### [CodeRepository](https://github.com/gutow/Langmuir_Trough.git) | [Docs](https://gutow.github.io/Langmuir_Trough)
 
 1. For development purposes clone the GIT repository.
 2. Create the virtual environment to run it in within the development
```

### Comparing `langmuir_trough-0.7.0/Langmuir_Trough.egg-info/SOURCES.txt` & `langmuir_trough-0.8.0/Langmuir_Trough.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.7.0/PKG-INFO` & `langmuir_trough-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: langmuir_trough
-Version: 0.7.0
-Summary: Controls and collects data from Gutow Lab Langmuir Trough.
-Home-page: https://github.com/gutow/Langmuir_Trough.git
-Author: Jonathan Gutow
-Author-email: gutow@uwosh.edu
-License: GPL-3.0+
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: JavaScript
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # Langmuir Trough
 This software is a custom controller and GUI for the research Langmuir trough 
 in the Gutow Lab at UW Oshkosh. It is written in Python and expects to run in a
 Jupyter notebook environment. However, all of the parts that are not elements
 of the user interface should work in a vanilla Python environment.
 
 Hardware requirements:
@@ -125,14 +108,25 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.0 (May 12, 2023)
+  * Added capability to do very slow compressions (< 1 cm/min) by moving the 
+    barriers intermittently at near their lowest continuous speed.
+  * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
+    This avoids round off errors in the html based data storage file.
+  * BUG_FIXES:
+    * Errors in conversion of speeds between units.
+    * Make start boost voltage direction dependent.
+    * Fix inconsistent sign on skimmer corrections.
+    * Correct hanging of GUI updates during barrier calibrations.
+    * Fix wrong target value when units were cm**2.
 * 0.7.0 (Apr. 28, 2023)
   * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
     tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
     `Trough_GUI.newCalculatedColumn()`.
   * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
     clobbers an already running notebook that is talking to the trough 
     A-to-D hardware.
@@ -148,19 +142,20 @@
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.8.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
-* Runs don't label graph axes reliably for x-axis units other than cm.
+* Runs don't label graph axes reliably for x-axis units other than cm. This 
+  appears to be associated with Latex in ipywidgets as well.
 
 ## Development
 
 ### [CodeRepository](https://github.com/gutow/Langmuir_Trough.git) | [Docs](https://gutow.github.io/Langmuir_Trough)
 
 1. For development purposes clone the GIT repository.
 2. Create the virtual environment to run it in within the development
```

### Comparing `langmuir_trough-0.7.0/README.md` & `langmuir_trough-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: langmuir_trough
+Version: 0.8.0
+Summary: Controls and collects data from Gutow Lab Langmuir Trough.
+Home-page: https://github.com/gutow/Langmuir_Trough.git
+Author: Jonathan Gutow
+Author-email: gutow@uwosh.edu
+License: GPL-3.0+
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: JavaScript
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # Langmuir Trough
 This software is a custom controller and GUI for the research Langmuir trough 
 in the Gutow Lab at UW Oshkosh. It is written in Python and expects to run in a
 Jupyter notebook environment. However, all of the parts that are not elements
 of the user interface should work in a vanilla Python environment.
 
 Hardware requirements:
@@ -108,14 +125,25 @@
     2. Issue the command to add this as a kernel to your personal space: 
     `$ python -m ipykernel install --user --name=<name-you-want-for-kernel>`.
     3. More information is available in the Jupyter/Ipython documentation. 
     A simple tutorial from Nikolai Jankiev (_Parametric Thoughts_) can be
      found [here](https://janakiev.com/til/jupyter-virtual-envs/). 
 
 ## Change Log
+* 0.8.0 (May 12, 2023)
+  * Added capability to do very slow compressions (< 1 cm/min) by moving the 
+    barriers intermittently at near their lowest continuous speed.
+  * Now record datapoint time_stamps as actual_time_stamp - run_time_stamp. 
+    This avoids round off errors in the html based data storage file.
+  * BUG_FIXES:
+    * Errors in conversion of speeds between units.
+    * Make start boost voltage direction dependent.
+    * Fix inconsistent sign on skimmer corrections.
+    * Correct hanging of GUI updates during barrier calibrations.
+    * Fix wrong target value when units were cm**2.
 * 0.7.0 (Apr. 28, 2023)
   * Added Access to [pandas_GUI](https://jupyterphysscilab.github.io/jupyter_Pandas_GUI)
     tools as `Trough_GUI.newPlot()`, `Trough_GUI.newFit()` and 
     `Trough_GUI.newCalculatedColumn()`.
   * BUG_FIX: Opening a new notebook and importing Trough_GUI no longer 
     clobbers an already running notebook that is talking to the trough 
     A-to-D hardware.
@@ -131,19 +159,20 @@
 * 0.5.1 (Mar. 9, 2023) 
   * Include `spidev` package in requirements. 
   * More details reported when unable to "find trough".
 * 0.5.0 (Mar. 4, 2023) First version with working GUI
 * 0.1.0 First pypi compatible package version.
 
 ## Known issues
-* 0.5.0 - 0.7.0 The estimated error on values converted to metric units 
+* 0.5.0 - 0.8.0 The estimated error on values converted to metric units 
   based on calibration fits appears to be too pessimistic.
 * Inconsistent rendering of Latex ipywidget labels with ipywidgets >= 8.0. 
   Until figured out requiring ipywidgets < 8.0.
-* Runs don't label graph axes reliably for x-axis units other than cm.
+* Runs don't label graph axes reliably for x-axis units other than cm. This 
+  appears to be associated with Latex in ipywidgets as well.
 
 ## Development
 
 ### [CodeRepository](https://github.com/gutow/Langmuir_Trough.git) | [Docs](https://gutow.github.io/Langmuir_Trough)
 
 1. For development purposes clone the GIT repository.
 2. Create the virtual environment to run it in within the development
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_Control/simulation.py` & `langmuir_trough-0.8.0/Trough/Trough_Control/simulation.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.7.0/Trough/Trough_Control/trough_util.py` & `langmuir_trough-0.8.0/Trough/Trough_Control/trough_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     Will run as separate process taking in commands through a pipe and
     returning data on demand through a second pipe.
     Iteration 1, collects data into a fifo and watches barrier position.
     :param Pipe CTLPipe: pipe commands come in on and messages go out on.
     :param Pipe DATAPipe: pipe data is sent out on
     """
     import time
+    from math import trunc
     import numpy as np
     from collections import deque
     from piplates import DAQC2plate as DAQC2
     from sys import exit
 
     def bundle_to_send(que_lst):
         """
@@ -304,15 +305,15 @@
         voltage is below the starting voltage.
         """
         DAC_V = calcDAC_V(speed, direction, maxcloseV, mincloseV, maxopenV,
                           minopenV)
         # print("speed:"+str(speed)+", direction:"+str(direction)+", DAC_V:"+str(DAC_V))
         if (DAC_V > startopenV) and (DAC_V < startcloseV) and (direction != 0):
             # need a boost to start moving
-            if speed == 1:
+            if direction == -1:
                 DAQC2.setDAC(0, 0, startcloseV)
             else:
                 DAQC2.setDAC(0, 0, startopenV)
             DAQC2.setDOUTbit(0, 0)
             time.sleep(0.25)
         DAQC2.setDAC(0, 0, DAC_V)
         DAQC2.setDOUTbit(0, 0)
@@ -655,28 +656,37 @@
         maxcloseV, mincloseV, startcloseV, maxopenV, minopenV, startopenV = motorcal(openlimit, closelimit)
     messages.append("Trough ready")
     DATAPipe.send(bundle_to_send(que_lst))
     messages.clear()
     speed = 0 # 0 to 1 fraction of maximum speed.
     direction = 0 # -1 close, 0 don't move, 1 open
     run = True
-    loopcount = 0
+    # cycles for doing very low speeds by stepping. If cycles_off = 0 then
+    # just runs continuously.
+    cycles_on = 1
+    cycles_off = 0
+    cycle_count = 0
+    moving_flag = False
     while run:
         poshigh = []
         poslow = []
         balhigh = []
         ballow = []
         thermhigh = []
         thermlow = []
 
+        if cycle_count >= (cycles_on+cycles_off):
+            cycle_count = 0
+        if cycle_count >= cycles_on:
+            DAQC2.clrDOUTbit(0, 0)  # switch off power/stop barriers
+        elif moving_flag:
+            DAQC2.setDOUTbit(0, 0)  # switch on power/start barriers
+
         starttime = time.time()
         stopat = starttime + timedelta - 0.200  # leave 200 ms for communications and control
-        #loopcount +=1
-        #print('Starting a data record: '+str(loopcount))
-        #itcount = 0
         while (time.time() < stopat):
             tempposlow = None
             tempposhigh= None
             tempballow = None
             tempbalhigh = None
             tempthermlow = None
             tempthermhigh = None
@@ -758,14 +768,16 @@
 
         # Check barrier positions
         if openlimit < openmin:
             openlimit = openmin
         if closelimit > closemax:
             closelimit = closemax
         barrier_at_limit = barrier_at_limit_check(openlimit,closelimit)
+        if barrier_at_limit:
+            moving_flag = False
         # TODO: Send warnings and error messages
         # Check command pipe and update command queue
         #print('Checking commands...')
         while CTLPipe.poll():
             cmd_deque.append(CTLPipe.recv())
         # Each command is a python list.
         #    element 1: cmd name (string)
@@ -774,14 +786,15 @@
         #print('Executing commands...')
         while len(cmd_deque) > 0:
             cmd = cmd_deque.popleft()
             # execute the command
             #print(str(cmd))
             if cmd[0] == 'Stop':
                 DAQC2.clrDOUTbit(0, 0)  # switch off power/stop barriers
+                moving_flag = False
             elif cmd[0] == 'Send':
                 #print('Got a "Send" command.')
                 # send current contents of the data deques
                 DATAPipe.send(bundle_to_send(que_lst))
                 # purge the sent content
                 time_stamp.clear()
                 pos_V.clear()
@@ -801,26 +814,46 @@
                     speed = 0
                 if (direction != -1) and (direction != 0) and (direction != 1):
                     direction = 0
                 closelimit = closemax
                 openlimit = openmin
                 start_barriers(speed, direction, maxcloseV, mincloseV, maxopenV,
                                minopenV)
+                moving_flag = True
             elif cmd[0] == 'Direction':
                 # set the direction
                 direction = cmd[1]
                 if (direction != -1) and (direction != 0) and (direction != 1):
                     direction = 0
             elif cmd[0] == 'Speed':
                 # set the speed
-                speed = cmd[1]
-                if speed > 1:
-                    speed = 1
-                if speed < 0:
-                    speed = 0
+                requested_speed = cmd[1]
+                if requested_speed > 1:
+                    requested_speed = 1
+                if requested_speed < 0:
+                    requested_speed = 0
+                if requested_speed < 0.1:
+                    # set up cycles to go at lower speeds
+                    ncycles = trunc(0.1/requested_speed) + 1
+                    if ncycles >= 2:
+                        cycles_on = 1
+                        cycles_off = ncycles - 1
+                        speed = requested_speed*ncycles
+                    else:
+                        ncycles = trunc(0.1/(0.1-requested_speed))
+                        cycles_on = ncycles - 1
+                        cycles_off = 1
+                        speed = requested_speed*ncycles/cycles_on
+                else:
+                    speed = requested_speed
+                speedstat=str("cycles_on="+str(cycles_on)+", cycles_off="
+                              +str(cycles_off)
+                              + ", requested speed="+str(requested_speed)+
+                                ", speed="+str(speed))
+                messages.append(speedstat)
                 pass
             elif cmd[0] == 'MoveTo':
                 # Move to fraction of open 0 .. 1.
                 # set the stop position
                 to_pos = (1.0-float(cmd[1]))*closemax + float(cmd[1])*openmin
                 # adjust direction if necessary
                 # get current position
@@ -831,14 +864,15 @@
                     openlimit = to_pos
                 else:
                     direction = -1
                     closelimit = to_pos
                 # start the barriers
                 start_barriers(speed, direction, maxcloseV, mincloseV, maxopenV,
                                minopenV)
+                moving_flag = True
                 pass
             elif cmd[0] == 'MotorCal':
                 # calibrate the voltages for starting motor and speeds
                 messages.append("Checking Motor Calibration. Please wait...")
                 DATAPipe.send(bundle_to_send(que_lst))
                 messages.clear()
                 maxcloseV, mincloseV, startcloseV, maxopenV, minopenV, startopenV = motorcal(
@@ -875,12 +909,14 @@
                 # Close connections
                 DATAPipe.close()
                 CTLPipe.close()
                 #   give up process id
                 return_barrier_monitoring_to_prev_process(ctlpid)
                 run = False
                 exit()
+        cycle_count += 1
         # Delay if have not used up all 200 ms
         used = time.time() - starttime
         if used < 0.495:
             time.sleep(0.495 - used)
+
         # shutdown automatically if no communication from controller?
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/Collect_data.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/Collect_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,41 +201,50 @@
                 direction = int(
                     sign(float(Barr_Target.value) - float(Bar_Sep.value)))
                 tempspeed = target_speed
                 temp_targ = float(Barr_Target.value)
             elif Barr_Units.value == "cm^2":
                 direction = int(
                     sign(float(Barr_Target.value) - float(Bar_Area.value)))
-                tempspeed = (target_speed - skimmer_correction) / width
+                tempspeed = target_speed/ width
                 temp_targ = \
                     sqcm_to_cm(float(Barr_Target.value), 0,
                                Trough_GUI.calibrations)[0]
             elif Barr_Units.value == "Angstrom^2/molec":
                 direction = int(sign(
                     float(Barr_Target.value) - float(Bar_Area_per_Molec.value)))
-                tempspeed = (target_speed - skimmer_correction) / width / 1e16 * float(
-                    moles_molec.value) * 6.02214076e23
+                tempspeed = angpermolec_to_sqcm(target_speed, 0, float(
+                    moles_molec.value))[0]
+                tempspeed = tempspeed/width
                 temp_targ = sqcm_to_cm(
                     *angpermolec_to_sqcm(float(Barr_Target.value), 0,
                                          float(moles_molec.value)),
                     Trough_GUI.calibrations)[0]
             if direction < 0:
                 target = \
                     Trough_GUI.calibrations.barriers_close.cal_inv(
                         float(temp_targ), 0)[
                         0]
-                speed = \
-                Trough_GUI.calibrations.speed_close.cal_inv(tempspeed, 0)[0]
+                if tempspeed <= 1.0:
+                    speed = \
+                        Trough_GUI.calibrations.speed_close.cal_inv(1.0, 0)[0]*tempspeed
+                else:
+                    speed = \
+                    Trough_GUI.calibrations.speed_close.cal_inv(tempspeed, 0)[0]
             else:
                 target = \
                     Trough_GUI.calibrations.barriers_open.cal_inv(
                         float(temp_targ), 0)[
                         0]
-                speed = \
-                Trough_GUI.calibrations.speed_open.cal_inv(tempspeed, 0)[0]
+                if tempspeed <= 1.0:
+                    speed = \
+                        Trough_GUI.calibrations.speed_open.cal_inv(1.0, 0)[0]*tempspeed
+                else:
+                    speed = \
+                    Trough_GUI.calibrations.speed_open.cal_inv(tempspeed, 0)[0]
             cmdsend.send(['Speed', speed])
             cmdsend.send(['Direction', direction])
             cmdsend.send(['MoveTo', target])
             trough_lock.release()
             # display data as collected and periodically update status widgets
             # spawn updater thread that updates both status widgets and the figure.
             updater = Thread(target=collect_data_updater,
@@ -584,15 +593,15 @@
     from pandas import DataFrame, concat
     import numpy as np
     from IPython import get_ipython
     Trough_GUI = get_ipython().user_ns["Trough_GUI"]
     plate_circumference = Trough_GUI.status_widgets.plate_circumference
     moles_molec = Trough_GUI.status_widgets.moles_molec
     # do all the calculations on the new data
-    time_stamp = np.array(datapkg[0])
+    time_stamp = np.array(datapkg[0])-run.timestamp
     pos_raw = np.array(datapkg[1])
     pos_raw_stdev = np.array(datapkg[2])
     bal_raw = np.array(datapkg[3])
     bal_raw_stdev = np.array(datapkg[4])
     temp_raw = np.array(datapkg[5])
     temp_raw_stdev = np.array(datapkg[6])
     sep_cm = None
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/Monitor_Calibrate.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/Monitor_Calibrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             # fit and save the data
             from pathlib import Path
             import time
             cal_path = Path('~/.Trough/calibrations').expanduser()
             params, stdev = calibrations.poly_fit(cal_bal_x, cal_bal_y, 1, 0.5)
             inv_params, inv_stdev = calibrations.poly_fit(cal_bal_y,
                                                           cal_bal_x, 1, 0.001)
-            calibrations.balance = Trough.Trough_GUI.calibration_utils. \
+            calibrations.balance = Trough_GUI.calibration_utils. \
                 Calibration(
                 'balance', 'mg', time.time(), params, stdev, inv_params,
                 inv_stdev, cal_bal_x, cal_bal_y)
             calibrations.write_cal(cal_path, calibrations.balance)
 
             # Calibrations have been updated so restart the status watcher
             Trough_GUI.run_updater.value = False
@@ -157,15 +157,15 @@
             # fit and save the data
             from pathlib import Path
             import time
             cal_path = Path('~/.Trough/calibrations').expanduser()
             params, stdev = calibrations.poly_fit(cal_temp_x, cal_temp_y, 3, 0.1)
             inv_params, inv_stdev = calibrations.poly_fit(cal_temp_y,
                                                           cal_temp_x, 3, 0.001)
-            calibrations.temperature = Trough.Trough_GUI.calibration_utils. \
+            calibrations.temperature = Trough_GUI.calibration_utils. \
                 Calibration(
                 'temperature', 'C', time.time(), params, stdev, inv_params,
                 inv_stdev, cal_temp_x, cal_temp_y)
             calibrations.write_cal(cal_path, calibrations.temperature)
 
             # Calibrations have been updated so restart the status watcher
             Trough_GUI.run_updater.value = False
@@ -298,17 +298,14 @@
                                        'temp_dev': datapkg[6][-1],
                                        'messages': datapkg[7]}
 
                         if calibrating_barr_direction == "open":
                             Trough_GUI.lastdirection.value = 1
                         else:
                             Trough_GUI.lastdirection.value = -1
-                        Trough.Trough_GUI.status_widgets.update_status(status_dict,
-                                                                       calibrations,
-                                                                       Trough_GUI.lastdirection)
                         if abs(target - position[-1]) < 0.01:
                             moving = False
                         waiting = False
             if time.time() < min_next_time:
                 time.sleep(min_next_time - time.time())
         trough_lock.release()
         tempindex_start = 0
@@ -326,15 +323,15 @@
             if abs(position[tempindex_end] - position[tempindex_end - 1]) > \
                     (positiondev[tempindex_end] ** 2 + \
                      positiondev[tempindex_end - 1] ** 2) ** 0.5:
                 if n_moving_end < 3:
                     n_moving_end += 1
             if n_moving_end < 3:
                 tempindex_end -= 1
-            if abs(position[tempindex_start] - position[tempindex_end + 1]) \
+            if abs(position[tempindex_start] - position[tempindex_start + 1]) \
                     > (positiondev[tempindex_start] ** 2 + \
                      positiondev[tempindex_start - 1] ** 2) ** 0.5:
                 if n_moving_start < 3:
                     n_moving_start += 1
             if n_moving_start < 3:
                 tempindex_start += 1
         if calibrating_barr_direction == 'open':
@@ -368,14 +365,20 @@
         trough_lock.release()
         return
 
     def on_calib_barr(change):
         import time
         nonlocal calibrating_barr_direction
         nonlocal calibrating_barr_step
+        nonlocal close_pos_x
+        nonlocal open_pos_y
+        nonlocal close_speed_x
+        nonlocal open_speed_x
+        nonlocal close_speed_y
+        nonlocal open_speed_y
         steps = None
         direction = 0
         just_finished_keep = False
         if Barr_Cal_Butt.description == 'Start Calibration':
             # begin the calibration by opening the trough
             Barr_Cal_Butt.description = 'Moving...'
             Barr_Cal_Butt.disabled = True
@@ -422,15 +425,15 @@
                 # position only
                 Barr_Cal_Butt.description = "Moving..."
                 Barr_Cal_Butt.disabled = True
                 trough_lock.acquire()
                 cmdsend.send(['Speed', steps[calibrating_barr_step]["speed"]])
                 cmdsend.send(['MoveTo', steps[calibrating_barr_step]["target"]])
                 trough_lock.release()
-                while abs(float(Barr_Raw.value) - steps[calibrating_barr_step]["target"]) < 0.01:
+                while abs(float(Barr_Raw.value) - steps[calibrating_barr_step]["target"]) > 0.01:
                     # We wait
                     pass
                 Barr_Cal_Butt.description = 'Keep'
                 Barr_Cal_Butt.disabled = False
                 return
             elif steps[calibrating_barr_step]["speed"]:
                 # speed only
@@ -458,27 +461,27 @@
             # fitting and save the data
             from pathlib import Path
             cal_path = Path('~/.Trough/calibrations').expanduser()
             # Opening Positions
             params, stdev = calibrations.poly_fit(open_pos_x, open_pos_y, 3, 0.1)
             inv_params, inv_stdev = calibrations.poly_fit(open_pos_y,
                                                           open_pos_x, 3, 0.001)
-            calibrations.barriers_open = Trough.Trough_GUI.calibration_utils.\
+            calibrations.barriers_open = Trough_GUI.calibration_utils.\
                 Calibration(
                 'barriers_open', 'cm', time.time(), params, stdev, inv_params,
                 inv_stdev, open_pos_x, open_pos_y, additional_data={
                     "trough width (cm)": float(Trough_Width.value),
                     "skimmer correction (cm^2)": float(Skimer_Correction.value)}
             )
             calibrations.write_cal(cal_path, calibrations.barriers_open)
             # Closing Positions
             params, stdev = calibrations.poly_fit(close_pos_x, close_pos_y, 3, 0.1)
             inv_params, inv_stdev = calibrations.poly_fit(close_pos_y,
                                                           close_pos_x, 3, 0.001)
-            calibrations.barriers_close = Trough.Trough_GUI.calibration_utils.\
+            calibrations.barriers_close = Trough_GUI.calibration_utils.\
                 Calibration(
                 'barriers_close', 'cm', time.time(), params, stdev, inv_params,
                 inv_stdev, close_pos_x, close_pos_y, additional_data={
                     "trough width (cm)": float(Trough_Width.value),
                     "skimmer correction (cm^2)": float(Skimer_Correction.value)}
             )
             calibrations.write_cal(cal_path, calibrations.barriers_close)
@@ -487,29 +490,29 @@
             for k in open_speed_y:
                 start = calibrations.barriers_open.cal_apply(k[0],0)[0]
                 end = calibrations.barriers_open.cal_apply(k[1],0)[0]
                 speed_cm_per_min.append(abs(start - end)*60/k[2])
             params, stdev = calibrations.poly_fit(open_speed_x, speed_cm_per_min, 3, 0.01)
             inv_params, inv_stdev = calibrations.poly_fit(speed_cm_per_min,
                                                           open_speed_x, 3, 0.001)
-            calibrations.speed_open = Trough.Trough_GUI.calibration_utils.Calibration(
+            calibrations.speed_open = Trough_GUI.calibration_utils.Calibration(
                 'speed_open', 'cm/min', time.time(), params, stdev, inv_params,
                 inv_stdev, open_speed_x, speed_cm_per_min)
             calibrations.write_cal(cal_path, calibrations.speed_open)
             # Closing Speeds
             speed_cm_per_min = []
             for k in close_speed_y:
                 start = calibrations.barriers_close.cal_apply(k[0],0)[0]
                 end = calibrations.barriers_close.cal_apply(k[1],0)[0]
                 speed_cm_per_min.append(abs(start - end)*60/k[2])
             params, stdev = calibrations.poly_fit(close_speed_x, speed_cm_per_min,
                                                   3, 0.01)
             inv_params, inv_stdev = calibrations.poly_fit(speed_cm_per_min,
                                                           close_speed_x, 3, 0.001)
-            calibrations.speed_close = Trough.Trough_GUI.calibration_utils.Calibration(
+            calibrations.speed_close = Trough_GUI.calibration_utils.Calibration(
                 'speed_close', 'cm/min', time.time(), params, stdev, inv_params,
                 inv_stdev, close_speed_x, speed_cm_per_min)
             calibrations.write_cal(cal_path, calibrations.speed_close)
 
             # Calibrations have been updated so restart the status watcher
             Trough_GUI.run_updater.value = False
             while Trough_GUI.updater_running.value:
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/__init__.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/calibration_utils.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/calibration_utils.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/command_widgets.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/command_widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,101 +47,92 @@
     if change['new'] == 'cm':
         _set_min_max(Barr_Target, round(calibrations.barriers_close.cal_apply(0.0,0.0)[0], 2),
                      round(calibrations.barriers_open.cal_apply(1.0, 0.0)[0],2))
         if Barr_Direction.value == "Open":
             Barr_Target.value = calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0]
             tempspeed = calibrations.speed_open.cal_apply(speed,0.0)[0]
             max = calibrations.speed_open.cal_apply(1.0, 0.0)[0]
-            min = calibrations.speed_open.cal_apply(0.0, 0.0)[0]
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         elif Barr_Direction.value == "Close":
             Barr_Target.value = calibrations.barriers_close.cal_apply(Barr_Target_Frac, 0.0)[0]
             tempspeed = calibrations.speed_close.cal_apply(speed,0.0)[0]
             max = calibrations.speed_close.cal_apply(1.0, 0.0)[0]
-            min = calibrations.speed_close.cal_apply(0.0, 0.0)[0]
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         else: # MoveTo case
             if _moveto_direction() == -1:
                 Barr_Target.value = calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0]
                 tempspeed = calibrations.speed_close.cal_apply(speed, 0.0)[0]
                 max = calibrations.speed_close.cal_apply(1.0, 0.0)[0]
-                min = calibrations.speed_close.cal_apply(0.0, 0.0)[0]
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             elif _moveto_direction() == 1:
                 Barr_Target.value = calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0]
                 tempspeed = calibrations.speed_open.cal_apply(speed, 0.0)[0]
                 max = calibrations.speed_open.cal_apply(1.0, 0.0)[0]
-                min = calibrations.speed_open.cal_apply(0.0, 0.0)[0]
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             pass
     if change['new'] == 'cm^2':
         max = calibrations.barriers_open.cal_apply(1.0, 0.0)[0]*float(width) +\
                           float(skimmer_correction)
-        min = calibrations.barriers_close.cal_apply(0.0,0.0)[0]*float(width) +\
-                          float(skimmer_correction)
+        min = 0
         _set_min_max(Barr_Target, round(min, 2), round(max, 2))
         if Barr_Direction.value == "Open":
             temptarg = calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                        float(width) + float(skimmer_correction)
             Barr_Target.value = temptarg
             tempspeed = calibrations.speed_open.cal_apply(speed,0.0)[0]*float(width) + \
                             float(skimmer_correction)
             max = calibrations.speed_open.cal_apply(1.0, 0.0)[0] * \
                   float(width) + \
                   float(skimmer_correction)
-            min = calibrations.speed_open.cal_apply(0.0, 0.0)[0] * \
-                  float(width) + \
-                  float(skimmer_correction)
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         elif Barr_Direction.value == "Close":
             temptarg = calibrations.barriers_close.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                        float(width) + float(skimmer_correction)
             Barr_Target.value = temptarg
             tempspeed = calibrations.speed_close.cal_apply(speed,0.0)[0]*float(width) + \
                             float(skimmer_correction)
             max = calibrations.speed_close.cal_apply(1.0, 0.0)[0] * \
                   float(width) + \
                   float(skimmer_correction)
-            min = calibrations.speed_close.cal_apply(0.0, 0.0)[0] * \
-                  float(width) + \
-                  float(skimmer_correction)
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         else: # MoveTo case
             if _moveto_direction() == -1:
                 temptarg = calibrations.barriers_close.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                            float(width) + float(skimmer_correction)
                 Barr_Target.value = temptarg
                 tempspeed = calibrations.speed_close.cal_apply(speed, 0.0)[0] * float(width) + \
                             float(skimmer_correction)
                 max = calibrations.speed_close.cal_apply(1.0, 0.0)[0] * \
                       float(width) + \
                       float(skimmer_correction)
-                min = calibrations.speed_close.cal_apply(0.0, 0.0)[0] * \
-                      float(width) + \
-                      float(skimmer_correction)
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             elif _moveto_direction() == 1:
                 temptarg = calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                            float(width) + float(skimmer_correction)
                 Barr_Target.value = temptarg
                 tempspeed = calibrations.speed_open.cal_apply(speed, 0.0)[0] * float(width) + \
                             float(skimmer_correction)
                 max = calibrations.speed_open.cal_apply(1.0, 0.0)[0] * \
                       float(width) + \
                       float(skimmer_correction)
-                min = calibrations.speed_open.cal_apply(0.0, 0.0)[0] * \
-                      float(width) + \
-                      float(skimmer_correction)
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             pass
     if change['new'] == 'Angstrom^2/molec':
         max = (calibrations.barriers_open.cal_apply(1.0,0.0)[0]*\
                             width + skimmer_correction)*\
                             1e16/moles_molec/6.02214076e23
@@ -156,33 +147,29 @@
             Barr_Target.value = temptarg
             tempspeed = (calibrations.speed_open.cal_apply(speed,0.0)[0]*width + \
                             skimmer_correction)*\
                             1e16/moles_molec/6.02214076e23
             max = (calibrations.speed_open.cal_apply(1.0, 0.0)[0] * \
                   width + skimmer_correction) * \
                   1e16 / moles_molec / 6.02214076e23
-            min = (calibrations.speed_open.cal_apply(0.0, 0.0)[0] * \
-                  width + skimmer_correction) * \
-                  1e16 / moles_molec / 6.02214076e23
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         elif Barr_Direction.value == "Close":
             temptarg = (calibrations.barriers_close.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                         width + skimmer_correction) * \
                        1e16 / moles_molec / 6.02214076e23
             Barr_Target.value = temptarg
             tempspeed = (calibrations.speed_close.cal_apply(speed,0.0)[0]*width + \
                             skimmer_correction)*\
                             1e16/moles_molec/6.02214076e23
             max = (calibrations.speed_close.cal_apply(1.0, 0.0)[0] * \
                   width + skimmer_correction) * \
                   1e16 / moles_molec / 6.02214076e23
-            min = (calibrations.speed_close.cal_apply(0.0, 0.0)[0] * \
-                  width + skimmer_correction) * \
-                  1e16 / moles_molec / 6.02214076e23
+            min = 0
             _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
             Barr_Speed.value = tempspeed
         else: # MoveTo case
             if _moveto_direction() == -1:
                 temptarg = (calibrations.barriers_close.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                             width + skimmer_correction) * \
                            1e16 / moles_molec / 6.02214076e23
@@ -190,34 +177,29 @@
                 tempspeed = calibrations.speed_close.cal_apply(speed, 0.0)[0] * float(width) + \
                             float(skimmer_correction) * \
                             1e16 / moles_molec / 6.02214076e23
                 max = calibrations.speed_close.cal_apply(1.0, 0.0)[0] * \
                       float(width) + \
                       float(skimmer_correction) * \
                       1e16 / moles_molec / 6.02214076e23
-                min = calibrations.speed_close.cal_apply(0.0, 0.0)[0] * \
-                      float(width) + \
-                      float(skimmer_correction) * \
-                      1e16 / moles_molec / 6.02214076e23
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             elif _moveto_direction() == 1:
                 temptarg = (calibrations.barriers_open.cal_apply(Barr_Target_Frac, 0.0)[0] * \
                             width + skimmer_correction) * \
                            1e16 / moles_molec / 6.02214076e23
                 Barr_Target.value = temptarg
                 tempspeed = (calibrations.speed_open.cal_apply(speed, 0.0)[0] * width + \
                             skimmer_correction) * \
                             1e16 / moles_molec / 6.02214076e23
                 max = (calibrations.speed_open.cal_apply(1.0, 0.0)[0] * \
                       width + skimmer_correction) * \
                       1e16 / moles_molec / 6.02214076e23
-                min = (calibrations.speed_open.cal_apply(0.0, 0.0)[0] * \
-                      width + skimmer_correction) * \
-                      1e16 / moles_molec / 6.02214076e23
+                min = 0
                 _set_min_max(Barr_Speed, round(min, 2), round(max, 2))
                 Barr_Speed.value = tempspeed
             pass
     pass
 
 Barr_Units = Dropdown(description="Units",
                       options=["cm", "cm^2", "Angstrom^2/molec"])
@@ -242,55 +224,69 @@
     pass
 
 Barr_Target = BoundedFloatText(value=10.0, min=0.0, max=12.6,
                                step=0.01, disabled=True)
 Barr_Speed = BoundedFloatText(description="Speed (/min)", value=5.0, min = 0.0,
                        max = 10.0, step = 0.01, disabled=False)
 def on_click_Start(change):
+    from Trough.Trough_GUI.conversions import sqcm_to_cm, angpermolec_to_sqcm
     from IPython import get_ipython
     cmdsend = get_ipython().user_ns["Trough_Control"].cmdsend
     calibrations = get_ipython().user_ns["Trough_GUI"].calibrations
     width = float(calibrations.barriers_open.additional_data["trough width (cm)"])
     skimmer_correction = float(calibrations.barriers_open.additional_data["skimmer correction (cm^2)"])
     moles_molec = float(get_ipython().user_ns["Trough_GUI"].status_widgets.moles_molec.value)
     trough_lock = get_ipython().user_ns["Trough_Control"].trough_lock
     lastdirection = get_ipython().user_ns["Trough_GUI"].lastdirection
     global speed
     if Barr_Units.value == 'cm':
         tempspeed = float(Barr_Speed.value)
         Barr_Target_Frac = calibrations.barriers_open.cal_inv(Barr_Target.value, 0)[0]
     elif Barr_Units.value == 'cm^2':
-        tempspeed = (Barr_Speed.value - skimmer_correction)/width
-        temptarg = (Barr_Target.value - skimmer_correction)/width
+        tempspeed = sqcm_to_cm(Barr_Speed.value,0,calibrations)[0]
+        temptarg = sqcm_to_cm(Barr_Target.value,0,calibrations)[0]
         Barr_Target_Frac = calibrations.barriers_open.cal_inv(temptarg, 0)[0]
     elif Barr_Units.value == 'Angstrom^2/molec':
-        tempspeed = (Barr_Speed.value - skimmer_correction)/width/1e16*moles_molec*6.02214076e23
-        temptarg = Barr_Target.value/1e16*moles_molec*6.02214076e23
-        temptarg = (temptarg - skimmer_correction)/width
+        tempspeed = angpermolec_to_sqcm(Barr_Speed.value, 0, moles_molec)[0]
+        tempspeed = tempspeed/width
+        temptarg = angpermolec_to_sqcm(Barr_Target.value, 0,moles_molec)[0]
+        temptarg = sqcm_to_cm(temptarg,0,calibrations)[0]
         Barr_Target_Frac = calibrations.barriers_open.cal_inv(temptarg, 0)[0]
     if Barr_Direction.value != 'Move To':
         direction = 0
         if Barr_Direction.value == 'Close':
             direction = -1
-            speed = calibrations.speed_close.cal_inv(tempspeed, 0)[0]
+            if tempspeed <= 1.0: # calibrations not good below this.
+                speed = calibrations.speed_close.cal_inv(1.0, 0)[0]*tempspeed
+            else:
+                speed = calibrations.speed_close.cal_inv(tempspeed, 0)[0]
         elif Barr_Direction.value == 'Open':
             direction = 1
-            speed = calibrations.speed_open.cal_inv(tempspeed, 0)[0]
+            if tempspeed <= 1.0: # calibrations not good below this.
+                speed = calibrations.speed_open.cal_inv(1.0, 0)[0]* tempspeed
+            else:
+                speed = calibrations.speed_open.cal_inv(tempspeed, 0)[0]
         trough_lock.acquire()
         cmdsend.send(['Speed', speed])
         cmdsend.send(['Direction', direction])
         cmdsend.send(['Start', ''])
         lastdirection.value = direction
         trough_lock.release()
     else:
         direction = _moveto_direction()
         if direction == -1:
-            speed = calibrations.speed_close.cal_inv(tempspeed, 0)[0]
+            if tempspeed <= 1.0: # calibrations not good below this.
+                speed = calibrations.speed_close.cal_inv(1.0, 0)[0]*tempspeed
+            else:
+                speed = calibrations.speed_close.cal_inv(tempspeed, 0)[0]
         else:
-            speed = calibrations.speed_open.cal_inv(tempspeed, 0)[0]
+            if tempspeed <= 1.0: # calibrations not good below this.
+                speed = calibrations.speed_open.cal_inv(1.0, 0)[0]*tempspeed
+            else:
+                speed = calibrations.speed_open.cal_inv(tempspeed, 0)[0]
         trough_lock.acquire()
         cmdsend.send(['Speed', speed])
         cmdsend.send(['Direction', direction])
         cmdsend.send(['MoveTo', Barr_Target_Frac])
         lastdirection.value = direction
         trough_lock.release()
     pass
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/conversions.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # TODO use conversion utilities more places
 def cm_to_sqcm(value, err, cals):
     """convert barrier separation in cm to trough area in sqcm"""
     from round_using_error import numbers_rndwitherr
     sqcm_err = err * float(cals.barriers_open.additional_data[ \
                      "trough width (cm)"])
     sqcm = value * float(cals.barriers_open.additional_data[ \
-                     "trough width (cm)"]) - float(cals.barriers_open. \
+                     "trough width (cm)"]) + float(cals.barriers_open. \
                      additional_data["skimmer correction (cm^2)"])
     return numbers_rndwitherr(sqcm, sqcm_err)
 
 def sqcm_to_cm(value, err, cals):
     """convert trough area in sqcm to barrier separation in cm"""
     from round_using_error import numbers_rndwitherr
     cm_err = err / float(cals.barriers_open.additional_data[ \
                      "trough width (cm)"])
-    cm = (value + float(cals.barriers_open. \
+    cm = (value - float(cals.barriers_open. \
                         additional_data["skimmer correction (cm^2)"])) \
                         / float(cals.barriers_open.additional_data[ \
                         "trough width (cm)"])
     return numbers_rndwitherr(cm, cm_err)
 
 def sqcm_to_angpermolec(value, err, moles):
     """convert trough area in sqcm to square angstroms per molecules"""
```

### Comparing `langmuir_trough-0.7.0/Trough/Trough_GUI/status_widgets.py` & `langmuir_trough-0.8.0/Trough/Trough_GUI/status_widgets.py`

 * *Files identical despite different names*

### Comparing `langmuir_trough-0.7.0/setup.py` & `langmuir_trough-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="langmuir_trough",
-    version="0.7.0",
+    version="0.8.0",
     description="Controls and collects data from Gutow Lab Langmuir Trough.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gutow/Langmuir_Trough.git",
     author="Jonathan Gutow",
     author_email="gutow@uwosh.edu",
     keywords="",
```

