# Comparing `tmp/scikit-kinematics-0.8.8.tar.gz` & `tmp/scikit_kinematics-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-kinematics-0.8.8.tar", last modified: Wed Dec 29 21:11:08 2021, max compression
+gzip compressed data, was "scikit_kinematics-0.9.0.tar", max compression
```

## Comparing `scikit-kinematics-0.8.8.tar` & `scikit_kinematics-0.9.0.tar`

### file list

```diff
@@ -1,108 +1,67 @@
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.517587 scikit-kinematics-0.8.8/
--rw-rw-rw-   0        0        0     4435 2021-12-29 16:41:59.000000 scikit-kinematics-0.8.8/CHANGES.txt
--rw-rw-rw-   0        0        0   101367 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/Errata.pdf
--rw-rw-rw-   0        0        0     1483 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/LICENSE.txt
--rw-rw-rw-   0        0        0      141 2021-12-29 17:22:08.000000 scikit-kinematics-0.8.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6822 2021-12-29 21:11:08.517587 scikit-kinematics-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0     6006 2021-12-29 16:42:19.000000 scikit-kinematics-0.8.8/README.md
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.432567 scikit-kinematics-0.8.8/docs/
--rw-rw-rw-   0        0        0      480 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/FAQ.txt
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.438568 scikit-kinematics-0.8.8/docs/Images/
--rw-rw-rw-   0        0        0    48140 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/GramSchmidt.jpg
--rw-rw-rw-   0        0        0    22001 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/skinematics.png
--rw-rw-rw-   0        0        0     6057 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_angle.png
--rw-rw-rw-   0        0        0     5166 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_normalize.png
--rw-rw-rw-   0        0        0     5552 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_plane_orientation.png
--rw-rw-rw-   0        0        0     5502 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_project.png
--rw-rw-rw-   0        0        0     6263 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_q_shortest_rotation.png
--rw-rw-rw-   0        0        0     7605 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/Images/vector_rotate_vector.png
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.443570 scikit-kinematics-0.8.8/docs/_static/
--rw-rw-rw-   0        0        0   128787 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/orientation_viewer.png
--rw-rw-rw-   0        0        0    11454 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/skinematics.ico
--rw-rw-rw-   0        0        0    22001 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/skinematics.png
--rw-rw-rw-   0        0        0   105983 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/viewer_large.png
--rw-rw-rw-   0        0        0    88294 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/viewer_small.png
--rw-rw-rw-   0        0        0    69321 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/_static/viewer_ts3.png
--rw-rw-rw-   0        0        0     9069 2021-12-29 16:43:51.000000 scikit-kinematics-0.8.8/docs/conf.py
--rw-rw-rw-   0        0        0     3032 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/imus.rst
--rw-rw-rw-   0        0        0     4175 2021-12-29 16:44:08.000000 scikit-kinematics-0.8.8/docs/index.rst
--rwxrwxrwx   0        0        0     6711 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/make.bat
--rw-rw-rw-   0        0        0      523 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/markers.rst
--rw-rw-rw-   0        0        0      598 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/misc.rst
--rw-rw-rw-   0        0        0     1367 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/quat.rst
--rw-rw-rw-   0        0        0     1562 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/rotmat.rst
--rw-rw-rw-   0        0        0      897 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/vector.rst
--rw-rw-rw-   0        0        0     1071 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/docs/view.rst
--rw-rw-rw-   0        0        0      110 2021-12-29 13:30:04.000000 scikit-kinematics-0.8.8/pyproject.toml
--rw-rw-rw-   0        0        0       59 2021-12-29 14:40:22.000000 scikit-kinematics-0.8.8/requirements.txt
--rw-rw-rw-   0        0        0     1158 2021-12-29 21:11:08.522587 scikit-kinematics-0.8.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.416563 scikit-kinematics-0.8.8/src/
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.462574 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/
--rw-rw-rw-   0        0        0     6822 2021-12-29 21:11:08.000000 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2675 2021-12-29 21:11:08.000000 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-29 21:11:08.000000 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2021-12-29 21:11:08.000000 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-12-29 21:11:08.000000 scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.470576 scikit-kinematics-0.8.8/src/skinematics/
--rw-rw-rw-   0        0        0     1032 2021-12-29 16:44:32.000000 scikit-kinematics-0.8.8/src/skinematics/__init__.py
--rw-rw-rw-   0        0        0    30154 2021-12-28 12:27:52.000000 scikit-kinematics-0.8.8/src/skinematics/imus.py
--rw-rw-rw-   0        0        0     5546 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/markers.py
--rw-rw-rw-   0        0        0     7045 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/misc.py
--rw-rw-rw-   0        0        0    33407 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/quat.py
--rw-rw-rw-   0        0        0    20014 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/rotmat.py
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.476578 scikit-kinematics-0.8.8/src/skinematics/sensors/
--rw-rw-rw-   0        0        0        0 2021-12-29 16:45:15.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/__init__.py
--rw-rw-rw-   0        0        0     2260 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/manual.py
--rw-rw-rw-   0        0        0     3586 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/polulu.py
--rw-rw-rw-   0        0        0     4775 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/xio.py
--rw-rw-rw-   0        0        0     4965 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/xio_ngimu.py
--rw-rw-rw-   0        0        0     2159 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/xsens.py
--rw-rw-rw-   0        0        0     2185 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/sensors/yei.py
--rw-rw-rw-   0        0        0      417 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.478578 scikit-kinematics-0.8.8/src/skinematics/simulations/
--rw-rw-rw-   0        0        0        0 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/src/skinematics/simulations/__init__.py
--rw-rw-rw-   0        0        0    11822 2021-04-29 09:54:22.000000 scikit-kinematics-0.8.8/src/skinematics/simulations/simulate_movements.py
--rw-rw-rw-   0        0        0    14041 2021-12-28 12:27:52.000000 scikit-kinematics-0.8.8/src/skinematics/vector.py
--rw-rw-rw-   0        0        0    34284 2021-10-01 11:25:25.000000 scikit-kinematics-0.8.8/src/skinematics/view.py
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.490580 scikit-kinematics-0.8.8/tests/
--rw-rw-rw-   0        0        0      114 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.499582 scikit-kinematics-0.8.8/tests/data/
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.505584 scikit-kinematics-0.8.8/tests/data/data_ngimu/
--rw-rw-rw-   0        0        0     1882 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/Settings.txt
--rw-rw-rw-   0        0        0      592 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/battery.csv
--rw-rw-rw-   0        0        0      243 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/humidity.csv
--rw-rw-rw-   0        0        0    28972 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/quaternion.csv
--rw-rw-rw-   0        0        0      457 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/rssi.csv
--rw-rw-rw-   0        0        0    57564 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/sensors.csv
--rw-rw-rw-   0        0        0      444 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_ngimu/temperature.csv
--rw-rw-rw-   0        0        0   284932 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_polulu.txt
-drwxrwxrwx   0        0        0        0 2021-12-29 21:11:08.515586 scikit-kinematics-0.8.8/tests/data/data_xio/
--rw-rw-rw-   0        0        0   369329 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033.BIN
--rw-rw-rw-   0        0        0     4793 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_CalBattAndTherm.csv
--rw-rw-rw-   0        0        0  1160611 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_CalInertialAndMag.csv
--rw-rw-rw-   0        0        0       60 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_Commands.csv
--rw-rw-rw-   0        0        0     2274 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_DateTime.csv
--rw-rw-rw-   0        0        0   214694 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_EulerAngles.csv
--rw-rw-rw-   0        0        0   308485 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_Quaternion.csv
--rw-rw-rw-   0        0        0     4271 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_Registers.csv
--rw-rw-rw-   0        0        0   633745 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xio/00033_RotationMatrix.csv
--rw-rw-rw-   0        0        0   124662 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_xsens.txt
--rw-rw-rw-   0        0        0   445277 2013-12-20 09:39:56.000000 scikit-kinematics-0.8.8/tests/data/data_xsens2.txt
--rw-rw-rw-   0        0        0   471888 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/data_yei.txt
--rw-rw-rw-   0        0        0   513962 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/data/planet_trajectory_2D.txt
--rw-rw-rw-   0        0        0   445277 2013-12-20 09:39:56.000000 scikit-kinematics-0.8.8/tests/data/walking_xsens_lowerLeg.txt
--rw-rw-rw-   0        0        0   443260 2013-12-20 09:39:52.000000 scikit-kinematics-0.8.8/tests/data/walking_xsens_upperLeg.txt
--rw-rw-rw-   0        0        0      587 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/positive_rotations.py
--rw-rw-rw-   0        0        0     8280 2021-12-28 12:27:52.000000 scikit-kinematics-0.8.8/tests/test_imus.py
--rw-rw-rw-   0        0        0     1890 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_markers.py
--rw-rw-rw-   0        0        0      746 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_misc.py
--rw-rw-rw-   0        0        0     8099 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_quat.py
--rw-rw-rw-   0        0        0     4345 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_rotmat.py
--rw-rw-rw-   0        0        0     1225 2021-12-29 21:01:51.000000 scikit-kinematics-0.8.8/tests/test_sensor_manual.py
--rw-rw-rw-   0        0        0      997 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_sensor_polulu.py
--rw-rw-rw-   0        0        0      965 2021-12-29 21:02:37.000000 scikit-kinematics-0.8.8/tests/test_sensor_xio.py
--rw-rw-rw-   0        0        0      993 2021-12-29 21:03:53.000000 scikit-kinematics-0.8.8/tests/test_sensor_xio_ngimu.py
--rw-rw-rw-   0        0        0     1210 2021-12-29 21:05:16.000000 scikit-kinematics-0.8.8/tests/test_sensor_xsens.py
--rw-rw-rw-   0        0        0      982 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_sensor_yei.py
--rw-rw-rw-   0        0        0      353 2020-07-05 14:44:42.000000 scikit-kinematics-0.8.8/tests/test_skinematics.py
--rw-rw-rw-   0        0        0     5436 2021-12-29 20:59:58.000000 scikit-kinematics-0.8.8/tests/test_vector.py
+-rw-r--r--   0        0        0     1483 2020-07-05 14:44:42.689371 scikit_kinematics-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1183 2023-05-12 15:17:26.999160 scikit_kinematics-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6006 2023-05-12 15:17:26.997160 scikit_kinematics-0.9.0/README.md
+-rw-r--r--   0        0        0     1032 2023-05-12 15:17:26.999160 scikit_kinematics-0.9.0/skinematics/__init__.py
+-rw-r--r--   0        0        0    29903 2023-05-12 15:17:27.000160 scikit_kinematics-0.9.0/skinematics/imus.py
+-rw-r--r--   0        0        0     5546 2023-05-12 15:17:27.000160 scikit_kinematics-0.9.0/skinematics/markers.py
+-rw-r--r--   0        0        0     7045 2023-05-12 15:17:27.000160 scikit_kinematics-0.9.0/skinematics/misc.py
+-rw-r--r--   0        0        0    33407 2023-05-12 15:17:27.001160 scikit_kinematics-0.9.0/skinematics/quat.py
+-rw-r--r--   0        0        0    20014 2023-05-12 15:17:27.001160 scikit_kinematics-0.9.0/skinematics/rotmat.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:17:27.001160 scikit_kinematics-0.9.0/skinematics/sensors/__init__.py
+-rw-r--r--   0        0        0      185 2023-05-12 15:24:37.267309 scikit_kinematics-0.9.0/skinematics/sensors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2367 2023-05-12 15:24:37.267309 scikit_kinematics-0.9.0/skinematics/sensors/__pycache__/vicon.cpython-39.pyc
+-rw-r--r--   0        0        0     2008 2023-05-12 15:24:37.268310 scikit_kinematics-0.9.0/skinematics/sensors/__pycache__/xsens.cpython-39.pyc
+-rw-r--r--   0        0        0     2260 2023-05-12 15:17:27.002160 scikit_kinematics-0.9.0/skinematics/sensors/manual.py
+-rw-r--r--   0        0        0     3590 2023-05-12 15:17:27.002160 scikit_kinematics-0.9.0/skinematics/sensors/polulu.py
+-rw-r--r--   0        0        0     2675 2023-05-12 15:24:37.268310 scikit_kinematics-0.9.0/skinematics/sensors/vicon.py
+-rw-r--r--   0        0        0     4775 2023-05-12 15:17:27.002160 scikit_kinematics-0.9.0/skinematics/sensors/xio.py
+-rw-r--r--   0        0        0     4967 2023-05-12 15:17:27.003161 scikit_kinematics-0.9.0/skinematics/sensors/xio_ngimu.py
+-rw-r--r--   0        0        0     2163 2023-05-12 15:17:27.003161 scikit_kinematics-0.9.0/skinematics/sensors/xsens.py
+-rw-r--r--   0        0        0     2185 2023-05-12 15:17:27.003161 scikit_kinematics-0.9.0/skinematics/sensors/yei.py
+-rw-r--r--   0        0        0      417 2023-05-12 15:17:27.004159 scikit_kinematics-0.9.0/skinematics/setup.py
+-rw-r--r--   0        0        0        0 2023-05-12 15:17:27.004159 scikit_kinematics-0.9.0/skinematics/simulations/__init__.py
+-rw-r--r--   0        0        0    11822 2023-05-12 15:17:27.004159 scikit_kinematics-0.9.0/skinematics/simulations/simulate_movements.py
+-rw-r--r--   0        0        0    14041 2023-05-12 15:17:27.005159 scikit_kinematics-0.9.0/skinematics/vector.py
+-rw-r--r--   0        0        0    34284 2023-05-12 15:17:27.005159 scikit_kinematics-0.9.0/skinematics/view.py
+-rw-r--r--   0        0        0      114 2020-07-05 14:44:42.720361 scikit_kinematics-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      592 2020-07-05 14:44:42.721361 scikit_kinematics-0.9.0/tests/data/data_ngimu/battery.csv
+-rw-r--r--   0        0        0      980 2020-07-05 14:44:42.721361 scikit_kinematics-0.9.0/tests/data/data_ngimu/Device.xml
+-rw-r--r--   0        0        0      243 2020-07-05 14:44:42.722360 scikit_kinematics-0.9.0/tests/data/data_ngimu/humidity.csv
+-rw-r--r--   0        0        0    28972 2020-07-05 14:44:42.723360 scikit_kinematics-0.9.0/tests/data/data_ngimu/quaternion.csv
+-rw-r--r--   0        0        0      457 2020-07-05 14:44:42.723360 scikit_kinematics-0.9.0/tests/data/data_ngimu/rssi.csv
+-rw-r--r--   0        0        0    57564 2020-07-05 14:44:42.724359 scikit_kinematics-0.9.0/tests/data/data_ngimu/sensors.csv
+-rw-r--r--   0        0        0     1882 2020-07-05 14:44:42.721361 scikit_kinematics-0.9.0/tests/data/data_ngimu/Settings.txt
+-rw-r--r--   0        0        0      444 2020-07-05 14:44:42.724359 scikit_kinematics-0.9.0/tests/data/data_ngimu/temperature.csv
+-rw-r--r--   0        0        0   284932 2020-07-05 14:44:42.726361 scikit_kinematics-0.9.0/tests/data/data_polulu.txt
+-rw-r--r--   0        0        0   369329 2020-07-05 14:44:42.731357 scikit_kinematics-0.9.0/tests/data/data_xio/00033.BIN
+-rw-r--r--   0        0        0     4793 2020-07-05 14:44:42.731357 scikit_kinematics-0.9.0/tests/data/data_xio/00033_CalBattAndTherm.csv
+-rw-r--r--   0        0        0  1160611 2020-07-05 14:44:42.739354 scikit_kinematics-0.9.0/tests/data/data_xio/00033_CalInertialAndMag.csv
+-rw-r--r--   0        0        0       60 2020-07-05 14:44:42.740354 scikit_kinematics-0.9.0/tests/data/data_xio/00033_Commands.csv
+-rw-r--r--   0        0        0     2274 2020-07-05 14:44:42.740354 scikit_kinematics-0.9.0/tests/data/data_xio/00033_DateTime.csv
+-rw-r--r--   0        0        0   214694 2020-07-05 14:44:42.742355 scikit_kinematics-0.9.0/tests/data/data_xio/00033_EulerAngles.csv
+-rw-r--r--   0        0        0   308485 2020-07-05 14:44:42.745353 scikit_kinematics-0.9.0/tests/data/data_xio/00033_Quaternion.csv
+-rw-r--r--   0        0        0     4271 2020-07-05 14:44:42.746352 scikit_kinematics-0.9.0/tests/data/data_xio/00033_Registers.csv
+-rw-r--r--   0        0        0   633745 2020-07-05 14:44:42.751350 scikit_kinematics-0.9.0/tests/data/data_xio/00033_RotationMatrix.csv
+-rw-r--r--   0        0        0   124662 2020-07-05 14:44:42.752352 scikit_kinematics-0.9.0/tests/data/data_xsens.txt
+-rw-r--r--   0        0        0   445277 2013-12-20 09:39:56.000000 scikit_kinematics-0.9.0/tests/data/data_xsens2.txt
+-rw-r--r--   0        0        0   471888 2020-07-05 14:44:42.759350 scikit_kinematics-0.9.0/tests/data/data_yei.txt
+-rw-r--r--   0        0        0   978464 2023-05-12 15:24:37.278309 scikit_kinematics-0.9.0/tests/data/LeftFoot-marche01.c3d
+-rw-r--r--   0        0        0   513962 2020-07-05 14:44:42.762349 scikit_kinematics-0.9.0/tests/data/planet_trajectory_2D.txt
+-rw-r--r--   0        0        0   445277 2013-12-20 09:39:56.000000 scikit_kinematics-0.9.0/tests/data/walking_xsens_lowerLeg.txt
+-rw-r--r--   0        0        0   443260 2013-12-20 09:39:52.000000 scikit_kinematics-0.9.0/tests/data/walking_xsens_upperLeg.txt
+-rw-r--r--   0        0        0      587 2020-07-05 14:44:42.770345 scikit_kinematics-0.9.0/tests/positive_rotations.py
+-rw-r--r--   0        0        0     7723 2023-05-12 15:17:27.005159 scikit_kinematics-0.9.0/tests/test_imus.py
+-rw-r--r--   0        0        0     1890 2020-07-05 14:44:42.771345 scikit_kinematics-0.9.0/tests/test_markers.py
+-rw-r--r--   0        0        0      746 2020-07-05 14:44:42.771345 scikit_kinematics-0.9.0/tests/test_misc.py
+-rw-r--r--   0        0        0     8099 2020-07-05 14:44:42.772344 scikit_kinematics-0.9.0/tests/test_quat.py
+-rw-r--r--   0        0        0     4345 2020-07-05 14:44:42.772344 scikit_kinematics-0.9.0/tests/test_rotmat.py
+-rw-r--r--   0        0        0     1219 2023-05-12 15:17:27.006160 scikit_kinematics-0.9.0/tests/test_sensor_manual.py
+-rw-r--r--   0        0        0      997 2020-07-05 14:44:42.774343 scikit_kinematics-0.9.0/tests/test_sensor_polulu.py
+-rw-r--r--   0        0        0     1212 2023-05-12 15:24:37.278309 scikit_kinematics-0.9.0/tests/test_sensor_vicon.py
+-rw-r--r--   0        0        0      959 2023-05-12 15:17:27.006160 scikit_kinematics-0.9.0/tests/test_sensor_xio.py
+-rw-r--r--   0        0        0      987 2023-05-12 15:17:27.007160 scikit_kinematics-0.9.0/tests/test_sensor_xio_ngimu.py
+-rw-r--r--   0        0        0     1204 2023-05-12 15:17:27.007160 scikit_kinematics-0.9.0/tests/test_sensor_xsens.py
+-rw-r--r--   0        0        0      982 2020-07-05 14:44:42.775343 scikit_kinematics-0.9.0/tests/test_sensor_yei.py
+-rw-r--r--   0        0        0      353 2020-07-05 14:44:42.776342 scikit_kinematics-0.9.0/tests/test_skinematics.py
+-rw-r--r--   0        0        0     5430 2023-05-12 15:17:27.008160 scikit_kinematics-0.9.0/tests/test_vector.py
+-rw-r--r--   0        0        0     7039 1970-01-01 00:00:00.000000 scikit_kinematics-0.9.0/PKG-INFO
```

### Comparing `scikit-kinematics-0.8.8/LICENSE.txt` & `scikit_kinematics-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/PKG-INFO` & `scikit_kinematics-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: scikit-kinematics
-Version: 0.8.8
-Summary: Python utilites for movements in 3d space
-Home-page: https://github.com/thomas-haslwanter/scikit-kinematics
-Author: Thomas Haslwanter
-Author-email: thomas.haslwanter@fh-ooe.at
-License: http://opensource.org/licenses/BSD-2-Clause
-Project-URL: Documentation, https://work.thaslwanter.at/skinematics/html
-Keywords: quaterions,rotations
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ![Title](docs/Images/skinematics.png)
 ===
 scikit-kinematics
 ===
 
 *scikit-kinematics* primarily contains functions for working with 3D
 kinematics, e.g quaternions and rotation matrices. This includes
