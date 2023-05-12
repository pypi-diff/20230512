# Comparing `tmp/picodaqa-1.1.0.tar.gz` & `tmp/picodaqa-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picodaqa-1.1.0.tar", last modified: Sat May  6 15:28:21 2023, max compression
+gzip compressed data, was "picodaqa-1.1.1.tar", last modified: Fri May 12 18:13:25 2023, max compression
```

## Comparing `picodaqa-1.1.0.tar` & `picodaqa-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/
--rw-r--r--   0 quast     (1000) users      (100)    10116 2023-05-06 15:28:21.000000 picodaqa-1.1.0/PKG-INFO
--rw-r--r--   0 quast     (1000) users      (100)     8349 2022-10-10 18:35:00.000000 picodaqa-1.1.0/README.md
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa/
--rw-r--r--   0 quast     (1000) users      (100)     2990 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/BarDisplay.py
--rw-r--r--   0 quast     (1000) users      (100)    21247 2021-12-04 17:30:18.000000 picodaqa-1.1.0/picodaqa/BufferMan.py
--rw-r--r--   0 quast     (1000) users      (100)     7301 2018-07-08 15:33:17.000000 picodaqa-1.1.0/picodaqa/DataGraphs.py
--rw-r--r--   0 quast     (1000) users      (100)     2912 2018-07-08 12:48:15.000000 picodaqa-1.1.0/picodaqa/DataLogger.py
--rw-r--r--   0 quast     (1000) users      (100)     5791 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/Oscilloscope.py
--rw-r--r--   0 quast     (1000) users      (100)     2531 2019-10-02 16:56:42.000000 picodaqa-1.1.0/picodaqa/RMeter.py
--rw-r--r--   0 quast     (1000) users      (100)     6287 2018-07-08 12:55:27.000000 picodaqa-1.1.0/picodaqa/VoltMeter.py
--rw-r--r--   0 quast     (1000) users      (100)      882 2019-10-02 16:56:42.000000 picodaqa-1.1.0/picodaqa/__init__.py
--rw-r--r--   0 quast     (1000) users      (100)      412 2023-05-06 15:28:17.000000 picodaqa-1.1.0/picodaqa/_version_info.py
--rw-r--r--   0 quast     (1000) users      (100)     4689 2023-05-06 15:23:04.000000 picodaqa-1.1.0/picodaqa/animHists.py
--rw-r--r--   0 quast     (1000) users      (100)     2502 2019-09-08 19:19:42.000000 picodaqa-1.1.0/picodaqa/mpBDisplay.py
--rw-r--r--   0 quast     (1000) users      (100)     4294 2018-04-10 16:28:40.000000 picodaqa-1.1.0/picodaqa/mpBufManCntrl.py
--rw-r--r--   0 quast     (1000) users      (100)     4379 2018-07-08 13:07:03.000000 picodaqa-1.1.0/picodaqa/mpDataGraphs.py
--rw-r--r--   0 quast     (1000) users      (100)     4561 2018-07-07 06:17:08.000000 picodaqa-1.1.0/picodaqa/mpDataLogger.py
--rw-r--r--   0 quast     (1000) users      (100)     1914 2018-03-10 19:32:27.000000 picodaqa-1.1.0/picodaqa/mpHists.py
--rw-r--r--   0 quast     (1000) users      (100)     2250 2018-04-10 16:29:11.000000 picodaqa-1.1.0/picodaqa/mpOsci.py
--rw-r--r--   0 quast     (1000) users      (100)     3048 2019-05-01 07:50:58.000000 picodaqa-1.1.0/picodaqa/mpRMeter.py
--rw-r--r--   0 quast     (1000) users      (100)     2219 2018-05-15 16:03:19.000000 picodaqa-1.1.0/picodaqa/mpVMeter.py
--rw-r--r--   0 quast     (1000) users      (100)    11336 2023-05-05 17:43:58.000000 picodaqa-1.1.0/picodaqa/picoConfig.py
--rw-r--r--   0 quast     (1000) users      (100)     2820 2018-03-11 09:01:11.000000 picodaqa-1.1.0/picodaqa/plotBufManInfo.py
--rw-r--r--   0 quast     (1000) users      (100)      917 2018-02-04 12:05:17.000000 picodaqa-1.1.0/picodaqa/read_config.py
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/
--rw-r--r--   0 quast     (1000) users      (100)    10116 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/PKG-INFO
--rw-r--r--   0 quast     (1000) users      (100)      626 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/SOURCES.txt
--rw-r--r--   0 quast     (1000) users      (100)        1 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/dependency_links.txt
--rw-r--r--   0 quast     (1000) users      (100)        9 2023-05-06 15:28:21.000000 picodaqa-1.1.0/picodaqa.egg-info/top_level.txt
--rw-r--r--   0 quast     (1000) users      (100)       38 2023-05-06 15:28:21.000000 picodaqa-1.1.0/setup.cfg
--rw-r--r--   0 quast     (1000) users      (100)     1508 2022-10-09 13:31:42.000000 picodaqa-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:13:25.989543 picodaqa-1.1.1/
+-rw-rw-r--   0 root         (0) root         (0)      288 2023-02-16 21:57:32.000000 picodaqa-1.1.1/AUTHORS
+-rw-rw-r--   0 root         (0) root         (0)     1348 2023-02-16 21:57:32.000000 picodaqa-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8925 2023-05-12 18:13:25.989543 picodaqa-1.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8349 2023-02-16 21:57:32.000000 picodaqa-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:13:25.989543 picodaqa-1.1.1/picodaqa/
+-rw-rw-r--   0 root         (0) root         (0)     2990 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/BarDisplay.py
+-rw-rw-r--   0 root         (0) root         (0)    21247 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/BufferMan.py
+-rw-rw-r--   0 root         (0) root         (0)     7301 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/DataGraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     2912 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/DataLogger.py
+-rw-rw-r--   0 root         (0) root         (0)     5791 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/Oscilloscope.py
+-rw-rw-r--   0 root         (0) root         (0)     2531 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/RMeter.py
+-rw-rw-r--   0 root         (0) root         (0)     6287 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/VoltMeter.py
+-rw-rw-r--   0 root         (0) root         (0)      882 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      412 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/_version_info.py
+-rw-rw-r--   0 root         (0) root         (0)     4569 2023-05-07 22:04:58.000000 picodaqa-1.1.1/picodaqa/animHists.py
+-rw-rw-r--   0 root         (0) root         (0)     2379 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpBDisplay.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpBufManCntrl.py
+-rw-rw-r--   0 root         (0) root         (0)     4256 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpDataGraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpDataLogger.py
+-rw-rw-r--   0 root         (0) root         (0)     1825 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpHists.py
+-rw-rw-r--   0 root         (0) root         (0)     2127 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpOsci.py
+-rw-rw-r--   0 root         (0) root         (0)     2913 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpRMeter.py
+-rw-rw-r--   0 root         (0) root         (0)     2096 2023-05-12 18:07:04.000000 picodaqa-1.1.1/picodaqa/mpVMeter.py
+-rw-rw-r--   0 root         (0) root         (0)    11336 2023-05-05 19:27:04.000000 picodaqa-1.1.1/picodaqa/picoConfig.py
+-rw-rw-r--   0 root         (0) root         (0)     2820 2023-05-05 19:32:19.000000 picodaqa-1.1.1/picodaqa/plotBufManInfo.py
+-rw-rw-r--   0 root         (0) root         (0)      917 2023-02-16 21:57:32.000000 picodaqa-1.1.1/picodaqa/read_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 18:13:25.989543 picodaqa-1.1.1/picodaqa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8925 2023-05-12 18:13:25.000000 picodaqa-1.1.1/picodaqa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-12 18:13:25.000000 picodaqa-1.1.1/picodaqa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 18:13:25.000000 picodaqa-1.1.1/picodaqa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-12 18:13:25.000000 picodaqa-1.1.1/picodaqa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 18:13:25.989543 picodaqa-1.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1508 2023-02-16 21:57:32.000000 picodaqa-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `picodaqa-1.1.0/PKG-INFO` & `picodaqa-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,172 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: picodaqa
-Version: 1.1.0
+Version: 1.1.1
 Summary: Data AcQuisition and analysis with PicoScope usb-oscilloscopes
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
-Description: # picoDAQ
-        
-        *python* Data AcQuisition and analysis with PicoScope usb-oscilloscopes
-        
-        The *usb*-oscilloscope series PicoSpope by Pico Technology (see <https://www.picotech.com>)
-        offers universal instruments that come with great software support, not only a graphical
-        interface offering the functionality known from oscilloscopes, but - most importantly for
-        this project - also with a software development kit (*SDK*) which makes it possible to use
-        the devices with a wide range of high-level languages.
-        
-        Provided here is a data acquisition system as is needed to record,  analyze, classify and
-        count the occurrence of wave forms such as provided for example by single-photon counters
-        or typical detectors common in quantum mechanical measurements or in nuclear, particle
-        physics and astro particle physics, e.g. photo tubes, Geiger counters, avalanche
-        photo-diodes or modern SiPMs.
-        
-        The random nature of such processes and the need to keep read-out dead times low requires
-        an input buffer and a buffer manager running as a background process. Data are provided
-        via the buffer manager interface to several consumer processes to analyze, check or
-        visualize data and analysis results. Such consumers may be obligatory ones, i.e. data
-        acquisition pauses if all input buffers are full and an obligatory consumer is still busy
-        processing. A second type of random consumers receives an event copy from the buffer manager
-        upon request, without pausing the data acquisition process. Typical examples of 
-        random consumers are displays of a subset of the wave forms or of intermediate
-        analysis results. Examples for such consumers are provided as part of this package,
-        running either as a 'thread' within the python interpreter or as sub-processes using
-        the 'multiprocessing' package.
-        
-        This project originated as a demonstration to analyze pulses from a photomultiplier (PM)
-        or a Silicon Photo Multiplier (SiPM) registering optical signals from  a detector, in the
-        simplest case a coffeepot filled with water and equipped with a PM to count muons from
-        cosmic rays. 
-        
-        ## List of implemented **Functions**:
-        
-        - class *picoConfig*:
-          - set up PicoScope time base, channel ranges and trigger
-          - set up the internal signal generator
-          - PicoScope configuration read from *json* or *yaml* file
-          - data acquisition of raw data from device
-        
-        - class *BufferMan*:
-          - acquire data (implemented as background thread)
-          - manage event data buffer and distribute to consumers
-          - configuration read from *json* or *yaml* file
-          - supports
-          
-            - *obligatory* consumers: data acquisition pauses until consumer done
-            - and *random* consumers: receive a copy of one event, data acquisition continues
-          
-        - module *AnimatedInstruments* (deprecated, to be removed soon)
-          - examples of animated graphical devices: a Buffer Manager display (using
-          class *plotBufManInfo), a VoltMeter (class *VoltMeter*), an Oscilloscope
-          (class *Ocscilloscope* and a ratemeter (class *RMeter*). The module must run as
-          a *python* *thread* in the same *python* interpreter as *BufferMan*
-        
-        - module *mpBufManCntrl*
-          - this sub-process receives status and logging information from the Buffer Manager
-          via a multiprocessing Queue and displays input rate history, filling level of the
-          buffers and the data-acquisition lifetime. Buttons at the bottom of the window allow
-          status changes (from RUNNING to PAUSED or vice versa) or to exit. A log-file at the
-          end contains a summary and, optionally, logging information. 
-        
-        - module *mpOsci*  
-          runs an instance of *Oscilloscpe* as a sub-process, and receives data from *BufferMan*
-          via a multiprocessing Queue.
-        
-        -  module *mpRMeter*    
-           runs an instance of the *RMeter* class as a sub-process, receiving via a multiprocessing Queue.
-        
-        - module *mpVMeter*  
-          runs an instance of the *VoltMeter* class as a sub-process, receiving data via a multiprocessing Queue. 
-        
-        - module *mpHists* 
-          runs an instance of the *animHists* class as a sub-process; receives input data via a
-          multiprocessing Queue. Data are formatted as lists of values. A normalized frequency distribution is
-          then updated and displayed.
-        
-        - module *mpBDisplay* 
-          - runs an instance of class BarDisplay and shows one (signed or unsigned) value per Channel
-          (e.g. peak Voltage, effective Voltage etc.). Values are passed to the sub-process via a
-          multiprocessing Queue.
-        
-        - module *mpDataLogger* 
-          runs an instance of the *DataLogger* class as a sub-process, displaying  values passed via a
-          multiprocessing Queue as a history plot. This module   is not implemented as a *BufferMan**
-          client (see example `runDataLogger`).
-        
-        - module *mpDataGraphs*  
-          runs an instance of the *DataGraphs* class as a sub-process, displaying values passed via a
-          multiprocessing Queue as a bar graph, a history plot or optionally - if two channels are
-          enabled - as xy-display. This module ist not implemented as a *BufferMan* client (see example
-          `runDataGraphs`)
-        
-        The script `runDAQ.py` gives an example of how to use all of the above. For a full demo,
-        connect the output of a PicoScope's signal generator to channel *B*, and eventually an
-        open cable to Channel *A* to see random noise. Use the configuration file `DAQconfig.yaml`,
-        which specifies the configuration files`BMconfig.yaml` for the Buffer Manager and `PSConfig.yaml`
-        for the PicoScope. As a hook for own extensions, user code may be included. An example for this
-        is shown in the configuration file `DAQ_Cosmo.json`, which points to a code snippet *anaDAQ.py*
-        to start some example consumers (code in`exampleConsumers.py`).
-        
-        
-        ## Examples
-        
-        The directory `examples/` contains configuration files and some special applications. 
-        
-        The script `runDataLogger.py` implements a data logger for rates below 20 Hz. Signals are
-        sampled with a PicoSocpe at a rate of 10 kHz over 20 ms and then averaged. 50 Hz noise is
-        thus eliminated, and a clean voltage signal is obtained. The history of the recorded voltages
-        is displayed using the module `mpDataLogger`. 
-        Similarly, `runDataGraphs` uses the same sampling mechanism to display the effective voltage
-        as bar graph, a history plot, and, optionally,   channel B vs. Channel A as an xy-graph if two
-        channels are enabled.
-        These examples directly read from the hardware device and therefore do not rely on the `BufferMan` class.
-        As a third simple example the script `runOsci.py` provides a simple oscilloscpe independent of BufferMan. 
-        
-        The script `runCosmo.py` is a modified version of `runDAQ.py` and depends on the code in
-        `pulseFilter.py`, which implements a convolution filter to search for characteristic signal
-        shapes in an input waveform. The example is tailored to identify short pulses from muon
-        detectors (e. g. the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt",
-        <http://www.teilchenwelt.de>, 
-        or the Kamiokanne-Experiment with photomultiplier readout and pulses shaped to a length of
-        approx. 150ns). A more complete and updated version has been moved to the project `picoCosmo`,
-        see <https://github.com/GuenterQuast/picoCosmo>. 
-        
-        
-        ## Installation of the package
-        
-        This python code is compatible with *python* versions and >=3.5. It was tested with PicoScope
-        device classes PS2000, PS2000a, PS3000a and PS4000 under Ubuntu, openSUSE Leap and on RaspberryPi.
-        Graphical displays are implemented with `matplotlib`.
-        
-        **Requirements:**
-        
-          - The low-level drivers and C-libraries contained in the Pico Technology
-            Software Development Kit are required,  *SDK* by Pico Technology,
-            see  https://www.picotech.com/downloads
-          - *python* bindings of the *pico-python* project by Colin O'Flynn
-            and Mark Harfouche, https://github.com/colinoflynn/pico-python
-        
-        *picoDAQ* presently consists of the modules in the direcoctry *picodaqa*, mentioned above,
-        and an example *python* script (*runDAQ.py*) with configuration examples (*.yaml* files) for
-        the data acquisition (*DAQconfig.yaml*), for the PicoScope Device (*PSconfig.yaml*) and for
-        the Buffer Mananger (*BMconfig.yaml*).
-        
-        After downloading all files from the git repository, connect your PicoScope and start from
-        the command line, e. g. `python runDAQ.py`. 
-        
-        You may run the script *make_dist.sh* to generate a *.whl* file in the subdirectory
-        *dist*, which can be installed via `pip install picodaqa_<vers>_<type>.whl`. Once
-        this is done, the provided examples can be copied to any directory. 
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+License-File: AUTHORS
+
+# picoDAQ
+
+*python* Data AcQuisition and analysis with PicoScope usb-oscilloscopes
+
+The *usb*-oscilloscope series PicoSpope by Pico Technology (see <https://www.picotech.com>)
+offers universal instruments that come with great software support, not only a graphical
+interface offering the functionality known from oscilloscopes, but - most importantly for
+this project - also with a software development kit (*SDK*) which makes it possible to use
+the devices with a wide range of high-level languages.
+
+Provided here is a data acquisition system as is needed to record,  analyze, classify and
+count the occurrence of wave forms such as provided for example by single-photon counters
+or typical detectors common in quantum mechanical measurements or in nuclear, particle
+physics and astro particle physics, e.g. photo tubes, Geiger counters, avalanche
+photo-diodes or modern SiPMs.
+
+The random nature of such processes and the need to keep read-out dead times low requires
+an input buffer and a buffer manager running as a background process. Data are provided
+via the buffer manager interface to several consumer processes to analyze, check or
+visualize data and analysis results. Such consumers may be obligatory ones, i.e. data
+acquisition pauses if all input buffers are full and an obligatory consumer is still busy
+processing. A second type of random consumers receives an event copy from the buffer manager
+upon request, without pausing the data acquisition process. Typical examples of 
+random consumers are displays of a subset of the wave forms or of intermediate
+analysis results. Examples for such consumers are provided as part of this package,
+running either as a 'thread' within the python interpreter or as sub-processes using
+the 'multiprocessing' package.
+
+This project originated as a demonstration to analyze pulses from a photomultiplier (PM)
+or a Silicon Photo Multiplier (SiPM) registering optical signals from  a detector, in the
+simplest case a coffeepot filled with water and equipped with a PM to count muons from
+cosmic rays. 
+
+## List of implemented **Functions**:
+
+- class *picoConfig*:
+  - set up PicoScope time base, channel ranges and trigger
+  - set up the internal signal generator
+  - PicoScope configuration read from *json* or *yaml* file
+  - data acquisition of raw data from device
+
+- class *BufferMan*:
+  - acquire data (implemented as background thread)
+  - manage event data buffer and distribute to consumers
+  - configuration read from *json* or *yaml* file
+  - supports
+  
+    - *obligatory* consumers: data acquisition pauses until consumer done
+    - and *random* consumers: receive a copy of one event, data acquisition continues
+  
+- module *AnimatedInstruments* (deprecated, to be removed soon)
+  - examples of animated graphical devices: a Buffer Manager display (using
+  class *plotBufManInfo), a VoltMeter (class *VoltMeter*), an Oscilloscope
+  (class *Ocscilloscope* and a ratemeter (class *RMeter*). The module must run as
+  a *python* *thread* in the same *python* interpreter as *BufferMan*
+
+- module *mpBufManCntrl*
+  - this sub-process receives status and logging information from the Buffer Manager
+  via a multiprocessing Queue and displays input rate history, filling level of the
+  buffers and the data-acquisition lifetime. Buttons at the bottom of the window allow
+  status changes (from RUNNING to PAUSED or vice versa) or to exit. A log-file at the
+  end contains a summary and, optionally, logging information. 
+
+- module *mpOsci*  
+  runs an instance of *Oscilloscpe* as a sub-process, and receives data from *BufferMan*
+  via a multiprocessing Queue.
+
+-  module *mpRMeter*    
+   runs an instance of the *RMeter* class as a sub-process, receiving via a multiprocessing Queue.
+
+- module *mpVMeter*  
+  runs an instance of the *VoltMeter* class as a sub-process, receiving data via a multiprocessing Queue. 
+
+- module *mpHists* 
+  runs an instance of the *animHists* class as a sub-process; receives input data via a
+  multiprocessing Queue. Data are formatted as lists of values. A normalized frequency distribution is
+  then updated and displayed.
+
+- module *mpBDisplay* 
+  - runs an instance of class BarDisplay and shows one (signed or unsigned) value per Channel
+  (e.g. peak Voltage, effective Voltage etc.). Values are passed to the sub-process via a
+  multiprocessing Queue.
+
+- module *mpDataLogger* 
+  runs an instance of the *DataLogger* class as a sub-process, displaying  values passed via a
+  multiprocessing Queue as a history plot. This module   is not implemented as a *BufferMan**
+  client (see example `runDataLogger`).
+
+- module *mpDataGraphs*  
+  runs an instance of the *DataGraphs* class as a sub-process, displaying values passed via a
+  multiprocessing Queue as a bar graph, a history plot or optionally - if two channels are
+  enabled - as xy-display. This module ist not implemented as a *BufferMan* client (see example
+  `runDataGraphs`)
+
+The script `runDAQ.py` gives an example of how to use all of the above. For a full demo,
+connect the output of a PicoScope's signal generator to channel *B*, and eventually an
+open cable to Channel *A* to see random noise. Use the configuration file `DAQconfig.yaml`,
+which specifies the configuration files`BMconfig.yaml` for the Buffer Manager and `PSConfig.yaml`
+for the PicoScope. As a hook for own extensions, user code may be included. An example for this
+is shown in the configuration file `DAQ_Cosmo.json`, which points to a code snippet *anaDAQ.py*
+to start some example consumers (code in`exampleConsumers.py`).
+
+
+## Examples
+
+The directory `examples/` contains configuration files and some special applications. 
+
+The script `runDataLogger.py` implements a data logger for rates below 20 Hz. Signals are
+sampled with a PicoSocpe at a rate of 10 kHz over 20 ms and then averaged. 50 Hz noise is
+thus eliminated, and a clean voltage signal is obtained. The history of the recorded voltages
+is displayed using the module `mpDataLogger`. 
+Similarly, `runDataGraphs` uses the same sampling mechanism to display the effective voltage
+as bar graph, a history plot, and, optionally,   channel B vs. Channel A as an xy-graph if two
+channels are enabled.
+These examples directly read from the hardware device and therefore do not rely on the `BufferMan` class.
+As a third simple example the script `runOsci.py` provides a simple oscilloscpe independent of BufferMan. 
+
+The script `runCosmo.py` is a modified version of `runDAQ.py` and depends on the code in
+`pulseFilter.py`, which implements a convolution filter to search for characteristic signal
+shapes in an input waveform. The example is tailored to identify short pulses from muon
+detectors (e. g. the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt",
+<http://www.teilchenwelt.de>, 
+or the Kamiokanne-Experiment with photomultiplier readout and pulses shaped to a length of
+approx. 150ns). A more complete and updated version has been moved to the project `picoCosmo`,
+see <https://github.com/GuenterQuast/picoCosmo>. 
+
+
+## Installation of the package
+
+This python code is compatible with *python* versions and >=3.5. It was tested with PicoScope
+device classes PS2000, PS2000a, PS3000a and PS4000 under Ubuntu, openSUSE Leap and on RaspberryPi.
+Graphical displays are implemented with `matplotlib`.
+
+**Requirements:**
+
+  - The low-level drivers and C-libraries contained in the Pico Technology
+    Software Development Kit are required,  *SDK* by Pico Technology,
+    see  https://www.picotech.com/downloads
+  - *python* bindings of the *pico-python* project by Colin O'Flynn
+    and Mark Harfouche, https://github.com/colinoflynn/pico-python
+
+*picoDAQ* presently consists of the modules in the direcoctry *picodaqa*, mentioned above,
+and an example *python* script (*runDAQ.py*) with configuration examples (*.yaml* files) for
+the data acquisition (*DAQconfig.yaml*), for the PicoScope Device (*PSconfig.yaml*) and for
+the Buffer Mananger (*BMconfig.yaml*).
+
+After downloading all files from the git repository, connect your PicoScope and start from
+the command line, e. g. `python runDAQ.py`. 
+
+You may run the script *make_dist.sh* to generate a *.whl* file in the subdirectory
+*dist*, which can be installed via `pip install picodaqa_<vers>_<type>.whl`. Once
+this is done, the provided examples can be copied to any directory. 
+
+
+
```

