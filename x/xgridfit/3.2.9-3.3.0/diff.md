# Comparing `tmp/xgridfit-3.2.9.tar.gz` & `tmp/xgridfit-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgridfit-3.2.9.tar", last modified: Sun Jan 15 21:58:54 2023, max compression
+gzip compressed data, was "xgridfit-3.3.0.tar", last modified: Thu May 11 21:56:49 2023, max compression
```

## Comparing `xgridfit-3.2.9.tar` & `xgridfit-3.3.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.490590 xgridfit-3.2.9/
--rw-r--r--   0 peterbaker   (504) staff       (20)    11326 2022-02-15 21:27:56.000000 xgridfit-3.2.9/LICENSE.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)      194 2022-11-13 00:11:12.000000 xgridfit-3.2.9/MANIFEST.in
--rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-15 21:58:54.490454 xgridfit-3.2.9/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1201 2022-12-20 02:07:53.000000 xgridfit-3.2.9/README.md
--rw-r--r--   0 peterbaker   (504) staff       (20)      647 2023-01-15 21:57:10.000000 xgridfit-3.2.9/pyproject.toml
--rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-01-15 21:58:54.490625 xgridfit-3.2.9/setup.cfg
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.476892 xgridfit-3.2.9/src/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.479380 xgridfit-3.2.9/src/xgridfit/
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.483377 xgridfit-3.2.9/src/xgridfit/Schemas/
--rw-r--r--   0 peterbaker   (504) staff       (20)    18674 2022-05-10 00:34:15.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rnc
--rw-r--r--   0 peterbaker   (504) staff       (20)    53112 2022-05-10 00:36:20.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rng
--rw-r--r--   0 peterbaker   (504) staff       (20)    19791 2022-05-10 00:37:24.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rnc
--rw-r--r--   0 peterbaker   (504) staff       (20)    52399 2022-05-10 00:38:33.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rng
--rw-r--r--   0 peterbaker   (504) staff       (20)    67775 2022-02-22 18:45:54.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.xsd
--rw-r--r--   0 peterbaker   (504) staff       (20)      634 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xi.xsd
--rw-r--r--   0 peterbaker   (504) staff       (20)      520 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/Schemas/xml.xsd
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.490065 xgridfit-3.2.9/src/xgridfit/XSL/
--rw-r--r--   0 peterbaker   (504) staff       (20)    14150 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/arithmetic.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    12610 2022-05-10 00:19:09.000000 xgridfit-3.2.9/src/xgridfit/XSL/compact.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     6397 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/delta.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    13321 2022-05-10 00:16:13.000000 xgridfit-3.2.9/src/xgridfit/XSL/expand.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    10023 2022-02-19 04:54:24.000000 xgridfit-3.2.9/src/xgridfit/XSL/expressions.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     4225 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/flow.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    30297 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/func-predef.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    38781 2022-02-22 20:39:35.000000 xgridfit-3.2.9/src/xgridfit/XSL/function.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    49445 2022-05-14 11:42:12.000000 xgridfit-3.2.9/src/xgridfit/XSL/graphics.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3271 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/measure.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3286 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/messages.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     2922 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/misc.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    52891 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/move-els.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    22545 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/move-lib.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)   109795 2022-05-07 00:22:27.000000 xgridfit-3.2.9/src/xgridfit/XSL/numbers.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    54518 2022-10-27 22:28:02.000000 xgridfit-3.2.9/src/xgridfit/XSL/points.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    13472 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/prep.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    11443 2022-02-15 21:27:56.000000 xgridfit-3.2.9/src/xgridfit/XSL/primitives.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)     3041 2023-01-15 21:57:51.000000 xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)    15661 2022-03-01 10:36:15.000000 xgridfit-3.2.9/src/xgridfit/XSL/xgfdata.xml
--rw-r--r--   0 peterbaker   (504) staff       (20)    22383 2022-10-28 03:23:36.000000 xgridfit-3.2.9/src/xgridfit/XSL/xgridfit-ft.xsl
--rw-r--r--   0 peterbaker   (504) staff       (20)      494 2022-11-09 05:09:18.000000 xgridfit-3.2.9/src/xgridfit/__init__.py
--rw-r--r--   0 peterbaker   (504) staff       (20)       22 2023-01-15 21:57:30.000000 xgridfit-3.2.9/src/xgridfit/version.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    43941 2023-01-15 04:58:44.000000 xgridfit-3.2.9/src/xgridfit/xgridfit.py
--rw-r--r--   0 peterbaker   (504) staff       (20)    17067 2022-12-31 00:16:25.000000 xgridfit-3.2.9/src/xgridfit/ygridfit.py
-drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-01-15 21:58:54.480623 xgridfit-3.2.9/src/xgridfit.egg-info/
--rw-r--r--   0 peterbaker   (504) staff       (20)     1609 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/PKG-INFO
--rw-r--r--   0 peterbaker   (504) staff       (20)     1218 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/SOURCES.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/dependency_links.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       52 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/entry_points.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)       61 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/requires.txt
--rw-r--r--   0 peterbaker   (504) staff       (20)        9 2023-01-15 21:58:54.000000 xgridfit-3.2.9/src/xgridfit.egg-info/top_level.txt
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.738750 xgridfit-3.3.0/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11326 2022-02-15 21:27:56.000000 xgridfit-3.3.0/LICENSE.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)      194 2023-02-14 18:00:23.000000 xgridfit-3.3.0/MANIFEST.in
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2538 2023-05-11 21:56:49.738625 xgridfit-3.3.0/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2127 2023-05-11 21:45:58.000000 xgridfit-3.3.0/README.md
+-rw-r--r--   0 peterbaker   (504) staff       (20)      650 2023-05-11 21:39:39.000000 xgridfit-3.3.0/pyproject.toml
+-rw-r--r--   0 peterbaker   (504) staff       (20)       38 2023-05-11 21:56:49.738783 xgridfit-3.3.0/setup.cfg
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.724727 xgridfit-3.3.0/src/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.728232 xgridfit-3.3.0/src/xgridfit/
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.732283 xgridfit-3.3.0/src/xgridfit/Schemas/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    18674 2022-05-10 00:34:15.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit-sh.rnc
+-rw-r--r--   0 peterbaker   (504) staff       (20)    53112 2022-05-10 00:36:20.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit-sh.rng
+-rw-r--r--   0 peterbaker   (504) staff       (20)    19791 2022-05-10 00:37:24.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.rnc
+-rw-r--r--   0 peterbaker   (504) staff       (20)    52399 2022-05-10 00:38:33.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.rng
+-rw-r--r--   0 peterbaker   (504) staff       (20)    67775 2022-02-22 18:45:54.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.xsd
+-rw-r--r--   0 peterbaker   (504) staff       (20)      634 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xi.xsd
+-rw-r--r--   0 peterbaker   (504) staff       (20)      520 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/Schemas/xml.xsd
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.738124 xgridfit-3.3.0/src/xgridfit/XSL/
+-rw-r--r--   0 peterbaker   (504) staff       (20)    14150 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/arithmetic.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    12610 2022-05-10 00:19:09.000000 xgridfit-3.3.0/src/xgridfit/XSL/compact.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     6397 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/delta.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13321 2022-05-10 00:16:13.000000 xgridfit-3.3.0/src/xgridfit/XSL/expand.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    10023 2022-02-19 04:54:24.000000 xgridfit-3.3.0/src/xgridfit/XSL/expressions.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     4225 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/flow.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    30297 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/func-predef.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    38781 2022-02-22 20:39:35.000000 xgridfit-3.3.0/src/xgridfit/XSL/function.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    49445 2022-05-14 11:42:12.000000 xgridfit-3.3.0/src/xgridfit/XSL/graphics.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3271 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/measure.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3286 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/messages.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2922 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/misc.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    52891 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/move-els.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22545 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/move-lib.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)   109795 2022-05-07 00:22:27.000000 xgridfit-3.3.0/src/xgridfit/XSL/numbers.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    54518 2022-10-27 22:28:02.000000 xgridfit-3.3.0/src/xgridfit/XSL/points.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    13472 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/prep.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    11443 2022-02-15 21:27:56.000000 xgridfit-3.3.0/src/xgridfit/XSL/primitives.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)     3041 2023-05-11 21:48:07.000000 xgridfit-3.3.0/src/xgridfit/XSL/std-vars.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)    15661 2022-03-01 10:36:15.000000 xgridfit-3.3.0/src/xgridfit/XSL/xgfdata.xml
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22436 2023-01-31 05:31:46.000000 xgridfit-3.3.0/src/xgridfit/XSL/xgridfit-ft.xsl
+-rw-r--r--   0 peterbaker   (504) staff       (20)      487 2023-05-09 03:06:51.000000 xgridfit-3.3.0/src/xgridfit/__init__.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)       22 2023-05-11 21:47:49.000000 xgridfit-3.3.0/src/xgridfit/version.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)     8108 2023-05-10 10:16:37.000000 xgridfit-3.3.0/src/xgridfit/xgfUFOWriter.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    65034 2023-05-09 11:23:19.000000 xgridfit-3.3.0/src/xgridfit/xgridfit-backup.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    56116 2023-05-11 12:21:51.000000 xgridfit-3.3.0/src/xgridfit/xgridfit.py
+-rw-r--r--   0 peterbaker   (504) staff       (20)    22984 2023-05-09 16:22:07.000000 xgridfit-3.3.0/src/xgridfit/ygridfit.py
+drwxr-xr-x   0 peterbaker   (504) staff       (20)        0 2023-05-11 21:56:49.729349 xgridfit-3.3.0/src/xgridfit.egg-info/
+-rw-r--r--   0 peterbaker   (504) staff       (20)     2538 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/PKG-INFO
+-rw-r--r--   0 peterbaker   (504) staff       (20)     1279 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/SOURCES.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        1 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/dependency_links.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       52 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/entry_points.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)       61 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/requires.txt
+-rw-r--r--   0 peterbaker   (504) staff       (20)        9 2023-05-11 21:56:49.000000 xgridfit-3.3.0/src/xgridfit.egg-info/top_level.txt
```

### Comparing `xgridfit-3.2.9/LICENSE.txt` & `xgridfit-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/README.md` & `xgridfit-3.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,37 @@
 # xgridfit-3
 A TrueType hinting language
 
 ---
 