@@ -37,17 +16,17 @@
 numpy, scipy, matplotlib, pandas, sympy, easygui
 
 Homepage
 --------
 
 <http://work.thaslwanter.at/skinematics/html/>
 
-Author: Thomas Haslwanter Date: 14-05-2021 Ver: 0.8.8 Licence: BSD
+Author: Thomas Haslwanter Date: 12-05-2023 Ver: 0.9.0 Licence: BSD
 2-Clause License (<http://opensource.org/licenses/BSD-2-Clause>)
-Copyright (c) 2021, Thomas Haslwanter All rights reserved.
+Copyright (c) 2023, Thomas Haslwanter All rights reserved.
 
 Installation
 ------------
 
 You can install scikit-kinematics with
 
 > pip install scikit-kinematics
@@ -212,9 +191,7 @@
 ===========
 
 - simulate_movements ... calculated ideal IMU-signals for combined rotations/translations
 
 ## Errata
 The file [Errata.pdf](Errata.pdf) contains the a list of mistakes in the manuscript, and
 the corresponding corrections.
-
-
```

### Comparing `scikit-kinematics-0.8.8/src/scikit_kinematics.egg-info/PKG-INFO` & `scikit_kinematics-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,220 +1,230 @@
-Metadata-Version: 2.1
-Name: scikit-kinematics
-Version: 0.8.8
-Summary: Python utilites for movements in 3d space
-Home-page: https://github.com/thomas-haslwanter/scikit-kinematics
-Author: Thomas Haslwanter
-Author-email: thomas.haslwanter@fh-ooe.at
-License: http://opensource.org/licenses/BSD-2-Clause
-Project-URL: Documentation, https://work.thaslwanter.at/skinematics/html
-Keywords: quaterions,rotations
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-![Title](docs/Images/skinematics.png)
-===
-scikit-kinematics
-===
-
-*scikit-kinematics* primarily contains functions for working with 3D
-kinematics, e.g quaternions and rotation matrices. This includes
-utilities to read in data from the following IMU-sensors: - polulu -
-XSens - xio - xio-NGIMU - YEI
-
-Compatible with Python &gt;= 3.5
-
-Dependencies
-------------
-
-numpy, scipy, matplotlib, pandas, sympy, easygui
-
-Homepage
---------
-
-<http://work.thaslwanter.at/skinematics/html/>
-
-Author: Thomas Haslwanter Date: 14-05-2021 Ver: 0.8.8 Licence: BSD
-2-Clause License (<http://opensource.org/licenses/BSD-2-Clause>)
-Copyright (c) 2021, Thomas Haslwanter All rights reserved.
-
-Installation
-------------
-
-You can install scikit-kinematics with
-
-> pip install scikit-kinematics
-
-and upgrade to a new version with
-
-> pip install --upgrade --no-deps scikit-kinematics
-
-IMUs
-====
-
-Analysis of signals from IMUs (intertial-measurement-units). Read in
-data, calculate orientation (with one of the algorithms below)
-
--   get\_data ... This method must be taken from one of the existing
-    sensors, or from your own sensor. Currenlty the following sensors
-    types are available:
-    -   XSens
-    -   xio (original, and NGIMU)
-    -   yei
-
-    \* polulu
--   calc\_position
-
-MARG Systems
-------------
-
--   imus.analytical ... Calculate orientation and position, from angular
-    velocity and linear acceleration
--   imus.kalman ... Calculate orientation from IMU-data using an
-    Extended Kalman Filter.
--   
-
-    imus.IMU ... Class for working with data from IMUs
-
-    :   -   imus.IMU.calc\_position ... calculate position
-        -   imus.IMU.setData ... set the properties of an IMU-object
-        -   imus.IMU.set\_qtype ... sets q\_type, and automatically
-            performs the relevant calculations.
-
--   imus.Madgwick ... Class for calculating the 3D orientation with the
-    Madgwick-algorithm
--   imus.Mahony ... Class for calculating the 3D orientation with the
-    Mahony-algorithm
-
-Markers
-=======
-
-Analysis of signals from video-based marker-recordings of 3D movements
-
--   markers.analyze\_3Dmarkers ... Kinematic analysis of
-    video-basedrecordings of 3D markers
--   markers.find\_trajectory ... Calculation of joint-movements from 3D
-    marker positions
-
-Quaternions
-===========
-
-Note that all these functions work with single quaternions and
-quaternion vectors, as well as with arrays containing these.
-
-Quaternion class
-----------------
-
--   
-
-    quat.Quaternion ... class, including overloading for multiplication and
-
-    :   division (e.g. "quatCombined = quat1 \* quat2"), import and
-        export
-
-Functions for working with quaternions
---------------------------------------
-
--   quat.q\_conj ... Conjugate quaternion
--   quat.q\_inv ... Quaternion inversion
--   quat.q\_mult ... Quaternion multiplication
--   quat.q\_scalar ... Extract the scalar part from a quaternion
--   quat.q\_vector ... Extract the vector part from a quaternion
--   quat.unit\_q ... Extend a quaternion vector to a unit quaternion.
-
-Conversion routines - quaternions
---------------------------------=
-
--   quat.calc\_angvel ... Calculates the velocity in space from
-    quaternions
--   quat.calc\_quat ... Calculate orientation from a starting
-    orientation and angular velocity.
--   quat.convert ... Convert quaternion to corresponding rotation matrix
-    or Gibbs vector
--   quat.deg2quat ... Convert number or axis angles to quaternion
-    vectors
--   quat.quat2seq ... Convert quaternions to sequention rotations
-    ("nautical" angles, etc)
--   quat.scale2deg ... Convert quaternion to corresponding axis angle
-
-Rotation Matrices
-=================
-
-Definition of rotation matrices
-------------------------------=
-
--   rotmat.R ... 3D rotation matrix for rotation about a coordinate axis
-
-Conversion Routines - rotation matrices
---------------------------------------=
-
--   rotmat.convert ... Convert a rotation matrix to the corresponding
-    quaternion
--   rotmat.seq2quat ... Convert nautical angles etc. to quaternions
--   rotmat.sequence ... Calculation of Euler, Fick, Helmholtz, ...
-    angles
-
-Symbolic matrices
------------------
-
--   rotmat.R\_s() ... symbolix matrix for rotation about a coordinate
-    axis
-
-For example, you can e.g. generate a Fick-matrix, with
-
-&gt;&gt;&gt; R\_Fick = R\_s(2, 'theta') \* R\_s(1, 'phi') \* R\_s(0,
-'psi')
-
-Spatial Transformation Matrices
--------------------------------
-
--   rotmat.stm ... spatial transformation matrix, for combined
-    rotations/translations
--   rotmat.stm\_s() ... symbolix spatial transformation matrix
-
-Denavit-Hartenberg Transformations
-----------------------------------
-
--   rotmat.dh ... Denavit-Hartenberg transformation matrix
--   rotmat.dh\_s ... symbolic Denavit-Hartenberg transformation matrix
-
-Vectors
-=======
-
-Routines for working with vectors These routines can be used with
-vectors, as well as with matrices containing a vector in each row.
-
--   vector.normalize ... Vector normalization
--   vector.project ... Projection of one vector onto another one
--   vector.GramSchmidt ... Gram-Schmidt orthogonalization of three
-    points
--   vector.q\_shortest\_rotation ... Quaternion indicating the shortest
-    rotation from one vector into another.
--   vector.rotate\_vector ... Rotation of a vector
--   vector.target2orient ... Convert target location into orientation
-    angles
-
-Interactive Data Analysis
-========================-
-
--   viewer.ts ... interactive viewer for time series data
--   view.orientation ... visualize and animate orientations, expressed
-    as quaternions.
-
-Simulations
-===========
-
-- simulate_movements ... calculated ideal IMU-signals for combined rotations/translations
-
-## Errata
-The file [Errata.pdf](Errata.pdf) contains the a list of mistakes in the manuscript, and
-the corresponding corrections.
-
-
+Metadata-Version: 2.1
+Name: scikit-kinematics
+Version: 0.9.0
+Summary: Python utilites for movements in 3d space
+Home-page: https://work.thaslwanter.at/skinematics/html
+License: BSD-3-Clause
+Keywords: quaterions,rotations
+Author: Thomas Haslwanter
+Author-email: thomas.haslwanter@fh-ooe.at
+Requires-Python: >=3.7
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: docutils (>=0.3)
+Requires-Dist: matplotlib (>=3.1)
+Requires-Dist: numpy (>=1.13.0)
+Requires-Dist: pandas (>=1.0)
+Requires-Dist: pygame (>=2.0)
+Requires-Dist: scipy (>=1.5)
+Requires-Dist: sympy (>=1.0)
+Project-URL: Repository, https://github.com/thomas-haslwanter/scikit-kinematics
+Description-Content-Type: text/markdown
+
+![Title](docs/Images/skinematics.png)
+===
+scikit-kinematics
+===
+
+*scikit-kinematics* primarily contains functions for working with 3D
+kinematics, e.g quaternions and rotation matrices. This includes
+utilities to read in data from the following IMU-sensors: - polulu -
+XSens - xio - xio-NGIMU - YEI
+
+Compatible with Python &gt;= 3.5
+
+Dependencies
+------------
+
+numpy, scipy, matplotlib, pandas, sympy, easygui
+
+Homepage
+--------
+
+<http://work.thaslwanter.at/skinematics/html/>
+
+Author: Thomas Haslwanter Date: 12-05-2023 Ver: 0.9.0 Licence: BSD
+2-Clause License (<http://opensource.org/licenses/BSD-2-Clause>)
+Copyright (c) 2023, Thomas Haslwanter All rights reserved.
+
+Installation
+------------
+
+You can install scikit-kinematics with
+
+> pip install scikit-kinematics
+
+and upgrade to a new version with
+
+> pip install --upgrade --no-deps scikit-kinematics
+
+IMUs
+====
+
+Analysis of signals from IMUs (intertial-measurement-units). Read in
+data, calculate orientation (with one of the algorithms below)
+
+-   get\_data ... This method must be taken from one of the existing
+    sensors, or from your own sensor. Currenlty the following sensors
+    types are available:
+    -   XSens
+    -   xio (original, and NGIMU)
+    -   yei
+
+    \* polulu
+-   calc\_position
+
+MARG Systems
+------------
+
+-   imus.analytical ... Calculate orientation and position, from angular
+    velocity and linear acceleration
+-   imus.kalman ... Calculate orientation from IMU-data using an
+    Extended Kalman Filter.
+-   
+
+    imus.IMU ... Class for working with data from IMUs
+
+    :   -   imus.IMU.calc\_position ... calculate position
+        -   imus.IMU.setData ... set the properties of an IMU-object
+        -   imus.IMU.set\_qtype ... sets q\_type, and automatically
+            performs the relevant calculations.
+
+-   imus.Madgwick ... Class for calculating the 3D orientation with the
+    Madgwick-algorithm
+-   imus.Mahony ... Class for calculating the 3D orientation with the
+    Mahony-algorithm
+
+Markers
+=======
+
+Analysis of signals from video-based marker-recordings of 3D movements
+
+-   markers.analyze\_3Dmarkers ... Kinematic analysis of
+    video-basedrecordings of 3D markers
+-   markers.find\_trajectory ... Calculation of joint-movements from 3D
+    marker positions
+
+Quaternions
+===========
+
+Note that all these functions work with single quaternions and
+quaternion vectors, as well as with arrays containing these.
+
+Quaternion class
+----------------
+
+-   
+
+    quat.Quaternion ... class, including overloading for multiplication and
+
+    :   division (e.g. "quatCombined = quat1 \* quat2"), import and
+        export
+
+Functions for working with quaternions
+--------------------------------------
+
+-   quat.q\_conj ... Conjugate quaternion
+-   quat.q\_inv ... Quaternion inversion
+-   quat.q\_mult ... Quaternion multiplication
+-   quat.q\_scalar ... Extract the scalar part from a quaternion
+-   quat.q\_vector ... Extract the vector part from a quaternion
+-   quat.unit\_q ... Extend a quaternion vector to a unit quaternion.
+
+Conversion routines - quaternions
+--------------------------------=
+
+-   quat.calc\_angvel ... Calculates the velocity in space from
+    quaternions
+-   quat.calc\_quat ... Calculate orientation from a starting
+    orientation and angular velocity.
+-   quat.convert ... Convert quaternion to corresponding rotation matrix
+    or Gibbs vector
+-   quat.deg2quat ... Convert number or axis angles to quaternion
+    vectors
+-   quat.quat2seq ... Convert quaternions to sequention rotations
+    ("nautical" angles, etc)
+-   quat.scale2deg ... Convert quaternion to corresponding axis angle
+
+Rotation Matrices
+=================
+
+Definition of rotation matrices
+------------------------------=
+
+-   rotmat.R ... 3D rotation matrix for rotation about a coordinate axis
+
+Conversion Routines - rotation matrices
+--------------------------------------=
+
+-   rotmat.convert ... Convert a rotation matrix to the corresponding
+    quaternion
+-   rotmat.seq2quat ... Convert nautical angles etc. to quaternions
+-   rotmat.sequence ... Calculation of Euler, Fick, Helmholtz, ...
+    angles
+
+Symbolic matrices
+-----------------
+
+-   rotmat.R\_s() ... symbolix matrix for rotation about a coordinate
+    axis
+
+For example, you can e.g. generate a Fick-matrix, with
+
+&gt;&gt;&gt; R\_Fick = R\_s(2, 'theta') \* R\_s(1, 'phi') \* R\_s(0,
+'psi')
+
+Spatial Transformation Matrices
+-------------------------------
+
+-   rotmat.stm ... spatial transformation matrix, for combined
+    rotations/translations
+-   rotmat.stm\_s() ... symbolix spatial transformation matrix
+
+Denavit-Hartenberg Transformations
+----------------------------------
+
+-   rotmat.dh ... Denavit-Hartenberg transformation matrix
+-   rotmat.dh\_s ... symbolic Denavit-Hartenberg transformation matrix
+
+Vectors
+=======
+
+Routines for working with vectors These routines can be used with
+vectors, as well as with matrices containing a vector in each row.
+
+-   vector.normalize ... Vector normalization
+-   vector.project ... Projection of one vector onto another one
+-   vector.GramSchmidt ... Gram-Schmidt orthogonalization of three
+    points
+-   vector.q\_shortest\_rotation ... Quaternion indicating the shortest
+    rotation from one vector into another.
+-   vector.rotate\_vector ... Rotation of a vector
+-   vector.target2orient ... Convert target location into orientation
+    angles
+
+Interactive Data Analysis
+========================-
+
+-   viewer.ts ... interactive viewer for time series data
+-   view.orientation ... visualize and animate orientations, expressed
+    as quaternions.
+
+Simulations
+===========
+
+- simulate_movements ... calculated ideal IMU-signals for combined rotations/translations
+
+## Errata
+The file [Errata.pdf](Errata.pdf) contains the a list of mistakes in the manuscript, and
+the corresponding corrections.
+
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/__init__.py` & `scikit_kinematics-0.9.0/skinematics/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 ------------
 numpy, scipy, matplotlib, pandas, sympy, pygame, pyOpenGL
 
 Homepage
 --------
 http://work.thaslwanter.at/skinematics/html/
 
-Copyright (c) 2021 Thomas Haslwanter <thomas.haslwanter@fh-ooe.at>
+Copyright (c) 2023 Thomas Haslwanter <thomas.haslwanter@fh-ooe.at>
 
 '''
 
 import importlib
 
 __author__ = "Thomas Haslwanter <thomas.haslwanter@fh-linz.at"
 __license__ = "BSD 2-Clause License"
-__version__ = "0.8.8"
+__version__ = "0.9.0"
 
 
 required_imports = ['markers', 'quat', 'rotmat', 'vector', 'sensors']
 optional_imports = ['imus', 'misc']
 
 __all__ = []
 for _m in required_imports:
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/imus.py` & `scikit_kinematics-0.9.0/skinematics/imus.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 recordings with inertial measurement units (IMUs), as well as functions and
 classes for the evaluation of IMU-data..
 
 The advantage of using an "abstract base class" is that it allows to write
 code that is independent of the IMU-sensor. All IMUs provide acceleration
 and angular velocities, and most of them also the direction of the local
 magnetic field. The specifics of each sensor are hidden in the sensor-object
-(specifically, in the "get\_data" method which has to be implemented once
+(specifically, in the "get_data" method which has to be implemented once
 for each sensor). Initialization of a sensor object includes a number of
 activities:
 
         - Reading in the data.
         - Making acceleration, angular\_velocity etc. accessible in a sensor-
           independent way
         - Calculating duration, totalSamples, etc.
         - Calculating orientation (expressed as "quat"), with the method
           specified in "q\_type"
 
 """
 
 #Author: Thomas Haslwanter
 
+import os
+import sys
 import numpy as np
 import matplotlib.pyplot as plt
-import pandas as pd 
+import pandas as pd
 import scipy as sp
 from scipy import constants     # for "g"
 from scipy.integrate import cumtrapz
-import re
 
 # The following construct is required since I want to run the module as a script
 # inside the skinematics-directory
-import os
-import sys
 
 file_dir = os.path.dirname(__file__)
 if file_dir not in sys.path:
     sys.path.insert(0, file_dir)
 
 import quat, vector, misc, rotmat
 
@@ -45,15 +44,15 @@
 # import deprecation
 import warnings
 
 # For the definition of the abstract base class IMU_Base
 import abc
 
 class IMU_Base(metaclass=abc.ABCMeta):
-    '''
+    """
     Abstract BaseClass for working with working with inertial measurement units (IMUs)
     A concrete class must be instantiated, which implements "get_data".
     (See example below.)
 
     Attributes:
         acc (Nx3 array) : 3D linear acceleration [m/s**2]
         dataType (string) : Type of data (commonly float)
@@ -86,49 +85,49 @@
              Local magnetic field, in the x-, y-, and z-direction
         rate: float
             sample rate [Hz]
 
 
     Examples
     --------
-    >>> # Set the in-file, initial sensor orientation 
+    >>> # Set the in-file, initial sensor orientation
     >>> in_file = r'tests/data/data_xsens.txt'
     >>> initial_orientation = np.array([[1,0,0],
     >>>                                 [0,0,-1],
     >>>                                 [0,1,0]])
-    >>>  
-    >>> # Choose a sensor 
+    >>>
+    >>> # Choose a sensor
     >>> from skinematics.sensors.xsens import XSens
     >>> from skinematics.sensors.manual import MyOwnSensor
     >>>
     >>> # Only read in the data
     >>> data = XSens(in_file, q_type=None)
     >>>
     >>> # Read in and evaluate the data
     >>> sensor = XSens(in_file=in_file, R_init=initial_orientation)
-    >>>  
+    >>>
     >>> # By default, the orientation quaternion gets automatically calculated,
     >>> #    using the option "analytical"
     >>> q_analytical = sensor.quat
-    >>>  
+    >>>
     >>> # Automatic re-calculation of orientation if "q_type" is changed
     >>> sensor.set_qtype('madgwick')
     >>> q_Madgwick = sensor.quat
-    >>>  
+    >>>
     >>> sensor.set_qtype('kalman')
     >>> q_Kalman = sensor.quat
     >>>
     >>> # Demonstrate how to fill up a sensor manually
     >>> in_data = {'rate':sensor.rate,
     >>>         'acc': sensor.acc,
     >>>         'omega':sensor.omega,
     >>>         'mag':sensor.mag}
     >>> my_sensor = MyOwnSensor(in_file='My own 123 sensor.', in_data=in_data)
 
-    '''
+    """
 
     @abc.abstractmethod
     def get_data(self, in_file=None, in_data=None):
         """Retrieve "rate", "acc", "omega", "mag" from the input source
         and set the corresponding values of "self".
         With some sensors, "rate" has to be provided, and is taken from "in_data".
         """
@@ -179,66 +178,66 @@
             # Get the data from "in_data"
             # In that case, "in_data"
             #   - must contain the fields ['acc', 'omega']
             #   - can contain the fields ['rate', 'mag']
             # self.source is set to "None"
             self._set_data(in_data)
 
-        else: 
+        else:
             # Set rate, acc, omega, mag
-            # Note: this is implemented in the concrete class, implenented in 
+            # Note: this is implemented in the concrete class, implenented in
             # the corresponding module in "sensors"
             self.source = in_file
             self.get_data(in_file, in_data)
 
         # Set information not determined by the IMU-data
         self.R_init = R_init
         self.pos_init = pos_init
 
         # Set the analysis method, and consolidate the object (see below)
         # This also means calculating the orientation quaternion!!
         self.set_qtype(q_type)
-        
+
         if q_type != None:
             if calculate_position:
                 self.calc_position()
 
-    def set_qtype(self, type_value):                
+    def set_qtype(self, type_value):
         """Sets q_type, and automatically performs the relevant calculations.
         q_type determines how the orientation is calculated.
         If "q_type" is "None", no orientation gets calculated; otherwise,
-        the orientation calculation is performed with 
+        the orientation calculation is performed with
         "_calc_orientation", using the option "q_type".
 
         It has to be one of the following values:
 
         * analytical
         * kalman
         * madgwick
         * mahony
         * None
 
         """
-        
+
         allowed_values = ['analytical',
                           'kalman',
                           'madgwick',
                           'mahony',
                           None]
-        
+
         if type_value in allowed_values:
             self.q_type = type_value
             if type_value == None:
                 self.quat = None
             else:
                 self._calc_orientation()
         else:
             raise ValueError('q_type must be one of the following: ' \
                              '{0}, not {1}'.format(allowed_values, value))
-        
+
 
     def _set_data(self, data):
         # Set the properties of an IMU-object directly
 
         if 'rate' not in data.keys():
             print('Set the "rate" to the default value (100 Hz).')
             data['rate'] = 100.0
@@ -249,36 +248,36 @@
         if 'mag' in data.keys():
             self.mag = data['mag']
         self.source = None
         self._set_info()
 
 
     def _calc_orientation(self):
-        '''
+        """
         Calculate the current orientation
 
         Parameters
         ----------
         type : string
                 - 'analytical' .... quaternion integration of angular velocity
                 - 'kalman' ..... quaternion Kalman filter
                 - 'madgwick' ... gradient descent method, efficient
                 - 'mahony' ....  formula from Mahony, as implemented by Madgwick
 
-        '''
+        """
 
         initialPosition = np.r_[0,0,0]
 
         method = self.q_type
         if method == 'analytical':
             (quaternion, position, velocity) = analytical(self.R_init,
                                                           self.omega,
                                                           initialPosition,
                                                           self.acc,
-                                                          self.rate) 
+                                                          self.rate)
 
         elif method == 'kalman':
             self._checkRequirements()
             quaternion = kalman(self.rate, self.acc, np.deg2rad(self.omega),
                                 self.mag)
 
         elif method == 'madgwick':
@@ -300,15 +299,15 @@
                 AHRS.Update(Gyr[t], Acc[t], Mag[t])
                 quaternion[t] = AHRS.Quaternion
 
         elif method == 'mahony':
             self._checkRequirements()
 
             # Initialize object
-            AHRS = Mahony(rate=np.float(self.rate), Kp=0.4)  # previously: Kp=0.5
+            AHRS = Mahony(rate=np.float64(self.rate), Kp=0.4)  # previously: Kp=0.5
             quaternion = np.zeros((self.totalSamples, 4))
 
             # The "Update"-function uses angular velocity in radian/s, and only
             # the directions of acceleration and magnetic field
             Gyr = self.omega
             Acc = vector.normalize(self.acc)
             Mag = vector.normalize(self.mag)
@@ -323,59 +322,59 @@
             print('Unknown orientation type: {0}'.format(method))
             return
 
         self.quat = quaternion
 
 
     def calc_position(self):
-        '''Calculate the position, assuming that the orientation is already known.'''
+        """Calculate the position, assuming that the orientation is already known."""
 
         initialPosition = self.pos_init
         # Acceleration, velocity, and position ----------------------------
         # From q and the measured acceleration, get the \frac{d^2x}{dt^2}
         g = constants.g
-        g_v = np.r_[0, 0, g] 
+        g_v = np.r_[0, 0, g]
         accReSensor = self.acc - vector.rotate_vector(g_v, quat.q_inv(self.quat))
         accReSpace = vector.rotate_vector(accReSensor, self.quat)
 
         # Position and Velocity through integration, assuming 0-velocity at t=0
         vel = np.nan*np.ones_like(accReSpace)
         pos = np.nan*np.ones_like(accReSpace)
 
         for ii in range(accReSpace.shape[1]):
-            vel[:,ii] = cumtrapz(accReSpace[:,ii],
-                                 dx=1./np.float(self.rate), initial=0)
-            pos[:,ii] = cumtrapz(vel[:,ii],
-                        dx=1./np.float(self.rate), initial=initialPosition[ii])
+            vel[:, ii] = cumtrapz(accReSpace[:, ii],
+                                 dx=1. / np.float64(self.rate), initial=0)
+            pos[:, ii] = cumtrapz(vel[:, ii],
+                        dx=1. / np.float64(self.rate), initial=initialPosition[ii])
 
         self.vel = vel
         self.pos = pos
 
     def _checkRequirements(self):
-        '''Check if all the necessary variables are available.'''
+        """Check if all the necessary variables are available."""
         required = [ 'rate', 'acc', 'omega', 'mag' ]
 
         for field in required:
             if field not in vars(self):
                 print('Cannot find {0} in calc_orientation!'.format(field))
 
     def _set_info(self):
-        '''Complete the information properties of that IMU'''
+        """Complete the information properties of that IMU"""
 
         self.totalSamples = len(self.omega)
-        self.duration = np.float(self.totalSamples)/self.rate # [sec]
+        self.duration = np.float64(self.totalSamples) / self.rate # [sec]
         self.dataType = str(self.omega.dtype)
 
 
 def analytical(R_initialOrientation=np.eye(3),
                omega=np.zeros((5,3)),
                initialPosition=np.zeros(3),
                accMeasured=np.column_stack((np.zeros((5,2)), 9.81*np.ones(5))),
                rate=100):
-    ''' Reconstruct position and orientation with an analytical solution,
+    """ Reconstruct position and orientation with an analytical solution,
     from angular velocity and linear acceleration.
     Assumes a start in a stationary position. No compensation for drift.
 
     Parameters
     ----------
     R_initialOrientation: ndarray(3,3)
         Rotation matrix describing the initial orientation of the sensor,
@@ -396,43 +395,43 @@
     pos : ndarray(N,3)
         Position in space [m]
     vel : ndarray(N,3)
         Velocity in space [m/s]
 
     Example
     -------
-     
+
     >>> q1, pos1 = analytical(R_initialOrientation, omega, initialPosition, acc, rate)
 
-    '''
+    """
 
     if omega.ndim == 1:
         raise ValueError('The input to "analytical" requires matrix inputs.')
-        
+
     # Transform recordings to angVel/acceleration in space --------------
 
     # Orientation of \vec{g} with the sensor in the "R_initialOrientation"
     g = constants.g
     g0 = np.linalg.inv(R_initialOrientation).dot(np.r_[0,0,g])
 
     # for the remaining deviation, assume the shortest rotation to there
-    q0 = vector.q_shortest_rotation(accMeasured[0], g0)    
-    
+    q0 = vector.q_shortest_rotation(accMeasured[0], g0)
+
     q_initial = rotmat.convert(R_initialOrientation, to='quat')
-    
+
     # combine the two, to form a reference orientation. Note that the sequence
     # is very important!
     q_ref = quat.q_mult(q_initial, q0)
-    
+
     # Calculate orientation q by "integrating" omega -----------------
     q = quat.calc_quat(omega, q_ref, rate, 'bf')
 
     # Acceleration, velocity, and position ----------------------------
     # From q and the measured acceleration, get the \frac{d^2x}{dt^2}
-    g_v = np.r_[0, 0, g] 
+    g_v = np.r_[0, 0, g]
     accReSensor = accMeasured - vector.rotate_vector(g_v, quat.q_inv(q))
     accReSpace = vector.rotate_vector(accReSensor, q)
 
     # Make the first position the reference position
     q = quat.q_mult(q, quat.q_inv(q[0]))
 
     # compensate for drift
@@ -446,25 +445,25 @@
     for ii in range(accReSpace.shape[1]):
         vel[:,ii] = cumtrapz(accReSpace[:,ii], dx=1./rate, initial=0)
         pos[:,ii] = cumtrapz(vel[:,ii], dx=1./rate, initial=initialPosition[ii])
 
     return (q, pos, vel)
 
 def kalman(rate, acc, omega, mag,
-           D = [0.4, 0.4, 0.4],          
+           D = [0.4, 0.4, 0.4],
            tau = [0.5, 0.5, 0.5],
            Q_k = None,
            R_k = None):
-    '''
+    """
     Calclulate the orientation from IMU magnetometer data.
 
     Parameters
     ----------
     rate : float
-    	   sample rate [Hz]	
+    	   sample rate [Hz]
     acc : (N,3) ndarray
     	  linear acceleration [m/sec^2]
     omega : (N,3) ndarray
     	  angular velocity [rad/sec]
     mag : (N,3) ndarray
     	  magnetic field orientation
     D : (,3) ndarray
@@ -479,89 +478,89 @@
           covariance matrix of process noises
           parameter for tuning the filter
           If set to "None", the defaults from Yun et al. are taken!
     R_k : None, or (7,7) ndarray
           covariance matrix of measurement noises
           parameter for tuning the filter; defaults from Yun et al.
           If set to "None", the defaults from Yun et al. are taken!
-          
+
 
     Returns
     -------
     qOut : (N,4) ndarray
     	   unit quaternion, describing the orientation relativ to the coordinate
            system spanned by the local magnetic field, and gravity
 
     Notes
     -----
     Based on "Design, Implementation, and Experimental Results of a Quaternion-
        Based Kalman Filter for Human Body Motion Tracking" Yun, X. and Bachman,
        E.R., IEEE TRANSACTIONS ON ROBOTICS, VOL. 22, 1216-1227 (2006)
 
-    '''
+    """
 
     numData = len(acc)
 
     # Set parameters for Kalman Filter
     tstep = 1./rate
-    
+
     # check input
     assert len(tau) == 3
     tau = np.array(tau)
 
-    # Initializations 
+    # Initializations
     x_k = np.zeros(7)	# state vector
     z_k = np.zeros(7)   # measurement vector
     z_k_pre = np.zeros(7)
     P_k = np.eye(7)		 # error covariance matrix P_k
 
     Phi_k = np.eye(7)    # discrete state transition matrix Phi_k
     for ii in range(3):
         Phi_k[ii,ii] = np.exp(-tstep/tau[ii])
 
     H_k = np.eye(7)		# Identity matrix
 
     D = np.r_[0.4, 0.4, 0.4]		# [rad^2/sec^2]; from Yun, 2006
-    
+
     if Q_k is None:
         # Set the default input, from Yun et al.
         Q_k = np.zeros((7,7)) 	# process noise matrix Q_k
         for ii in range(3):
             Q_k[ii,ii] =  D[ii]/(2*tau[ii])  * ( 1-np.exp(-2*tstep/tau[ii]) )
     else:
         # Check the shape of the input
         assert Q_k.shape == (7,7)
 
     # Evaluate measurement noise covariance matrix R_k
     if R_k is None:
         # Set the default input, from Yun et al.
         r_angvel = 0.01;      # [rad**2/sec**2]; from Yun, 2006
         r_quats = 0.0001;     # from Yun, 2006
-        
+
         r_ii = np.zeros(7)
         for ii in range(3):
             r_ii[ii] = r_angvel
         for ii in range(4):
             r_ii[ii+3] = r_quats
-            
-        R_k = np.diag(r_ii)    
+
+        R_k = np.diag(r_ii)
     else:
         # Check the shape of the input
         assert R_k.shape == (7,7)
 
     # Calculation of orientation for every time step
     qOut = np.zeros( (numData,4) )
 
     for ii in range(numData):
         accelVec  = acc[ii,:]
         magVec    = mag[ii,:]
         angvelVec = omega[ii,:]
         z_k_pre = z_k.copy()  # watch out: by default, Python passes the reference!!
 
-        # Evaluate quaternion based on acceleration and magnetic field data 
+        # Evaluate quaternion based on acceleration and magnetic field data
         accelVec_n = vector.normalize(accelVec)
         magVec_hor = magVec - accelVec_n * (accelVec_n @ magVec)
         magVec_n   = vector.normalize(magVec_hor)
         basisVectors = np.column_stack( [magVec_n,
                                 np.cross(accelVec_n, magVec_n), accelVec_n] )
         quatRef = quat.q_inv(rotmat.convert(basisVectors, to='quat')).ravel()
 
@@ -578,15 +577,15 @@
 
         # Evaluate discrete state transition matrix Phi_k
         Delta = np.zeros((7,7))
         Delta[3,:] = np.r_[-x_k[4], -x_k[5], -x_k[6],      0, -x_k[0], -x_k[1], -x_k[2]]
         Delta[4,:] = np.r_[ x_k[3], -x_k[6],  x_k[5], x_k[0],       0,  x_k[2], -x_k[1]]
         Delta[5,:] = np.r_[ x_k[6],  x_k[3], -x_k[4], x_k[1], -x_k[2],       0,  x_k[0]]
         Delta[6,:] = np.r_[-x_k[5],  x_k[4],  x_k[3], x_k[2],  x_k[1], -x_k[0],       0]
-        
+
         Delta *= tstep/2
         Phi_k += Delta
 
         # Update error covariance matrix
         P_k = (np.eye(7) - K_k) @ P_k
 
         # Projection of state
@@ -603,48 +602,48 @@
 
     # Make the first position the reference position
     qOut = quat.q_mult(qOut, quat.q_inv(qOut[0]))
 
     return qOut
 
 class Madgwick:
-    '''Madgwick's gradient descent filter.
+    """Madgwick's gradient descent filter.
 
         Parameters
         ----------
         rate : double
             sample rate [Hz]
         Beta : double
             algorithm gain
         Quaternion : array, shape (N,4)
             output quaternion describing the Earth relative to the sensor
-        '''
+        """
 
     def __init__(self, rate=256.0, Beta=1.0, Quaternion=[1,0,0,0]):
-        '''Initialization '''
-        
+        """Initialization """
+
         self.rate = rate
         self.SamplePeriod = 1/self.rate
         self.Beta = Beta
         self.Quaternion = Quaternion
 
     def Update(self, Gyroscope, Accelerometer, Magnetometer):
-        '''Calculate the best quaternion to the given measurement values.
-        
+        """Calculate the best quaternion to the given measurement values.
+
         Parameters
         ----------
         Gyroscope : array, shape (,3)
             Angular velocity [rad/s]
         Accelerometer : array, shape (,3)
             Linear acceleration (Only the direction is used, so units don't matter.)
         Magnetometer : array, shape (,3)
             Orientation of local magenetic field.
             (Again, only the direction is used, so units don't matter.)
-            
-        '''
+
+        """
 
         q = self.Quaternion; # short name local variable for readability
 
         # Reference direction of Earth's magnetic field
         h = vector.rotate_vector(Magnetometer, q)
         b = np.hstack((0, np.sqrt(h[0]**2+h[1]**2), 0, h[2]))
 
@@ -671,49 +670,49 @@
         qDot = 0.5 * quat.q_mult(q, np.hstack([0, Gyroscope])) - self.Beta * step
 
         # Integrate to yield quaternion
         q = q + qDot * self.SamplePeriod
         self.Quaternion = vector.normalize(q).flatten()
 
 class Mahony:
-    '''Madgwick's implementation of Mayhony's AHRS algorithm
+    """Madgwick's implementation of Mayhony's AHRS algorithm
 
         Parameters
         ----------
         rate : double
             sample rate [Hz]
         Kp : algorithm proportional gain
         Ki : algorithm integral gain
         Quaternion : output quaternion describing the Earth relative to the sensor
-    '''
+    """
     def __init__(self, rate=256.0, Kp=1.0, Ki=0, Quaternion=[1,0,0,0]):
-        '''Initialization '''
-        
+        """Initialization """
+
         self.rate = rate
         self.SamplePeriod = 1/self.rate
         self.Kp = Kp
         self.Ki = Ki
         self.Quaternion = Quaternion
         self._eInt = [0, 0, 0]  # integral error
 
     def Update(self, Gyroscope, Accelerometer, Magnetometer):
-        '''Calculate the best quaternion to the given measurement values.
-        
+        """Calculate the best quaternion to the given measurement values.
+
         Parameters
         ----------
         Gyroscope : array, shape (,3)
             Angular velocity [rad/s]
         Accelerometer : array, shape (,3)
             Linear acceleration (Only the direction is used, so units don't
             matter.)
         Magnetometer : array, shape (,3)
             Orientation of local magenetic field.
             (Again, only the direction is used, so units don't matter.)
-            
-        '''
+
+        """
 
         q = self.Quaternion; # short name local variable for readability
 
         # Reference direction of Earth's magnetic field
         h = vector.rotate_vector(Magnetometer, q)
         b = np.hstack((0, np.sqrt(h[0]**2+h[1]**2), 0, h[2]))
 
@@ -722,52 +721,52 @@
             2*(q[1]*q[3] - q[0]*q[2]),
             2*(q[0]*q[1] + q[2]*q[3]),
             q[0]**2 - q[1]**2 - q[2]**2 + q[3]**2])
 
         w = np.array([
             2*b[1]*(0.5 - q[2]**2 - q[3]**2) + 2*b[3]*(q[1]*q[3] - q[0]*q[2]),
             2*b[1]*(q[1]*q[2] - q[0]*q[3]) + 2*b[3]*(q[0]*q[1] + q[2]*q[3]),
-            2*b[1]*(q[0]*q[2] + q[1]*q[3]) + 2*b[3]*(0.5 - q[1]**2 - q[2]**2)]) 
+            2*b[1]*(q[0]*q[2] + q[1]*q[3]) + 2*b[3]*(0.5 - q[1]**2 - q[2]**2)])
 
         # Error is sum of cross product between estimated direction and measured
         # direction of fields
-        e = np.cross(Accelerometer, v) + np.cross(Magnetometer, w) 
+        e = np.cross(Accelerometer, v) + np.cross(Magnetometer, w)
 
         if self.Ki > 0:
-            self._eInt += e * self.SamplePeriod  
+            self._eInt += e * self.SamplePeriod
         else:
-            self._eInt = np.array([0, 0, 0], dtype=np.float)
+            self._eInt = np.array([0, 0, 0], dtype=np.float64)
 
         # Apply feedback terms
-        Gyroscope += self.Kp * e + self.Ki * self._eInt;            
+        Gyroscope += self.Kp * e + self.Ki * self._eInt;
 
         # Compute rate of change of quaternion
         qDot = 0.5 * quat.q_mult(q, np.hstack([0, Gyroscope])).flatten()
 
         # Integrate to yield quaternion
         q += qDot * self.SamplePeriod
 
         self.Quaternion = vector.normalize(q)
 
 
 
 if __name__ == '__main__':
-    '''
+    """
     in_file = r'../others/skinematics-invalid-sqrt.txt'
     import pandas as pd
-    
+
     data = pd.read_csv(in_file, delimiter='\t')
     omega = data.filter(regex='Gyr*').values
-    acc = data.filter(regex='Acc*').values    
+    acc = data.filter(regex='Acc*').values
     analytical(omega = omega, accMeasured=acc)
-    
-    '''
+
+    """
     from sensors.xsens import XSens
 
-    in_file = r'tests/data/data_xsens.txt'
+    in_file = r'../../tests/data/data_xsens.txt'
     initial_orientation = np.array([ [1,0,0],
                                      [0,0,-1],
                                      [0,1,0]])
 
     #in_file = r'tests/data/data_xsens2.txt'
     #initial_orientation = np.array([[0,0,-1],
                                     #[1, 0, 0],
@@ -780,27 +779,27 @@
     # By default, the orientation quaternion gets automatically calculated,
     # using "analytical"
     q_analytical = sensor.quat
 
 
     def show_result(imu_data):
         "Dummy function, to simplify the visualization"
-        
+
         fig, axs = plt.subplots(3,1)
         axs[0].plot(imu_data.omega)
         axs[0].set_ylabel('Omega')
         axs[0].set_title(imu_data.q_type)
         axs[1].plot(imu_data.acc)
         axs[1].set_ylabel('Acc')
         axs[2].plot(imu_data.quat[:,1:])
         axs[2].set_ylabel('Quat')
-        plt.show()    
-        
+        plt.show()
+
     show_result(sensor)
-    
+
     # Automatic re-calculation of orientation if "q_type" is changed
     sensor.set_qtype('madgwick')
     q_Madgwick = sensor.quat
 
     show_result(sensor)
 
     sensor.set_qtype('kalman')
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/markers.py` & `scikit_kinematics-0.9.0/skinematics/markers.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/misc.py` & `scikit_kinematics-0.9.0/skinematics/misc.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/quat.py` & `scikit_kinematics-0.9.0/skinematics/quat.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/rotmat.py` & `scikit_kinematics-0.9.0/skinematics/rotmat.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/manual.py` & `scikit_kinematics-0.9.0/skinematics/sensors/manual.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/polulu.py` & `scikit_kinematics-0.9.0/skinematics/sensors/polulu.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             rate = in_data['rate']
             
             # Get the data, and label them
             data = pd.read_csv(in_file, header=None, delim_whitespace=True, engine='python')
             data.columns = ['acc_x', 'acc_y', 'acc_z', 'gyr_x', 'gyr_y', 'gyr_z', 'mag_x', 'mag_y', 'mag_z', 'taccgyr', 'tmag']
             
             # interpolate with a manually set rate. Note that this sensor acquires exactly 25 seconds!
-            dt = 1/np.float(rate)
+            dt = 1/np.float64(rate)
             t_lin = np.arange(0, 25, dt)
     
             data_interp = pd.DataFrame()
             # Different sampling times for acc/gyr and for mag!
             for ii in range(6):
                 data_interp[data.keys()[ii]] = np.interp(t_lin*1000, data['taccgyr'], data.iloc[:,ii])
             for ii in range(6,9):
@@ -96,8 +96,8 @@
     
     import matplotlib.pyplot as plt    
     
     plt.plot(my_sensor.acc)    
     plt.show()
     print(my_sensor.rate)
     print('Done')
-    
+
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/xio.py` & `scikit_kinematics-0.9.0/skinematics/sensors/xio.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/xio_ngimu.py` & `scikit_kinematics-0.9.0/skinematics/sensors/xio_ngimu.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         lines = in_file.readlines()
     
     # Get the send rates
     for line in lines:
         if line.find('rate') > 0:
             # e.g.: "/rate/quaternion, 50f"
             param_full, val_txt = line.split()
-            value = np.float(val_txt[:-1])  # skip the "f"
+            value = np.float64(val_txt[:-1])  # skip the "f"
             param = param_full.split('/')[2][:-1]
             if value > 0:
                 rates[param] = value
             else:
                 rates[param] = None
 
     return rates
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/xsens.py` & `scikit_kinematics-0.9.0/skinematics/sensors/xsens.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         '''
         
         # Get the sampling rate from the second line in the file
         try:
             fh = open(in_file)
             fh.readline()
             line = fh.readline()
-            rate = np.float(line.split(':')[1].split('H')[0])
+            rate = np.float64(line.split(':')[1].split('H')[0])
             fh.close()
     
         except FileNotFoundError:
             print('{0} does not exist!'.format(in_file))
             return -1
     
         # Read the data
@@ -70,8 +70,8 @@
     my_sensor = XSens(in_file=r'..\tests\data\data_xsens.txt')    
     
     import matplotlib.pyplot as plt    
     
     plt.plot(my_sensor.quat[:,1:])    
     plt.show()
     print('Done')
-    
+
```

### Comparing `scikit-kinematics-0.8.8/src/skinematics/sensors/yei.py` & `scikit_kinematics-0.9.0/skinematics/sensors/yei.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/simulations/simulate_movements.py` & `scikit_kinematics-0.9.0/skinematics/simulations/simulate_movements.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/vector.py` & `scikit_kinematics-0.9.0/skinematics/vector.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/src/skinematics/view.py` & `scikit_kinematics-0.9.0/skinematics/view.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_ngimu/Settings.txt` & `scikit_kinematics-0.9.0/tests/data/data_ngimu/Settings.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_ngimu/battery.csv` & `scikit_kinematics-0.9.0/tests/data/data_ngimu/battery.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_ngimu/quaternion.csv` & `scikit_kinematics-0.9.0/tests/data/data_ngimu/quaternion.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_ngimu/sensors.csv` & `scikit_kinematics-0.9.0/tests/data/data_ngimu/sensors.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_polulu.txt` & `scikit_kinematics-0.9.0/tests/data/data_polulu.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033.BIN` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033.BIN`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_CalBattAndTherm.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_CalBattAndTherm.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_CalInertialAndMag.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_CalInertialAndMag.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_DateTime.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_DateTime.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_EulerAngles.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_EulerAngles.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_Quaternion.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_Quaternion.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_Registers.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_Registers.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xio/00033_RotationMatrix.csv` & `scikit_kinematics-0.9.0/tests/data/data_xio/00033_RotationMatrix.csv`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xsens.txt` & `scikit_kinematics-0.9.0/tests/data/data_xsens.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_xsens2.txt` & `scikit_kinematics-0.9.0/tests/data/data_xsens2.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/data_yei.txt` & `scikit_kinematics-0.9.0/tests/data/data_yei.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/planet_trajectory_2D.txt` & `scikit_kinematics-0.9.0/tests/data/planet_trajectory_2D.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/walking_xsens_lowerLeg.txt` & `scikit_kinematics-0.9.0/tests/data/walking_xsens_lowerLeg.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/data/walking_xsens_upperLeg.txt` & `scikit_kinematics-0.9.0/tests/data/walking_xsens_upperLeg.txt`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/positive_rotations.py` & `scikit_kinematics-0.9.0/tests/positive_rotations.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_imus.py` & `scikit_kinematics-0.9.0/tests/test_imus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,240 @@
-#from .context import skinematics
+# from .context import skinematics
 import sys
 import os
+
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', '..'))
+sys.path.insert(0, os.path.join(myPath, "..", ".."))
 
 import unittest
 import numpy as np
 import matplotlib.pyplot as plt
 from numpy import sin, cos, array, r_, vstack, abs, tile, pi
 from numpy.linalg import norm
 import os
 from skinematics import imus, quat, vector, rotmat
 from time import sleep
 from skinematics.simulations.simulate_movements import simulate_imu
 
+
 class TestSequenceFunctions(unittest.TestCase):
-    
     def setUp(self):
-        
+
         # Those are currently not needed
-        #self.qz  = r_[cos(0.1), 0,   0,    sin(0.1)]
-        #self.qy  = r_[cos(0.1), 0, sin(0.1), 0]
-        #self.quatMat = vstack((self.qz,self.qy))
-        #self.q3x = r_[sin(0.1),  0,     0]
-        #self.q3y = r_[  0,   sin(0.1), 0]
-        #self.delta = 1e-4
-        
-       # Simulate IMU-data
-        duration_movement = 1    # [sec]
-        duration_total = 1       # [sec]
-        rate = 100               # [Hz]
-        
-        B0 = vector.normalize([1, 0, 1])    # geomagnetic field, re earth
-        
+        # self.qz  = r_[cos(0.1), 0,   0,    sin(0.1)]
+        # self.qy  = r_[cos(0.1), 0, sin(0.1), 0]
+        # self.quatMat = vstack((self.qz,self.qy))
+        # self.q3x = r_[sin(0.1),  0,     0]
+        # self.q3y = r_[  0,   sin(0.1), 0]
+        # self.delta = 1e-4
+
+        # Simulate IMU-data
+        duration_movement = 1  # [sec]
+        duration_total = 1  # [sec]
+        rate = 100  # [Hz]
+
+        B0 = vector.normalize([1, 0, 1])  # geomagnetic field, re earth
+
         rotation_axis = [0, 1, 0]
         angle = 90
-        
-        translation = [1,0,0]
+
+        translation = [1, 0, 0]
         distance = 0
-        
-        self.q_init = [0,0,0]
-        self.pos_init = [0,0,0]
-        
-        self.imu_signals, self.body_pos_orient =  simulate_imu(rate,
-                    duration_movement,
-                    duration_total,
-                    q_init = self.q_init,
-                    rotation_axis = rotation_axis,
-                    deg = angle,
-                    pos_init = self.pos_init,
-                    direction = translation,
-                    distance = distance,
-                    B0=B0) 
 
-        
+        self.q_init = [0, 0, 0]
+        self.pos_init = [0, 0, 0]
+
+        self.imu_signals, self.body_pos_orient = simulate_imu(
+            rate,
+            duration_movement,
+            duration_total,
+            q_init=self.q_init,
+            rotation_axis=rotation_axis,
+            deg=angle,
+            pos_init=self.pos_init,
+            direction=translation,
+            distance=distance,
+            B0=B0,
+        )
+
     def test_analytical(self):
-        
+
         # Analyze the simulated data with "analytical"
         imu = self.imu_signals
-        
-        q, pos, vel = imus.analytical(R_initialOrientation=np.eye(3),
-                         omega = imu['omega'],
-                         initialPosition=np.zeros(3),
-                         accMeasured = imu['gia'],
-                         rate = imu['rate'])                         
-        
+
+        q, pos, vel = imus.analytical(
+            R_initialOrientation=np.eye(3),
+            omega=imu["omega"],
+            initialPosition=np.zeros(3),
+            accMeasured=imu["gia"],
+            rate=imu["rate"],
+        )
+
         # and then check, if the position is [0,0,0], and the orientation-quat = [0, sin(45), 0]
-        self.assertTrue(np.max(np.abs(pos[-1]))<0.001)      # less than 1mm
-        
+        self.assertTrue(np.max(np.abs(pos[-1])) < 0.001)  # less than 1mm
+
         result = quat.q_vector(q[-1])
-        correct = array([ 0.,  np.sin(np.deg2rad(45)),  0.])
-        error = norm(result-correct)
+        correct = array([0.0, np.sin(np.deg2rad(45)), 0.0])
+        error = norm(result - correct)
         self.assertAlmostEqual(error, 0)
-        
-        
-    def test_kalman(self):
-        
-        # Analyze the simulated data with "kalman"
-        imu = self.imu_signals
-        q_kalman = imus.kalman(imu['rate'], imu['gia'], imu['omega'], imu['magnetic'])
-        
-        # and then check, if the quat_vector = [0, sin(45), 0]
-        result = quat.q_vector(q_kalman[-1])                    # [0, 0.46, 0]
-        correct = array([ 0.,  np.sin(np.deg2rad(45)),  0.])    # [0, 0.71, 0]
-        error = norm(result-correct)
-        self.assertAlmostEqual(error, 0, places=2)  # It is not clear why the Kalman filter is not more accurate
-        
-        # Get data
-        inFile = os.path.join(myPath, 'data', 'data_xsens.txt')
-        from skinematics.sensors.xsens import XSens
-        
-        initialPosition = array([0,0,0])
-        R_initialOrientation = rotmat.R(0,90)
-        
-        sensor = XSens(in_file=inFile, R_init = R_initialOrientation, pos_init = initialPosition, q_type='kalman')
-        print(sensor.source)
-        q = sensor.quat
-        
+
+    # def test_kalman(self):
+
+    #     # Analyze the simulated data with "kalman"
+    #     imu = self.imu_signals
+    #     q_kalman = imus.kalman(imu["rate"], imu["gia"], imu["omega"], imu["magnetic"])
+
+    #     # and then check, if the quat_vector = [0, sin(45), 0]
+    #     result = quat.q_vector(q_kalman[-1])  # [0, 0.46, 0]
+    #     correct = array([0.0, np.sin(np.deg2rad(45)), 0.0])  # [0, 0.71, 0]
+    #     error = norm(result - correct)
+    #     self.assertAlmostEqual(
+    #         error, 0, places=2
+    #     )  # It is not clear why the Kalman filter is not more accurate
+
+    #     # Get data
+    #     inFile = os.path.join(myPath, "data", "data_xsens.txt")
+    #     from skinematics.sensors.xsens import XSens
+
+    #     initialPosition = array([0, 0, 0])
+    #     R_initialOrientation = rotmat.R(0, 90)
+
+    #     sensor = XSens(
+    #         in_file=inFile,
+    #         R_init=R_initialOrientation,
+    #         pos_init=initialPosition,
+    #         q_type="kalman",
+    #     )
+    #     print(sensor.source)
+    #     q = sensor.quat
+
     def test_madgwick(self):
-        
+
         from skinematics.sensors.manual import MyOwnSensor
-        
+
         ## Get data
         imu = self.imu_signals
-        in_data = {'rate' : imu['rate'],
-            'acc' : imu['gia'],
-            'omega' : imu['omega'],
-            'mag' : imu['magnetic']}
-        
-        my_sensor = MyOwnSensor(in_file='Simulated sensor-data', in_data=in_data,
-                                R_init = quat.convert(self.q_init, to='rotmat'),
-                                pos_init = self.pos_init, 
-                                q_type = 'madgwick')
-        
+        in_data = {
+            "rate": imu["rate"],
+            "acc": imu["gia"],
+            "omega": imu["omega"],
+            "mag": imu["magnetic"],
+        }
+
+        my_sensor = MyOwnSensor(
+            in_file="Simulated sensor-data",
+            in_data=in_data,
+            R_init=quat.convert(self.q_init, to="rotmat"),
+            pos_init=self.pos_init,
+            q_type="madgwick",
+        )
+
         # and then check, if the quat_vector = [0, sin(45), 0]
         q_madgwick = my_sensor.quat
-        
+
         result = quat.q_vector(q_madgwick[-1])
-        correct = array([ 0.,  np.sin(np.deg2rad(45)),  0.])
-        error = norm(result-correct)
-        
-        #self.assertAlmostEqual(error, 0)
+        correct = array([0.0, np.sin(np.deg2rad(45)), 0.0])
+        error = norm(result - correct)
+
+        # self.assertAlmostEqual(error, 0)
         self.assertTrue(error < 1e-3)
-        
+
         ##inFile = os.path.join(myPath, 'data', 'data_xsens.txt')
         ##from skinematics.sensors.xsens import XSens
-        
+
         ##initialPosition = array([0,0,0])
         ##R_initialOrientation = rotmat.R(0,90)
-        
+
         ##sensor = XSens(in_file=inFile, R_init = R_initialOrientation, pos_init = initialPosition, q_type='madgwick')
         ##q = sensor.quat
-        
-        
+
     def test_mahony(self):
-        
+
         from skinematics.sensors.manual import MyOwnSensor
-        
+
         ## Get data
         imu = self.imu_signals
-        in_data = {'rate' : imu['rate'],
-            'acc' : imu['gia'],
-            'omega' : imu['omega'],
-            'mag' : imu['magnetic']}
-        
-        my_sensor = MyOwnSensor(in_file='Simulated sensor-data', in_data=in_data,
-                                R_init = quat.convert(self.q_init, to='rotmat'),
-                                pos_init = self.pos_init, 
-                                q_type = 'mahony')
-        
+        in_data = {
+            "rate": imu["rate"],
+            "acc": imu["gia"],
+            "omega": imu["omega"],
+            "mag": imu["magnetic"],
+        }
+
+        my_sensor = MyOwnSensor(
+            in_file="Simulated sensor-data",
+            in_data=in_data,
+            R_init=quat.convert(self.q_init, to="rotmat"),
+            pos_init=self.pos_init,
+            q_type="mahony",
+        )
+
         # and then check, if the quat_vector = [0, sin(45), 0]
         q_mahony = my_sensor.quat
-        
+
         result = quat.q_vector(q_mahony[-1])
-        correct = array([ 0.,  np.sin(np.deg2rad(45)),  0.])
-        error = norm(result-correct)
-        
-        #self.assertAlmostEqual(error, 0)
+        correct = array([0.0, np.sin(np.deg2rad(45)), 0.0])
+        error = norm(result - correct)
+
+        # self.assertAlmostEqual(error, 0)
         self.assertTrue(error < 1e-3)
-        
+
         ### Get data
         ##inFile = os.path.join(myPath, 'data', 'data_xsens.txt')
         ##from skinematics.sensors.xsens import XSens
-        
+
         ##initialPosition = array([0,0,0])
         ##R_initialOrientation = rotmat.R(0,90)
-        
+
         ##sensor = XSens(in_file=inFile, R_init = R_initialOrientation, pos_init = initialPosition, q_type='mahony')
         ##q = sensor.quat
-        
+
     def test_IMU_calc_orientation_position(self):
         """Currently, this only tests if the two functions are running through"""
-        
+
         # Get data, with a specified input from an XSens system
-        inFile = os.path.join(myPath, 'data', 'data_xsens.txt')
-        initial_orientation = np.array([[1,0,0],
-                                       [0,0,-1],
-                                       [0,1,0]])
-        initial_position = np.r_[0,0,0]
-        
+        inFile = os.path.join(myPath, "data", "data_xsens.txt")
+        initial_orientation = np.array([[1, 0, 0], [0, 0, -1], [0, 1, 0]])
+        initial_position = np.r_[0, 0, 0]
+
         from skinematics.sensors.xsens import XSens
-        sensor = XSens(in_file=inFile, R_init=initial_orientation, pos_init=initial_position)
+
+        sensor = XSens(
+            in_file=inFile, R_init=initial_orientation, pos_init=initial_position
+        )
         sensor.calc_position()
-        print('done')
-        
+        print("done")
+
     def test_set_qtype(self):
         """Tests if the test crashes on any of the existing qtype options"""
-        
+
         # Get data
-        inFile = os.path.join(myPath, 'data', 'data_xsens.txt')
+        inFile = os.path.join(myPath, "data", "data_xsens.txt")
         from skinematics.sensors.xsens import XSens
-        
-        initialPosition = array([0,0,0])
-        R_initialOrientation = rotmat.R(0,90)
-        
-        sensor = XSens(in_file=inFile, R_init = R_initialOrientation, pos_init = initialPosition, q_type='kalman') 
-        
-        
-        allowed_values = ['analytical',
-                          'kalman',
-                          'madgwick',
-                          'mahony',
-                          None]        
-        
+
+        initialPosition = array([0, 0, 0])
+        R_initialOrientation = rotmat.R(0, 90)
+
+        sensor = XSens(
+            in_file=inFile,
+            R_init=R_initialOrientation,
+            pos_init=initialPosition,
+            q_type="kalman",
+        )
+
+        allowed_values = ["analytical", "kalman", "madgwick", "mahony", None]
+
         for sensor_type in allowed_values:
             sensor.set_qtype(sensor_type)
-            print('{0} is running'.format(sensor_type))
-        
-        
-if __name__ == '__main__':
+            print("{0} is running".format(sensor_type))
+
+
+if __name__ == "__main__":
     suite = unittest.TestSuite()
-    suite.addTest(TestSequenceFunctions(methodName='test_set_qtype'))
+    suite.addTest(TestSequenceFunctions(methodName="test_set_qtype"))
     runner = unittest.TextTestRunner()
     runner.run(suite)
-    
-    #unittest.main()
-    
-    print('Thanks for using programs from Thomas!')
+
+    # unittest.main()
+
+    print("Thanks for using programs from Thomas!")
     sleep(0.2)
```

### Comparing `scikit-kinematics-0.8.8/tests/test_markers.py` & `scikit_kinematics-0.9.0/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_misc.py` & `scikit_kinematics-0.9.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_quat.py` & `scikit_kinematics-0.9.0/tests/test_quat.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_rotmat.py` & `scikit_kinematics-0.9.0/tests/test_rotmat.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_manual.py` & `scikit_kinematics-0.9.0/tests/test_sensor_manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 Author: Thomas Haslwanter
 '''
 
 import sys
 import os
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', 'src','skinematics'))
+sys.path.insert(0, os.path.join(myPath, '..', 'skinematics'))
 
 import unittest
 import imus
 from time import sleep
 from sensors.xsens import XSens
 from sensors.manual import MyOwnSensor
```

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_polulu.py` & `scikit_kinematics-0.9.0/tests/test_sensor_polulu.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_xio.py` & `scikit_kinematics-0.9.0/tests/test_sensor_xio.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Author: Thomas Haslwanter
 
 import numpy as np
 import sys
 import os
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', 'src','skinematics'))
+sys.path.insert(0, os.path.join(myPath, '..', 'skinematics'))
 
 import unittest
 import imus
 from time import sleep
 from sensors.xio import XIO
 
 class TestSequenceFunctions(unittest.TestCase):
```

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_xio_ngimu.py` & `scikit_kinematics-0.9.0/tests/test_sensor_xio_ngimu.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Author: Thomas Haslwanter
 
 import numpy as np
 import sys
 import os
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', 'src','skinematics'))
+sys.path.insert(0, os.path.join(myPath, '..', 'skinematics'))
 
 import unittest
 import imus
 from time import sleep
 from sensors.xio_ngimu import NGIMU
 
 class TestSequenceFunctions(unittest.TestCase):
```

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_xsens.py` & `scikit_kinematics-0.9.0/tests/test_sensor_xsens.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # Author: Thomas Haslwanter
 
 import sys
 import os
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', 'src','skinematics'))
+sys.path.insert(0, os.path.join(myPath, '..', 'skinematics'))
 
 import unittest
 import imus
 from time import sleep
 from sensors.xsens import XSens
 
 class TestSequenceFunctions(unittest.TestCase):
```

### Comparing `scikit-kinematics-0.8.8/tests/test_sensor_yei.py` & `scikit_kinematics-0.9.0/tests/test_sensor_yei.py`

 * *Files identical despite different names*

### Comparing `scikit-kinematics-0.8.8/tests/test_vector.py` & `scikit_kinematics-0.9.0/tests/test_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import sys
 import os
 myPath = os.path.dirname(os.path.abspath(__file__))
-sys.path.insert(0, os.path.join(myPath, '..', 'src','skinematics'))
+sys.path.insert(0, os.path.join(myPath, '..', 'skinematics'))
 
 from numpy.linalg import norm
 import unittest
 
 import vector, quat
 
 class TestSequenceFunctions(unittest.TestCase):
```