### Comparing `picodaqa-1.1.0/README.md` & `picodaqa-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/BarDisplay.py` & `picodaqa-1.1.1/picodaqa/BarDisplay.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/BufferMan.py` & `picodaqa-1.1.1/picodaqa/BufferMan.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/DataGraphs.py` & `picodaqa-1.1.1/picodaqa/DataGraphs.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/DataLogger.py` & `picodaqa-1.1.1/picodaqa/DataLogger.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/Oscilloscope.py` & `picodaqa-1.1.1/picodaqa/Oscilloscope.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/RMeter.py` & `picodaqa-1.1.1/picodaqa/RMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/VoltMeter.py` & `picodaqa-1.1.1/picodaqa/VoltMeter.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/__init__.py` & `picodaqa-1.1.1/picodaqa/__init__.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/animHists.py` & `picodaqa-1.1.1/picodaqa/animHists.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
 
   # create figure
     ncols = int(np.sqrt(self.nHist))
     nrows = ncols
     if ncols * nrows < self.nHist: nrows +=1
     if ncols * nrows < self.nHist: ncols +=1
     self.fig, axarray = plt.subplots(nrows=nrows, ncols=ncols,
-                                          figsize=(3.*ncols, 2.*nrows) )
-    #!   deprecated sind vers. 3.4 self.fig.canvas.set_window_title(name)
-    self.fig.canvas.manager.set_window_title(name)
+                                     num=name, figsize=(3.*ncols, 2.*nrows) )
     self.fig.subplots_adjust(left=0.25/ncols, bottom=0.25/nrows, right=0.975, top=0.95,
                              wspace=0.35, hspace=0.35)
 # sort axes in linear array
     self.axes = []
     if self.nHist == 1:
       self.axes = [axarray]
     elif self.nHist == 2:
```

### Comparing `picodaqa-1.1.0/picodaqa/mpBDisplay.py` & `picodaqa-1.1.1/picodaqa/mpBDisplay.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,16 +73,14 @@
       button = Tk.Button(master=root, text='Quit', command=sys.exit)
       button.pack(side=Tk.BOTTOM)
 
 # set up matplotlib animation
       interval = 1
       BDAnim = anim.FuncAnimation(figBD, BD, yieldEvt_fromQ,
                          interval=interval, init_func=BD.init,
-                         blit=True, fargs=None, repeat=True, save_count=None)
-                       # save_count=None is a (temporary) work-around 
-                       #     to fix memory leak in animate
+                         blit=True, fargs=None, repeat=True, cache_frame_data=False)
       Tk.mainloop()
    
   except Exception as e:
     print('*==* mpBDisplay: terminating')
     print(e)
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpBufManCntrl.py` & `picodaqa-1.1.1/picodaqa/mpBufManCntrl.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,14 +140,12 @@
                               args=(T, ) ) 
     wrthread.daemon = True
     wrthread.start()
 
 # set up matplotlib animation for rate history
     BMiAnim = anim.FuncAnimation(figBMi, BMi, sequence_gen,
                      interval=interval, init_func=BMi.init,
-                     blit=True, fargs=None, repeat=True, save_count=None) 
-                         # save_count=None is a (temporary) work-around 
-                         #     to fix memory leak in animate
+                     blit=True, fargs=None, repeat=True, cache_frame_data=False)
     Tk.mainloop()
   except:
     print('*==* mpBufManInfo: termination signal received')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpDataGraphs.py` & `picodaqa-1.1.1/picodaqa/mpDataGraphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,13 +139,11 @@
   canvas.get_tk_widget().pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
   canvas._tkcanvas.pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
 
 # set up matplotlib animation
   tw = max(WaitTime-50., 0.5) # smaller than WaitTime to allow for processing
   DGAnim = anim.FuncAnimation(figDG, DG, yieldEvt_fromQ,
                          interval = tw, init_func = DG.init,
-                         blit=True, fargs=None, repeat=True, save_count=None)
-                       # save_count=None is a (temporary) work-around 
-                       #     to fix memory leak in animate
+                         blit=True, fargs=None, repeat=True, cache_frame_data=False)
   Tk.mainloop()
   print('*==* mpDataGraphs: terminating')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpDataLogger.py` & `picodaqa-1.1.1/picodaqa/mpDataLogger.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,17 +141,15 @@
   canvas._tkcanvas.pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
 
 
 # set up matplotlib animation
   tw = max(WaitTime - 20., 0.5) # smaller than WaitTime to allow for processing
   VMAnim = anim.FuncAnimation(figDL, DL, yieldEvt_fromQ,
                          interval = tw , init_func=DL.init,
-                         blit=True, fargs=None, repeat=True, save_count=None)
-                       # save_count=None is a (temporary) work-around 
-                       #     to fix memory leak in animate
+                         blit=True, fargs=None, repeat=True, cache_frame_data=False)
   try:
     Tk.mainloop()
    
   except:
     print('*==* mpDataLogger: termination signal recieved')
   sys.exit()
 # -- end def mpDataLogger()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpHists.py` & `picodaqa-1.1.1/picodaqa/mpHists.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
   try:
     H = animHists(Hdescripts, name)
     figH = H.fig
 # set up matplotlib animation
     HAnim = anim.FuncAnimation(figH, H, yieldData_fromQ, 
                         init_func=H.init, interval=interval, blit=True,
-                        fargs=None, repeat=True, save_count=None)
-                             # save_count=None is a (temporary) work-around 
-                             #     to fix memory leak in animate
+                        fargs=None, repeat=True, cache_frame_data=False)
+                        #    save_count=None)
     plt.show()
   
   except:
     print('*==* mpHist: termination signal recieved')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpOsci.py` & `picodaqa-1.1.1/picodaqa/mpOsci.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,13 @@
     canvas._tkcanvas.pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
     button = Tk.Button(master=root, text='Quit', command=sys.exit)
     button.pack(side=Tk.BOTTOM)
 
 # set up matplotlib animation
     osciAnim = anim.FuncAnimation(figOs, Osci, yieldEvt_fromQ, 
                   init_func=Osci.init, interval=interval, blit=True,
-                  fargs=None, repeat=True, save_count=None)
-                       # save_count=None is a (temporary) work-around 
-                       #     to fix memory leak in animate
+                  fargs=None, repeat=True, cache_frame_data=False)
     Tk.mainloop()
    
   except:
     print('*==* mpOsci: termination signal recieved')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpRMeter.py` & `picodaqa-1.1.1/picodaqa/mpRMeter.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,15 +89,13 @@
   canvas.get_tk_widget().pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
   canvas._tkcanvas.pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
 
 # set up matplotlib animation
   try:
     RMAnim = anim.FuncAnimation(figRM, RM, yieldEvt_fromQ, 
                         init_func=RM.init, interval=interval, blit=True,
-                        fargs=None, repeat=True, save_count=None)
-                             # save_count=None is a (temporary) work-around 
-                             #     to fix memory leak in animate
+                        fargs=None, repeat=True, cache_frame_data=False)
     Tk.mainloop()
    
   except:
     print('*==* mpRMeter: termination signal received')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/mpVMeter.py` & `picodaqa-1.1.1/picodaqa/mpVMeter.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,16 +59,14 @@
   canvas._tkcanvas.pack(side=Tk.TOP, fill=Tk.BOTH, expand=1)
   button = Tk.Button(master=root, text='Quit', command=sys.exit)
   button.pack(side=Tk.BOTTOM)
 
 # set up matplotlib animation
   VMAnim = anim.FuncAnimation(figVM, VM, yieldEvt_fromQ,
                          interval=WaitTime, init_func=VM.init,
-                         blit=True, fargs=None, repeat=True, save_count=None)
-                       # save_count=None is a (temporary) work-around 
-                       #     to fix memory leak in animate
+                         blit=True, fargs=None, repeat=True, cache_frame_data=False)
   try:
     Tk.mainloop()
    
   except:
     print('*==* mpVMeter: termination signal recieved')
   sys.exit()