-Xgridfit is an language for hinting TrueType fonts. It is an XML-based language, similar to (and in fact inspired by) XSLT. It has been around since before 2006, but version 3 was reborn as a (largely) Python program with Python dependencies. Xgridfit through version 2 was verbose and awkward to use. Version 3 featured a new compact syntax, and the current version (3.2.5) adds a YAML-based language focused on describing the positions of points relative to the origin of a glyph's grid or to other points rather than issuing commands for positioning them. This language (call it Ygridfit) is simple and easy to write, but its main purpose is to support **ygt**, a graphical hinting tool.
+Xgridfit is an language for hinting TrueType fonts. It is an XML-based language, similar to (and in fact inspired by) XSLT. It has been around since before 2006, but version 3 was reborn as a (largely) Python program with Python dependencies. Xgridfit through version 2 was verbose and awkward to use. Version 3 featured a new compact syntax, and version 3.2.10 added a YAML-based language focused on describing the positions of points relative to the origin of a glyph's grid or to other points rather than issuing commands for positioning them. This language (call it Ygridfit) is simple and easy to write, but its main purpose is to support **ygt**, a graphical hinting tool.
 
 Documentation of the XML-based language (both full and compact syntax), is available at the [GitHub development site](https://github.com/psb1558/xgridfit-3).
 
-There is no release for the current version (3.2.5) at GitHub. Instead, install by downloading from PyPi:
+There is no release for the current version (3.2.18) at GitHub. Instead, install by downloading from PyPi:
 ```
 pip install xgridfit
 ```
-Alternatively, download the code from this site, change to the project's root directory (the one with the file `pyproject.toml` in it), and type:
+Alternatively, download the code from GitHub, change to the project's root directory (the one with the file `pyproject.toml` in it), and type:
 ```
 pip install .
 ```
+Version 3.3.0  merges most of main() (command line) and the former compile_all (called from Ygt) into one routine (run()). This enables 
+merge-mode for Ygt.
+
+Version 3.2.18 logs certain errors rather than exiting (an improvement when a backend for Ygt).
+
+Version 3.2.17 has its own code for exporting to UFO rather than relying on ufoLib2.
+
+Version 3.2.16 adds support for deltas in the YAML notation.
+
+Version 3.2.15 fixes a bug that made a muddle of the cvar table, and removes an obnoxious message.
+
+Version 3.2.14 is revised to accommmodate the new organization of cvar data in ygt.
+
+Version 3.2.13 has small changes to maintain compatibility with ygt
+
+Version 3.2.12 changes from fontTools.ufoLib to ufoLib2 for editing UFOs.
+
+Version 3.2.11 adds the ability to save instructions and associated data to a UFO (version 3)
+
+Version 3.2.10 supports "min" (minimum distance) attribute for hints and emits fewer messages when run from ygt.
```

### Comparing `xgridfit-3.2.9/pyproject.toml` & `xgridfit-3.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xgridfit"
-version = "3.2.9"
+version = "3.3.0"
 authors = [
     { name="Peter S. Baker", email="b.tarde@mail.com" },
 ]
 description = "An XML-based hinting language for TrueType fonts"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.10.4"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "lxml >= 4.8.8",
```

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rnc` & `xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit-sh.rnc`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit-sh.rng` & `xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit-sh.rng`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rnc` & `xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.rnc`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.rng` & `xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.rng`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xgridfit.xsd` & `xgridfit-3.3.0/src/xgridfit/Schemas/xgridfit.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xi.xsd` & `xgridfit-3.3.0/src/xgridfit/Schemas/xi.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/Schemas/xml.xsd` & `xgridfit-3.3.0/src/xgridfit/Schemas/xml.xsd`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/arithmetic.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/arithmetic.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/compact.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/compact.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/delta.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/delta.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/expand.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/expand.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/expressions.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/expressions.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/flow.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/flow.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/func-predef.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/func-predef.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/function.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/function.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/graphics.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/graphics.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/measure.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/measure.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/messages.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/messages.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/misc.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/misc.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/move-els.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/move-els.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/move-lib.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/move-lib.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/numbers.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/numbers.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/points.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/points.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/prep.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/prep.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/primitives.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/primitives.xsl`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/std-vars.xsl`

 * *Files 0% similar despite different names*

#### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/std-vars.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/std-vars.xsl`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <xsl:stylesheet xmlns:xsl="http://www.w3.org/1999/XSL/Transform" xmlns:xgf="http://xgridfit.sourceforge.net/Xgridfit2" version="1.0" exclude-result-prefixes="xgf">
   <!--
       This file is part of xgridfit, version 3.
       Licensed under the Apache License, Version 2.0.
       Copyright (c) 2006-20 by Peter S. Baker
   -->
-  <xsl:variable name="xgf-version" select="'3.2.9'"/>
+  <xsl:variable name="xgf-version" select="'3.3.0'"/>
   <!--
       First in the Storage Area is a block of locations used by legacy
       code (e.g. from ttfautohint). Next come some
       reserved locations used by Xgridfit to track state
       information. Next is the global variable area and finally a
       growable variable frame area.
   -->
```

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/xgfdata.xml` & `xgridfit-3.3.0/src/xgridfit/XSL/xgfdata.xml`

 * *Files identical despite different names*

### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/xgridfit-ft.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/xgridfit-ft.xsl`

 * *Files 0% similar despite different names*

#### Comparing `xgridfit-3.2.9/src/xgridfit/XSL/xgridfit-ft.xsl` & `xgridfit-3.3.0/src/xgridfit/XSL/xgridfit-ft.xsl`

```diff
@@ -415,21 +415,22 @@
       <xsl:with-param name="tuple" select="."/>
     </xsl:call-template>
     <xsl:text>),</xsl:text>
   </xsl:template>
   <xsl:template match="xgf:region">
     <xsl:text>'</xsl:text>
     <xsl:value-of select="@tag"/>
-    <xsl:text>': (</xsl:text>
+    <xsl:text>': (0,</xsl:text>
+    <!-- <xsl:text>0, </xsl:text>
     <xsl:value-of select="@bot"/>
-    <xsl:text>,</xsl:text>
+    <xsl:text>, </xsl:text> -->
     <xsl:value-of select="@peak"/>
-    <xsl:text>,</xsl:text>
-    <xsl:value-of select="@top"/>
-    <xsl:text>),</xsl:text>
+    <xsl:text>, 0),</xsl:text>
+    <!-- <xsl:value-of select="@top"/>
+    <xsl:text>), </xsl:text> -->
   </xsl:template>
   <xsl:template name="get-cvar-coordinates">
     <xsl:param name="tuple"/>
     <xsl:variable name="cvvs" select="$tuple/xgf:cvv"/>
     <xsl:text>[</xsl:text>
     <xsl:for-each select="/xgf:xgridfit/xgf:control-value">
       <xsl:variable name="cvname" select="@name"/>
```

### Comparing `xgridfit-3.2.9/src/xgridfit/xgridfit.py` & `xgridfit-3.3.0/src/xgridfit/xgridfit-backup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from fontTools import ttLib
 from fontTools import subset
 from fontTools.ttLib import ttFont, tables, newTable, TTFont
 from fontTools.ttLib.tables.TupleVariation import TupleVariation
 from fontTools.ufoLib.filenames import userNameToFileName
+from fontTools.pens.hashPointPen import HashPointPen
 from lxml import etree
 from ast import literal_eval
 try:
     from .version import __version__
 except ImportError:
     from version import __version__
 try:
     from .ygridfit import ygridfit_parse, ygridfit_parse_obj
 except ImportError:
     from ygridfit import ygridfit_parse, ygridfit_parse_obj
-from tempfile import mkstemp, NamedTemporaryFile, SpooledTemporaryFile
+from .xgfUFOWriter import xgfUFOWriter
+from tempfile import SpooledTemporaryFile
 import sys
 import os
 import argparse
 import array
 import re
 import pkg_resources
 import unicodedata
@@ -28,31 +30,37 @@
 
 neutral_instructions = [ 'IUP', 'RDTG', 'ROFF', 'RTDG', 'RTG', 'RTHG', 'RUTG',
                          'SFVTCA', 'SFVTPV', 'SPVTCA', 'SVTCA', 'FLIPOFF',
                          'FLIPON' ]
 
 # How many numbers popped by each instruction (-1 means a variable number)
 
-pop_instructions = { 'ALIGNPTS': 2, 'ALIGNRP': -1, 'IP': -1, 'MDAP': 1,
-                     'MIAP': 2, 'MIRP': 2, 'MDRP': 1, 'SHP': -1, 'SLOOP': 1,
-                     'SRP0': 1, 'SRP1': 1, 'SRP2': 1, 'CALL': 1, 'SFVTL': 2,
-                     'SPVTL': 2, 'SDPVTL': 2, 'ISECT': 5, 'MSIRP': 2, 'SCFS': 2,
-                     'SCVTCI': 1, 'SFVFS': 2, 'SHC': 1, 'SHZ': 1, 'SMD': 1,
-                     'SPVFS': 2, 'SROUND': 1, 'SSW': 1, 'SSWCI': 1, 'SZP0': 1,
-                     'SZP1': 1, 'SZP2': 1, 'SZPS': 1, 'UTP': 1, 'WCVTF': 2,
-                     'WCVTP': 2, 'WS': 2 }
+pop_instructions = { 'ALIGNPTS': 2, 'ALIGNRP': -1, 'IP': -1,   'MDAP': 1,
+                     'MIAP': 2,     'MIRP': 2,     'MDRP': 1,  'SHP': -1,  'SLOOP': 1,
+                     'SRP0': 1,     'SRP1': 1,     'SRP2': 1,  'CALL': 1,  'SFVTL': 2,
+                     'SPVTL': 2,    'SDPVTL': 2,   'ISECT': 5, 'MSIRP': 2, 'SCFS': 2,
+                     'SCVTCI': 1,   'SFVFS': 2,    'SHC': 1,   'SHZ': 1,   'SMD': 1,
+                     'SPVFS': 2,    'SROUND': 1,   'SSW': 1,   'SSWCI': 1, 'SZP0': 1,
+                     'SZP1': 1,     'SZP2': 1,     'SZPS': 1,  'UTP': 1,   'WCVTF': 2,
+                     'WCVTP': 2,    'WS': 2 }
 
 byte_push_instructions = [ 'PUSHB', 'NPUSHB' ]
 
 maxInstructions = 200
 
 quietcount = 0
 
 coordinateFuzz = 1
 
+ufo_mode = False
+
+class xgfGlyphObject:
+    def __init__(self):
+        self.lib = None
+
 def get_file_path(fn):
     return pkg_resources.resource_filename(__name__, fn)
 
 def wipe_font(fo):
     """Delete all TrueType programming in the font."""
     for g_name in fo['glyf'].glyphs:
         glyph = fo['glyf'][g_name]
@@ -69,14 +77,17 @@
     except Exception:
         pass
     try:
         del fo['cvt ']
     except Exception:
         pass
 
+def wipe_font_ufo(ufo):
+    pass
+
 def install_glyph_program(nm, fo, asm):
     """ name of the glyph, the font object, the instructions in one big string."""
     try:
         global maxInstructions
         g = fo['glyf'][nm]
         g.program = tables.ttProgram.Program()
         g.program.fromAssembly(asm)
@@ -84,14 +95,33 @@
         if b > maxInstructions:
             maxInstructions = b
     except KeyError:
         print("Unable to install glyph '" + nm + "'. Make sure the glyph's")
         print("name is correct and that it exists in the font.")
         sys.exit(1)
 
+def install_glyph_program_ufo(uw, gnm, asm, hash):
+    try:
+        global maxInstructions
+        p = tables.ttProgram.Program()
+        p.fromAssembly(asm)
+        b = len(p.getBytecode())
+        if b > maxInstructions:
+            maxInstructions = b
+        uw.install_glyph_program(gnm, hash, asm)
+        #glyph = ufo[nm]
+        #if not "public.truetype.instructions" in glyph.lib:
+        #    glyph.lib["public.truetype.instructions"] = {}
+        #glyph.lib["public.truetype.instructions"]["formatVersion"] = "1"
+        #glyph.lib["public.truetype.instructions"]["assembly"] = str(asm)
+    except Exception as e:
+        print("error in install_glyph_program_ufo:")
+        print(e.args)
+        print(e)
+
 def is_number(s):
     try:
         int(s)
         return True
     except ValueError:
         return False
 
@@ -189,27 +219,66 @@
         assert base == len(fo['cvt '].values)
         for c in cvs:
             fo['cvt '].values.append(c)
     else:
         fo['cvt '] = ttFont.newTable('cvt ')
         setattr(fo['cvt '],'values',array.array('h', cvs))
 
+def install_cvt_ufo(uw, ufo_lib_tree, cvs, base):
+    #cvt_dict = {}
+    #if base > 0:
+    #    cvt_index = base
+    #    try:
+    #        old_cvt_dict = ufo.lib["public.truetype.instructions"]["controlValue"]
+    #    except Exception:
+    #        old_cvt_dict = {}
+    #else:
+    #    cvt_index = 0
+    #for c in cvs:
+    #    cvt_dict[str(cvt_index)] = c
+    #    cvt_index += 1
+    #if base > 0:
+    #    cvt_dict.update(old_cvt_dict)
+    uw.install_cvt(ufo_lib_tree, cvs)
+    #if base == 0 or not "public.truetype.instructions" in ufo.lib:
+    #    ufo.lib["public.truetype.instructions"] = {}
+    #ufo.lib["public.truetype.instructions"]["formatVersion"] = "1"
+    #ufo.lib["public.truetype.instructions"]["controlValue"] = cvt_dict
+
 def install_functions(fo, fns, base):
     """If base greater than zero, we append our own functions to those already
     in the font. If not, generate a new fpgm table."""
     if base > 0:
         oldfpgm = "\n".join(fo['fpgm'].program.getAssembly())
         newfpgm = oldfpgm + "\n" + str(fns)
         fo['fpgm'].program.fromAssembly(newfpgm)
         fo['fpgm'].program.getBytecode()
     else:
         fo['fpgm'] = ttFont.newTable('fpgm')
         fo['fpgm'].program = tables.ttProgram.Program()
         fo['fpgm'].program.fromAssembly(str(fns))
 
+def install_functions_ufo(uw, ufo_lib_tree, fns, base):
+    #oldfpgm = ""
+    #if base > 0:
+    #    try:
+    #        oldfpgm = "\n".join(ufo.lib["public.truetype.instructions"]["fontProgram"])
+    #    except Exception as e:
+    #        print("error in install_functions_ufo:")
+    #        print(e.args)
+    #        print(e)
+    #        pass
+    #newfpgm = oldfpgm + str(fns)
+    uw.install_lib_item(ufo_lib_tree, "fontProgram", fns)
+    #if not "public.truetype.instructions" in ufo.lib:
+    #    ufo.lib["public.truetype.instructions"] = {}
+    #ufo.lib["public.truetype.instructions"]["formatVersion"] = "1"
+    #ufo.lib["public.truetype.instructions"]["fontProgram"] = newfpgm
+
+
 def install_prep(fo, pr, keepold, replace):
     """If keepold is True, we append our own prep table to the existing one.
     It is up to the Xgridfit programmer to make sure that no conflicts arise
     (though if there's a duplication--for example, instructions being disabled
     at a different ppem in the new code than in the old, the new code will
     take precedence.)"""
     if keepold and not replace:
@@ -217,14 +286,49 @@
         newprep = oldprep + "\n" + str(pr)
         fo['prep'].program.fromAssembly(newprep)
     else:
         fo['prep'] = ttFont.newTable('prep')
         fo['prep'].program = tables.ttProgram.Program()
         fo['prep'].program.fromAssembly(str(pr))
 
+def install_prep_ufo(uw, ufo_lib_tree, pr, keepold, replace):
+    #oldprep = ""
+    #if keepold and not replace:
+    #    try:
+    #        oldprep = "\n".join(ufo.lib["public.truetype.instructions"]["controlValueProgram"])
+    #    except Exception as e:
+    #        print("error in install_prep_ufo:")
+    #        print(e.args)
+    #        print(e)
+    #        # pass
+    #newprep = oldprep + str(pr)
+    uw.install_lib_item(ufo_lib_tree, "controlValueProgram", pr)
+    #if not "public.truetype.instructions" in ufo.lib:
+    #    ufo.lib["public.truetype.instructions"] = {}
+    #ufo.lib["public.truetype.instructions"]["formatVersion"] = "1"
+    #ufo.lib["public.truetype.instructions"]["controlValueProgram"] = newprep
+
+def install_properties_ufo(uw, ufo_lib_tree, d):
+    # keys can be:
+    # maxFunctionDefs: int
+    # maxInstructionDefs: int
+    # maxStackElements: int
+    # maxStorage: int
+    # maxSizeOfInstructions: int
+    # maxTwilightPoints: int
+    # maxZones: int
+    #if not "public.truetype.instructions" in ufo.lib:
+    #    ufo.lib["public.truetype.instructions"] = {}
+    #ufo.lib["public.truetype.instructions"]["formatVersion"] = "1"
+    k = d.keys()
+    for kk in k:
+        uw.install_lib_item(ufo_lib_tree, kk, d[kk])
+        # ufo.lib["public.truetype.instructions"][kk] = d[kk]
+    
+
 # Compare two dictionaries. It would be easier to do an equality test, but
 # I can't be sure two otherwise matching dictionaries aren't in a different
 # order.
 
 def _axes_match(dict1, dict2):
     try:
         assert len(dict1) == len(dict2)
@@ -336,28 +440,37 @@
 
 def make_coordinate_index(glist, fo):
     """ Make an index for lookup by coordinates. The key will look like:
         glyphname@123x456
      glyph list, the font object. 
     """
     coordinateIndex = {}
+    bad_glyphs = []
     for gn in glist:
-        currentGlyph = fo['glyf'][gn]
-        if not currentGlyph.isComposite():
-            c = currentGlyph.getCoordinates(fo['glyf'])
-            pointIndex = 0
-            for point in zip(c[0], c[2]):
-                if point[1] & 0x01 == 0x01:
-                    pp = gn + "@" + str(point[0]).replace('(','').replace(')','').replace(',','x').replace(' ','')
-                    coordinateIndex[pp] = pointIndex
-                pointIndex += 1
-    return coordinateIndex
+        try:
+            currentGlyph = fo['glyf'][gn]
+            if not currentGlyph.isComposite():
+                c = currentGlyph.getCoordinates(fo['glyf'])
+                pointIndex = 0
+                for point in zip(c[0], c[2]):
+                    if point[1] & 0x01 == 0x01:
+                        pp = gn + "@" + str(point[0]).replace('(','').replace(')','').replace(',','x').replace(' ','')
+                        coordinateIndex[pp] = pointIndex
+                    pointIndex += 1
+        except Exception as e:
+            print("Error in glyph " + str(gn))
+            print("Removing it from glyphs list")
+            bad_glyphs.append(gn)
+    if len(bad_glyphs) > 0:
+        for gn in bad_glyphs:
+            glist.remove(gn)
+    return coordinateIndex, bad_glyphs
 
 def make_reverse_coordinate_index(glist, fo):
-    idx = make_coordinate_index(glist, fo)
+    idx, bad = make_coordinate_index(glist, fo)[0]
     return {val: key for key, val in idx.items()}
 
 def rewrite_point_string(original_point_string, coordinateIndex, coord_pattern, glyph_name,
                          xoffset, yoffset, crash=True):
     """ Determines whether original_point_string is a pair of coordinates for
         a point, and if so, looks up the point number in coordinateIndex. If
         not, simply returns the original value. In theory, this should leave
@@ -385,32 +498,34 @@
         except KeyError:
             point_number = coordinateFuzzyMatch(coord_id, coordinateIndex)
             try:
                 int(point_number)
             except TypeError:
                 if crash:
                     print("In glyph " + glyph_name + ", can't resolve coordinates " + matched_string)
-                    sys.exit(1)
+                    # sys.exit(1)
+                    return original_point_string, False
                 else:
                     if quietcount < 2:
                         print("Can't resolve coordinate " + original_point_string + "; falling back to value")
-                    raise Exception("Can't resolve coordinate")
+                    # raise Exception("Can't resolve coordinate")
+                    return original_point_string, False
 
         # Reassemble the expression.
         string_counter = 0
         substitute_string = ""
         for string_bit in split_string:
             if string_counter == string_index:
                 substitute_string = substitute_string + str(point_number)
             else:
                 substitute_string = substitute_string + string_bit
             string_counter += 1
-        return substitute_string
+        return substitute_string, True
     else:
-        return original_point_string
+        return original_point_string, True
 
 def coordinateFuzzyMatch(coordID, coordinateIndex):
     # This is an extremely inefficient search, executed only if no match found
     # without it. Construct a box around the coordinate (default is 2x2), and
     # for each position in that box, construct a potential key for
     # coordinateIndex. If we find a match, we issue a warning and go on. If
     # not, return None and (probably) crash.
@@ -439,243 +554,675 @@
         Xcounter += 1
     return None
 
 def coordinates_to_points(glist, xgffile, coordinateIndex, ns):
     """ glyph list, xgf program, coordinate index, namespaces.
         surveys all the glyph programs in the file and changes coordinate
         pairs (e.g. {125;-3}) to point numbers. """
+    bad_glyphs = []
     coord_pattern = re.compile(r'(\{[0-9\-]{1,4};[0-9\-]{1,4}\})')
     gPathString = "/xgf:xgridfit/xgf:glyph[@ps-name='{gnm}']"
     for gn in glist:
+        good_val = True
         try:
             xoffset = xgffile.xpath(gPathString.format(gnm=gn), namespaces=ns)[0].attrib['xoffset']
         except (KeyError, IndexError):
             xoffset = "0"
         try:
             yoffset = xgffile.xpath(gPathString.format(gnm=gn), namespaces=ns)[0].attrib['yoffset']
         except (KeyError, IndexError):
             yoffset = "0"
 
         points = xgffile.xpath((gPathString + "/descendant::xgf:point").format(gnm=gn), namespaces=ns)
         for p in points:
-            p.attrib['num'] = rewrite_point_string(p.attrib['num'],
-                                                   coordinateIndex,
-                                                   coord_pattern,
-                                                   gn,
-                                                   xoffset,
-                                                   yoffset)
+            p.attrib['num'], good_val = rewrite_point_string(p.attrib['num'],
+                                                             coordinateIndex,
+                                                             coord_pattern,
+                                                             gn,
+                                                             xoffset,
+                                                             yoffset)
         wparams = xgffile.xpath((gPathString + "/descendant::xgf:with-param").format(gnm=gn), namespaces=ns)
         for p in wparams:
             try:
-                # print(gn + ": converting " + p.attrib['value'])
-                p.attrib['value'] = rewrite_point_string(p.attrib['value'],
-                                                         coordinateIndex,
-                                                         coord_pattern,
-                                                         gn,
-                                                         xoffset,
-                                                         yoffset)
+                p.attrib['value'], good_val = rewrite_point_string(p.attrib['value'],
+                                                                   coordinateIndex,
+                                                                   coord_pattern,
+                                                                   gn,
+                                                                   xoffset,
+                                                                   yoffset)
             except:
                 pass
 
         params = xgffile.xpath((gPathString + "/descendant::xgf:param").format(gnm=gn), namespaces=ns)
         for p in params:
-            p.attrib['value'] = rewrite_point_string(p.attrib['value'],
-                                                     coordinateIndex,
-                                                     coord_pattern,
-                                                     gn,
-                                                     xoffset,
-                                                     yoffset)
+            p.attrib['value'], good_val = rewrite_point_string(p.attrib['value'],
+                                                               coordinateIndex,
+                                                               coord_pattern,
+                                                               gn,
+                                                               xoffset,
+                                                               yoffset)
 
         constants = xgffile.xpath((gPathString + "/descendant::xgf:constant").format(gnm=gn), namespaces=ns)
         for c in constants:
             orig_value = c.attrib['value']
             try:
                 orig_coord = c.attrib['coordinate']
-                point_num = rewrite_point_string(orig_coord,
-                                                 coordinateIndex,
-                                                 coord_pattern,
-                                                 gn,
-                                                 xoffset,
-                                                 yoffset,
-                                                 False)
+                point_num, good_val = rewrite_point_string(orig_coord,
+                                                           coordinateIndex,
+                                                           coord_pattern,
+                                                           gn,
+                                                           xoffset,
+                                                           yoffset,
+                                                           False)
                 if str(point_num) != orig_value:
                     if quietcount < 2:
                         print("Warning: In glyph '" + gn + "', changing value " + orig_value + " to " +
                               str(point_num) + " after coordinate " + orig_coord)
                     c.attrib['value'] = str(point_num)
             except:
-                c.attrib['value'] = rewrite_point_string(orig_value,
-                                                         coordinateIndex,
-                                                         coord_pattern,
-                                                         gn,
-                                                         xoffset,
-                                                         yoffset)
+                c.attrib['value'], good_val = rewrite_point_string(orig_value,
+                                                                   coordinateIndex,
+                                                                   coord_pattern,
+                                                                   gn,
+                                                                   xoffset,
+                                                                   yoffset)
+        if not good_val:
+            bad_glyphs.append(gn)
+    if len(bad_glyphs):
+        for b in bad_glyphs:
+            del glist[b]
+    return bad_glyphs
 
 def validate(f, syntax, noval):
     if noval and quietcount < 1:
         print("Skipping validation")
     else:
         schemadir = "Schemas/"
         schemafile = "xgridfit.rng"
         if syntax == "compact":
             schemafile = "xgridfit-sh.rng"
         schemapath = get_file_path(schemadir + schemafile)
         schema = etree.RelaxNG(etree.parse(schemapath))
         schema.assertValid(f)
 
-def compile_all(font, yaml, new_file_name):
+def compile_list(font: ttFont, yaml: dict, gname: str) -> tuple:
+    """
+        Compile code either for a single glyph or a list of glyphs. This will
+        generate a hinted font (as a SpooledTemporaryFile) with *only* those glyphs
+        in it. It returns this open file, plus a name:gid dict and a list of
+        glyphs that failed to compile.
+    """
+    # No output to console.
+    failed_glyph_list = []
+    global quietcount
+    quietcount = 3
+    if type(gname) is list:
+        xgffile = ygridfit_parse_obj(yaml, glyph_list=gname)
+    else:
+        xgffile = ygridfit_parse_obj(yaml, single_glyph=gname)
+    ns = {"xgf": "http://xgridfit.sourceforge.net/Xgridfit2",
+          "xi": "http://www.w3.org/2001/XInclude",
+          "xsl": "http://www.w3.org/1999/XSL/Transform"}
+    thisFont = font
+    wipe_font(thisFont)
+    xslfile = etree.parse(get_file_path("XSL/xgridfit-ft.xsl"))
+    etransform = etree.XSLT(xslfile)
+    if type(gname) is str:
+        glyph_list = [gname]
+    else:
+        glyph_list = gname
+    coordinateIndex, bad = make_coordinate_index(glyph_list, thisFont)
+    if len(bad):
+        failed_glyph_list.extend(bad)
+    bad = coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    if len(bad):
+        failed_glyph_list.extend(bad)
+    safe_calls = etransform(xgffile, **{"stack-safe-list": "'yes'"})
+    safe_calls = literal_eval(str(safe_calls))
+    cvt_list = str(etransform(xgffile, **{"get-cvt-list": "'yes'"}))
+    cvt_list = literal_eval("[" + cvt_list + "]")
+    install_cvt(thisFont, cvt_list, 0)
+    cvar_count = len(xgffile.xpath("/xgf:xgridfit/xgf:cvar", namespaces=ns))
+    if cvar_count > 0:
+        tuple_store = literal_eval(str(etransform(xgffile, **{"get-cvar": "'yes'"})))
+        install_cvar(thisFont, tuple_store, False, 0)
+    predef_functions = int(xslfile.xpath("/xsl:stylesheet/xsl:variable[@name='predefined-functions']",
+                                         namespaces=ns)[0].attrib['select'])
+    maxFunction = etransform(xgffile, **{"function-count": "'yes'"})
+    maxFunction = int(maxFunction) + predef_functions
+    thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
+    thisFont['maxp'].maxTwilightPoints = 25
+    thisFont['maxp'].maxStorage = 64
+    thisFont['maxp'].maxStackElements = 256
+    thisFont['maxp'].maxFunctionDefs = maxFunction
+    thisFont['head'].flags |= 0b0000000000001000
+    fpgm_code = etransform(xgffile, **{"fpgm-only": "'yes'"})
+    install_functions(thisFont, fpgm_code, 0)
+    prep_code = etransform(xgffile, **{"prep-only": "'yes'"})
+    install_prep(thisFont, prep_code, False, True)
+    for g in glyph_list:
+        try:
+            gt = "'" + g + "'"
+            glyph_args = {'singleGlyphId': gt}
+            #if initgraphics:
+            #    glyph_args['init_graphics'] = "'" + initgraphics + "'"
+            g_inst = etransform(xgffile, **glyph_args)
+            # g_inst_final = compact_instructions(str(g_inst), safe_calls)
+            # install_glyph_program(g, thisFont, g_inst_final)
+            # g_inst_final = str(g_inst)
+            # install_glyph_program(g, thisFont, g_inst_final)
+            install_glyph_program(g, thisFont, str(g_inst))
+        except Exception as e:
+            print(e)
+            for entry in etransform.error_log:
+                if quietcount < 3:
+                    print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+            failed_glyph_list.append(g)
+    try:
+        # Grab the font, subset it with just the one glyph we're
+        # previewing, and write it to a spooled temporary file.
+        tf = SpooledTemporaryFile(max_size=1000000, mode='b')
+        options = subset.Options(glyph_names=True)
+        options.layout_features = ["*"]
+        subsetter = subset.Subsetter(options)
+        subsetter.populate(glyphs=glyph_list)
+        subsetter.subset(thisFont)
+        glyph_id = {}
+        for g in glyph_list:
+            glyph_id[g] = thisFont.getGlyphID(g)
+        # temp diagnostic:
+        # thisFont.save("temp_font.ttf", 1)
+        thisFont.save(tf, 1)
+        tf.seek(0)
+    except Exception as e:
+        print(e)
+    # Return: a handle to the temp file, the index of the target glyph, a list of
+    # glyphs for which complilation failed
+    return tf, glyph_id, failed_glyph_list
+
+def compile_all(font: ttFont, yaml: dict, new_file_name: str) -> list:
+    global ufo_mode
+    failed_glyph_list = []
     xgffile = ygridfit_parse_obj(yaml)
     ns = {"xgf": "http://xgridfit.sourceforge.net/Xgridfit2",
           "xi": "http://www.w3.org/2001/XInclude",
           "xsl": "http://www.w3.org/1999/XSL/Transform"}
-    # thisFont = ttLib.TTFont(font)
+    split_fn = os.path.splitext(new_file_name)
+    extension = split_fn[1]
+    ufo_mode = (extension == ".ufo")
     thisFont = font
     functionBase = 0     # Offset to account for functions in existing font
     cvtBase      = 0     # Offset to account for CVs in existing font
     storageBase  = 0     # Offset to account for storage in existing font
     maxStack     = 256   # Our (generous) default stack size
     twilightBase = 0     # Offset to account for twilight space in existing font
     wipe_font(thisFont)
     xslfile = etree.parse(get_file_path("XSL/xgridfit-ft.xsl"))
     etransform = etree.XSLT(xslfile)
-    # glyph_list = [gname]
     glyph_list = str(etransform(xgffile, **{"get-glyph-list": "'yes'"}))
     glyph_list = list(glyph_list.split(" "))
-    coordinateIndex = make_coordinate_index(glyph_list, thisFont)
-    coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    coordinateIndex, bad = make_coordinate_index(glyph_list, thisFont)
+    if len(bad) > 0:
+        failed_glyph_list.extend(bad)
+    bad = coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    if len(bad) > 0:
+        failed_glyph_list.extend(bad)
     safe_calls = etransform(xgffile, **{"stack-safe-list": "'yes'"})
     safe_calls = literal_eval(str(safe_calls))
     cvt_list = str(etransform(xgffile, **{"get-cvt-list": "'yes'"}))
     cvt_list = literal_eval("[" + cvt_list + "]")
-    install_cvt(thisFont, cvt_list, cvtBase)
+    uw = None
+    if ufo_mode:
+        uw = xgfUFOWriter(new_file_name)
+    ufo_lib_tree = None
+    if ufo_mode:
+        ufo_lib_tree = uw.open_lib()
+        uw.install_cvt(ufo_lib_tree, cvt_list)
+        # install_cvt_ufo(uw, ufo_lib_tree, cvt_list, cvtBase)
+    else:
+        install_cvt(thisFont, cvt_list, cvtBase)
+
     cvar_count = len(xgffile.xpath("/xgf:xgridfit/xgf:cvar", namespaces=ns))
-    if cvar_count > 0:
+    if cvar_count > 0 and not ufo_mode:
         tuple_store = literal_eval(str(etransform(xgffile, **{"get-cvar": "'yes'"})))
         install_cvar(thisFont, tuple_store, False, cvtBase)
     predef_functions = int(xslfile.xpath("/xsl:stylesheet/xsl:variable[@name='predefined-functions']",
                                          namespaces=ns)[0].attrib['select'])
     maxFunction = etransform(xgffile, **{"function-count": "'yes'"})
     maxFunction = int(maxFunction) + predef_functions + functionBase
-    thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
-    thisFont['maxp'].maxTwilightPoints = twilightBase + 25
-    thisFont['maxp'].maxStorage = storageBase + 64
-    thisFont['maxp'].maxStackElements = maxStack
-    thisFont['maxp'].maxFunctionDefs = maxFunction
-    thisFont['head'].flags |= 0b0000000000001000
     fpgm_code = etransform(xgffile, **{"fpgm-only": "'yes'"})
-    install_functions(thisFont, fpgm_code, functionBase)
+    if ufo_mode:
+        install_functions_ufo(uw, ufo_lib_tree, fpgm_code, functionBase)
+    else:
+        install_functions(thisFont, fpgm_code, functionBase)
     prep_code = etransform(xgffile, **{"prep-only": "'yes'"})
-    install_prep(thisFont, prep_code, False, True)
-    failed_glyph_list = []
+    if ufo_mode:
+        install_prep_ufo(uw, ufo_lib_tree, prep_code, False, True)
+    else:
+        install_prep(thisFont, prep_code, False, True)
     for g in glyph_list:
         try:
             gt = "'" + g + "'"
             glyph_args = {'singleGlyphId': gt}
             #if initgraphics:
             #    glyph_args['init_graphics'] = "'" + initgraphics + "'"
             g_inst = etransform(xgffile, **glyph_args)
             g_inst_final = compact_instructions(str(g_inst), safe_calls)
-            install_glyph_program(g, thisFont, g_inst_final)
+            if ufo_mode:
+                ttglyph = thisFont['glyf'][g]
+                ttwidth = thisFont["hmtx"][g][0]
+                hash_pen = HashPointPen(ttwidth, thisFont.getGlyphSet())
+                ttglyph.drawPoints(hash_pen, thisFont["glyf"])
+                install_glyph_program_ufo(uw, g, g_inst_final, hash_pen.hash)
+            else:
+                install_glyph_program(g, thisFont, g_inst_final)
         except Exception as e:
+            print("error in compile_all:")
+            print(e.args)
             print(e)
             for entry in etransform.error_log:
-                print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+                if quietcount < 3:
+                    print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
             # sys.exit(1)
             failed_glyph_list.append(g)
-    with thisFont as f:
-        f.save(new_file_name, 1)
+    try:
+        if ufo_mode:
+            d = {"maxSizeOfInstructions": maxInstructions + 50,
+                 "maxTwilightPoints": twilightBase + 25,
+                 "maxStorage": 64,
+                 "maxStackElements": maxStack,
+                 "maxFunctionDefs": maxFunction}
+            install_properties_ufo(uw, ufo_lib_tree, d)
+            uw.save_lib(ufo_lib_tree)
+        else:
+            thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
+            thisFont['maxp'].maxTwilightPoints = twilightBase + 25
+            thisFont['maxp'].maxStorage = storageBase + 64
+            thisFont['maxp'].maxStackElements = maxStack
+            thisFont['maxp'].maxFunctionDefs = maxFunction
+            thisFont['head'].flags |= 0b0000000000001000
+            with thisFont as f:
+                f.save(new_file_name, 1)
+    except Exception as e:
+        print("Error while installing maxp and head settings:")
+        print(e.args)
+        print(e)
     return failed_glyph_list
 
-def compile_one(font, yaml, gname):
-    """ A quick and dirty function to support the GUI. It compiles code for a
-        single glyph (or a list) and generates the font with that code (and supporting
-        stuff--cvt, cvar, prep, fpgm, maxp). This can then be used to display
-        a preview of the glyph.
-    """
-    if type(gname) is list:
-        xgffile = ygridfit_parse_obj(yaml, glyph_list=gname)
+
+def run(
+        inputfile,
+        quiet = -1,
+        outputfile = None,
+        inputfont = None,
+        outputfont = None,
+        skipval = False,
+        skipcomp = False,
+        expandonly = False,
+        compactonly = False,
+        yconvonly = False,
+        mergemode = False,
+        initgraphics = "yes",
+        assume_y = "no",
+        glyphlist = None,
+        replaceprep = False,
+        saveprograms = False,
+        nocompact = False,
+        cfuzz = 1,
+        source: str = "xgf",
+        font: ttFont = None,
+        yaml: dict = None,
+    ):
+
+    # Return a tuple: (error_msg: str, failed glyphs: list)
+
+    global maxInstructions, quietcount, ufo_mode, coordinateFuzz
+
+    if quiet >= 0:
+        quietcount = quiet
+
+    if quietcount < 1:
+        print("Opening the Xgridfit file ...")
+
+    failed_glyph_list = []
+
+    if cfuzz > 1:
+        coordinateFuzz = cfuzz
+
+    source_ext = os.path.splitext(inputfile)[1]
+    if source_ext == ".yaml":
+        if quietcount < 1:
+            print("Converting yaml source to Xgridfit")
+        xgffile = ygridfit_parse(inputfile)
     else:
-        xgffile = ygridfit_parse_obj(yaml, single_glyph=gname)
+        xgffile = etree.parse(inputfile)
+
+    # We'll need namespaces
+
     ns = {"xgf": "http://xgridfit.sourceforge.net/Xgridfit2",
           "xi": "http://www.w3.org/2001/XInclude",
           "xsl": "http://www.w3.org/1999/XSL/Transform"}
-    thisFont = font
+    
+    split_fn = os.path.splitext(outputfont)
+    extension = split_fn[1]
+    ufo_mode = (extension == ".ufo")
+
+    # Next determine whether we are using long tagnames or short. Best way
+    # is to find out which tag is used for the required <pre-program> (<prep>)
+    # element. If we don't find it, print an error message and exit. Here's
+    # where we validate too; and if we're only expanding or compacting a file,
+    # do that and exit before we go to the trouble of opening the font.
+    if quietcount < 1:
+        print("Validating ...")
+
+    # This block validates XGF code, expands compact to normal pre-compilation,
+    # checks for the presence of a prep program, and saves transformed code if
+    # necessary, including converted ygt code. None of this is necessary if
+    # source if ygt.
+    if source == "xgf":
+        if len(xgffile.xpath("/xgf:xgridfit/xgf:prep", namespaces=ns)):
+            # first validate
+            validate(xgffile, "compact", skipval)
+            # as we can't use the compact syntax, always expand
+            if quietcount < 1:
+                print("Expanding compact to normal syntax ...")
+            xslfile = get_file_path("XSL/expand.xsl")
+            etransform = etree.XSLT(etree.parse(xslfile))
+            xgffile = etransform(xgffile)
+            if expandonly:
+                tstr = str(xgffile)
+                tstr = tstr.replace('xgf:','')
+                tstr = tstr.replace('xmlns:xgf="http://xgridfit.sourceforge.net/Xgridfit2"','')
+                if outputfile:
+                    of = open(outputfile, "w")
+                    of.write(tstr)
+                    of.close()
+                else:
+                    print(tstr)
+                sys.exit(0)
+        elif len(xgffile.xpath("/xgf:xgridfit/xgf:pre-program", namespaces=ns)):
+            # validate(xgffile, "normal", skipval)
+            if compactonly or yconvonly:
+                if compactonly:
+                    xslfile = get_file_path("XSL/compact.xsl")
+                    etransform = etree.XSLT(etree.parse(xslfile))
+                    xgffile = etransform(xgffile)
+                    tstr = str(xgffile)
+                    tstr = tstr.replace('xgf:','')
+                    tstr = tstr.replace('xmlns:xgf="http://xgridfit.sourceforge.net/Xgridfit2"','')
+                    tstr = tstr.replace(' >','>')
+                if yconvonly:
+                    tstr = str(etree.tostring(xgffile).decode())
+                    # tstr = str(xgffile)
+                if outputfile:
+                    of = open(outputfile, "w")
+                    of.write(tstr)
+                    of.close()
+                else:
+                    print(tstr)
+                sys.exit(0)
+        else:
+            print("The xgridfit program must contain a pre-program (prep) element,")
+            print("even if it's empty.")
+            sys.exit(1)
+
+    # Don't do this if called from ygt.
+    if source == "ygt" and skipcomp and quietcount < 1:
+        print("Skipping compilation")
+        sys.exit(0)
+
+    # Now open the font. If in xgf mode, we open a file. If ygt, we operate
+    # on the fontTools font passed to us in the font parameter.
+
+    if source == "xgf":
+        if quietcount < 1:
+            print("Opening and evaluating the font ...")
+        if not inputfont:
+            inputfont = xgffile.xpath("/xgf:xgridfit/xgf:inputfont/text()", namespaces=ns)[0]
+        if not inputfont:
+            err = "No font to read"
+            return (err, failed_glyph_list)
+        thisFont = ttLib.TTFont(inputfont)
+    else:
+        thisFont = font
+
+    # If we're in merge-mode, we need to know some things about the current state
+    # of it; otherwise we just wipe it.
+
     functionBase = 0     # Offset to account for functions in existing font
     cvtBase      = 0     # Offset to account for CVs in existing font
     storageBase  = 0     # Offset to account for storage in existing font
     maxStack     = 256   # Our (generous) default stack size
     twilightBase = 0     # Offset to account for twilight space in existing font
-    wipe_font(thisFont)
+    if mergemode:
+        maxInstructions = max(maxInstructions, thisFont['maxp'].maxSizeOfInstructions)
+        storageBase = thisFont['maxp'].maxStorage
+        maxStack = max(maxStack, thisFont['maxp'].maxStackElements)
+        functionBase = thisFont['maxp'].maxFunctionDefs
+        twilightBase = thisFont['maxp'].maxTwilightPoints
+        try:
+            cvtBase = len(getattr(thisFont['cvt '], 'values'))
+        except:
+            cvtBase = 0
+    else:
+        wipe_font(thisFont)
+
+    # Get the xsl file, change some defaults (only relevant in merge-mode),
+    # and get a transform object
+
     xslfile = etree.parse(get_file_path("XSL/xgridfit-ft.xsl"))
+    if mergemode:
+        xslfile.xpath("/xsl:stylesheet/xsl:param[@name='function-base']",
+                      namespaces=ns)[0].attrib['select'] = str(functionBase)
+        xslfile.xpath("/xsl:stylesheet/xsl:param[@name='cvt-base']",
+                      namespaces=ns)[0].attrib['select'] = str(cvtBase)
+        xslfile.xpath("/xsl:stylesheet/xsl:param[@name='storage-base']",
+                      namespaces=ns)[0].attrib['select'] = str(storageBase)
     etransform = etree.XSLT(xslfile)
-    if type(gname) is str:
-        glyph_list = [gname]
+
+    # Get a list of the glyphs to compile
+
+    if quietcount < 1:
+        print("Getting glyph list ...")
+
+    if glyphlist:
+        # a list passed in as a command-line argument. If called from ygt,
+        # we won't have this.
+        glyph_list = glyphlist
     else:
-        glyph_list = gname
-    coordinateIndex = make_coordinate_index(glyph_list, thisFont)
-    coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+        # all the glyph programs in the file
+        glyph_list = str(etransform(xgffile, **{"get-glyph-list": "'yes'"}))
+    glyph_list = list(glyph_list.split(" "))
+    no_compact_list = str(etransform(xgffile, **{"get-no-compact-list": "'yes'"}))
+    if no_compact_list == None:
+        no_compact_list = []
+    else:
+        no_compact_list = list(no_compact_list.split(" "))
+
+    # Now that we have a glyph list, we can make the coordinate index
+    # and substitute point numbers for coordinates.
+
+    coordinateIndex, bad = make_coordinate_index(glyph_list, thisFont)
+    if len(bad):
+        failed_glyph_list.extend(bad)
+    bad = coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    if len(bad):
+        failed_glyph_list.extend(bad)
+
+    # Back to the xgf file. We're also going to need a list of stack-safe
+    # functions in this font.
+
+    if quietcount < 1:
+        print("Getting list of safe function calls ...")
+
     safe_calls = etransform(xgffile, **{"stack-safe-list": "'yes'"})
     safe_calls = literal_eval(str(safe_calls))
+
+    # If this is ufo_mode, open the ufo with xgfUFOWriter.
+    uw = None
+    if ufo_mode:
+        uw = xgfUFOWriter(outputfont)
+
+    # Get cvt
+
+    if quietcount < 1:
+        print("Building control-value table ...")
+
     cvt_list = str(etransform(xgffile, **{"get-cvt-list": "'yes'"}))
     cvt_list = literal_eval("[" + cvt_list + "]")
-    install_cvt(thisFont, cvt_list, cvtBase)
+    ufo_lib_tree = None
+    if ufo_mode:
+        ufo_lib_tree = uw.open_lib()
+        uw.install_cvt(ufo_lib_tree, cvt_list)
+    else:
+        install_cvt(thisFont, cvt_list, cvtBase)
+
+    # Test whether we have a cvar element (i.e. this is a variable font)
+
     cvar_count = len(xgffile.xpath("/xgf:xgridfit/xgf:cvar", namespaces=ns))
-    if cvar_count > 0:
+    if cvar_count > 0 and not ufo_mode:
+        if quietcount < 1:
+            print("Building cvar table ...")
         tuple_store = literal_eval(str(etransform(xgffile, **{"get-cvar": "'yes'"})))
-        install_cvar(thisFont, tuple_store, False, cvtBase)
+        install_cvar(thisFont, tuple_store, mergemode, cvtBase)
+
+    if quietcount < 1:
+        print("Building fpgm table ...")
+
     predef_functions = int(xslfile.xpath("/xsl:stylesheet/xsl:variable[@name='predefined-functions']",
                                          namespaces=ns)[0].attrib['select'])
     maxFunction = etransform(xgffile, **{"function-count": "'yes'"})
     maxFunction = int(maxFunction) + predef_functions + functionBase
-    thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
-    thisFont['maxp'].maxTwilightPoints = twilightBase + 25
-    thisFont['maxp'].maxStorage = storageBase + 64
-    thisFont['maxp'].maxStackElements = maxStack
-    thisFont['maxp'].maxFunctionDefs = maxFunction
-    thisFont['head'].flags |= 0b0000000000001000
+
     fpgm_code = etransform(xgffile, **{"fpgm-only": "'yes'"})
-    install_functions(thisFont, fpgm_code, functionBase)
+    if ufo_mode:
+        install_functions_ufo(uw, ufo_lib_tree, fpgm_code, functionBase)
+    else:
+        install_functions(thisFont, fpgm_code, functionBase)
+
+    if saveprograms:
+        instf = open("fpgm.instructions", "w")
+        instf.write(str(fpgm_code))
+        instf.close
+
+    if quietcount < 1:
+        print("Building prep table ...")
+
     prep_code = etransform(xgffile, **{"prep-only": "'yes'"})
-    install_prep(thisFont, prep_code, False, True)
-    failed_glyph_list = []
+    if ufo_mode:
+        install_prep_ufo(uw, ufo_lib_tree, prep_code, False, True)
+    else:
+        install_prep(thisFont, prep_code, mergemode, replaceprep)
+
+    if saveprograms:
+        instf = open("prep.instructions", "w")
+        instf.write(str(prep_code))
+        instf.close
+
+    # Now loop through the glyphs for which there is code.
+
+    cycler = 0
     for g in glyph_list:
+        if quietcount < 1:
+            print("Processing glyph " + g)
+        elif quietcount < 2 and cycler == 4:
+            print(".", end=" ", flush=True)
+        cycler += 1
+        if cycler == 5:
+            cycler = 0
         try:
             gt = "'" + g + "'"
             glyph_args = {'singleGlyphId': gt}
-            #if initgraphics:
-            #    glyph_args['init_graphics'] = "'" + initgraphics + "'"
+            if initgraphics:
+                glyph_args['init_graphics'] = "'" + initgraphics + "'"
+            if assume_y:
+                glyph_args['assume-always-y'] = "'" + assume_y + "'"
             g_inst = etransform(xgffile, **glyph_args)
-            g_inst_final = compact_instructions(str(g_inst), safe_calls)
-            install_glyph_program(g, thisFont, g_inst_final)
         except Exception as e:
             print(e)
             for entry in etransform.error_log:
-                print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+                if quietcount < 3:
+                    print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+            # sys.exit(1)
             failed_glyph_list.append(g)
+            continue
+        # Two lines added for (possible) debugging
+        for entry in etransform.error_log:
+            if quietcount < 3:
+                print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+        if nocompact or g in no_compact_list:
+            g_inst_final = str(g_inst)
+        else:
+            g_inst_final = compact_instructions(str(g_inst), safe_calls)
+        if ufo_mode:
+            ttglyph = thisFont['glyf'][g]
+            ttwidth = thisFont["hmtx"][g][0]
+            hash_pen = HashPointPen(ttwidth, thisFont.getGlyphSet())
+            ttglyph.drawPoints(hash_pen, thisFont["glyf"])
+            install_glyph_program_ufo(uw, g, g_inst_final, hash_pen.hash)
+        else:
+            install_glyph_program(g, thisFont, g_inst_final)
+        if saveprograms:
+            gfn = userNameToFileName(g) + ".instructions"
+            gfnfile = open(gfn, "w")
+            if nocompact or g in no_compact_list:
+                gfnfile.write(g_inst_final)
+            else:
+                gfnfile.write("Uncompacted:\n\n")
+                gfnfile.write(str(g_inst))
+                gfnfile.write("\n\nCompacted:\n\n")
+                gfnfile.write(g_inst_final)
+            gfnfile.close
+    if quietcount == 1:
+        print("")
+
+    if quietcount < 1:
+        print("Hinted " + str(len(glyph_list)) + " glyphs.")
+        print("Cleaning up and writing the new font")
+    if len(failed_glyph_list) and source == "xgf":
+        print("There were problems with these glyphs:")
+        for f in failed_glyph_list:
+            print(f, end = " ")
+            print()
     try:
-        # New procedure: grab the font, subset it with just the one glyph we're
-        # previewing, and write it to a spooled temporary file.
-        tf = SpooledTemporaryFile(max_size=1000000, mode='b')
-        options = subset.Options(glyph_names=True)
-        options.layout_features = []
-        subsetter = subset.Subsetter(options)
-        subsetter.populate(glyphs=glyph_list)
-        subsetter.subset(thisFont)
-        glyph_id = {}
-        for g in glyph_list:
-            glyph_id[g] = thisFont.getGlyphID(g)
-        thisFont.save(tf, 1)
-        tf.seek(0)
+        if ufo_mode:
+            d = {"maxSizeOfInstructions": maxInstructions + 50,
+                 "maxTwilightPoints": twilightBase + 25,
+                 "maxStorage": 64,
+                 "maxStackElements": maxStack,
+                 "maxFunctionDefs": maxFunction}
+            install_properties_ufo(uw, ufo_lib_tree, d)
+            uw.save_lib(ufo_lib_tree)
+        else:
+            thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
+            thisFont['maxp'].maxTwilightPoints = twilightBase + 25
+            thisFont['maxp'].maxStorage = storageBase + 64
+            thisFont['maxp'].maxStackElements = maxStack
+            thisFont['maxp'].maxFunctionDefs = maxFunction
+            thisFont['head'].flags |= 0b0000000000001000
     except Exception as e:
+        print("Error while installing maxp and head settings:")
+        print(e.args)
         print(e)
-    # Return: a handle to the temp file, the index of the target glyph, a list of
-    # glyphs for which complilation failed
-    return tf, glyph_id, failed_glyph_list
-
-
+    if skipcomp:
+        if quietcount < 1:
+            print("As --nocompilation flag is set, exiting without writing font file.")
+        sys.exit(0)
+    if not outputfont:
+        outputfont = str(xgffile.xpath("/xgf:xgridfit/xgf:outputfont/text()",
+                                       namespaces=ns)[0])
+    if not outputfont:
+        print("Need the filename of a font to write. Use the --outputfont")
+        print("command-line argument or the <outputfont> element in your")
+        print("Xgridfit file.")
+        sys.exit(1)
+    if not ufo_mode:
+        with thisFont as f:
+            f.save(outputfont, 1)
+        # thisFont.save(outputfont, 1)
 
 
 def main():
 
     global maxInstructions, quietcount
 
     # First read the command-line arguments. At minimum we need the inputfile.
@@ -740,15 +1287,16 @@
 
     if quietcount < 1:
         print("Opening the Xgridfit file ...")
 
     if cfuzz > 1:
         coordinateFuzz = cfuzz
 
-    if os.path.splitext(inputfile)[1] == ".yaml":
+    source_ext = os.path.splitext(inputfile)[1]
+    if source_ext == ".yaml":
         if quietcount < 1:
             print("Converting yaml source to Xgridfit")
         xgffile = ygridfit_parse(inputfile)
         # print(xgffile)
     else:
         xgffile = etree.parse(inputfile)
 
@@ -882,16 +1430,22 @@
         no_compact_list = []
     else:
         no_compact_list = list(no_compact_list.split(" "))
 
     # Now that we have a glyph list, we can make the coordinate index
     # and substitute point numbers for coordinates.
 
-    coordinateIndex = make_coordinate_index(glyph_list, thisFont)
-    coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    failed_glyph_list = []
+
+    coordinateIndex, bad = make_coordinate_index(glyph_list, thisFont)
+    if len(bad):
+        failed_glyph_list.extend(bad)
+    bad = coordinates_to_points(glyph_list, xgffile, coordinateIndex, ns)
+    if len(bad):
+        failed_glyph_list.extend(bad)
 
     # Back to the xgf file. We're also going to need a list of stack-safe
     # functions in this font.
 
     if quietcount < 1:
         print("Getting list of safe function calls ...")
 
@@ -959,19 +1513,23 @@
                 glyph_args['init_graphics'] = "'" + initgraphics + "'"
             if assume_y:
                 glyph_args['assume-always-y'] = "'" + assume_y + "'"
             g_inst = etransform(xgffile, **glyph_args)
         except Exception as e:
             print(e)
             for entry in etransform.error_log:
-                print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
-            sys.exit(1)
+                if quietcount < 3:
+                    print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+            # sys.exit(1)
+            failed_glyph_list.append(g)
+            continue
         # Two lines added for (possible) debugging
         for entry in etransform.error_log:
-            print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
+            if quietcount < 3:
+                print('message from line %s, col %s: %s' % (entry.line, entry.column, entry.message))
         if nocompact or g in no_compact_list:
             g_inst_final = str(g_inst)
         else:
             g_inst_final = compact_instructions(str(g_inst), safe_calls)
         install_glyph_program(g, thisFont, g_inst_final)
         if saveprograms:
             gfn = userNameToFileName(g) + ".instructions"
@@ -985,14 +1543,19 @@
                 gfnfile.write(g_inst_final)
             gfnfile.close
     print("")
 
     if quietcount < 1:
         print("Hinted " + str(len(glyph_list)) + " glyphs.")
         print("Cleaning up and writing the new font")
+    if len(failed_glyph_list):
+        print("There were problems with these glyphs:")
+        for f in failed_glyph_list:
+            print(f, end = " ")
+            print()
     thisFont['maxp'].maxSizeOfInstructions = maxInstructions + 50
     thisFont['maxp'].maxTwilightPoints = twilightBase + 25
     thisFont['maxp'].maxStorage = storageBase + 64
     thisFont['maxp'].maxStackElements = maxStack
     thisFont['maxp'].maxFunctionDefs = maxFunction
     thisFont['head'].flags |= 0b0000000000001000
     if skipcomp:
```

### Comparing `xgridfit-3.2.9/src/xgridfit/ygridfit.py` & `xgridfit-3.3.0/src/xgridfit/ygridfit.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,75 @@
 import uuid
 # import logging
 
 XGF_NAMESPACE = "http://xgridfit.sourceforge.net/Xgridfit2"
 XGF = "{%s}" % XGF_NAMESPACE
 NSMAP = {None: XGF_NAMESPACE}
 
-MOVETYPES = ["move", "whitespace", "blackspace", "stem", "grayspace"]
+MOVETYPES = ["move", "whitedist", "blackdist", "stem", "graydist"]
+
+DELTA_TRANSLATE = {
+    4.0:    "8/2",
+    3.5:    "7/2",
+    3.0:    "6/2",
+    2.5:    "5/2",
+    2.0:    "4/2",
+    1.5:    "3/2",
+    1.0:    "8/8",
+    0.875:  "7/8",
+    0.75:   "6/8",
+    0.625:  "5/8",
+    0.5:    "4/8",
+    0.375:  "3/8",
+    0.25:   "2/8",
+    0.125:  "1/8",
+    -0.125: "-1/8",
+    -0.25:  "-2/8",
+    -0.375: "-3/8",
+    -0.5:   "-4/8",
+    -0.625: "-5/8",
+    -0.75:  "-6/8",
+    -0.875: "-7/8",
+    -1.0:   "-8/8",
+    -1.5:   "-3/2",
+    -2.0:   "-4.2",
+    -2.5:   "-5/2",
+    -3.0:   "-6/2",
+    -3.5:   "-7/2",
+    -4.0:   "-8/2",
+}
+
+DEFAULT_TYPES = [
+    "minimum-distance",
+    "control-value-cut-in",
+    "single-width",
+    "single-width-cut-in",
+    "delta-base",
+    "delta-shift",
+    "delta-break",
+    "push-break",
+    "max-twilight-points",
+    "max-storage",
+    "max-stack",
+    "use-truetype-defaults",
+    "cleartype",
+    "round-state",
+    "function-base",
+    "compile-globals",
+    "init-graphics",
+    "color",
+    "assume-always-y",
+]
+
+def closest_cv_delta(val):
+    if val:
+        l = list(DELTA_TRANSLATE.keys())
+        return l[min(range(len(l)), key = lambda i: abs(l[i] - val))]
+    return 
+
 
 # logging.basicConfig(filename='ygridfit.log', encoding='utf-8', level=logging.DEBUG)
 
 def build_cvt(source, xgf_doc):
     ck = source.keys()
     for c in ck:
         cvt_entry = source[c]
@@ -27,31 +87,65 @@
             try:
                 cvt_element.set("color", cvt_entry['col'])
             except KeyError:
                 pass
         else:
             cvt_element.set("value", str(cvt_entry))
 
+def build_cvar_from_masters(source, xgf_doc):
+    # First survey cvt, gathering all var entries in a dict:
+    # {master-id: {cv-id: val}}
+    # Then iterate through the masters, plugging in the variant
+    # CVs. Should end in exactly the same place as with
+    # build_cvar.
+    cvt_source = source["cvt"]
+    masters_source = source["masters"]
+    cvar_list = []
+    k = masters_source.keys()
+    # kk is an id that identifies a master internally. It associates variant
+    # CVs with their masters.
+    for kk in k:
+        new_cvar_entry = {"regions": [], "vals": []}
+        vars = masters_source[kk]["vals"]
+        tag_k = vars.keys()
+        for tag_kk in tag_k:
+            new_cvar_entry["regions"].append({"tag": tag_kk, "val": vars[tag_kk]})
+        # Search the cvt for variant CVs with kk as the "nm" key.
+        # This could be way more efficient. Make a dict before embarking on this loop?
+        cv_list = new_cvar_entry["vals"]
+        cvt_k = cvt_source.keys()
+        for cvt_kk in cvt_k:
+            cvt_entry = cvt_source[cvt_kk]
+            if "var" in cvt_entry:
+                var = cvt_entry["var"]
+                tags = var.keys()
+                for tags_k in tags:
+                    if tags_k == kk:
+                        cv_list.append({"nm": cvt_kk, "val": var[tags_k]})
+        if len(cv_list) > 0:
+            cvar_list.append(new_cvar_entry)
+    build_cvar(cvar_list, xgf_doc)
+
 def build_cvar(source, xgf_doc):
     cvar_element = etree.SubElement(xgf_doc, XGF + "cvar")
     for c in source:
         tuple_element = etree.SubElement(cvar_element, XGF + "tuple")
         for r in c["regions"]:
             region_element = etree.SubElement(tuple_element, XGF + "region")
             region_element.set("tag", r["tag"])
-            region_element.set("bot", str(r["bot"]))
-            region_element.set("top", str(r["top"]))
-            region_element.set("peak", str(r["peak"]))
+            # region_element.set("bot", str(r["bot"]))
+            # region_element.set("top", str(r["top"]))
+            region_element.set("peak", str(r["val"]))
         for v in c["vals"]:
             value_element = etree.SubElement(tuple_element, XGF + "cvv")
             value_element.set("name", v["nm"])
             value_element.set("value", str(v["val"]))
 
 def point_key(p):
-    lk = {"align": 0, "interpolate": 1, "shift": 2, "stem": 3, "whitespace": 3, "blackspace": 3, "grayspace": 3, "move": 3}
+    lk = {"align": 0, "interpolate": 1, "shift": 2, "stem": 3, "whitedist": 3, "blackdist": 3, "graydist": 3, "move": 3}
     try:
         k = lk[p['rel']]
     except (ValueError, KeyError):
         k = 3
     return k
 
 def is_rounded(source, dflt):
@@ -109,27 +203,31 @@
         move_type = "move"
     if move_type in MOVETYPES:
         move_element = etree.SubElement(parent_el, XGF + "move")
         color = None
         if "col" in source:
             color = source['col']
         else:
-            if move_type == "whitespace":
+            if move_type == "whitedist":
                 color = "white"
-            elif move_type == "stem" or move_type == "blackspace":
+            elif move_type == "stem" or move_type == "blackdist":
                 color = "black"
         if color:
             move_element.set("color", color)
         distance = None
         if 'dist' in source:
             distance = str(source['dist'])
         if 'pos' in source:
             distance = str(source['pos'])
         if distance:
             move_element.set("distance", distance)
+        if 'min' in source:
+            min_dist = source['min']
+            if type(min_dist) is bool:
+                move_element.set("min-distance", translate_bool(min_dist))
         if not is_rounded(source, True):
             move_element.set("round", "no")
         else:
             try:
                 if type(source['round']) is str:
                     move_element.set("round", source['round'])
             except Exception:
@@ -236,16 +334,17 @@
             # xysection[skk].sort(key=point_key)
             for p in xysection[skk]:
                 if "macro" in p or "function" in p:
                     build_macro_function_call(p, glyph_element)
                 else:
                     build_point(p, glyph_element)
     except KeyError:
-        if axis == "y":
-            print("Warning: no y points in glyph " + nm)
+        pass
+        #if axis == "y":
+        #    print("Warning: no y points in glyph " + nm)
 
 def build_glyph_program(nm, source, xgf_doc):
     glyph_element = etree.SubElement(xgf_doc, XGF + "glyph")
     glyph_element.set("ps-name", nm)
     if "props" in source:
         p = source['props']
         if "assume-y" in p:
@@ -293,37 +392,97 @@
     if "out" in source:
         output_el = etree.SubElement(xgf_doc, XGF + "outputfont")
         output_el.text = source['out']
 
 def build_defaults(source, xgf_doc):
     source_keys = source.keys()
     for d in source_keys:
-        default_el = etree.SubElement(xgf_doc, XGF + "default")
-        default_el.set("type", d)
-        v = source[d]
-        if type(v) is bool:
-            if v:
-                valstring = "yes"
+        # ignore anything not recognized by Xgridfit (ygt's internal defaults)
+        if d in DEFAULT_TYPES:
+            default_el = etree.SubElement(xgf_doc, XGF + "default")
+            default_el.set("type", d)
+            v = source[d]
+            if type(v) is bool:
+                valstring = translate_bool(v)
             else:
-                valstring = "no"
-        else:
-            valstring = str(v)
-        default_el.set("value", valstring)
+                valstring = str(v)
+            default_el.set("value", valstring)
 
 def build_cvt_settings(source, cvt_source, xgf_doc):
     prep_el = etree.SubElement(xgf_doc, XGF + "pre-program")
     if "code" in source:
         newcode = source['code'].replace("\n", "")
         newxml = etree.XML(newcode)
         for n in newxml:
             prep_el.append(n)
-    size_blocks = {}
     k = cvt_source.keys()
+    # Round the CVs for which rounding has been requested.
     for kk in k:
         cvt_entry = cvt_source[kk]
+        if "round" in cvt_entry and cvt_entry["round"]:
+            round_el = etree.SubElement(prep_el, XGF + "round")
+            round_el.set("value", kk)
+    # Next the deltas. First sort first into blocks by "delta-shift" value.
+    shift_blocks = {}
+    for kk in k:
+        cvt_entry = cvt_source[kk]
+        if "deltas" in cvt_entry:
+            delta_list = cvt_entry["deltas"]
+            # Rem each entry in the delta_list has a size and a distance. The
+            # distance encapsulates two values: dist and shift. A list of
+            # deltas has to be sorted by size (resolution).
+            new_delta_list = sorted(delta_list, key=lambda s: s['size'])
+            for d in new_delta_list:
+                val = d["distance"]
+                dist = 0.0
+                sh =   8
+                if type(val) is str and "/" in val:
+                    r = val.split("/", 1)
+                    try:
+                        dist = int(r[0])
+                        sh   = int(r[1])
+                    except Exception:
+                        pass
+                else:
+                    try:
+                        val = DELTA_TRANSLATE[closest_cv_delta(float(val))]
+                        r = val.split("/", 1)
+                        dist = int(r[0])
+                        sh   = int(r[1])
+                    except Exception as e:
+                        pass
+                if dist != 0 and dist >= -8 and dist <= 8:
+                    if not sh in shift_blocks:
+                        shift_blocks[sh] = []
+                    shift_blocks[sh].append({"name": kk, "size": d["size"], "distance": dist})
+    if len(shift_blocks) > 0:
+        s = shift_blocks.keys()
+        for ss in s:
+            dshift = etree.SubElement(prep_el, XGF + "set-delta-shift")
+            dshift.set("units-per-pixel", str(ss))
+            cv_delta = etree.SubElement(prep_el, XGF + "control-value-delta")
+            dblock = shift_blocks[ss]
+            for dd in dblock:
+                try:
+                    dset_el = etree.SubElement(cv_delta, XGF + "delta-set")
+                    dset_el.set("cv", dd["name"])
+                    # Subtract the delta base. This can't be changed in ygt.
+                    dset_el.set("size", str(int(dd["size"]) - 9))
+                    dset_el.set("distance", str(int(dd["distance"])))
+                except Exception as e:
+                    pass
+        dshift = etree.SubElement(prep_el, XGF + "set-delta-shift")
+        dshift.set("units-per-pixel", str(8))
+    # Now the "same as" entries. First sort into blocks by size, then go through
+    # each block, creating "set-control-value" commands.
+    size_blocks = {}
+    for kk in k:
+        cvt_entry = cvt_source[kk]
+        # Surveying "same as" properties in CV list. First sort into blocks
+        # by size.
         if "same-as" in cvt_entry:
             sa = cvt_entry["same-as"]
             if "below" in sa:
                 below_key = (sa["below"]["ppem"], "<")
                 if not below_key in size_blocks:
                     size_blocks[below_key] = []
                 block = {}
@@ -421,16 +580,22 @@
             build_input_output(y_doc[k], xgf_doc)
         elif k == "defaults":
             build_defaults(y_doc[k], xgf_doc)
         elif k == "prep":
             build_cvt_settings(y_doc[k], y_doc["cvt"], xgf_doc)
         elif k == "cvt":
             build_cvt(y_doc[k], xgf_doc)
+        elif k == "masters":
+            try:
+                build_cvar_from_masters(y_doc, xgf_doc)
+            except Exception as e:
+                pass
         elif k == "cvar":
-            build_cvar(y_doc[k], xgf_doc)
+            if not "masters" in y_doc:
+                build_cvar(y_doc[k], xgf_doc)
         elif k == "functions":
             build_functions(y_doc[k], xgf_doc)
         elif k == "macros":
             build_macros(y_doc[k], xgf_doc)
         elif k == "glyphs":
             if not single_glyph and not glyph_list:
                 g_keys = y_doc[k].keys()
```

### Comparing `xgridfit-3.2.9/src/xgridfit.egg-info/SOURCES.txt` & `xgridfit-3.3.0/src/xgridfit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 src/xgridfit/__init__.py
 src/xgridfit/version.py
+src/xgridfit/xgfUFOWriter.py
+src/xgridfit/xgridfit-backup.py
 src/xgridfit/xgridfit.py
 src/xgridfit/ygridfit.py
 src/xgridfit.egg-info/PKG-INFO
 src/xgridfit.egg-info/SOURCES.txt
 src/xgridfit.egg-info/dependency_links.txt
 src/xgridfit.egg-info/entry_points.txt
 src/xgridfit.egg-info/requires.txt
```

