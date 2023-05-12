# Comparing `tmp/PH-units-1.1.0.tar.gz` & `tmp/PH-units-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PH-units-1.1.0.tar", last modified: Wed Apr 26 11:35:47 2023, max compression
+gzip compressed data, was "dist/PH-units-1.1.1.tar", last modified: Fri May 12 11:02:18 2023, max compression
```

## Comparing `PH-units-1.1.0.tar` & `PH-units-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/
--rw-r--r--   0 runner     (501) staff       (20)       66 2023-04-26 11:33:52.000000 PH-units-1.1.0/.gitattributes
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1781 2023-04-26 11:33:52.000000 PH-units-1.1.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-04-26 11:33:52.000000 PH-units-1.1.0/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      699 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        9 2023-04-26 11:35:47.000000 PH-units-1.1.0/PH_units.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2776 2023-04-26 11:35:47.000000 PH-units-1.1.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1689 2023-04-26 11:33:52.000000 PH-units-1.1.0/README.md
--rw-r--r--   0 runner     (501) staff       (20)    18761 2023-04-26 11:33:52.000000 PH-units-1.1.0/Untitled clipping.textClipping
--rw-r--r--   0 runner     (501) staff       (20)       50 2023-04-26 11:33:52.000000 PH-units-1.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5159 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/converter.py
--rw-r--r--   0 runner     (501) staff       (20)     1908 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/parser.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/tests/test_energy.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-26 11:35:47.000000 PH-units-1.1.0/ph_units/unit_types/
--rw-r--r--   0 runner     (501) staff       (20)     2784 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      371 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/_base.py
--rw-r--r--   0 runner     (501) staff       (20)      442 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/area.py
--rw-r--r--   0 runner     (501) staff       (20)     2655 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/energy.py
--rw-r--r--   0 runner     (501) staff       (20)     2571 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/envelope.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/length.py
--rw-r--r--   0 runner     (501) staff       (20)     2072 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/power.py
--rw-r--r--   0 runner     (501) staff       (20)     1176 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/speed.py
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/temperature.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/volume.py
--rw-r--r--   0 runner     (501) staff       (20)     1705 2023-04-26 11:33:52.000000 PH-units-1.1.0/ph_units/unit_types/volume_flow.py
--rw-r--r--   0 runner     (501) staff       (20)      219 2023-04-26 11:33:52.000000 PH-units-1.1.0/sandbox.py
--rw-r--r--   0 runner     (501) staff       (20)      832 2023-04-26 11:35:47.000000 PH-units-1.1.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      263 2023-04-26 11:33:52.000000 PH-units-1.1.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/
+-rw-r--r--   0 runner     (501) staff       (20)       66 2023-05-12 11:00:52.000000 PH-units-1.1.1/.gitattributes
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1781 2023-05-12 11:00:52.000000 PH-units-1.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-05-12 11:00:52.000000 PH-units-1.1.1/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/PH_units.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-05-12 11:02:18.000000 PH-units-1.1.1/PH_units.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      638 2023-05-12 11:02:18.000000 PH-units-1.1.1/PH_units.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-12 11:02:18.000000 PH-units-1.1.1/PH_units.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        9 2023-05-12 11:02:18.000000 PH-units-1.1.1/PH_units.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2023-05-12 11:02:18.000000 PH-units-1.1.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2023-05-12 11:00:52.000000 PH-units-1.1.1/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       50 2023-05-12 11:00:52.000000 PH-units-1.1.1/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/ph_units/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5159 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/converter.py
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/parser.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-12 11:02:18.000000 PH-units-1.1.1/ph_units/unit_types/
+-rw-r--r--   0 runner     (501) staff       (20)     2784 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      371 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)      442 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/area.py
+-rw-r--r--   0 runner     (501) staff       (20)     2655 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/energy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2571 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/envelope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/length.py
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     1176 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/speed.py
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/temperature.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/volume.py
+-rw-r--r--   0 runner     (501) staff       (20)     1705 2023-05-12 11:00:52.000000 PH-units-1.1.1/ph_units/unit_types/volume_flow.py
+-rw-r--r--   0 runner     (501) staff       (20)      219 2023-05-12 11:00:52.000000 PH-units-1.1.1/sandbox.py
+-rw-r--r--   0 runner     (501) staff       (20)      832 2023-05-12 11:02:18.000000 PH-units-1.1.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      263 2023-05-12 11:00:52.000000 PH-units-1.1.1/setup.py
```

### Comparing `PH-units-1.1.0/.github/workflows/ci.yaml` & `PH-units-1.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/LICENSE` & `PH-units-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/PH_units.egg-info/PKG-INFO` & `PH-units-1.1.1/PH_units.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.0/PH_units.egg-info/SOURCES.txt` & `PH-units-1.1.1/PH_units.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 .gitattributes
 LICENSE
 README.md
-Untitled clipping.textClipping
 dev-requirements.txt
 sandbox.py
 setup.cfg
 setup.py
 .github/workflows/ci.yaml
 PH_units.egg-info/PKG-INFO
 PH_units.egg-info/SOURCES.txt
 PH_units.egg-info/dependency_links.txt
 PH_units.egg-info/top_level.txt
 ph_units/__init__.py
 ph_units/converter.py
 ph_units/parser.py
-ph_units/tests/test_energy.py
 ph_units/unit_types/__init__.py
 ph_units/unit_types/_base.py
 ph_units/unit_types/area.py
 ph_units/unit_types/energy.py
 ph_units/unit_types/envelope.py
 ph_units/unit_types/length.py
 ph_units/unit_types/power.py
```

### Comparing `PH-units-1.1.0/PKG-INFO` & `PH-units-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PH-units
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tools for working with common Passive House unit types
 Home-page: https://github.com/PH-Tools/PH_units
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PH-Units:
         A package for converting common Passive House unit types (IP | SI).
```

### Comparing `PH-units-1.1.0/README.md` & `PH-units-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/converter.py` & `PH-units-1.1.1/ph_units/converter.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/parser.py` & `PH-units-1.1.1/ph_units/parser.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/__init__.py` & `PH-units-1.1.1/ph_units/unit_types/__init__.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/energy.py` & `PH-units-1.1.1/ph_units/unit_types/energy.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/envelope.py` & `PH-units-1.1.1/ph_units/unit_types/envelope.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/length.py` & `PH-units-1.1.1/ph_units/unit_types/length.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/power.py` & `PH-units-1.1.1/ph_units/unit_types/power.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/speed.py` & `PH-units-1.1.1/ph_units/unit_types/speed.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/temperature.py` & `PH-units-1.1.1/ph_units/unit_types/temperature.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/volume.py` & `PH-units-1.1.1/ph_units/unit_types/volume.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/ph_units/unit_types/volume_flow.py` & `PH-units-1.1.1/ph_units/unit_types/volume_flow.py`

 * *Files identical despite different names*

### Comparing `PH-units-1.1.0/setup.cfg` & `PH-units-1.1.1/setup.cfg`

 * *Files identical despite different names*