```

### Comparing `picodaqa-1.1.0/picodaqa/picoConfig.py` & `picodaqa-1.1.1/picodaqa/picoConfig.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/plotBufManInfo.py` & `picodaqa-1.1.1/picodaqa/plotBufManInfo.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa/read_config.py` & `picodaqa-1.1.1/picodaqa/read_config.py`

 * *Files identical despite different names*

### Comparing `picodaqa-1.1.0/picodaqa.egg-info/PKG-INFO` & `picodaqa-1.1.1/picodaqa.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,172 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: picodaqa
-Version: 1.1.0
+Version: 1.1.1
 Summary: Data AcQuisition and analysis with PicoScope usb-oscilloscopes
 Home-page: https://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
-Description: # picoDAQ
-        
-        *python* Data AcQuisition and analysis with PicoScope usb-oscilloscopes
-        
-        The *usb*-oscilloscope series PicoSpope by Pico Technology (see <https://www.picotech.com>)
-        offers universal instruments that come with great software support, not only a graphical
-        interface offering the functionality known from oscilloscopes, but - most importantly for
-        this project - also with a software development kit (*SDK*) which makes it possible to use
-        the devices with a wide range of high-level languages.
-        
-        Provided here is a data acquisition system as is needed to record,  analyze, classify and
-        count the occurrence of wave forms such as provided for example by single-photon counters
-        or typical detectors common in quantum mechanical measurements or in nuclear, particle
-        physics and astro particle physics, e.g. photo tubes, Geiger counters, avalanche
-        photo-diodes or modern SiPMs.
-        
-        The random nature of such processes and the need to keep read-out dead times low requires
-        an input buffer and a buffer manager running as a background process. Data are provided
-        via the buffer manager interface to several consumer processes to analyze, check or
-        visualize data and analysis results. Such consumers may be obligatory ones, i.e. data
-        acquisition pauses if all input buffers are full and an obligatory consumer is still busy
-        processing. A second type of random consumers receives an event copy from the buffer manager
-        upon request, without pausing the data acquisition process. Typical examples of 
-        random consumers are displays of a subset of the wave forms or of intermediate
-        analysis results. Examples for such consumers are provided as part of this package,
-        running either as a 'thread' within the python interpreter or as sub-processes using
-        the 'multiprocessing' package.
-        
-        This project originated as a demonstration to analyze pulses from a photomultiplier (PM)
-        or a Silicon Photo Multiplier (SiPM) registering optical signals from  a detector, in the
-        simplest case a coffeepot filled with water and equipped with a PM to count muons from
-        cosmic rays. 
-        
-        ## List of implemented **Functions**:
-        
-        - class *picoConfig*:
-          - set up PicoScope time base, channel ranges and trigger
-          - set up the internal signal generator
-          - PicoScope configuration read from *json* or *yaml* file
-          - data acquisition of raw data from device
-        
-        - class *BufferMan*:
-          - acquire data (implemented as background thread)
-          - manage event data buffer and distribute to consumers
-          - configuration read from *json* or *yaml* file
-          - supports
-          
-            - *obligatory* consumers: data acquisition pauses until consumer done
-            - and *random* consumers: receive a copy of one event, data acquisition continues
-          
-        - module *AnimatedInstruments* (deprecated, to be removed soon)
-          - examples of animated graphical devices: a Buffer Manager display (using
-          class *plotBufManInfo), a VoltMeter (class *VoltMeter*), an Oscilloscope
-          (class *Ocscilloscope* and a ratemeter (class *RMeter*). The module must run as
-          a *python* *thread* in the same *python* interpreter as *BufferMan*
-        
-        - module *mpBufManCntrl*
-          - this sub-process receives status and logging information from the Buffer Manager
-          via a multiprocessing Queue and displays input rate history, filling level of the
-          buffers and the data-acquisition lifetime. Buttons at the bottom of the window allow
-          status changes (from RUNNING to PAUSED or vice versa) or to exit. A log-file at the
-          end contains a summary and, optionally, logging information. 
-        
-        - module *mpOsci*  
-          runs an instance of *Oscilloscpe* as a sub-process, and receives data from *BufferMan*
-          via a multiprocessing Queue.
-        
-        -  module *mpRMeter*    
-           runs an instance of the *RMeter* class as a sub-process, receiving via a multiprocessing Queue.
-        
-        - module *mpVMeter*  
-          runs an instance of the *VoltMeter* class as a sub-process, receiving data via a multiprocessing Queue. 
-        
-        - module *mpHists* 
-          runs an instance of the *animHists* class as a sub-process; receives input data via a
-          multiprocessing Queue. Data are formatted as lists of values. A normalized frequency distribution is
-          then updated and displayed.
-        
-        - module *mpBDisplay* 
-          - runs an instance of class BarDisplay and shows one (signed or unsigned) value per Channel
-          (e.g. peak Voltage, effective Voltage etc.). Values are passed to the sub-process via a
-          multiprocessing Queue.
-        
-        - module *mpDataLogger* 
-          runs an instance of the *DataLogger* class as a sub-process, displaying  values passed via a
-          multiprocessing Queue as a history plot. This module   is not implemented as a *BufferMan**
-          client (see example `runDataLogger`).
-        
-        - module *mpDataGraphs*  
-          runs an instance of the *DataGraphs* class as a sub-process, displaying values passed via a
-          multiprocessing Queue as a bar graph, a history plot or optionally - if two channels are
-          enabled - as xy-display. This module ist not implemented as a *BufferMan* client (see example
-          `runDataGraphs`)
-        
-        The script `runDAQ.py` gives an example of how to use all of the above. For a full demo,
-        connect the output of a PicoScope's signal generator to channel *B*, and eventually an
-        open cable to Channel *A* to see random noise. Use the configuration file `DAQconfig.yaml`,
-        which specifies the configuration files`BMconfig.yaml` for the Buffer Manager and `PSConfig.yaml`
-        for the PicoScope. As a hook for own extensions, user code may be included. An example for this
-        is shown in the configuration file `DAQ_Cosmo.json`, which points to a code snippet *anaDAQ.py*
-        to start some example consumers (code in`exampleConsumers.py`).
-        
-        
-        ## Examples
-        
-        The directory `examples/` contains configuration files and some special applications. 
-        
-        The script `runDataLogger.py` implements a data logger for rates below 20 Hz. Signals are
-        sampled with a PicoSocpe at a rate of 10 kHz over 20 ms and then averaged. 50 Hz noise is
-        thus eliminated, and a clean voltage signal is obtained. The history of the recorded voltages
-        is displayed using the module `mpDataLogger`. 
-        Similarly, `runDataGraphs` uses the same sampling mechanism to display the effective voltage
-        as bar graph, a history plot, and, optionally,   channel B vs. Channel A as an xy-graph if two
-        channels are enabled.
-        These examples directly read from the hardware device and therefore do not rely on the `BufferMan` class.
-        As a third simple example the script `runOsci.py` provides a simple oscilloscpe independent of BufferMan. 
-        
-        The script `runCosmo.py` is a modified version of `runDAQ.py` and depends on the code in
-        `pulseFilter.py`, which implements a convolution filter to search for characteristic signal
-        shapes in an input waveform. The example is tailored to identify short pulses from muon
-        detectors (e. g. the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt",
-        <http://www.teilchenwelt.de>, 
-        or the Kamiokanne-Experiment with photomultiplier readout and pulses shaped to a length of
-        approx. 150ns). A more complete and updated version has been moved to the project `picoCosmo`,
-        see <https://github.com/GuenterQuast/picoCosmo>. 
-        
-        
-        ## Installation of the package
-        
-        This python code is compatible with *python* versions and >=3.5. It was tested with PicoScope
-        device classes PS2000, PS2000a, PS3000a and PS4000 under Ubuntu, openSUSE Leap and on RaspberryPi.
-        Graphical displays are implemented with `matplotlib`.
-        
-        **Requirements:**
-        
-          - The low-level drivers and C-libraries contained in the Pico Technology
-            Software Development Kit are required,  *SDK* by Pico Technology,
-            see  https://www.picotech.com/downloads
-          - *python* bindings of the *pico-python* project by Colin O'Flynn
-            and Mark Harfouche, https://github.com/colinoflynn/pico-python
-        
-        *picoDAQ* presently consists of the modules in the direcoctry *picodaqa*, mentioned above,
-        and an example *python* script (*runDAQ.py*) with configuration examples (*.yaml* files) for
-        the data acquisition (*DAQconfig.yaml*), for the PicoScope Device (*PSconfig.yaml*) and for
-        the Buffer Mananger (*BMconfig.yaml*).
-        
-        After downloading all files from the git repository, connect your PicoScope and start from
-        the command line, e. g. `python runDAQ.py`. 
-        
-        You may run the script *make_dist.sh* to generate a *.whl* file in the subdirectory
-        *dist*, which can be installed via `pip install picodaqa_<vers>_<type>.whl`. Once
-        this is done, the provided examples can be copied to any directory. 
-        
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+License-File: AUTHORS
+
+# picoDAQ
+
+*python* Data AcQuisition and analysis with PicoScope usb-oscilloscopes
+
+The *usb*-oscilloscope series PicoSpope by Pico Technology (see <https://www.picotech.com>)
+offers universal instruments that come with great software support, not only a graphical
+interface offering the functionality known from oscilloscopes, but - most importantly for
+this project - also with a software development kit (*SDK*) which makes it possible to use
+the devices with a wide range of high-level languages.
+
+Provided here is a data acquisition system as is needed to record,  analyze, classify and
+count the occurrence of wave forms such as provided for example by single-photon counters
+or typical detectors common in quantum mechanical measurements or in nuclear, particle
+physics and astro particle physics, e.g. photo tubes, Geiger counters, avalanche
+photo-diodes or modern SiPMs.
+
+The random nature of such processes and the need to keep read-out dead times low requires
+an input buffer and a buffer manager running as a background process. Data are provided
+via the buffer manager interface to several consumer processes to analyze, check or
+visualize data and analysis results. Such consumers may be obligatory ones, i.e. data
+acquisition pauses if all input buffers are full and an obligatory consumer is still busy
+processing. A second type of random consumers receives an event copy from the buffer manager
+upon request, without pausing the data acquisition process. Typical examples of 
+random consumers are displays of a subset of the wave forms or of intermediate
+analysis results. Examples for such consumers are provided as part of this package,
+running either as a 'thread' within the python interpreter or as sub-processes using
+the 'multiprocessing' package.
+
+This project originated as a demonstration to analyze pulses from a photomultiplier (PM)
+or a Silicon Photo Multiplier (SiPM) registering optical signals from  a detector, in the
+simplest case a coffeepot filled with water and equipped with a PM to count muons from
+cosmic rays. 
+
+## List of implemented **Functions**:
+
+- class *picoConfig*:
+  - set up PicoScope time base, channel ranges and trigger
+  - set up the internal signal generator
+  - PicoScope configuration read from *json* or *yaml* file
+  - data acquisition of raw data from device
+
+- class *BufferMan*:
+  - acquire data (implemented as background thread)
+  - manage event data buffer and distribute to consumers
+  - configuration read from *json* or *yaml* file
+  - supports
+  
+    - *obligatory* consumers: data acquisition pauses until consumer done
+    - and *random* consumers: receive a copy of one event, data acquisition continues
+  
+- module *AnimatedInstruments* (deprecated, to be removed soon)
+  - examples of animated graphical devices: a Buffer Manager display (using
+  class *plotBufManInfo), a VoltMeter (class *VoltMeter*), an Oscilloscope
+  (class *Ocscilloscope* and a ratemeter (class *RMeter*). The module must run as
+  a *python* *thread* in the same *python* interpreter as *BufferMan*
+
+- module *mpBufManCntrl*
+  - this sub-process receives status and logging information from the Buffer Manager
+  via a multiprocessing Queue and displays input rate history, filling level of the
+  buffers and the data-acquisition lifetime. Buttons at the bottom of the window allow
+  status changes (from RUNNING to PAUSED or vice versa) or to exit. A log-file at the
+  end contains a summary and, optionally, logging information. 
+
+- module *mpOsci*  
+  runs an instance of *Oscilloscpe* as a sub-process, and receives data from *BufferMan*
+  via a multiprocessing Queue.
+
+-  module *mpRMeter*    
+   runs an instance of the *RMeter* class as a sub-process, receiving via a multiprocessing Queue.
+
+- module *mpVMeter*  
+  runs an instance of the *VoltMeter* class as a sub-process, receiving data via a multiprocessing Queue. 
+
+- module *mpHists* 
+  runs an instance of the *animHists* class as a sub-process; receives input data via a
+  multiprocessing Queue. Data are formatted as lists of values. A normalized frequency distribution is
+  then updated and displayed.
+
+- module *mpBDisplay* 
+  - runs an instance of class BarDisplay and shows one (signed or unsigned) value per Channel
+  (e.g. peak Voltage, effective Voltage etc.). Values are passed to the sub-process via a
+  multiprocessing Queue.
+
+- module *mpDataLogger* 
+  runs an instance of the *DataLogger* class as a sub-process, displaying  values passed via a
+  multiprocessing Queue as a history plot. This module   is not implemented as a *BufferMan**
+  client (see example `runDataLogger`).
+
+- module *mpDataGraphs*  
+  runs an instance of the *DataGraphs* class as a sub-process, displaying values passed via a
+  multiprocessing Queue as a bar graph, a history plot or optionally - if two channels are
+  enabled - as xy-display. This module ist not implemented as a *BufferMan* client (see example
+  `runDataGraphs`)
+
+The script `runDAQ.py` gives an example of how to use all of the above. For a full demo,
+connect the output of a PicoScope's signal generator to channel *B*, and eventually an
+open cable to Channel *A* to see random noise. Use the configuration file `DAQconfig.yaml`,
+which specifies the configuration files`BMconfig.yaml` for the Buffer Manager and `PSConfig.yaml`
+for the PicoScope. As a hook for own extensions, user code may be included. An example for this
+is shown in the configuration file `DAQ_Cosmo.json`, which points to a code snippet *anaDAQ.py*
+to start some example consumers (code in`exampleConsumers.py`).
+
+
+## Examples
+
+The directory `examples/` contains configuration files and some special applications. 
+
+The script `runDataLogger.py` implements a data logger for rates below 20 Hz. Signals are
+sampled with a PicoSocpe at a rate of 10 kHz over 20 ms and then averaged. 50 Hz noise is
+thus eliminated, and a clean voltage signal is obtained. The history of the recorded voltages
+is displayed using the module `mpDataLogger`. 
+Similarly, `runDataGraphs` uses the same sampling mechanism to display the effective voltage
+as bar graph, a history plot, and, optionally,   channel B vs. Channel A as an xy-graph if two
+channels are enabled.
+These examples directly read from the hardware device and therefore do not rely on the `BufferMan` class.
+As a third simple example the script `runOsci.py` provides a simple oscilloscpe independent of BufferMan. 
+
+The script `runCosmo.py` is a modified version of `runDAQ.py` and depends on the code in
+`pulseFilter.py`, which implements a convolution filter to search for characteristic signal
+shapes in an input waveform. The example is tailored to identify short pulses from muon
+detectors (e. g. the scintillator panels of the *CosMO*-experiment by "Netzwerk Teilchenwelt",
+<http://www.teilchenwelt.de>, 
+or the Kamiokanne-Experiment with photomultiplier readout and pulses shaped to a length of
+approx. 150ns). A more complete and updated version has been moved to the project `picoCosmo`,
+see <https://github.com/GuenterQuast/picoCosmo>. 
+
+
+## Installation of the package
+
+This python code is compatible with *python* versions and >=3.5. It was tested with PicoScope
+device classes PS2000, PS2000a, PS3000a and PS4000 under Ubuntu, openSUSE Leap and on RaspberryPi.
+Graphical displays are implemented with `matplotlib`.
+
+**Requirements:**
+
+  - The low-level drivers and C-libraries contained in the Pico Technology
+    Software Development Kit are required,  *SDK* by Pico Technology,
+    see  https://www.picotech.com/downloads
+  - *python* bindings of the *pico-python* project by Colin O'Flynn
+    and Mark Harfouche, https://github.com/colinoflynn/pico-python
+
+*picoDAQ* presently consists of the modules in the direcoctry *picodaqa*, mentioned above,
+and an example *python* script (*runDAQ.py*) with configuration examples (*.yaml* files) for
+the data acquisition (*DAQconfig.yaml*), for the PicoScope Device (*PSconfig.yaml*) and for
+the Buffer Mananger (*BMconfig.yaml*).
+
+After downloading all files from the git repository, connect your PicoScope and start from
+the command line, e. g. `python runDAQ.py`. 
+
+You may run the script *make_dist.sh* to generate a *.whl* file in the subdirectory
+*dist*, which can be installed via `pip install picodaqa_<vers>_<type>.whl`. Once
+this is done, the provided examples can be copied to any directory. 
+
+
+
```

### Comparing `picodaqa-1.1.0/picodaqa.egg-info/SOURCES.txt` & `picodaqa-1.1.1/picodaqa.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS
+LICENSE
 README.md
 setup.py
 picodaqa/BarDisplay.py
 picodaqa/BufferMan.py
 picodaqa/DataGraphs.py
 picodaqa/DataLogger.py
 picodaqa/Oscilloscope.py
```

### Comparing `picodaqa-1.1.0/setup.py` & `picodaqa-1.1.1/setup.py`

 * *Files identical despite different names*

