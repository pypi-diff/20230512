# Comparing `tmp/zivid-2.8.0.2.9.0.tar.gz` & `tmp/zivid-2.9.0.2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zivid-2.8.0.2.9.0.tar", last modified: Wed Apr  5 10:27:51 2023, max compression
+gzip compressed data, was "zivid-2.9.0.2.9.0.tar", last modified: Fri May 12 10:49:54 2023, max compression
```

## Comparing `zivid-2.8.0.2.9.0.tar` & `zivid-2.9.0.2.9.0.tar`

### file list

```diff
@@ -1,116 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.629205 zivid-2.8.0.2.9.0/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1521 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11088 2023-04-05 10:27:51.629205 zivid-2.8.0.2.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9048 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.613204 zivid-2.8.0.2.9.0/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.613204 zivid-2.8.0.2.9.0/modules/_zivid/
--rw-r--r--   0 root         (0) root         (0)     2579 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/_zivid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.617204 zivid-2.8.0.2.9.0/modules/zivid/
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.617204 zivid-2.8.0.2.9.0/modules/zivid/_calibration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_calibration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2442 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_calibration/detector.py
--rw-r--r--   0 root         (0) root         (0)     5729 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_calibration/hand_eye.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_calibration/multi_camera.py
--rw-r--r--   0 root         (0) root         (0)      725 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_calibration/pose.py
--rw-r--r--   0 root         (0) root         (0)     5961 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_suggest_settings_parameters.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/_version.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/application.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/calibration.py
--rw-r--r--   0 root         (0) root         (0)     3994 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/camera.py
--rw-r--r--   0 root         (0) root         (0)    12172 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/camera_info.py
--rw-r--r--   0 root         (0) root         (0)    15349 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/camera_intrinsics.py
--rw-r--r--   0 root         (0) root         (0)    10749 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/camera_state.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/capture_assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.617204 zivid-2.8.0.2.9.0/modules/zivid/experimental/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/experimental/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13657 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/experimental/calibration.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/firmware.py
--rw-r--r--   0 root         (0) root         (0)     3443 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/frame.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/frame_2d.py
--rw-r--r--   0 root         (0) root         (0)    13873 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/frame_info.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/image.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/matrix4x4.py
--rw-r--r--   0 root         (0) root         (0)     5548 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/sdk_version.py
--rw-r--r--   0 root         (0) root         (0)   119278 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/settings.py
--rw-r--r--   0 root         (0) root         (0)    21003 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/modules/zivid/settings_2d.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     5125 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.621204 zivid-2.8.0.2.9.0/src/
--rw-r--r--   0 root         (0) root         (0)     1185 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.621204 zivid-2.8.0.2.9.0/src/Calibration/
--rw-r--r--   0 root         (0) root         (0)     2084 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Calibration/Calibration.cpp
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Calibration/Detector.cpp
--rw-r--r--   0 root         (0) root         (0)     1450 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Calibration/HandEye.cpp
--rw-r--r--   0 root         (0) root         (0)     1190 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Calibration/MultiCamera.cpp
--rw-r--r--   0 root         (0) root         (0)      602 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Calibration/Pose.cpp
--rw-r--r--   0 root         (0) root         (0)      859 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/CaptureAssistant.cpp
--rw-r--r--   0 root         (0) root         (0)     2757 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/DataModel.cpp
--rw-r--r--   0 root         (0) root         (0)      833 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Firmware.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.621204 zivid-2.8.0.2.9.0/src/InfieldCorrection/
--rw-r--r--   0 root         (0) root         (0)     2967 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/InfieldCorrection/InfieldCorrection.cpp
--rw-r--r--   0 root         (0) root         (0)     3159 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Matrix4x4.cpp
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/NodeType.cpp
--rw-r--r--   0 root         (0) root         (0)     7007 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasableArray2D.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasableCamera.cpp
--rw-r--r--   0 root         (0) root         (0)      825 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasableFrame.cpp
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasableFrame2D.cpp
--rw-r--r--   0 root         (0) root         (0)     1777 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasableImage.cpp
--rw-r--r--   0 root         (0) root         (0)     1400 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/ReleasablePointCloud.cpp
--rw-r--r--   0 root         (0) root         (0)      881 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/SingletonApplication.cpp
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Version.cpp
--rw-r--r--   0 root         (0) root         (0)     2519 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Wrapper.cpp
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/Wrapper.h.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.613204 zivid-2.8.0.2.9.0/src/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.625205 zivid-2.8.0.2.9.0/src/include/ZividPython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.625205 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/
--rw-r--r--   0 root         (0) root         (0)      176 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/Calibration.h
--rw-r--r--   0 root         (0) root         (0)      221 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/Detector.h
--rw-r--r--   0 root         (0) root         (0)      381 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/HandEye.h
--rw-r--r--   0 root         (0) root         (0)      313 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/MultiCamera.h
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Calibration/Pose.h
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/CaptureAssistant.h
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/DataModel.h
--rw-r--r--   0 root         (0) root         (0)    11092 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/DataModelWrapper.h
--rw-r--r--   0 root         (0) root         (0)      166 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/DependentFalse.h
--rw-r--r--   0 root         (0) root         (0)      170 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Firmware.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.625205 zivid-2.8.0.2.9.0/src/include/ZividPython/InfieldCorrection/
--rw-r--r--   0 root         (0) root         (0)      702 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/InfieldCorrection/InfieldCorrection.h
--rw-r--r--   0 root         (0) root         (0)      733 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Matrix.h
--rw-r--r--   0 root         (0) root         (0)      162 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Matrix4x4.h
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/NodeType.h
--rw-r--r--   0 root         (0) root         (0)     8164 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Releasable.h
--rw-r--r--   0 root         (0) root         (0)      851 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableArray2D.h
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableCamera.h
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableFrame.h
--rw-r--r--   0 root         (0) root         (0)      656 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableFrame2D.h
--rw-r--r--   0 root         (0) root         (0)      567 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableImage.h
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasablePointCloud.h
--rw-r--r--   0 root         (0) root         (0)      950 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/SingletonApplication.h
--rw-r--r--   0 root         (0) root         (0)     1344 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Traits.h
--rw-r--r--   0 root         (0) root         (0)      168 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Version.h
--rw-r--r--   0 root         (0) root         (0)     7721 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/src/include/ZividPython/Wrappers.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 10:27:51.629205 zivid-2.8.0.2.9.0/test/
--rw-r--r--   0 root         (0) root         (0)     1812 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_application.py
--rw-r--r--   0 root         (0) root         (0)     2955 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_camera.py
--rw-r--r--   0 root         (0) root         (0)     3281 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_camera_capture.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_camera_info.py
--rw-r--r--   0 root         (0) root         (0)     2389 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_camera_state.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_camera_user_data.py
--rw-r--r--   0 root         (0) root         (0)     5521 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_capture_assistant.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_datamodel_save_load.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_firmware.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_frame.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_frame_2d.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_frame_info.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_image_2d.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_matrix4x4.py
--rw-r--r--   0 root         (0) root         (0)     9504 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_region_of_interest.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_samples.py
--rw-r--r--   0 root         (0) root         (0)    37998 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_settings.py
--rw-r--r--   0 root         (0) root         (0)     6533 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_settings_2d.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_versioning.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-04-05 10:26:08.000000 zivid-2.8.0.2.9.0/test/test_zivid_module_content.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1521 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11196 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9148 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.094758 zivid-2.9.0.2.9.0/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.094758 zivid-2.9.0.2.9.0/modules/_zivid/
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/_zivid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.094758 zivid-2.9.0.2.9.0/modules/zivid/
+-rw-r--r--   0 root         (0) root         (0)      829 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/modules/zivid/_calibration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_calibration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_calibration/detector.py
+-rw-r--r--   0 root         (0) root         (0)     5729 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_calibration/hand_eye.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_calibration/multi_camera.py
+-rw-r--r--   0 root         (0) root         (0)      725 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_calibration/pose.py
+-rw-r--r--   0 root         (0) root         (0)     5959 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_suggest_settings_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/application.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/calibration.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/camera.py
+-rw-r--r--   0 root         (0) root         (0)    12168 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/camera_info.py
+-rw-r--r--   0 root         (0) root         (0)    15346 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/camera_intrinsics.py
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/camera_state.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/capture_assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/modules/zivid/experimental/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/experimental/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13657 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/experimental/calibration.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/firmware.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/frame.py
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/frame_2d.py
+-rw-r--r--   0 root         (0) root         (0)    13868 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/frame_info.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/image.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/matrix4x4.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/sdk_version.py
+-rw-r--r--   0 root         (0) root         (0)   119247 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/settings.py
+-rw-r--r--   0 root         (0) root         (0)    20998 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/modules/zivid/settings_2d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/modules/zivid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11196 2023-05-12 10:49:54.000000 zivid-2.9.0.2.9.0/modules/zivid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3279 2023-05-12 10:49:54.000000 zivid-2.9.0.2.9.0/modules/zivid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 10:49:54.000000 zivid-2.9.0.2.9.0/modules/zivid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-12 10:49:54.000000 zivid-2.9.0.2.9.0/modules/zivid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-12 10:49:54.000000 zivid-2.9.0.2.9.0/modules/zivid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5124 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/src/
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/src/Calibration/
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Calibration/Calibration.cpp
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Calibration/Detector.cpp
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Calibration/HandEye.cpp
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Calibration/MultiCamera.cpp
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Calibration/Pose.cpp
+-rw-r--r--   0 root         (0) root         (0)      859 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/CaptureAssistant.cpp
+-rw-r--r--   0 root         (0) root         (0)     2757 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/DataModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      833 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Firmware.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.098758 zivid-2.9.0.2.9.0/src/InfieldCorrection/
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/InfieldCorrection/InfieldCorrection.cpp
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Matrix4x4.cpp
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/NodeType.cpp
+-rw-r--r--   0 root         (0) root         (0)     9703 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasableArray2D.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasableCamera.cpp
+-rw-r--r--   0 root         (0) root         (0)      825 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasableFrame.cpp
+-rw-r--r--   0 root         (0) root         (0)      656 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasableFrame2D.cpp
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasableImage.cpp
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/ReleasablePointCloud.cpp
+-rw-r--r--   0 root         (0) root         (0)      881 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/SingletonApplication.cpp
+-rw-r--r--   0 root         (0) root         (0)      491 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Version.cpp
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Wrapper.cpp
+-rw-r--r--   0 root         (0) root         (0)      318 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/Wrapper.h.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.094758 zivid-2.9.0.2.9.0/src/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/src/include/ZividPython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/Calibration.h
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/Detector.h
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/HandEye.h
+-rw-r--r--   0 root         (0) root         (0)      313 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/MultiCamera.h
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Calibration/Pose.h
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/CaptureAssistant.h
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/DataModel.h
+-rw-r--r--   0 root         (0) root         (0)    11092 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/DataModelWrapper.h
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/DependentFalse.h
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Firmware.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/src/include/ZividPython/InfieldCorrection/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/InfieldCorrection/InfieldCorrection.h
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Matrix.h
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Matrix4x4.h
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/NodeType.h
+-rw-r--r--   0 root         (0) root         (0)     8164 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Releasable.h
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableArray2D.h
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableCamera.h
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableFrame.h
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableFrame2D.h
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableImage.h
+-rw-r--r--   0 root         (0) root         (0)      925 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasablePointCloud.h
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/SingletonApplication.h
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Traits.h
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Version.h
+-rw-r--r--   0 root         (0) root         (0)     7721 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/src/include/ZividPython/Wrappers.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 10:49:54.102758 zivid-2.9.0.2.9.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_application.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_camera.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_camera_capture.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_camera_info.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_camera_state.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_camera_user_data.py
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_capture_assistant.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_datamodel_save_load.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_firmware.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_frame.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_frame_2d.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_frame_info.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_image_2d_bgra.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_image_2d_rgba.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_matrix4x4.py
+-rw-r--r--   0 root         (0) root         (0)    11033 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_region_of_interest.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_samples.py
+-rw-r--r--   0 root         (0) root         (0)    37998 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6533 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_settings_2d.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_versioning.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-05-12 10:48:34.000000 zivid-2.9.0.2.9.0/test/test_zivid_module_content.py
```

### Comparing `zivid-2.8.0.2.9.0/CMakeLists.txt` & `zivid-2.9.0.2.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/LICENSE` & `zivid-2.9.0.2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/PKG-INFO` & `zivid-2.9.0.2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zivid
-Version: 2.8.0.2.9.0
+Version: 2.9.0.2.9.0
 Summary: Defining the Future of 3D Machine Vision
 Home-page: https://www.zivid.com
 Author: Zivid AS
 Author-email: customersuccess@zivid.com
 License: BSD 3-Clause
 Description: # Zivid Python
         
