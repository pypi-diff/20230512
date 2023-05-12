# Comparing `tmp/hystoc-0.1.tar.gz` & `tmp/hystoc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hystoc-0.1.tar", last modified: Thu May 11 14:59:39 2023, max compression
+gzip compressed data, was "hystoc-0.1.1.tar", last modified: Fri May 12 10:56:05 2023, max compression
```

## Comparing `hystoc-0.1.tar` & `hystoc-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-11 14:59:39.519511 hystoc-0.1/
--rw-r--r--   0 ibenes   (30286) speech     (361)     1071 2023-03-23 14:34:43.000000 hystoc-0.1/LICENSE
--rw-r--r--   0 ibenes   (30286) speech     (361)     3269 2023-05-11 14:59:39.518511 hystoc-0.1/PKG-INFO
--rw-r--r--   0 ibenes   (30286) speech     (361)     1537 2023-05-11 14:59:29.000000 hystoc-0.1/README.md
-drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-11 14:59:39.492511 hystoc-0.1/hystoc/
--rw-r--r--   0 ibenes   (30286) speech     (361)      808 2023-05-11 14:58:51.000000 hystoc-0.1/hystoc/cn_utils.py
--rw-r--r--   0 ibenes   (30286) speech     (361)     3167 2023-04-21 12:14:08.000000 hystoc-0.1/hystoc/confusion_networks.py
--rw-r--r--   0 ibenes   (30286) speech     (361)     7287 2023-05-11 14:58:29.000000 hystoc-0.1/hystoc/fuse_nbest.py
--rw-r--r--   0 ibenes   (30286) speech     (361)     1995 2023-05-11 14:34:40.000000 hystoc-0.1/hystoc/io_utils.py
--rw-r--r--   0 ibenes   (30286) speech     (361)     2965 2023-05-11 14:58:34.000000 hystoc-0.1/hystoc/nbest_to_confidence.py
-drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-11 14:59:39.513511 hystoc-0.1/hystoc.egg-info/
--rw-r--r--   0 ibenes   (30286) speech     (361)     3269 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/PKG-INFO
--rw-r--r--   0 ibenes   (30286) speech     (361)      332 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/SOURCES.txt
--rw-r--r--   0 ibenes   (30286) speech     (361)        1 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/dependency_links.txt
--rw-r--r--   0 ibenes   (30286) speech     (361)      110 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/entry_points.txt
--rw-r--r--   0 ibenes   (30286) speech     (361)        6 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/requires.txt
--rw-r--r--   0 ibenes   (30286) speech     (361)        7 2023-05-11 14:59:39.000000 hystoc-0.1/hystoc.egg-info/top_level.txt
--rw-r--r--   0 ibenes   (30286) speech     (361)      761 2023-05-11 14:58:39.000000 hystoc-0.1/pyproject.toml
--rw-r--r--   0 ibenes   (30286) speech     (361)       38 2023-05-11 14:59:39.520511 hystoc-0.1/setup.cfg
+drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-12 10:56:05.339464 hystoc-0.1.1/
+-rw-r--r--   0 ibenes   (30286) speech     (361)     1071 2023-03-23 14:34:43.000000 hystoc-0.1.1/LICENSE
+-rw-r--r--   0 ibenes   (30286) speech     (361)     5093 2023-05-12 10:56:05.318464 hystoc-0.1.1/PKG-INFO
+-rw-r--r--   0 ibenes   (30286) speech     (361)     3359 2023-05-12 10:49:20.000000 hystoc-0.1.1/README.md
+drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-12 10:56:05.141464 hystoc-0.1.1/hystoc/
+-rw-r--r--   0 ibenes   (30286) speech     (361)      808 2023-05-11 14:58:51.000000 hystoc-0.1.1/hystoc/cn_utils.py
+-rw-r--r--   0 ibenes   (30286) speech     (361)     3167 2023-04-21 12:14:08.000000 hystoc-0.1.1/hystoc/confusion_networks.py
+-rw-r--r--   0 ibenes   (30286) speech     (361)     2965 2023-05-11 14:58:34.000000 hystoc-0.1.1/hystoc/hystoc_confidences.py
+-rw-r--r--   0 ibenes   (30286) speech     (361)     7287 2023-05-12 10:52:12.000000 hystoc-0.1.1/hystoc/hystoc_fusion.py
+-rw-r--r--   0 ibenes   (30286) speech     (361)     1995 2023-05-11 14:34:40.000000 hystoc-0.1.1/hystoc/io_utils.py
+drwxr-xr-x   0 ibenes   (30286) speech     (361)        0 2023-05-12 10:56:05.313464 hystoc-0.1.1/hystoc.egg-info/
+-rw-r--r--   0 ibenes   (30286) speech     (361)     5093 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/PKG-INFO
+-rw-r--r--   0 ibenes   (30286) speech     (361)      334 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/SOURCES.txt
+-rw-r--r--   0 ibenes   (30286) speech     (361)        1 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/dependency_links.txt
+-rw-r--r--   0 ibenes   (30286) speech     (361)      112 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/entry_points.txt
+-rw-r--r--   0 ibenes   (30286) speech     (361)        6 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/requires.txt
+-rw-r--r--   0 ibenes   (30286) speech     (361)        7 2023-05-12 10:56:04.000000 hystoc-0.1.1/hystoc.egg-info/top_level.txt
+-rw-r--r--   0 ibenes   (30286) speech     (361)      765 2023-05-12 10:55:56.000000 hystoc-0.1.1/pyproject.toml
+-rw-r--r--   0 ibenes   (30286) speech     (361)       38 2023-05-12 10:56:05.340464 hystoc-0.1.1/setup.cfg
```

### Comparing `hystoc-0.1/LICENSE` & `hystoc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hystoc-0.1/hystoc/cn_utils.py` & `hystoc-0.1.1/hystoc/cn_utils.py`

 * *Files identical despite different names*

### Comparing `hystoc-0.1/hystoc/confusion_networks.py` & `hystoc-0.1.1/hystoc/confusion_networks.py`

 * *Files identical despite different names*

### Comparing `hystoc-0.1/hystoc/fuse_nbest.py` & `hystoc-0.1.1/hystoc/hystoc_fusion.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,18 +148,18 @@
 
     if args.temperature < 0.0:
         raise ValueError(f'Temperatures below zero make no sense (got {args.temperature})')
 
     system_outputs = []
     for i in range(0, len(args.hyps_scores_files), 2):
         with open(args.hyps_scores_files[i]) as f:
