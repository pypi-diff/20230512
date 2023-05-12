# Comparing `tmp/nspyre_drivers-0.1.5.tar.gz` & `tmp/nspyre-drivers-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nspyre_drivers-0.1.5.tar", max compression
+gzip compressed data, was "nspyre-drivers-0.1.6.tar", max compression
```

## Comparing `nspyre_drivers-0.1.5.tar` & `nspyre-drivers-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,81 @@
--rw-r--r--   0        0        0     1067 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/LICENSE
--rw-r--r--   0        0        0     2200 2022-11-17 05:46:12.468729 nspyre_drivers-0.1.5/README.md
--rw-r--r--   0        0        0     1005 2022-11-17 05:46:51.844871 nspyre_drivers-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/agiltron/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/agiltron/ffsw/__init__.py
--rw-r--r--   0        0        0     2739 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/agiltron/ffsw/ffsw.py
--rw-r--r--   0        0        0        0 2022-11-17 05:31:15.477552 nspyre_drivers-0.1.5/src/drivers/arduino/__init__.py
--rw-r--r--   0        0        0       97 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/README.md
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/__init__.py
--rw-r--r--   0        0        0     6485 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/arduino_gpio.py
--rw-r--r--   0        0        0     3204 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/pin_server/pin_server.ino
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/__init__.py
--rw-r--r--   0        0        0     4163 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_gpio.py
--rw-r--r--   0        0        0      630 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_server/README.txt
--rw-r--r--   0        0        0      828 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.py
--rw-r--r--   0        0        0      238 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.service
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/dli_pdu/__init__.py
--rw-r--r--   0        0        0     6848 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/dli_pdu/dli_pdu.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/dlnsec/__init__.py
--rw-r--r--   0        0        0     3357 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/dlnsec/dlnsec.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/luminox/__init__.py
--rw-r--r--   0        0        0     2333 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/luminox/luminox.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/oceanoptics/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 05:31:46.853639 nspyre_drivers-0.1.5/src/drivers/oceanoptics/hr2000es/__init__.py
--rw-r--r--   0        0        0     7058 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/oceanoptics/hr2000es/hr2000es.py
--rw-r--r--   0        0        0        0 2022-11-17 05:31:55.989665 nspyre_drivers-0.1.5/src/drivers/rigol/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/rigol/dp832/__init__.py
--rw-r--r--   0        0        0     6284 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/rigol/dp832/dp832.py
--rw-r--r--   0        0        0        0 2022-11-17 05:32:05.445692 nspyre_drivers-0.1.5/src/drivers/rohde_schwarz/__init__.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/rohde_schwarz/hmp4040/__init__.py
--rw-r--r--   0        0        0     5808 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/rohde_schwarz/hmp4040/hmp4040.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/__init__.py
--rw-r--r--   0        0        0      134 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/cld1010/99-thorlabs-cld1010.rules
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/cld1010/__init__.py
--rw-r--r--   0        0        0     2971 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/cld1010/cld1010.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/fw102c/__init__.py
--rw-r--r--   0        0        0     6208 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/fw102c/fw102c.py
--rw-r--r--   0        0        0      130 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/pm100d/99-thorlabs-pm100d.rules
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/pm100d/__init__.py
--rw-r--r--   0        0        0     1647 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/thorlabs/pm100d/pm100d.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/ximea/__init__.py
--rw-r--r--   0        0        0     1344 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/ximea/ximea.py
--rw-r--r--   0        0        0        0 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/zaber/__init__.py
--rw-r--r--   0        0        0     2707 2022-11-14 15:22:55.030280 nspyre_drivers-0.1.5/src/drivers/zaber/zaber.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 nspyre_drivers-0.1.5/setup.py
--rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 nspyre_drivers-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2207 2022-11-25 18:59:25.317444 nspyre-drivers-0.1.6/README.md
+-rw-r--r--   0        0        0     1089 2023-05-12 01:53:02.605358 nspyre-drivers-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/__init__.py
+-rw-r--r--   0        0        0     4705 2023-03-27 22:46:52.628435 nspyre-drivers-0.1.6/src/nspyre_drivers/acton/sp2150i/sp2150i.py
+-rw-r--r--   0        0        0     2432 2023-04-19 16:51:24.805369 nspyre-drivers-0.1.6/src/nspyre_drivers/acton/sp2150i/sp2150i_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/agiltron/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/agiltron/ffsw/__init__.py
+-rw-r--r--   0        0        0     2702 2022-11-25 19:19:37.649299 nspyre-drivers-0.1.6/src/nspyre_drivers/agiltron/ffsw/ffsw.py
+-rw-r--r--   0        0        0     2739 2023-04-19 16:53:37.961355 nspyre-drivers-0.1.6/src/nspyre_drivers/agiltron/ffsw/ffsw_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/__init__.py
+-rw-r--r--   0        0        0       97 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/README.md
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/__init__.py
+-rw-r--r--   0        0        0     6524 2022-11-25 19:18:48.001298 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/arduino_gpio.py
+-rw-r--r--   0        0        0     2247 2023-04-19 16:54:58.685347 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/arduino_gpio_gui.py
+-rw-r--r--   0        0        0     3204 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/pin_server/pin_server.ino
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/__init__.py
+-rw-r--r--   0        0        0     4163 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_gpio.py
+-rw-r--r--   0        0        0     2275 2023-04-19 16:57:27.885333 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_gpio_gui.py
+-rw-r--r--   0        0        0      630 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_server/README.txt
+-rw-r--r--   0        0        0      828 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.py
+-rw-r--r--   0        0        0      238 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.service
+-rw-r--r--   0        0        0        0 2022-10-10 02:55:46.407563 nspyre-drivers-0.1.6/src/nspyre_drivers/cobolt/__init__.py
+-rw-r--r--   0        0        0     3513 2023-04-19 17:07:52.573280 nspyre-drivers-0.1.6/src/nspyre_drivers/cobolt/cobolt_gui.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:10:42.105267 nspyre-drivers-0.1.6/src/nspyre_drivers/cv2_cam/__init__.py
+-rw-r--r--   0        0        0     4864 2023-04-19 17:09:39.229272 nspyre-drivers-0.1.6/src/nspyre_drivers/cv2_cam/cv2_cam_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/dli_pdu/__init__.py
+-rw-r--r--   0        0        0     6848 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/dli_pdu/dli_pdu.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/dlnsec/__init__.py
+-rw-r--r--   0        0        0     3359 2022-12-15 21:50:22.058057 nspyre-drivers-0.1.6/src/nspyre_drivers/dlnsec/dlnsec.py
+-rw-r--r--   0        0        0     3787 2023-04-19 17:12:23.677260 nspyre-drivers-0.1.6/src/nspyre_drivers/dlnsec/dlnsec_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/luminox/__init__.py
+-rw-r--r--   0        0        0     2348 2022-11-25 19:16:51.669293 nspyre-drivers-0.1.6/src/nspyre_drivers/luminox/luminox.py
+-rw-r--r--   0        0        0        0 2022-12-01 23:20:03.610644 nspyre-drivers-0.1.6/src/nspyre_drivers/ni/__init__.py
+-rw-r--r--   0        0        0     5357 2023-03-27 22:46:52.628435 nspyre-drivers-0.1.6/src/nspyre_drivers/ni/daq.py
+-rw-r--r--   0        0        0    11593 2022-12-01 23:24:33.650527 nspyre-drivers-0.1.6/src/nspyre_drivers/ni/ni_motion_controller.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/__init__.py
+-rw-r--r--   0        0        0     7166 2023-03-27 22:46:52.628435 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/hr2000es.py
+-rw-r--r--   0        0        0     4258 2023-04-19 17:19:59.501192 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/hr2000es_gui.py
+-rw-r--r--   0        0        0   475241 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/PythonOceanDirect_User_Manual.rtf
+-rw-r--r--   0        0        0     2299 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/C/CExampleForOceanDirect.c
+-rw-r--r--   0        0        0     4290 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/CPlusPlus/CPlusPlusExampeForOceanDirect.cpp
+-rw-r--r--   0        0        0     5576 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/CPlusPlus/buffering.cpp
+-rw-r--r--   0        0        0     3818 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/CSharp/CSharpExampleForOceanDirect.cs
+-rw-r--r--   0        0        0    12784 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/LabVIEW/LabVIEW 2010/Labview2010ExampleForOceanDirect.vi
+-rw-r--r--   0        0        0    18867 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/LabVIEW/LabVIEW 2020/Labview2020ExampleForOceanDirect.vi
+-rw-r--r--   0        0        0     2660 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/MATLAB/MATLAB VVV/MatlabExampleForOceanDirect.m
+-rw-r--r--   0        0        0    20509 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/Python/Python VVV/PythonExampleForOceanDirect.py
+-rw-r--r--   0        0        0       65 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/README.md
+-rw-r--r--   0        0        0    38245 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/oceandirect/sample_pack/oceandirectsamples-v2.zip
+-rw-r--r--   0        0        0        0 2022-11-25 18:35:28.149673 nspyre-drivers-0.1.6/src/nspyre_drivers/pi/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-10 02:55:46.299563 nspyre-drivers-0.1.6/src/nspyre_drivers/pi/pi710/__init__.py
+-rw-r--r--   0        0        0    13614 2022-11-17 16:07:09.253467 nspyre-drivers-0.1.6/src/nspyre_drivers/pi/pi710/pi710.py
+-rw-r--r--   0        0        0  1044555 2023-04-18 23:31:48.542450 nspyre-drivers-0.1.6/src/nspyre_drivers/rfsoc/tProcv2_UG_v0.docx
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rigol/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rigol/dp832/__init__.py
+-rw-r--r--   0        0        0     6284 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rigol/dp832/dp832.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rohde_schwarz/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rohde_schwarz/hmp4040/__init__.py
+-rw-r--r--   0        0        0     5808 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/rohde_schwarz/hmp4040/hmp4040.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/__init__.py
+-rw-r--r--   0        0        0      134 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/cld1010/99-thorlabs-cld1010.rules
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/cld1010/__init__.py
+-rw-r--r--   0        0        0     2968 2022-12-14 23:59:06.821375 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/cld1010/cld1010.py
+-rw-r--r--   0        0        0     5010 2023-04-19 17:00:10.133318 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/cld1010/cld1010_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/fw102c/__init__.py
+-rw-r--r--   0        0        0     6199 2022-11-25 19:18:12.677297 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/fw102c/fw102c.py
+-rw-r--r--   0        0        0     1579 2023-04-19 17:16:36.525229 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/fw102c/fw102c_gui.py
+-rw-r--r--   0        0        0      130 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/pm100d/99-thorlabs-pm100d.rules
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/pm100d/__init__.py
+-rw-r--r--   0        0        0     1647 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/pm100d/pm100d.py
+-rw-r--r--   0        0        0     2576 2023-04-19 17:22:50.629167 nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/pm100d/pm100d_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/ximea/__init__.py
+-rw-r--r--   0        0        0     1349 2022-11-25 19:07:11.429367 nspyre-drivers-0.1.6/src/nspyre_drivers/ximea/ximea.py
+-rw-r--r--   0        0        0     5492 2022-11-25 19:08:36.549353 nspyre-drivers-0.1.6/src/nspyre_drivers/ximea/ximea_gui.py
+-rw-r--r--   0        0        0        0 2022-11-25 18:32:31.961702 nspyre-drivers-0.1.6/src/nspyre_drivers/zaber/__init__.py
+-rw-r--r--   0        0        0     2766 2022-11-25 19:20:28.573299 nspyre-drivers-0.1.6/src/nspyre_drivers/zaber/zaber.py
+-rw-r--r--   0        0        0     5115 2023-05-12 01:54:19.512327 nspyre-drivers-0.1.6/setup.py
+-rw-r--r--   0        0        0     3339 2023-05-12 01:54:19.512518 nspyre-drivers-0.1.6/PKG-INFO
```

### Comparing `nspyre_drivers-0.1.5/LICENSE` & `nspyre-drivers-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/README.md` & `nspyre-drivers-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 Reboot for the changes to take effect.
 
 ## Usage
 
 After installation, you can use drivers with, e.g.:
 
 ```python
-from drivers.rohde_schwarz.hmp4040.hmp4040 import HMP4040
+from nspyre_drivers.rohde_schwarz.hmp4040.hmp4040 import HMP4040
 with HMP4040('TCPIP::192.168.0.10::5025::SOCKET') as power_supply:
 	# set the power supply channel 1 to 5V
 	power_supply.set_voltage(1, 5.0)
 ```
 
 See the source for all of the available drivers and the import paths.
