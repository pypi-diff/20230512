# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a1.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a1.tar", last modified: Tue Mar 14 22:06:13 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a2.tar", last modified: Fri May 12 19:40:41 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1.tar` & `ovos-PHAL-plugin-homeassistant-0.0.2a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    25743 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-14 22:06:06.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-14 22:06:12.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-14 22:06:13.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:06:12.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-14 22:06:12.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-14 22:06:12.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-14 22:06:12.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 22:06:13.067482 ovos-PHAL-plugin-homeassistant-0.0.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-14 22:06:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    25743 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-12 19:40:35.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-12 19:40:41.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 19:40:40.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 19:40:41.274837 ovos-PHAL-plugin-homeassistant-0.0.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-12 19:40:32.000000 ovos-PHAL-plugin-homeassistant-0.0.2a2/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a1/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a2/setup.py`

 * *Files identical despite different names*