-            scores = load_scores_dict(f)
+            hyps = load_hyps_dict(f)
 
         with open(args.hyps_scores_files[i+1]) as f:
-            hyps = load_hyps_dict(f)
+            scores = load_scores_dict(f)
 
         system_outputs.append((scores, hyps))
 
         if scores.keys() != hyps.keys():
             logging.error('Not matching segments!')
             logging.error('In files {args.hyps_scores_files[i]} and {args.hyps_scores_files[i+1]}')
             logging.error(f'Only in scores: {scores.keys() - hyps.keys()}')
```

### Comparing `hystoc-0.1/hystoc/io_utils.py` & `hystoc-0.1.1/hystoc/io_utils.py`

 * *Files identical despite different names*

### Comparing `hystoc-0.1/hystoc/nbest_to_confidence.py` & `hystoc-0.1.1/hystoc/hystoc_confidences.py`

 * *Files identical despite different names*

### Comparing `hystoc-0.1/pyproject.toml` & `hystoc-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = [ "setuptools>=61" ]
 
 [project]
 name = "hystoc"
-version = "0.1"
+version = "0.1.1"
 description = "Toolkit for obtaining word-level confidences"
 readme = "README.md"
 requires-python = ">=3.6"
 license = {file = "LICENSE"}
 keywords = ["Confidence estimation", "ASR"]
 
 authors = [
@@ -28,9 +28,9 @@
 [project.urls]
 repository = "https://github.com/BUTSpeechFIT/hystoc"
 
 [tool.setuptools.package-dir]
 "hystoc" = "hystoc"
 
 [project.scripts]
-hystoc-confidences = "hystoc.nbest_to_confidence:main"
-hystoc-fusion = "hystoc.fuse_nbest:main"
+hystoc-confidences = "hystoc.hystoc_confidences:main"
+hystoc-fusion = "hystoc.hystoc_fusion:main"
```