```

### Comparing `nspyre_drivers-0.1.5/pyproject.toml` & `nspyre-drivers-0.1.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 [tool.poetry]
 name = "nspyre-drivers"
-version = "0.1.5"
+version = "0.1.6"
 description = "A set of Python drivers for lab instrumentation."
 authors = [
 	"Jacob Feder <jacobsfeder@gmail.com>",
 	"Ben Soloway",
 	"Will Burke",
 	"Kimberly Carrillo Rivera"
 ]
 maintainers = [
 	"Jacob Feder <jacobsfeder@gmail.com>"
 ]
 readme = "README.md"
-packages = [{include = "drivers", from = "src"}]
+packages = [{include = "nspyre_drivers", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyvisa = "*"
 pyvisa-py = "*"
 pyserial = "*"
 pyusb = "*"
+numpy = "*"
 # extras
 requests = { version = "*", optional = true }
+beautifulsoup4 = { version = "*", optional = true }
 dlipower = { version = "*", optional = true }
 seabreeze = { version = "*", optional = true }
 ximea-py = { version = "*", optional = true }
 zaber-motion = { version = "*", optional = true }
-numpy = { version = "*", optional = true }
+nidaqmx = { version = "*", optional = true }
 
 [tool.poetry.extras]
 beaglebone = ["requests"]
 dli_pdu = ["dlipower", "beautifulsoup4"]
 oceanoptics = ["seabreeze"]
-ximea = ["ximea-py", "numpy"]
+ximea = ["ximea-py"]
 zaber = ["zaber-motion"]
+nidaq = ["nidaqmx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/agiltron/ffsw/ffsw.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/agiltron/ffsw/ffsw.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 """
 import serial
 import logging
 
 logger = logging.getLogger(__name__)
 
 class FFSW():
-    def __init__(self, com_port: str):
-        self.com_port = com_port
+    def __init__(self, serial_port: str):
+        self.serial_port = serial_port
 
     def _read(self):
-        response = self.serial_port.read(4)
+        response = self.conn.read(4)
         logger.debug(f'response [{response}]')
         return response
 
     def _write(self, msg):
-        self.serial_port.write(msg)
+        self.conn.write(msg)
         logger.debug(f'sent command [{msg}]')
 
     def get_sn(self):
         self._write(b"\x01\x03\x00\x00")
         a = self._read()[8::] #higher bits
         self._write(b"\x01\x04\x00\x00")
         b = self._read()[8::] #lower bits
@@ -55,33 +55,33 @@
         return port
 
     def get_temp(self):
         self._write(b"\x01\x22\x00\x00")
         return self._read()
 
     def open(self):
-        self.serial_port = serial.Serial(port=self.com_port, baudrate=9600, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE, bytesize=serial.EIGHTBITS)
+        self.conn = serial.Serial(port=self.serial_port, baudrate=9600, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE, bytesize=serial.EIGHTBITS)
 
     def close(self):
-        self.serial_port.close()
+        self.conn.close()
 
     def __enter__(self):
         self.open()
-        self.serial_port.flush()
+        self.conn.flush()
         return self
 
     def __exit__(self, *args):
-        self.serial_port.flush()
+        self.conn.flush()
         self.close()
 
 
 if __name__ == '__main__':
     with FFSW('/dev/serial/by-id/usb-FTDI_FT232R_USB_UART_AU03N2AV-if00-port0') as switch:
         print('flushing buffer')
-        print(switch.serial_port.flush())
+        print(switch.conn.flush())
         print('setting port 1')
         print(switch.set_port(1))
         print('getting port after setting port 1')
         print(switch.get_port())
         print('setting port 2')
         print(switch.set_port(2))
         print('getting port after setting port 2')
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/arduino_gpio.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/arduino_gpio.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,28 @@
         # args: pin id, state
         pin_state_changed = QtCore.Signal(int, bool)
         # args: dac channel, dac raw value
         dac_val_changed = QtCore.Signal(str, int)
         # args: dac channel, dac voltage
         dac_voltage_changed = QtCore.Signal(str, float)
 
-    def __init__(self, com_port: str, pins=None, baud=115200,
-                    write_timeout:float = 3.0, timeout: float = 3.0):
+    def __init__(self, serial_port: str, pins=None, baud=115200, 
+                    timeout: float = 3.0):
         """Args:
-            com_port: serial COM port (see pyserial docs)
+            serial_port: serial COM port (see pyserial docs)
             npins: number of digital pins
             baud: baudrate
             timeout: read timeout (s)
         """
         super().__init__()
 
+        self.serial_port = serial_port
+        self.baud = baud
+        self.timeout = timeout
+
         # available pins
         if pins is not None:
             self.pins = pins
         else:
             # assume arduino UNO
             self.pins = list(range(2, 13))
 
@@ -54,23 +58,23 @@
             'VA': 0,
             'VB': 1,
             'VC': 2,
             'VD': 3,
         }
 
     def open(self):
-        self.serial_port = serial.Serial(com_port, baudrate=baud, timeout=timeout)
-        logger.info(f'connected to Arduino @ [{com_port}]')
+        self.conn = serial.Serial(self.serial_port, baudrate=self.baud, timeout=self.timeout)
+        logger.info(f'connected to Arduino @ [{self.serial_port}]')
         # this is required due to a funky issue with the arduino uno
         # (it restarts the arduino when opening the serial port, so we have to wait for it to boot)
         # https://stackoverflow.com/questions/1618141/pyserial-problem-with-arduino-works-with-the-python-shell-but-not-in-a-program/4941880#4941880
         time.sleep(2)
 
     def close(self):
-        self.serial_port.close()
+        self.conn.close()
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, *args):
         self.close()
@@ -84,29 +88,29 @@
             arg2: second argument for command
             tries: the number of times that the communication has been attempted
 
         Returns:
             The device response as a string
         """
         msg = cmd.encode('ascii') + bytes([arg1, arg2, arg3])
-        logger.debug(f'writing packet 0x{msg.hex()} to Arduino [{self.serial_port}]')
-        self.serial_port.write(msg)
+        logger.debug(f'writing packet 0x{msg.hex()} to Arduino [{self.conn}]')
+        self.conn.write(msg)
         # response the Arduino sends when it's ready for the next command
         ok_resp = b'rdy\n'
         # response from the Arduino
         resp = b''
         while ok_resp not in resp:
-            resp += self.serial_port.read(1)
+            resp += self.conn.read(1)
             logger.debug(f'Arduino responded with [{resp.decode("ascii", "ignore").encode("unicode_escape")} (ascii)] [{resp.hex()}(hex)]')
             if resp == b'':
                 raise RuntimeError('Error in communication with Arduino program. No Response.')
         if b'error' in resp:
             if tries < 5:
                 # shift one byte so that hopefully it reads correctly next time
-                self.serial_port.write(bytes([0]))
+                self.conn.write(bytes([0]))
                 self._send_cmd(cmd, arg1, arg2, arg3, tries=tries + 1)
             else:
                 # if it's failed too many times, give up
                 raise RuntimeError(f'Error in communication with Arduino program. Arduino program error:\n{resp}')
         return resp
 
     def set_pin(self, pin, state, emit=True):
@@ -120,18 +124,18 @@
         Raises:
             ValueError: invalid pin
         """
         if pin not in self.pins:
             raise ValueError(f'Pin is invalid. Available pins:\n{self.pins}')
         if state:
             self._send_cmd('o', pin, 1)
-            logger.debug(f'Set Arduino@{self.serial_port} pin [{pin}] HIGH')
+            logger.debug(f'Set Arduino@{self.conn} pin [{pin}] HIGH')
         else:
             self._send_cmd('o', pin, 0)
-            logger.debug(f'Set Arduino@{self.serial_port} pin [{pin}] LOW')
+            logger.debug(f'Set Arduino@{self.conn} pin [{pin}] LOW')
         if gui and emit:
             self.pin_state_changed.emit(pin, state)
 
     def set_dac(self, ch, val, emit=True):
         """Set the output voltage of the connected MCP4728 quad DAC.
 
         Args:
@@ -144,15 +148,15 @@
         """
         if ch not in self.dac_chs:
             raise ValueError(f'DAC channel is invalid. Available channels:\n{self.dac_chs.keys()}')
         if val < 0 or val > 4095 or not isinstance(val, int):
             raise ValueError('val must be an int in the range 0 < val < 4095')
 
         self._send_cmd('d', self.dac_chs[ch], val & 0xFF, (val & 0xFF00) >> 8)
-        logger.debug(f'Set Arduino@{self.serial_port} dac ch [{ch}] to [{val}]')
+        logger.debug(f'Set Arduino@{self.conn} dac ch [{ch}] to [{val}]')
 
         if gui and emit:
             self.dac_val_changed.emit(ch, val)
 
     def set_voltage(self, ch, volt, emit=True):
         """Set DAC output voltage
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/arduino/arduino_gpio/pin_server/pin_server.ino` & `nspyre-drivers-0.1.6/src/nspyre_drivers/arduino/arduino_gpio/pin_server/pin_server.ino`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_gpio.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_gpio.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_server/README.txt` & `nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_server/README.txt`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/beaglebone/beaglebone_gpio/beaglebone_server/gpio_flask_server.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/dli_pdu/dli_pdu.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/dli_pdu/dli_pdu.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/dlnsec/dlnsec.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/dlnsec/dlnsec.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,51 +9,52 @@
 import logging
 
 import serial
 
 logger = logging.getLogger(__name__)
 
 class DLnsec():
-    def __init__(self, com_port: str, timeout=1.0):
+    def __init__(self, serial_port: str, timeout=1.0):
         """
         Args:
-            com_port: serial COM port (see pyserial docs)
+            serial_port: serial COM port (see pyserial docs)
         """
-        self.com_port = com_port
+        self.serial_port = serial_port
         self.timeout = timeout
 
     def open(self):
         """Connect to the laser."""
-        self.serial_port = serial.Serial(com_port, baudrate=9600, timeout=timeout)
-        self.serial_port.reset_input_buffer()
-        self.serial_port.reset_output_buffer()
+        self.conn = serial.Serial(self.serial_port, baudrate=9600, timeout=self.timeout)
+        self.conn.reset_input_buffer()
+        self.conn.reset_output_buffer()
         self.reboot()
         # query the laser serial number
         self.idn = self._query('*IDN')
         if not self.idn:
             raise RuntimeError('Failed getting laser ID number')
-        logging.info(f'Connected to DLnsec [{self.idn}]')
+        logger.info(f'Connected to DLnsec [{self.idn}]')
 
     def close(self):
         """Disconnect from the laser."""
-        self.serial_port.close()
+        self.conn.close()
 
     def __enter__(self):
+        self.open()
         return self
 
     def __exit__(self, *args):
         self.off()
         self.close()
 
     def _send_raw(self, msg):
         """Send a command to the laser."""
         # add a newline and encode the message into a binary string
         msg_bin = (msg + '\n').encode('ascii')
         # send the message on the serial port
-        self.serial_port.write(msg_bin)
+        self.conn.write(msg_bin)
         logger.debug(f'Sent message to DLnsec: [{msg}]')
         # wait for the laser to process the message
         time.sleep(0.1)
 
     def _send(self, msg):
         """Send a command to the laser and check for errors."""
         # number of times to try sending the command
@@ -75,15 +76,15 @@
                 # wait a moment before trying again
                 time.sleep(0.25)
 
     def _query(self, msg):
         """Send a query command to the laser and return the response."""
         self._send_raw(msg)
         # receive the response
-        response = self.serial_port.read_until(b'\n\r')
+        response = self.conn.read_until(b'\n\r')
         response = response.decode('ascii').strip('\n\r')
         logger.debug(f'Response from DLnsec: [{response}]')
 
         return response
 
     def power(self, p):
         """Set the output power (integer percentage)"""
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/luminox/luminox.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/luminox/luminox.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 import serial
 import logging
 import time
 
 logger = logging.getLogger(__name__)
 
 class LOX_02:
-    def __init__(self, com_port: str):
+    def __init__(self, serial_port: str):
         """Args:
-            com_port: serial COM port (see pyserial docs)
+            serial_port: serial COM port (see pyserial docs)
         """
-        self.com_port = com_port
+        self.serial_port = serial_port
 
     def open(self):
-        self.serial_port = serial.Serial(self.com_port)
+        self.serial_port = serial.Serial(self.serial_port)
         self.mode_poll()
         self.serial_port.reset_input_buffer()
 
     def close(self):
         self.serial_port.close()
 
     def __enter__(self):
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/oceanoptics/hr2000es/hr2000es.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/oceanoptics/hr2000es/hr2000es.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,15 +114,17 @@
             logger.info('Set spectrometer to Normal ("Free Running") Mode')
             self.spec.trigger_mode(mode)
         elif mode == 3:
             logger.info('Set spectrometer to External Hardware Edge Trigger Mode')
             logger.info("An external trigger rising edge will start the acquisition. Only one acquisition will be performed for each External Trigger pulse, no matter what the pulses' duration is.")
             self.spec.trigger_mode(mode)
         else:
-            raise ValueError(f"Invalid mode selection OR if 1,2 I don't know what the mode is: {mode}")
+            self.spec.trigger_mode(mode)
+            logger.info(f"Warning not sure what mode {mode} is.")
+            #raise ValueError(f"Invalid mode selection OR if 1,2 I don't know what the mode is: {mode}")
 
     # def _set_trigger_mode(self, mode):
     #   self.spec.trigger_mode(mode)
     #
     # def _set_trigger(self, mode):
     #   p = multiprocessing.Process(target=self._set_trigger_mode, args=(mode,))
     #   p.start()
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/rigol/dp832/dp832.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/rigol/dp832/dp832.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/rohde_schwarz/hmp4040/hmp4040.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/rohde_schwarz/hmp4040/hmp4040.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/thorlabs/cld1010/cld1010.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/cld1010/cld1010.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,20 @@
         self.close()
 
     def __str__(self):
         return f'{self.address} {self.idn}'
 
     def open(self):
         try:
-            self.device = self.rm.open_resource(self.address)
+            self.laser = self.rm.open_resource(self.address)
         except Exception as err:
             raise ConnectionError(f'Failed connecting to CLD1010 @ [{self.address}]') from err
         # 1 second timeout
-        self.device.timeout = 1000
-        self.idn = self.device.query('*IDN?')
+        self.laser.timeout = 1000
+        self.idn = self.laser.query('*IDN?')
         logger.info(f'Connected to CLD1010 [{self}].')
         return self
 
     def close(self):
         self.laser.close()
 
     def idn(self):
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/thorlabs/fw102c/fw102c.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/fw102c/fw102c.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 """
 import serial
 import logging
 
 logger = logging.getLogger(__name__)
 
 class FW102C:
-    def __init__(self, com_port: str, channel_mapping=None, baud=115200, timeout: float = 10.0):
+    def __init__(self, serial_port: str, channel_mapping=None, baud=115200, timeout: float = 10.0):
         """Args:
-            com_port: serial COM port (see pyserial docs)
+            serial_port: serial COM port (see pyserial docs)
             channel_mapping: dictionary mapping an identifier to a channel, which can be used instead of the channel number e.g.
             {'filter1': 1, 'filter2': 2}
             baud: 9600 or 115200
             timeout: read timeout
         """
         self.channel_mapping = channel_mapping
-        self.com_port = com_port
+        self.serial_port = serial_port
         self.baud = baud
         self.timeout = timeout
 
     def __str__(self):
-        return f'{self.address} {self.idn}'
+        return f'{self.serial_port} {self.idn}'
 
     def __enter__(self):
         self.open()
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def close(self):
-        self.serial_port.close()
+        self.conn.close()
 
     def open(self):
-        self.serial_port = serial.Serial(self.com_port, baudrate=self.baud, timeout=self.timeout)
+        self.conn = serial.Serial(self.serial_port, baudrate=self.baud, timeout=self.timeout)
         # send a dummy command to clear any previous messages
         self.idn = self._query('*idn')
         logger.info(f'Connected to [{self}].')
 
     def _send_cmd(self, cmd):
         """Format and send a command to the device.
         
@@ -51,16 +51,16 @@
             cmd: the command to send, e.g. '*idn?'
         
         Returns:
             The device response as a string (with the '>' stripped)
         """
         logger.debug(f'sending message [{cmd}]')
         cmd += '\r'
-        self.serial_port.write(cmd.encode('ascii'))
-        response = self.serial_port.read_until('> '.encode('ascii')).decode('ascii')
+        self.conn.write(cmd.encode('ascii'))
+        response = self.conn.read_until('> '.encode('ascii')).decode('ascii')
         if '> ' not in response: 
             raise RuntimeError('Timed out waiting for response')
         # strip preceding message and trailing '\r> '
         trimmed_response = response[len(cmd):-3]
         logger.debug(f'received response [{trimmed_response}]')
         return trimmed_response
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/thorlabs/pm100d/pm100d.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/thorlabs/pm100d/pm100d.py`

 * *Files identical despite different names*

### Comparing `nspyre_drivers-0.1.5/src/drivers/ximea/ximea.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/ximea/ximea.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.connect()
         return self
 
     def __exit__(self, *args):
         self.disconnect()
 
     def connect(self):
-        if serial_number is not None:
+        if self.serial_number is not None:
             self.driver = ximea.xiapi.open_device_by_SN(serial_number)
         else:
             # create instance for first connected camera
             self.driver = ximea.xiapi.Camera()
 
         self.driver.open_device()
         # default settings
```

### Comparing `nspyre_drivers-0.1.5/src/drivers/zaber/zaber.py` & `nspyre-drivers-0.1.6/src/nspyre_drivers/zaber/zaber.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def __init__(self, axis_mapping, serial_port=None):
         """
         Args:
             serial_port: serial COM port (see pyserial docs). Leave as None to detect automatically (linux only).
             axis_mapping: dictionary mapping an axis peripheral id (int) to the axis name (str)
         """
         self.axis_mapping = axis_mapping
-        self.com_port = com_port
+        self.serial_port = serial_port
 
     def __getitem__(self, key):
         """Return the zaber axis object associated with the given key."""
         if key in self.axes:
             return self.axes[key]
         else:
             raise KeyError(f'Zaber axis key [{key}] not found')
@@ -35,22 +35,23 @@
     def __iter__(self):
         return self.axes.__iter__()
 
     def __next__(self):
         return self.axes.__next__()
 
     def __enter__(self):
+        self.open()
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def open(self):
-        if self.com_port:
-            self.conn = Connection.open_serial_port(com_port)
+        if self.serial_port is not None:
+            self.conn = Connection.open_serial_port(self.serial_port)
             logger.debug(f'Found {len(device_list)} devices')
         else:
             # detect any connected Zaber serial devices
             zaber_serial_ports = Path('/dev/serial/by-id/').glob('usb-Zaber_Technologies_Inc.*')
             self.conn = None
             for s in zaber_serial_ports:
                 # connect to the first one and then exit the loop
@@ -63,14 +64,14 @@
         logger.debug(f'Found [{len(self.devices)}] zaber devices')
 
         self.axes = OrderedDict()
         for device in self.devices:
             for i in range(1, device.axis_count + 1):
                 axis = device.get_axis(i)
                 logger.debug(f'Found Zaber axis [{axis}] with peripheral id [{axis.peripheral_id}]')
-                if axis.peripheral_id in axis_mapping:
-                    axis_key = axis_mapping[axis.peripheral_id]
+                if axis.peripheral_id in self.axis_mapping:
+                    axis_key = self.axis_mapping[axis.peripheral_id]
                     logger.debug(f'Associated zaber axis [{axis_key}] with peripheral id [{axis.peripheral_id}]')
                     self.axes[axis_key] = axis
 
     def close(self):
         self.conn.close()
```

### Comparing `nspyre_drivers-0.1.5/PKG-INFO` & `nspyre-drivers-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: nspyre-drivers
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of Python drivers for lab instrumentation.
 Author: Jacob Feder
 Author-email: jacobsfeder@gmail.com
 Maintainer: Jacob Feder
 Maintainer-email: jacobsfeder@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: beaglebone
-Provides-Extra: dli-pdu
+Provides-Extra: dli_pdu
+Provides-Extra: nidaq
 Provides-Extra: oceanoptics
 Provides-Extra: ximea
 Provides-Extra: zaber
-Requires-Dist: dlipower; extra == "dli-pdu"
-Requires-Dist: numpy; extra == "ximea"
+Requires-Dist: beautifulsoup4; extra == "dli_pdu"
+Requires-Dist: dlipower; extra == "dli_pdu"
+Requires-Dist: nidaqmx; extra == "nidaq"
+Requires-Dist: numpy
 Requires-Dist: pyserial
 Requires-Dist: pyusb
 Requires-Dist: pyvisa
 Requires-Dist: pyvisa-py
 Requires-Dist: requests; extra == "beaglebone"
 Requires-Dist: seabreeze; extra == "oceanoptics"
 Requires-Dist: ximea-py; extra == "ximea"
@@ -83,15 +85,15 @@
 Reboot for the changes to take effect.
 
 ## Usage
 
 After installation, you can use drivers with, e.g.:
 
 ```python
-from drivers.rohde_schwarz.hmp4040.hmp4040 import HMP4040
+from nspyre_drivers.rohde_schwarz.hmp4040.hmp4040 import HMP4040
 with HMP4040('TCPIP::192.168.0.10::5025::SOCKET') as power_supply:
 	# set the power supply channel 1 to 5V
 	power_supply.set_voltage(1, 5.0)
 ```
 
 See the source for all of the available drivers and the import paths.
```