@@ -91,14 +91,15 @@
             import zivid
             app = zivid.Application()
             camera = app.connect_camera()
             settings = zivid.Settings(acquisitions=[zivid.Settings.Acquisition()])
             frame = camera.capture(settings)
             xyz = frame.point_cloud().copy_data("xyz") # Get point coordinates as [Height,Width,3] float array
             rgba = frame.point_cloud().copy_data("rgba") # Get point colors as [Height,Width,4] uint8 array
+            bgra = frame.point_cloud().copy_data("bgra") # Get point colors as [Height,Width,4] uint8 array
         
         ### Capture Assistant
         
         Instead of manually adjusting settings, the Capture Assistant may be used to find the optimal settings for your scene:
         
             import zivid
             app = zivid.Application()
@@ -171,23 +172,23 @@
         
         Please visit [Zivid Knowledge Base][zivid-knowledge-base-url] for general information on using Zivid 3D cameras. If you cannot find a solution to your issue, please contact customersuccess@zivid.com.
         
         ## Test matrix
         
         | Operating System | Python version            |
         | :--------------- | :------------------------ |
+        | Ubuntu 23.04     | 3.11                      |
+        | Ubuntu 22.10     | 3.10                      |
         | Ubuntu 22.04     | 3.10                      |
         | Ubuntu 20.04     | 3.8                       |
         | Ubuntu 18.04     | 3.6                       |
-        | Fedora 30        | 3.7                       |
-        | Fedora 33        | 3.9                       |
-        | Fedora 34        | 3.9                       |
+        | Fedora 37        | 3.11                      |
+        | Fedora 36        | 3.10                      |
         | Fedora 35        | 3.10                      |
         | Windows 10       | 3.7, 3.8, 3.9, 3.10, 3.11 |
-        | Arch Linux       | latest                    |
         
         [header-image]: https://www.zivid.com/hubfs/softwarefiles/images/zivid-generic-github-header.png
         [ci-badge]: https://img.shields.io/github/actions/workflow/status/zivid/zivid-python/main.yml?branch=master
         [ci-url]: https://github.com/zivid/zivid-python/actions?query=workflow%3A%22Main+CI+workflow%22+branch%3Amaster
         [pypi-badge]: https://img.shields.io/pypi/v/zivid.svg
         [pypi-url]: https://pypi.org/project/zivid
```

### Comparing `zivid-2.8.0.2.9.0/README.md` & `zivid-2.9.0.2.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     import zivid
     app = zivid.Application()
     camera = app.connect_camera()
     settings = zivid.Settings(acquisitions=[zivid.Settings.Acquisition()])
     frame = camera.capture(settings)
     xyz = frame.point_cloud().copy_data("xyz") # Get point coordinates as [Height,Width,3] float array
     rgba = frame.point_cloud().copy_data("rgba") # Get point colors as [Height,Width,4] uint8 array
+    bgra = frame.point_cloud().copy_data("bgra") # Get point colors as [Height,Width,4] uint8 array
 
 ### Capture Assistant
 
 Instead of manually adjusting settings, the Capture Assistant may be used to find the optimal settings for your scene:
 
     import zivid
     app = zivid.Application()
@@ -163,23 +164,23 @@
 
 Please visit [Zivid Knowledge Base][zivid-knowledge-base-url] for general information on using Zivid 3D cameras. If you cannot find a solution to your issue, please contact customersuccess@zivid.com.
 
 ## Test matrix
 
 | Operating System | Python version            |
 | :--------------- | :------------------------ |
+| Ubuntu 23.04     | 3.11                      |
+| Ubuntu 22.10     | 3.10                      |
 | Ubuntu 22.04     | 3.10                      |
 | Ubuntu 20.04     | 3.8                       |
 | Ubuntu 18.04     | 3.6                       |
-| Fedora 30        | 3.7                       |
-| Fedora 33        | 3.9                       |
-| Fedora 34        | 3.9                       |
+| Fedora 37        | 3.11                      |
+| Fedora 36        | 3.10                      |
 | Fedora 35        | 3.10                      |
 | Windows 10       | 3.7, 3.8, 3.9, 3.10, 3.11 |
-| Arch Linux       | latest                    |
 
 [header-image]: https://www.zivid.com/hubfs/softwarefiles/images/zivid-generic-github-header.png
 [ci-badge]: https://img.shields.io/github/actions/workflow/status/zivid/zivid-python/main.yml?branch=master
 [ci-url]: https://github.com/zivid/zivid-python/actions?query=workflow%3A%22Main+CI+workflow%22+branch%3Amaster
 [pypi-badge]: https://img.shields.io/pypi/v/zivid.svg
 [pypi-url]: https://pypi.org/project/zivid
```

### Comparing `zivid-2.8.0.2.9.0/modules/_zivid/__init__.py` & `zivid-2.9.0.2.9.0/modules/_zivid/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,19 @@
     ctypes.WinDLL(str(pyd_files[0]), winmode=0)
 
 try:
     from _zivid._zivid import (  # pylint: disable=import-error,no-name-in-module
         __version__,
         Application,
         Array2DColorRGBA,
+        Array2DColorBGRA,
         Array2DNormalXYZ,
         Array2DPointXYZ,
         Array2DPointXYZColorRGBA,
+        Array2DPointXYZColorBGRA,
         Array2DPointXYZW,
         Array2DPointZ,
         Array2DSNR,
         Camera,
         CameraIntrinsics,
         CameraState,
         firmware,
@@ -52,14 +54,15 @@
         FrameInfo,
         PointCloud,
         Settings,
         version,
         Settings2D,
         Frame2D,
         ImageRGBA,
+        ImageBGRA,
         CameraInfo,
         infield_correction,
         Matrix4x4,
         data_model,
     )
 except ImportError as ex:
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/__init__.py` & `zivid-2.9.0.2.9.0/modules/zivid/__init__.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/_calibration/detector.py` & `zivid-2.9.0.2.9.0/modules/zivid/_calibration/detector.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/_calibration/hand_eye.py` & `zivid-2.9.0.2.9.0/modules/zivid/_calibration/hand_eye.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/_calibration/multi_camera.py` & `zivid-2.9.0.2.9.0/modules/zivid/_calibration/multi_camera.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/_calibration/pose.py` & `zivid-2.9.0.2.9.0/modules/zivid/_calibration/pose.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/_suggest_settings_parameters.py` & `zivid-2.9.0.2.9.0/modules/zivid/_suggest_settings_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # pylint: disable=too-many-lines,protected-access,too-few-public-methods,too-many-arguments,line-too-long,missing-function-docstring,missing-class-docstring,redefined-builtin,too-many-branches,too-many-boolean-expressions
 import datetime
 import _zivid
 
 
 class SuggestSettingsParameters:
     class AmbientLightFrequency:
-
         hz50 = "hz50"
         hz60 = "hz60"
         none = "none"
 
         _valid_values = {
             "hz50": _zivid.capture_assistant.SuggestSettingsParameters.AmbientLightFrequency.hz50,
             "hz60": _zivid.capture_assistant.SuggestSettingsParameters.AmbientLightFrequency.hz60,
@@ -22,15 +21,14 @@
             return list(cls._valid_values.keys())
 
     def __init__(
         self,
         ambient_light_frequency=_zivid.capture_assistant.SuggestSettingsParameters.AmbientLightFrequency().value,
         max_capture_time=_zivid.capture_assistant.SuggestSettingsParameters.MaxCaptureTime().value,
     ):
-
         if isinstance(
             ambient_light_frequency,
             _zivid.capture_assistant.SuggestSettingsParameters.AmbientLightFrequency.enum,
         ):
             self._ambient_light_frequency = _zivid.capture_assistant.SuggestSettingsParameters.AmbientLightFrequency(
                 ambient_light_frequency
             )
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/application.py` & `zivid-2.9.0.2.9.0/modules/zivid/application.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/camera.py` & `zivid-2.9.0.2.9.0/modules/zivid/camera.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/camera_info.py` & `zivid-2.9.0.2.9.0/modules/zivid/camera_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 class CameraInfo:
     class Revision:
         def __init__(
             self,
             major=_zivid.CameraInfo.Revision.Major().value,
             minor=_zivid.CameraInfo.Revision.Minor().value,
         ):
-
             if isinstance(major, (int,)):
                 self._major = _zivid.CameraInfo.Revision.Major(major)
             else:
                 raise TypeError(
                     "Unsupported type, expected: (int,), got {value_type}".format(
                         value_type=type(major)
                     )
@@ -68,15 +67,14 @@
             return str(_to_internal_camera_info_revision(self))
 
     class UserData:
         def __init__(
             self,
             max_size_bytes=_zivid.CameraInfo.UserData.MaxSizeBytes().value,
         ):
-
             if isinstance(max_size_bytes, (int,)):
                 self._max_size_bytes = _zivid.CameraInfo.UserData.MaxSizeBytes(
                     max_size_bytes
                 )
             else:
                 raise TypeError(
                     "Unsupported type, expected: (int,), got {value_type}".format(
@@ -104,15 +102,14 @@
                 return True
             return False
 
         def __str__(self):
             return str(_to_internal_camera_info_user_data(self))
 
     class Model:
-
         zividOnePlusLarge = "zividOnePlusLarge"
         zividOnePlusMedium = "zividOnePlusMedium"
         zividOnePlusSmall = "zividOnePlusSmall"
         zividTwo = "zividTwo"
         zividTwoL100 = "zividTwoL100"
 
         _valid_values = {
@@ -132,15 +129,14 @@
         firmware_version=_zivid.CameraInfo.FirmwareVersion().value,
         model=_zivid.CameraInfo.Model().value,
         model_name=_zivid.CameraInfo.ModelName().value,
         serial_number=_zivid.CameraInfo.SerialNumber().value,
         revision=None,
         user_data=None,
     ):
-
         if isinstance(firmware_version, (str,)):
             self._firmware_version = _zivid.CameraInfo.FirmwareVersion(firmware_version)
         else:
             raise TypeError(
                 "Unsupported type, expected: (str,), got {value_type}".format(
                     value_type=type(firmware_version)
                 )
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/camera_intrinsics.py` & `zivid-2.9.0.2.9.0/modules/zivid/camera_intrinsics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         def __init__(
             self,
             cx=_zivid.CameraIntrinsics.CameraMatrix.CX().value,
             cy=_zivid.CameraIntrinsics.CameraMatrix.CY().value,
             fx=_zivid.CameraIntrinsics.CameraMatrix.FX().value,
             fy=_zivid.CameraIntrinsics.CameraMatrix.FY().value,
         ):
-
             if isinstance(
                 cx,
                 (
                     float,
                     int,
                 ),
             ):
@@ -175,15 +174,14 @@
             self,
             k1=_zivid.CameraIntrinsics.Distortion.K1().value,
             k2=_zivid.CameraIntrinsics.Distortion.K2().value,
             k3=_zivid.CameraIntrinsics.Distortion.K3().value,
             p1=_zivid.CameraIntrinsics.Distortion.P1().value,
             p2=_zivid.CameraIntrinsics.Distortion.P2().value,
         ):
-
             if isinstance(
                 k1,
                 (
                     float,
                     int,
                 ),
             ):
@@ -375,15 +373,14 @@
             return str(_to_internal_camera_intrinsics_distortion(self))
 
     def __init__(
         self,
         camera_matrix=None,
         distortion=None,
     ):
-
         if camera_matrix is None:
             camera_matrix = self.CameraMatrix()
         if not isinstance(camera_matrix, self.CameraMatrix):
             raise TypeError(
                 "Unsupported type: {value}".format(value=type(camera_matrix))
             )
         self._camera_matrix = camera_matrix
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/camera_state.py` & `zivid-2.9.0.2.9.0/modules/zivid/camera_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
             self,
             dmd=_zivid.CameraState.Temperature.DMD().value,
             general=_zivid.CameraState.Temperature.General().value,
             led=_zivid.CameraState.Temperature.LED().value,
             lens=_zivid.CameraState.Temperature.Lens().value,
             pcb=_zivid.CameraState.Temperature.PCB().value,
         ):
-
             if isinstance(
                 dmd,
                 (
                     float,
                     int,
                 ),
             ):
@@ -210,15 +209,14 @@
 
     def __init__(
         self,
         available=_zivid.CameraState.Available().value,
         connected=_zivid.CameraState.Connected().value,
         temperature=None,
     ):
-
         if isinstance(available, (bool,)):
             self._available = _zivid.CameraState.Available(available)
         else:
             raise TypeError(
                 "Unsupported type, expected: (bool,), got {value_type}".format(
                     value_type=type(available)
                 )
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/capture_assistant.py` & `zivid-2.9.0.2.9.0/modules/zivid/capture_assistant.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/experimental/calibration.py` & `zivid-2.9.0.2.9.0/modules/zivid/experimental/calibration.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/firmware.py` & `zivid-2.9.0.2.9.0/modules/zivid/firmware.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/frame.py` & `zivid-2.9.0.2.9.0/modules/zivid/frame.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/frame_2d.py` & `zivid-2.9.0.2.9.0/modules/zivid/frame_2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains the Frame class."""
 import _zivid
 from zivid.settings_2d import _to_settings2d
+from zivid.camera_info import _to_camera_info
 from zivid.camera_state import _to_camera_state
 from zivid.frame_info import _to_frame_info
 from zivid.image import Image
 
 
 class Frame2D:
     """A 2D frame captured by a Zivid camera.
@@ -39,14 +40,22 @@
         """Get color (RGBA) image from the frame.
 
         Returns:
             An image instance containing RGBA data
         """
         return Image(self.__impl.image_rgba())
 
+    def image_bgra(self):
+        """Get color (BGRA) image from the frame.
+
+        Returns:
+            An image instance containing BGRA data
+        """
+        return Image(self.__impl.image_bgra())
+
     @property
     def settings(self):
         """Get the settings used to capture this frame.
 
         Returns:
             A Settings2D instance
         """
@@ -66,14 +75,23 @@
         """Get information collected at the time of the capture.
 
         Returns:
             A FrameInfo instance
         """
         return _to_frame_info(self.__impl.info)
 
+    @property
+    def camera_info(self):
+        """Get information about the camera used to capture the frame.
+
+        Returns:
+            A CameraInfo instance
+        """
+        return _to_camera_info(self.__impl.camera_info)
+
     def release(self):
         """Release the underlying resources."""
         try:
             impl = self.__impl
         except AttributeError:
             pass
         else:
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/frame_info.py` & `zivid-2.9.0.2.9.0/modules/zivid/frame_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 class FrameInfo:
     class SoftwareVersion:
         def __init__(
             self,
             core=_zivid.FrameInfo.SoftwareVersion.Core().value,
         ):
-
             if isinstance(core, (str,)):
                 self._core = _zivid.FrameInfo.SoftwareVersion.Core(core)
             else:
                 raise TypeError(
                     "Unsupported type, expected: (str,), got {value_type}".format(
                         value_type=type(core)
                     )
@@ -45,15 +44,14 @@
 
     class SystemInfo:
         class CPU:
             def __init__(
                 self,
                 model=_zivid.FrameInfo.SystemInfo.CPU.Model().value,
             ):
-
                 if isinstance(model, (str,)):
                     self._model = _zivid.FrameInfo.SystemInfo.CPU.Model(model)
                 else:
                     raise TypeError(
                         "Unsupported type, expected: (str,), got {value_type}".format(
                             value_type=type(model)
                         )
@@ -84,15 +82,14 @@
 
         class ComputeDevice:
             def __init__(
                 self,
                 model=_zivid.FrameInfo.SystemInfo.ComputeDevice.Model().value,
                 vendor=_zivid.FrameInfo.SystemInfo.ComputeDevice.Vendor().value,
             ):
-
                 if isinstance(model, (str,)):
                     self._model = _zivid.FrameInfo.SystemInfo.ComputeDevice.Model(model)
                 else:
                     raise TypeError(
                         "Unsupported type, expected: (str,), got {value_type}".format(
                             value_type=type(model)
                         )
@@ -151,15 +148,14 @@
 
         def __init__(
             self,
             operating_system=_zivid.FrameInfo.SystemInfo.OperatingSystem().value,
             cpu=None,
             compute_device=None,
         ):
-
             if isinstance(operating_system, (str,)):
                 self._operating_system = _zivid.FrameInfo.SystemInfo.OperatingSystem(
                     operating_system
                 )
             else:
                 raise TypeError(
                     "Unsupported type, expected: (str,), got {value_type}".format(
@@ -232,15 +228,14 @@
 
     def __init__(
         self,
         time_stamp=_zivid.FrameInfo.TimeStamp().value,
         software_version=None,
         system_info=None,
     ):
-
         if isinstance(time_stamp, (datetime.datetime,)):
             self._time_stamp = _zivid.FrameInfo.TimeStamp(time_stamp)
         else:
             raise TypeError(
                 "Unsupported type, expected: (datetime.datetime,), got {value_type}".format(
                     value_type=type(time_stamp)
                 )
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/image.py` & `zivid-2.9.0.2.9.0/modules/zivid/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
         Args:
             impl:   Reference to internal/back-end instance.
 
         Raises:
             TypeError: If argument does not match the expected internal class.
         """
-        if not isinstance(impl, _zivid.ImageRGBA):
+        if not isinstance(impl, (_zivid.ImageRGBA, _zivid.ImageBGRA)):
             raise TypeError(
-                "Unsupported type for argument impl. Got {}, expected {}".format(
-                    type(impl), type(_zivid.ImageRGBA)
+                "Unsupported type for argument impl. Got {}, expected {} or {}".format(
+                    type(impl), type(_zivid.ImageRGBA), type(_zivid.ImageBGRA)
                 )
             )
         self.__impl = impl
 
     @property
     def height(self):
         """Get the height of the image (number of rows).
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/matrix4x4.py` & `zivid-2.9.0.2.9.0/modules/zivid/matrix4x4.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/point_cloud.py` & `zivid-2.9.0.2.9.0/modules/zivid/point_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,19 @@
         """Copy point cloud data from GPU to numpy array.
 
         Supported data formats:
         xyz:        ndarray(Height,Width,3) of float
         xyzw:       ndarray(Height,Width,4) of float
         z:          ndarray(Height,Width)   of float
         rgba:       ndarray(Height,Width,4) of uint8
+        bgra:       ndarray(Height,Width,4) of uint8
         normals:    ndarray(Height,Width,3) of float
         snr:        ndarray(Height,Width)   of float
         xyzrgba:    ndarray(Height,Width)   of composite dtype (accessed with e.g. arr["x"])
+        xyzbgra:    ndarray(Height,Width)   of composite dtype (accessed with e.g. arr["x"])
 
         Args:
             data_format: A string specifying the data to be copied
 
         Returns:
             A numpy array with the requested data.
 
@@ -77,17 +79,19 @@
         self.__impl.assert_not_released()
 
         data_formats = {
             "xyz": _zivid.Array2DPointXYZ,
             "xyzw": _zivid.Array2DPointXYZW,
             "z": _zivid.Array2DPointZ,
             "rgba": _zivid.Array2DColorRGBA,
+            "bgra": _zivid.Array2DColorBGRA,
             "normals": _zivid.Array2DNormalXYZ,
             "snr": _zivid.Array2DSNR,
             "xyzrgba": _zivid.Array2DPointXYZColorRGBA,
+            "xyzbgra": _zivid.Array2DPointXYZColorBGRA,
         }
         try:
             data_format_class = data_formats[data_format]
         except KeyError as ex:
             raise ValueError(
                 "Unsupported data format: {data_format}. Supported formats: {all_formats}".format(
                     data_format=data_format, all_formats=list(data_formats.keys())
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/settings.py` & `zivid-2.9.0.2.9.0/modules/zivid/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         def __init__(
             self,
             aperture=_zivid.Settings.Acquisition.Aperture().value,
             brightness=_zivid.Settings.Acquisition.Brightness().value,
             exposure_time=_zivid.Settings.Acquisition.ExposureTime().value,
             gain=_zivid.Settings.Acquisition.Gain().value,
         ):
-
             if (
                 isinstance(
                     aperture,
                     (
                         float,
                         int,
                     ),
@@ -184,15 +183,14 @@
             return str(_to_internal_settings_acquisition(self))
 
     class Diagnostics:
         def __init__(
             self,
             enabled=_zivid.Settings.Diagnostics.Enabled().value,
         ):
-
             if isinstance(enabled, (bool,)) or enabled is None:
                 self._enabled = _zivid.Settings.Diagnostics.Enabled(enabled)
             else:
                 raise TypeError(
                     "Unsupported type, expected: (bool,) or None, got {value_type}".format(
                         value_type=type(enabled)
                     )
@@ -219,15 +217,14 @@
             return False
 
         def __str__(self):
             return str(_to_internal_settings_diagnostics(self))
 
     class Experimental:
         class Engine:
-
             phase = "phase"
             stripe = "stripe"
 
             _valid_values = {
                 "phase": _zivid.Settings.Experimental.Engine.phase,
                 "stripe": _zivid.Settings.Experimental.Engine.stripe,
             }
@@ -236,15 +233,14 @@
             def valid_values(cls):
                 return list(cls._valid_values.keys())
 
         def __init__(
             self,
             engine=_zivid.Settings.Experimental.Engine().value,
         ):
-
             if (
                 isinstance(engine, _zivid.Settings.Experimental.Engine.enum)
                 or engine is None
             ):
                 self._engine = _zivid.Settings.Experimental.Engine(engine)
             elif isinstance(engine, str):
                 self._engine = _zivid.Settings.Experimental.Engine(
@@ -297,15 +293,14 @@
             class Balance:
                 def __init__(
                     self,
                     blue=_zivid.Settings.Processing.Color.Balance.Blue().value,
                     green=_zivid.Settings.Processing.Color.Balance.Green().value,
                     red=_zivid.Settings.Processing.Color.Balance.Red().value,
                 ):
-
                     if (
                         isinstance(
                             blue,
                             (
                                 float,
                                 int,
                             ),
@@ -444,15 +439,14 @@
                     return False
 
                 def __str__(self):
                     return str(_to_internal_settings_processing_color_balance(self))
 
             class Experimental:
                 class Mode:
-
                     automatic = "automatic"
                     toneMapping = "toneMapping"
                     useFirstAcquisition = "useFirstAcquisition"
 
                     _valid_values = {
                         "automatic": _zivid.Settings.Processing.Color.Experimental.Mode.automatic,
                         "toneMapping": _zivid.Settings.Processing.Color.Experimental.Mode.toneMapping,
@@ -463,15 +457,14 @@
                     def valid_values(cls):
                         return list(cls._valid_values.keys())
 
                 def __init__(
                     self,
                     mode=_zivid.Settings.Processing.Color.Experimental.Mode().value,
                 ):
-
                     if (
                         isinstance(
                             mode,
                             _zivid.Settings.Processing.Color.Experimental.Mode.enum,
                         )
                         or mode is None
                     ):
@@ -535,15 +528,14 @@
 
             def __init__(
                 self,
                 gamma=_zivid.Settings.Processing.Color.Gamma().value,
                 balance=None,
                 experimental=None,
             ):
-
                 if (
                     isinstance(
                         gamma,
                         (
                             float,
                             int,
                         ),
@@ -639,15 +631,14 @@
                 class Removal:
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Cluster.Removal.Enabled().value,
                         max_neighbor_distance=_zivid.Settings.Processing.Filters.Cluster.Removal.MaxNeighborDistance().value,
                         min_area=_zivid.Settings.Processing.Filters.Cluster.Removal.MinArea().value,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Cluster.Removal.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -781,15 +772,14 @@
                             )
                         )
 
                 def __init__(
                     self,
                     removal=None,
                 ):
-
                     if removal is None:
                         removal = self.Removal()
                     if not isinstance(removal, self.Removal):
                         raise TypeError(
                             "Unsupported type: {value}".format(value=type(removal))
                         )
                     self._removal = removal
@@ -818,15 +808,14 @@
                 class ContrastDistortion:
                     class Correction:
                         def __init__(
                             self,
                             enabled=_zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Correction.Enabled().value,
                             strength=_zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Correction.Strength().value,
                         ):
-
                             if isinstance(enabled, (bool,)) or enabled is None:
                                 self._enabled = _zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Correction.Enabled(
                                     enabled
                                 )
                             else:
                                 raise TypeError(
                                     "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -914,15 +903,14 @@
 
                     class Removal:
                         def __init__(
                             self,
                             enabled=_zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Removal.Enabled().value,
                             threshold=_zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Removal.Threshold().value,
                         ):
-
                             if isinstance(enabled, (bool,)) or enabled is None:
                                 self._enabled = _zivid.Settings.Processing.Filters.Experimental.ContrastDistortion.Removal.Enabled(
                                     enabled
                                 )
                             else:
                                 raise TypeError(
                                     "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1009,15 +997,14 @@
                             )
 
                     def __init__(
                         self,
                         correction=None,
                         removal=None,
                     ):
-
                         if correction is None:
                             correction = self.Correction()
                         if not isinstance(correction, self.Correction):
                             raise TypeError(
                                 "Unsupported type: {value}".format(
                                     value=type(correction)
                                 )
@@ -1074,15 +1061,14 @@
                 class HoleFilling:
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Experimental.HoleFilling.Enabled().value,
                         hole_size=_zivid.Settings.Processing.Filters.Experimental.HoleFilling.HoleSize().value,
                         strictness=_zivid.Settings.Processing.Filters.Experimental.HoleFilling.Strictness().value,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Experimental.HoleFilling.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1198,15 +1184,14 @@
                         )
 
                 def __init__(
                     self,
                     contrast_distortion=None,
                     hole_filling=None,
                 ):
-
                     if contrast_distortion is None:
                         contrast_distortion = self.ContrastDistortion()
                     if not isinstance(contrast_distortion, self.ContrastDistortion):
                         raise TypeError(
                             "Unsupported type: {value}".format(
                                 value=type(contrast_distortion)
                             )
@@ -1261,15 +1246,14 @@
             class Noise:
                 class Removal:
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Noise.Removal.Enabled().value,
                         threshold=_zivid.Settings.Processing.Filters.Noise.Removal.Threshold().value,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Noise.Removal.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1353,15 +1337,14 @@
                             _to_internal_settings_processing_filters_noise_removal(self)
                         )
 
                 def __init__(
                     self,
                     removal=None,
                 ):
-
                     if removal is None:
                         removal = self.Removal()
                     if not isinstance(removal, self.Removal):
                         raise TypeError(
                             "Unsupported type: {value}".format(value=type(removal))
                         )
                     self._removal = removal
@@ -1389,15 +1372,14 @@
             class Outlier:
                 class Removal:
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Outlier.Removal.Enabled().value,
                         threshold=_zivid.Settings.Processing.Filters.Outlier.Removal.Threshold().value,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Outlier.Removal.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1483,15 +1465,14 @@
                             )
                         )
 
                 def __init__(
                     self,
                     removal=None,
                 ):
-
                     if removal is None:
                         removal = self.Removal()
                     if not isinstance(removal, self.Removal):
                         raise TypeError(
                             "Unsupported type: {value}".format(value=type(removal))
                         )
                     self._removal = removal
@@ -1516,15 +1497,14 @@
                 def __str__(self):
                     return str(_to_internal_settings_processing_filters_outlier(self))
 
             class Reflection:
                 class Removal:
                     class Experimental:
                         class Mode:
-
                             global_ = "global"
                             local = "local"
 
                             _valid_values = {
                                 "global": _zivid.Settings.Processing.Filters.Reflection.Removal.Experimental.Mode.global_,
                                 "local": _zivid.Settings.Processing.Filters.Reflection.Removal.Experimental.Mode.local,
                             }
@@ -1533,15 +1513,14 @@
                             def valid_values(cls):
                                 return list(cls._valid_values.keys())
 
                         def __init__(
                             self,
                             mode=_zivid.Settings.Processing.Filters.Reflection.Removal.Experimental.Mode().value,
                         ):
-
                             if (
                                 isinstance(
                                     mode,
                                     _zivid.Settings.Processing.Filters.Reflection.Removal.Experimental.Mode.enum,
                                 )
                                 or mode is None
                             ):
@@ -1606,15 +1585,14 @@
                             )
 
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Reflection.Removal.Enabled().value,
                         experimental=None,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Reflection.Removal.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1676,15 +1654,14 @@
                             )
                         )
 
                 def __init__(
                     self,
                     removal=None,
                 ):
-
                     if removal is None:
                         removal = self.Removal()
                     if not isinstance(removal, self.Removal):
                         raise TypeError(
                             "Unsupported type: {value}".format(value=type(removal))
                         )
                     self._removal = removal
@@ -1714,15 +1691,14 @@
             class Smoothing:
                 class Gaussian:
                     def __init__(
                         self,
                         enabled=_zivid.Settings.Processing.Filters.Smoothing.Gaussian.Enabled().value,
                         sigma=_zivid.Settings.Processing.Filters.Smoothing.Gaussian.Sigma().value,
                     ):
-
                         if isinstance(enabled, (bool,)) or enabled is None:
                             self._enabled = _zivid.Settings.Processing.Filters.Smoothing.Gaussian.Enabled(
                                 enabled
                             )
                         else:
                             raise TypeError(
                                 "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -1808,15 +1784,14 @@
                             )
                         )
 
                 def __init__(
                     self,
                     gaussian=None,
                 ):
-
                     if gaussian is None:
                         gaussian = self.Gaussian()
                     if not isinstance(gaussian, self.Gaussian):
                         raise TypeError(
                             "Unsupported type: {value}".format(value=type(gaussian))
                         )
                     self._gaussian = gaussian
@@ -1846,15 +1821,14 @@
                 cluster=None,
                 experimental=None,
                 noise=None,
                 outlier=None,
                 reflection=None,
                 smoothing=None,
             ):
-
                 if cluster is None:
                     cluster = self.Cluster()
                 if not isinstance(cluster, self.Cluster):
                     raise TypeError(
                         "Unsupported type: {value}".format(value=type(cluster))
                     )
                 self._cluster = cluster
@@ -1987,15 +1961,14 @@
                 return str(_to_internal_settings_processing_filters(self))
 
         def __init__(
             self,
             color=None,
             filters=None,
         ):
-
             if color is None:
                 color = self.Color()
             if not isinstance(color, self.Color):
                 raise TypeError("Unsupported type: {value}".format(value=type(color)))
             self._color = color
 
             if filters is None:
@@ -2038,15 +2011,14 @@
                 self,
                 enabled=_zivid.Settings.RegionOfInterest.Box.Enabled().value,
                 extents=_zivid.Settings.RegionOfInterest.Box.Extents().value,
                 point_a=_zivid.Settings.RegionOfInterest.Box.PointA().value,
                 point_b=_zivid.Settings.RegionOfInterest.Box.PointB().value,
                 point_o=_zivid.Settings.RegionOfInterest.Box.PointO().value,
             ):
-
                 if isinstance(enabled, (bool,)) or enabled is None:
                     self._enabled = _zivid.Settings.RegionOfInterest.Box.Enabled(
                         enabled
                     )
                 else:
                     raise TypeError(
                         "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -2231,15 +2203,14 @@
 
         class Depth:
             def __init__(
                 self,
                 enabled=_zivid.Settings.RegionOfInterest.Depth.Enabled().value,
                 range=_zivid.Settings.RegionOfInterest.Depth.Range().value,
             ):
-
                 if isinstance(enabled, (bool,)) or enabled is None:
                     self._enabled = _zivid.Settings.RegionOfInterest.Depth.Enabled(
                         enabled
                     )
                 else:
                     raise TypeError(
                         "Unsupported type, expected: (bool,) or None, got {value_type}".format(
@@ -2309,15 +2280,14 @@
                 return str(_to_internal_settings_region_of_interest_depth(self))
 
         def __init__(
             self,
             box=None,
             depth=None,
         ):
-
             if box is None:
                 box = self.Box()
             if not isinstance(box, self.Box):
                 raise TypeError("Unsupported type: {value}".format(value=type(box)))
             self._box = box
 
             if depth is None:
@@ -2358,15 +2328,14 @@
         self,
         acquisitions=None,
         diagnostics=None,
         experimental=None,
         processing=None,
         region_of_interest=None,
     ):
-
         if acquisitions is None:
             self._acquisitions = []
         elif isinstance(acquisitions, (collections.abc.Iterable,)):
             self._acquisitions = []
             for item in acquisitions:
                 if isinstance(item, self.Acquisition):
                     self._acquisitions.append(item)
```

### Comparing `zivid-2.8.0.2.9.0/modules/zivid/settings_2d.py` & `zivid-2.9.0.2.9.0/modules/zivid/settings_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         def __init__(
             self,
             aperture=_zivid.Settings2D.Acquisition.Aperture().value,
             brightness=_zivid.Settings2D.Acquisition.Brightness().value,
             exposure_time=_zivid.Settings2D.Acquisition.ExposureTime().value,
             gain=_zivid.Settings2D.Acquisition.Gain().value,
         ):
-
             if (
                 isinstance(
                     aperture,
                     (
                         float,
                         int,
                     ),
@@ -188,15 +187,14 @@
             class Balance:
                 def __init__(
                     self,
                     blue=_zivid.Settings2D.Processing.Color.Balance.Blue().value,
                     green=_zivid.Settings2D.Processing.Color.Balance.Green().value,
                     red=_zivid.Settings2D.Processing.Color.Balance.Red().value,
                 ):
-
                     if (
                         isinstance(
                             blue,
                             (
                                 float,
                                 int,
                             ),
@@ -342,15 +340,14 @@
                     return str(_to_internal_settings2d_processing_color_balance(self))
 
             def __init__(
                 self,
                 gamma=_zivid.Settings2D.Processing.Color.Gamma().value,
                 balance=None,
             ):
-
                 if (
                     isinstance(
                         gamma,
                         (
                             float,
                             int,
                         ),
@@ -417,15 +414,14 @@
             def __str__(self):
                 return str(_to_internal_settings2d_processing_color(self))
 
         def __init__(
             self,
             color=None,
         ):
-
             if color is None:
                 color = self.Color()
             if not isinstance(color, self.Color):
                 raise TypeError("Unsupported type: {value}".format(value=type(color)))
             self._color = color
 
         @property
@@ -447,15 +443,14 @@
             return str(_to_internal_settings2d_processing(self))
 
     def __init__(
         self,
         acquisitions=None,
         processing=None,
     ):
-
         if acquisitions is None:
             self._acquisitions = []
         elif isinstance(acquisitions, (collections.abc.Iterable,)):
             self._acquisitions = []
             for item in acquisitions:
                 if isinstance(item, self.Acquisition):
                     self._acquisitions.append(item)
```

### Comparing `zivid-2.8.0.2.9.0/setup.py` & `zivid-2.9.0.2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import platform
 import subprocess
 from sys import version_info
 from pathlib import Path
 from pkgutil import iter_modules
 from skbuild import setup
 
+
 # To be replaced by: from setuptools_scm import get_version
 def get_version():
-    return "2.8.0"
+    return "2.9.0"
 
 
 def _zivid_sdk_version():
     return "2.9.0"
 
 
 def _zivid_python_version():
@@ -35,15 +36,15 @@
 
 
 def _python_version():
     return "{}.{}.{}".format(*version_info)
 
 
 def _make_message_box(*message):
-    width = max([len(e) for e in message])
+    width = max(len(e) for e in message)
 
     box_bar = "+-" + "-" * width + "-+"
     empty_line = "\n| " + " " * width + " |\n"
     message_lines = ["| " + line + " " * (width - len(line)) + " |" for line in message]
 
     return (
         "\n\n" + box_bar + "\n" + empty_line.join(message_lines) + "\n" + box_bar + "\n"
```

### Comparing `zivid-2.8.0.2.9.0/src/CMakeLists.txt` & `zivid-2.9.0.2.9.0/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Calibration/Calibration.cpp` & `zivid-2.9.0.2.9.0/src/Calibration/Calibration.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Calibration/Detector.cpp` & `zivid-2.9.0.2.9.0/src/Calibration/Detector.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Calibration/HandEye.cpp` & `zivid-2.9.0.2.9.0/src/Calibration/HandEye.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Calibration/MultiCamera.cpp` & `zivid-2.9.0.2.9.0/src/Calibration/MultiCamera.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Calibration/Pose.cpp` & `zivid-2.9.0.2.9.0/src/Calibration/Pose.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/CaptureAssistant.cpp` & `zivid-2.9.0.2.9.0/src/CaptureAssistant.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/DataModel.cpp` & `zivid-2.9.0.2.9.0/src/DataModel.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Firmware.cpp` & `zivid-2.9.0.2.9.0/src/Firmware.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/InfieldCorrection/InfieldCorrection.cpp` & `zivid-2.9.0.2.9.0/src/InfieldCorrection/InfieldCorrection.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Matrix4x4.cpp` & `zivid-2.9.0.2.9.0/src/Matrix4x4.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/ReleasableArray2D.cpp` & `zivid-2.9.0.2.9.0/src/ReleasableArray2D.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 {
 #pragma pack(push)
     struct PointXYZColorRGBA
     {
         float x, y, z;
         uint8_t r, g, b, a;
     };
+
+    struct PointXYZColorBGRA
+    {
+        float x, y, z;
+        uint8_t b, g, r, a;
+    };
 #pragma pack(pop)
 
     template<typename NativeType, typename WrapperType, size_t depth>
     py::buffer_info pointCloudDataBuffer(ZividPython::ReleasableArray2D<NativeType> &arrayWrapper)
     {
         static_assert(depth > 0, "Depth of array must be one or higher");
         static_assert(sizeof(WrapperType) * depth == sizeof(NativeType), "Unexpected data format");
@@ -67,14 +73,27 @@
         static_assert(std::is_same_v<WrapperType, decltype(NativeType::b)>);
         static_assert(std::is_same_v<WrapperType, decltype(NativeType::a)>);
 
         pyClass.def(py::init<>(&pointCloudDataCopier<NativeType>))
             .def_buffer(pointCloudDataBuffer<NativeType, WrapperType, 4>);
     }
 
+    void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::ColorBGRA>> pyClass)
+    {
+        using WrapperType = uint8_t;
+        using NativeType = Zivid::ColorBGRA;
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::b)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::g)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::r)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::a)>);
+
+        pyClass.def(py::init<>(&pointCloudDataCopier<NativeType>))
+            .def_buffer(pointCloudDataBuffer<NativeType, WrapperType, 4>);
+    }
+
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::NormalXYZ>> pyClass)
     {
         using WrapperType = float;
         using NativeType = Zivid::NormalXYZ;
         static_assert(std::is_same_v<WrapperType, decltype(NativeType::x)>);
         static_assert(std::is_same_v<WrapperType, decltype(NativeType::y)>);
         static_assert(std::is_same_v<WrapperType, decltype(NativeType::z)>);
@@ -143,8 +162,37 @@
         static_assert(offsetof(NativeColor, b) == offsetof(WrapperType, b) - offsetof(WrapperType, r));
         static_assert(offsetof(NativeColor, a) == offsetof(WrapperType, a) - offsetof(WrapperType, r));
 
         PYBIND11_NUMPY_DTYPE(WrapperType, x, y, z, r, g, b, a);
         pyClass.def(py::init<>(&pointCloudDataCopier<NativeType>))
             .def_buffer(pointCloudDataBuffer<NativeType, WrapperType, 1>);
     }
+
+    void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointXYZColorBGRA>> pyClass)
+    {
+        using WrapperType = PointXYZColorBGRA;
+        using NativeType = Zivid::PointXYZColorBGRA;
+        using NativePoint = decltype(NativeType::point);
+        using NativeColor = decltype(NativeType::color);
+        static_assert(std::is_same_v<decltype(WrapperType::x), decltype(NativePoint::x)>);
+        static_assert(std::is_same_v<decltype(WrapperType::y), decltype(NativePoint::y)>);
+        static_assert(std::is_same_v<decltype(WrapperType::z), decltype(NativePoint::z)>);
+        static_assert(std::is_same_v<decltype(WrapperType::b), decltype(NativeColor::b)>);
+        static_assert(std::is_same_v<decltype(WrapperType::g), decltype(NativeColor::g)>);
+        static_assert(std::is_same_v<decltype(WrapperType::r), decltype(NativeColor::r)>);
+        static_assert(std::is_same_v<decltype(WrapperType::a), decltype(NativeColor::a)>);
+        // Additional layout checks for composite types
+        static_assert(offsetof(NativeType, point) == offsetof(WrapperType, x));
+        static_assert(offsetof(NativeType, color) == offsetof(WrapperType, b));
+        static_assert(offsetof(NativePoint, x) == offsetof(WrapperType, x));
+        static_assert(offsetof(NativePoint, y) == offsetof(WrapperType, y));
+        static_assert(offsetof(NativePoint, z) == offsetof(WrapperType, z));
+        static_assert(offsetof(NativeColor, b) == 0);
+        static_assert(offsetof(NativeColor, g) == offsetof(WrapperType, g) - offsetof(WrapperType, b));
+        static_assert(offsetof(NativeColor, r) == offsetof(WrapperType, r) - offsetof(WrapperType, b));
+        static_assert(offsetof(NativeColor, a) == offsetof(WrapperType, a) - offsetof(WrapperType, b));
+
+        PYBIND11_NUMPY_DTYPE(WrapperType, x, y, z, b, g, r, a);
+        pyClass.def(py::init<>(&pointCloudDataCopier<NativeType>))
+            .def_buffer(pointCloudDataBuffer<NativeType, WrapperType, 1>);
+    }
 } // namespace ZividPython
```

### Comparing `zivid-2.8.0.2.9.0/src/ReleasableCamera.cpp` & `zivid-2.9.0.2.9.0/src/ReleasableCamera.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/ReleasableFrame.cpp` & `zivid-2.9.0.2.9.0/src/ReleasableFrame.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/ReleasableFrame2D.cpp` & `zivid-2.9.0.2.9.0/src/ReleasableFrame2D.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -7,10 +7,12 @@
 namespace ZividPython
 {
     void wrapClass(pybind11::class_<ReleasableFrame2D> pyClass)
     {
         pyClass.def_property_readonly("settings", &ReleasableFrame2D::settings)
             .def_property_readonly("state", &ReleasableFrame2D::state)
             .def_property_readonly("info", &ReleasableFrame2D::info)
-            .def("image_rgba", &ReleasableFrame2D::imageRGBA);
+            .def_property_readonly("camera_info", &ReleasableFrame2D::cameraInfo)
+            .def("image_rgba", &ReleasableFrame2D::imageRGBA)
+            .def("image_bgra", &ReleasableFrame2D::imageBGRA);
     }
 } // namespace ZividPython
```

### Comparing `zivid-2.8.0.2.9.0/src/ReleasableImage.cpp` & `zivid-2.9.0.2.9.0/src/ReleasableImage.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -28,19 +28,54 @@
         return py::buffer_info{ dataPtr,
                                 dataSize,
                                 py::format_descriptor<WrapperType>::format(),
                                 dim,
                                 { height, width, depth },
                                 { dataSize * width * depth, dataSize * depth, dataSize } };
     }
+
+    py::buffer_info imageBGRADataBuffer(ZividPython::ReleasableImageBGRA &image)
+    {
+        using WrapperType = uint8_t;
+        using NativeType = Zivid::ColorBGRA;
+
+        constexpr py::ssize_t dim = 3;
+        constexpr py::ssize_t depth = 4;
+        constexpr py::ssize_t dataSize = sizeof(WrapperType);
+
+        static_assert(dataSize * depth == sizeof(NativeType));
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::b)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::g)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::r)>);
+        static_assert(std::is_same_v<WrapperType, decltype(NativeType::a)>);
+
+        auto *dataPtr = static_cast<void *>(const_cast<NativeType *>(image.impl().data()));
+        const auto height = static_cast<py::ssize_t>(image.impl().height());
+        const auto width = static_cast<py::ssize_t>(image.impl().width());
+
+        return py::buffer_info{ dataPtr,
+                                dataSize,
+                                py::format_descriptor<WrapperType>::format(),
+                                dim,
+                                { height, width, depth },
+                                { dataSize * width * depth, dataSize * depth, dataSize } };
+    }
 } // namespace
 
 namespace ZividPython
 {
     void wrapClass(pybind11::class_<ReleasableImageRGBA> pyClass)
     {
         pyClass.def_buffer(imageRGBADataBuffer)
             .def("save", &ReleasableImageRGBA::save, py::arg("file_name"))
             .def("width", &ReleasableImageRGBA::width)
             .def("height", &ReleasableImageRGBA::height);
     }
+
+    void wrapClass(pybind11::class_<ReleasableImageBGRA> pyClass)
+    {
+        pyClass.def_buffer(imageBGRADataBuffer)
+            .def("save", &ReleasableImageBGRA::save, py::arg("file_name"))
+            .def("width", &ReleasableImageBGRA::width)
+            .def("height", &ReleasableImageBGRA::height);
+    }
 } // namespace ZividPython
```

### Comparing `zivid-2.8.0.2.9.0/src/ReleasablePointCloud.cpp` & `zivid-2.9.0.2.9.0/src/ReleasablePointCloud.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/SingletonApplication.cpp` & `zivid-2.9.0.2.9.0/src/SingletonApplication.cpp`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/Wrapper.cpp` & `zivid-2.9.0.2.9.0/src/Wrapper.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -39,23 +39,26 @@
     ZIVID_PYTHON_WRAP_CLASS_AS_RELEASABLE(module, Camera);
     ZIVID_PYTHON_WRAP_CLASS_AS_RELEASABLE(module, Frame);
     ZIVID_PYTHON_WRAP_CLASS_AS_RELEASABLE(module, Frame2D);
 
     ZIVID_PYTHON_WRAP_CLASS_BUFFER(module, Matrix4x4);
 
     ZIVID_PYTHON_WRAP_CLASS_BUFFER_AS_RELEASABLE(module, ImageRGBA);
+    ZIVID_PYTHON_WRAP_CLASS_BUFFER_AS_RELEASABLE(module, ImageBGRA);
     ZIVID_PYTHON_WRAP_CLASS_BUFFER_AS_RELEASABLE(module, PointCloud);
 
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, ColorRGBA);
+    ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, ColorBGRA);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, NormalXYZ);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, PointXYZ);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, PointXYZW);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, PointZ);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, SNR);
     ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, PointXYZColorRGBA);
+    ZIVID_PYTHON_WRAP_ARRAY2D_BUFFER_AS_RELEASABLE(module, PointXYZColorBGRA);
 
     ZIVID_PYTHON_WRAP_NAMESPACE_AS_SUBMODULE(module, Firmware);
     ZIVID_PYTHON_WRAP_NAMESPACE_AS_SUBMODULE(module, Version);
     ZIVID_PYTHON_WRAP_NAMESPACE_AS_SUBMODULE(module, Calibration);
     ZIVID_PYTHON_WRAP_NAMESPACE_AS_SUBMODULE(module, CaptureAssistant);
     ZIVID_PYTHON_WRAP_NAMESPACE_AS_SUBMODULE(module, InfieldCorrection);
 }
```

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/DataModelWrapper.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/DataModelWrapper.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/InfieldCorrection/InfieldCorrection.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/InfieldCorrection/InfieldCorrection.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/Matrix.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/Matrix.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/Releasable.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/Releasable.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableArray2D.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableArray2D.h`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 namespace ZividPython
 {
     template<typename NativeType>
     using ReleasableArray2D = Releasable<Zivid::Array2D<NativeType>>;
 
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::SNR>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::ColorRGBA>> pyClass);
+    void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::ColorBGRA>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::NormalXYZ>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointXYZ>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointXYZW>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointZ>> pyClass);
     void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointXYZColorRGBA>> pyClass);
+    void wrapClass(pybind11::class_<ReleasableArray2D<Zivid::PointXYZColorBGRA>> pyClass);
 
 } // namespace ZividPython
```

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableCamera.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableCamera.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableFrame.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableFrame.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasableImage.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasableImage.h`

 * *Files 17% similar despite different names*

```diff
@@ -12,9 +12,20 @@
         using Releasable<Zivid::Image<Zivid::ColorRGBA>>::Releasable;
 
         ZIVID_PYTHON_FORWARD_1_ARGS(save, const std::string &, fileName)
         ZIVID_PYTHON_FORWARD_0_ARGS(width)
         ZIVID_PYTHON_FORWARD_0_ARGS(height)
     };
 
+    class ReleasableImageBGRA : public Releasable<Zivid::Image<Zivid::ColorBGRA>>
+    {
+    public:
+        using Releasable<Zivid::Image<Zivid::ColorBGRA>>::Releasable;
+
+        ZIVID_PYTHON_FORWARD_1_ARGS(save, const std::string &, fileName)
+        ZIVID_PYTHON_FORWARD_0_ARGS(width)
+        ZIVID_PYTHON_FORWARD_0_ARGS(height)
+    };
+
     void wrapClass(pybind11::class_<ReleasableImageRGBA> pyClass);
+    void wrapClass(pybind11::class_<ReleasableImageBGRA> pyClass);
 } // namespace ZividPython
```

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/ReleasablePointCloud.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/ReleasablePointCloud.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/SingletonApplication.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/SingletonApplication.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/Traits.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/Traits.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/src/include/ZividPython/Wrappers.h` & `zivid-2.9.0.2.9.0/src/include/ZividPython/Wrappers.h`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_application.py` & `zivid-2.9.0.2.9.0/test/test_application.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_camera.py` & `zivid-2.9.0.2.9.0/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_camera_capture.py` & `zivid-2.9.0.2.9.0/test/test_camera_capture.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_camera_info.py` & `zivid-2.9.0.2.9.0/test/test_camera_info.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_camera_state.py` & `zivid-2.9.0.2.9.0/test/test_camera_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
     pcb = file_camera.state.temperature.pcb
     assert pcb is not None
     assert isinstance(pcb, numbers.Real)
 
 
 def test_illegal_set_state(file_camera):
-
     with pytest.raises(AttributeError):
         file_camera.state = file_camera.state
 
 
 def test_equal_state():
     from zivid.camera_state import CameraState
```

### Comparing `zivid-2.8.0.2.9.0/test/test_camera_user_data.py` & `zivid-2.9.0.2.9.0/test/test_camera_user_data.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_capture_assistant.py` & `zivid-2.9.0.2.9.0/test/test_capture_assistant.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_datamodel_save_load.py` & `zivid-2.9.0.2.9.0/test/test_datamodel_save_load.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         "CameraState",
         "CameraInfo",
         "FrameInfo",
         "capture_assistant.SuggestSettingsParameters",
     ],
 )
 def test_basic_save_load(application, datamodel_yml_dir, datamodel):
-
     from operator import attrgetter
     from pathlib import Path
     from tempfile import TemporaryDirectory
     import zivid
 
     filename = datamodel.split(".")[-1] + ".yml"
     load_path = datamodel_yml_dir / filename
```

### Comparing `zivid-2.8.0.2.9.0/test/test_firmware.py` & `zivid-2.9.0.2.9.0/test/test_firmware.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_frame.py` & `zivid-2.9.0.2.9.0/test/test_frame.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_frame_2d.py` & `zivid-2.9.0.2.9.0/test/test_frame_2d.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,46 @@
+import numpy as np
 import pytest
 
 
 @pytest.mark.physical_camera
 def test_image_context_manager(physical_camera_frame_2d):
     import zivid
 
-    with physical_camera_frame_2d.image_rgba() as image:
-        assert image is not None
-        assert isinstance(image, zivid.Image)
+    with physical_camera_frame_2d.image_rgba() as image_rgba:
+        assert image_rgba is not None
+        assert isinstance(image_rgba, zivid.Image)
+
+    with physical_camera_frame_2d.image_bgra() as image_bgra:
+        assert image_bgra is not None
+        assert isinstance(image_bgra, zivid.Image)
 
 
 @pytest.mark.physical_camera
 def test_image(physical_camera_frame_2d):
     import zivid
 
-    image = physical_camera_frame_2d.image_rgba()
-    assert image is not None
-    assert isinstance(image, zivid.Image)
+    image_rgba = physical_camera_frame_2d.image_rgba()
+    assert image_rgba is not None
+    assert isinstance(image_rgba, zivid.Image)
+
+    image_bgra = physical_camera_frame_2d.image_bgra()
+    assert image_bgra is not None
+    assert isinstance(image_bgra, zivid.Image)
+
+
+@pytest.mark.physical_camera
+def test_image_rgba_bgra_correspondence(physical_camera_frame_2d):
+    rgba = physical_camera_frame_2d.image_rgba().copy_data()
+    bgra = physical_camera_frame_2d.image_bgra().copy_data()
+
+    np.testing.assert_array_equal(bgra[:, :, 0], rgba[:, :, 2])
+    np.testing.assert_array_equal(bgra[:, :, 1], rgba[:, :, 1])
+    np.testing.assert_array_equal(bgra[:, :, 2], rgba[:, :, 0])
+    np.testing.assert_array_equal(bgra[:, :, 3], rgba[:, :, 3])
 
 
 @pytest.mark.physical_camera
 def test_state(physical_camera_frame_2d):
     import zivid
 
     state = physical_camera_frame_2d.state
@@ -34,14 +54,23 @@
 
     info = physical_camera_frame_2d.info
     assert info is not None
     assert isinstance(info, zivid.FrameInfo)
 
 
 @pytest.mark.physical_camera
+def test_camera_info(physical_camera_frame_2d):
+    from zivid.camera_info import CameraInfo
+
+    camera_info = physical_camera_frame_2d.camera_info
+    assert camera_info
+    assert isinstance(camera_info, CameraInfo)
+
+
+@pytest.mark.physical_camera
 def test_settings(physical_camera_frame_2d):
     import zivid
 
     settings_2d = physical_camera_frame_2d.settings
     assert settings_2d is not None
     assert isinstance(settings_2d, zivid.Settings2D)
 
@@ -59,7 +88,12 @@
     import zivid
 
     settings_2d = zivid.Settings2D(acquisitions=[zivid.Settings2D.Acquisition()])
     with physical_camera.capture(settings_2d) as frame_2d:
         frame_2d.image_rgba()
     with pytest.raises(RuntimeError):
         frame_2d.image_rgba()
+
+    with physical_camera.capture(settings_2d) as frame_2d:
+        frame_2d.image_bgra()
+    with pytest.raises(RuntimeError):
+        frame_2d.image_bgra()
```

### Comparing `zivid-2.8.0.2.9.0/test/test_frame_info.py` & `zivid-2.9.0.2.9.0/test/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_image_2d.py` & `zivid-2.9.0.2.9.0/test/test_image_2d_bgra.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import pytest
 
 
 @pytest.mark.physical_camera
-def test_copy_data(physical_camera_image_2d):
+def test_copy_data(physical_camera_image_2d_bgra):
     import numpy as np
 
-    image = physical_camera_image_2d
-    rgba = image.copy_data()
-    assert rgba is not None
-    assert isinstance(rgba, np.ndarray)
-    assert rgba.shape == (image.height, image.width, 4)
-    assert rgba.dtype == np.uint8
+    image = physical_camera_image_2d_bgra
+    bgra = image.copy_data()
+    assert bgra is not None
+    assert isinstance(bgra, np.ndarray)
+    assert bgra.shape == (image.height, image.width, 4)
+    assert bgra.dtype == np.uint8
 
 
 @pytest.mark.physical_camera
-def test_save_path(physical_camera_image_2d):
+def test_save_path(physical_camera_image_2d_bgra):
     from pathlib import Path
 
-    physical_camera_image_2d.save(Path("some_file.png"))
+    physical_camera_image_2d_bgra.save(Path("some_file.png"))
 
 
 @pytest.mark.physical_camera
-def test_save_string(physical_camera_image_2d):
-    physical_camera_image_2d.save("some_file.png")
+def test_save_string(physical_camera_image_2d_bgra):
+    physical_camera_image_2d_bgra.save("some_file.png")
 
 
 @pytest.mark.physical_camera
 def test_to_array_context_manager(physical_camera_frame_2d):
-    with physical_camera_frame_2d.image_rgba() as image_2d:
+    with physical_camera_frame_2d.image_bgra() as image_2d:
         image_2d.copy_data()
     with pytest.raises(RuntimeError):
         image_2d.copy_data()
 
 
 @pytest.mark.physical_camera
 def test_save_context_manager(physical_camera_frame_2d):
-    with physical_camera_frame_2d.image_rgba() as image_2d:
+    with physical_camera_frame_2d.image_bgra() as image_2d:
         image_2d.save("some_file.png")
     with pytest.raises(RuntimeError):
         image_2d.save("some_file.png")
 
 
 @pytest.mark.physical_camera
-def test_height(physical_camera_image_2d):
-    height = physical_camera_image_2d.height
+def test_height(physical_camera_image_2d_bgra):
+    height = physical_camera_image_2d_bgra.height
 
     assert height is not None
     assert isinstance(height, int)
 
 
 @pytest.mark.physical_camera
-def test_width(physical_camera_image_2d):
-    width = physical_camera_image_2d.width
+def test_width(physical_camera_image_2d_bgra):
+    width = physical_camera_image_2d_bgra.width
 
     assert width is not None
     assert isinstance(width, int)
```

### Comparing `zivid-2.8.0.2.9.0/test/test_matrix4x4.py` & `zivid-2.9.0.2.9.0/test/test_matrix4x4.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_point_cloud.py` & `zivid-2.9.0.2.9.0/test/test_point_cloud.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 def test_point_cloud_copy_data(point_cloud):
     import numpy as np
 
     # Copy all possible formats
     xyz = point_cloud.copy_data("xyz")
     xyzw = point_cloud.copy_data("xyzw")
     xyzrgba = point_cloud.copy_data("xyzrgba")
+    xyzbgra = point_cloud.copy_data("xyzbgra")
     rgba = point_cloud.copy_data("rgba")
+    bgra = point_cloud.copy_data("bgra")
     normals = point_cloud.copy_data("normals")
     depth = point_cloud.copy_data("z")
     snr = point_cloud.copy_data("snr")
     assert isinstance(xyz, np.ndarray)
     assert isinstance(xyzw, np.ndarray)
     assert isinstance(xyzrgba, np.ndarray)
+    assert isinstance(xyzbgra, np.ndarray)
     assert isinstance(rgba, np.ndarray)
+    assert isinstance(bgra, np.ndarray)
     assert isinstance(normals, np.ndarray)
     assert isinstance(depth, np.ndarray)
     assert isinstance(snr, np.ndarray)
 
     # Check errors when argument is wrong or missing
     with pytest.raises(ValueError):
         point_cloud.copy_data("bogus-format")
@@ -29,48 +33,73 @@
 
 def test_point_cloud_xyzw(point_cloud):
     import numpy as np
 
     xyz = point_cloud.copy_data("xyz")
     xyzw = point_cloud.copy_data("xyzw")
     xyzrgba = point_cloud.copy_data("xyzrgba")
+    xyzbgra = point_cloud.copy_data("xyzbgra")
     depth = point_cloud.copy_data("z")
 
     assert depth.shape == (point_cloud.height, point_cloud.width)
     assert xyz.shape == (point_cloud.height, point_cloud.width, 3)
     assert xyzw.shape == (point_cloud.height, point_cloud.width, 4)
     assert depth.dtype == np.float32
     assert xyz.dtype == np.float32
     assert xyzw.dtype == np.float32
     assert xyzrgba["x"].dtype == np.float32
     assert xyzrgba["y"].dtype == np.float32
     assert xyzrgba["z"].dtype == np.float32
+    assert xyzbgra["x"].dtype == np.float32
+    assert xyzbgra["y"].dtype == np.float32
+    assert xyzbgra["z"].dtype == np.float32
     np.testing.assert_array_equal(xyz[:, :, 2], depth)
     np.testing.assert_array_equal(xyz[:, :, 0], xyzw[:, :, 0])
     np.testing.assert_array_equal(xyz[:, :, 1], xyzw[:, :, 1])
     np.testing.assert_array_equal(xyz[:, :, 2], xyzw[:, :, 2])
 
 
 def test_point_cloud_rgba(point_cloud):
     import numpy as np
 
     xyzrgba = point_cloud.copy_data("xyzrgba")
+    xyzbgra = point_cloud.copy_data("xyzbgra")
     rgba = point_cloud.copy_data("rgba")
+    bgra = point_cloud.copy_data("bgra")
 
     assert rgba.shape == (point_cloud.height, point_cloud.width, 4)
+    assert bgra.shape == (point_cloud.height, point_cloud.width, 4)
     assert xyzrgba.shape == (point_cloud.height, point_cloud.width)
+    assert xyzbgra.shape == (point_cloud.height, point_cloud.width)
     assert rgba.dtype == np.uint8
+    assert bgra.dtype == np.uint8
     assert xyzrgba["r"].dtype == np.uint8
     assert xyzrgba["g"].dtype == np.uint8
     assert xyzrgba["b"].dtype == np.uint8
     assert xyzrgba["a"].dtype == np.uint8
     np.testing.assert_array_equal(rgba[:, :, 0], xyzrgba["r"])
     np.testing.assert_array_equal(rgba[:, :, 1], xyzrgba["g"])
     np.testing.assert_array_equal(rgba[:, :, 2], xyzrgba["b"])
     np.testing.assert_array_equal(rgba[:, :, 3], xyzrgba["a"])
+    assert xyzbgra["b"].dtype == np.uint8
+    assert xyzbgra["g"].dtype == np.uint8
+    assert xyzbgra["r"].dtype == np.uint8
+    assert xyzbgra["a"].dtype == np.uint8
+    np.testing.assert_array_equal(bgra[:, :, 0], xyzbgra["b"])
+    np.testing.assert_array_equal(bgra[:, :, 1], xyzbgra["g"])
+    np.testing.assert_array_equal(bgra[:, :, 2], xyzbgra["r"])
+    np.testing.assert_array_equal(bgra[:, :, 3], xyzbgra["a"])
+    np.testing.assert_array_equal(xyzbgra["r"], xyzrgba["r"])
+    np.testing.assert_array_equal(xyzbgra["g"], xyzrgba["g"])
+    np.testing.assert_array_equal(xyzbgra["b"], xyzrgba["b"])
+    np.testing.assert_array_equal(xyzbgra["a"], xyzrgba["a"])
+    np.testing.assert_array_equal(bgra[:, :, 0], rgba[:, :, 2])
+    np.testing.assert_array_equal(bgra[:, :, 1], rgba[:, :, 1])
+    np.testing.assert_array_equal(bgra[:, :, 2], rgba[:, :, 0])
+    np.testing.assert_array_equal(bgra[:, :, 3], rgba[:, :, 3])
 
 
 def test_point_cloud_normals(point_cloud):
     import numpy as np
 
     normals = point_cloud.copy_data("normals")
 
@@ -251,31 +280,28 @@
 
     # Check result
     assert height_orig // 2 // 3 == point_cloud_new.height
     assert width_orig // 2 // 3 == point_cloud_new.width
 
 
 def test_height_context_manager(frame):
-
     with frame.point_cloud() as point_cloud:
         point_cloud.height
     with pytest.raises(RuntimeError):
         point_cloud.height
 
 
 def test_width_context_manager(frame):
-
     with frame.point_cloud() as point_cloud:
         point_cloud.width
     with pytest.raises(RuntimeError):
         point_cloud.width
 
 
 def test_copy_data_context_manager(frame):
-
     with frame.point_cloud() as point_cloud:
         point_cloud.copy_data(data_format="xyzrgba")
     with pytest.raises(RuntimeError):
         point_cloud.copy_data(data_format="xyzrgba")
     with pytest.raises(RuntimeError):
         point_cloud.copy_data(data_format=123)
     with pytest.raises(TypeError):
```

### Comparing `zivid-2.8.0.2.9.0/test/test_region_of_interest.py` & `zivid-2.9.0.2.9.0/test/test_region_of_interest.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_samples.py` & `zivid-2.9.0.2.9.0/test/test_samples.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_settings.py` & `zivid-2.9.0.2.9.0/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_settings_2d.py` & `zivid-2.9.0.2.9.0/test/test_settings_2d.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_versioning.py` & `zivid-2.9.0.2.9.0/test/test_versioning.py`

 * *Files identical despite different names*

### Comparing `zivid-2.8.0.2.9.0/test/test_zivid_module_content.py` & `zivid-2.9.0.2.9.0/test/test_zivid_module_content.py`

 * *Files identical despite different names*

