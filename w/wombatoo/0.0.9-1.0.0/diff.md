# Comparing `tmp/wombatoo-0.0.9.tar.gz` & `tmp/wombatoo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-oqicaxkm\wombatoo-0.0.9.tar", last modified: Fri May 12 12:37:50 2023, max compression
+gzip compressed data, was "C:\Users\Prashant\Desktop\wombatoo\dist\.tmp-hwaifx5g\wombatoo-1.0.0.tar", last modified: Fri May 12 13:57:28 2023, max compression
```

## Comparing `wombatoo-0.0.9.tar` & `wombatoo-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/
--rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-0.0.9/LICENSE.md
--rw-rw-rw-   0        0        0      409 2023-05-12 12:37:50.000000 wombatoo-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-01 13:09:37.000000 wombatoo-0.0.9/README.md
--rw-rw-rw-   0        0        0      723 2023-05-12 12:31:13.000000 wombatoo-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 12:37:50.000000 wombatoo-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo/
--rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-0.0.9/src/wombatoo/DataCard.txt
--rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-0.0.9/src/wombatoo/__init__.py
--rw-rw-rw-   0        0        0     8754 2023-05-12 12:30:57.000000 wombatoo-0.0.9/src/wombatoo/wombatoo.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 12:37:50.000000 wombatoo-0.0.9/src/wombatoo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 13:57:28.000000 wombatoo-1.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-05-01 06:13:40.000000 wombatoo-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1780 2023-05-12 13:57:28.000000 wombatoo-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1400 2023-05-12 13:52:09.000000 wombatoo-1.0.0/README.md
+-rw-rw-rw-   0        0        0      727 2023-05-12 13:57:00.000000 wombatoo-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 13:57:28.000000 wombatoo-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo/
+-rw-rw-rw-   0        0        0      189 2023-04-11 16:01:38.000000 wombatoo-1.0.0/src/wombatoo/DataCard.txt
+-rw-rw-rw-   0        0        0        0 2023-05-01 07:27:57.000000 wombatoo-1.0.0/src/wombatoo/__init__.py
+-rw-rw-rw-   0        0        0     8754 2023-05-12 12:41:34.000000 wombatoo-1.0.0/src/wombatoo/wombatoo.py
+drwxrwxrwx   0        0        0        0 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/
+-rw-rw-rw-   0        0        0     1780 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 13:57:28.000000 wombatoo-1.0.0/src/wombatoo.egg-info/top_level.txt
```

### Comparing `wombatoo-0.0.9/LICENSE.md` & `wombatoo-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wombatoo-0.0.9/pyproject.toml` & `wombatoo-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
                     
 [project]
 name = "wombatoo"
-version = "0.0.9"
+version = "1.0.0"
 authors = [
   { name="Prashant Singh", email="prashdash112@gmail.com" },
 ]
 description = "A Data-Ops tool for devs"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = ["numpy==1.23.5",
@@ -19,9 +19,9 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 wombatoo = ["*.txt"]
 
 [project.urls]
-"Homepage" = "https://github.com/prashdash112/wombat"
-"Bug Tracker" = "https://github.com/prashdash112/wombat/issues"
+"Homepage" = "https://github.com/prashdash112/wombatoo"
+"Bug Tracker" = "https://github.com/prashdash112/wombatoo/issues"
```

### Comparing `wombatoo-0.0.9/src/wombatoo/wombatoo.py` & `wombatoo-1.0.0/src/wombatoo/wombatoo.py`

 * *Files identical despite different names*

