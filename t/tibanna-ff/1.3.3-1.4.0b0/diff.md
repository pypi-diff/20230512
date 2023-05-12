# Comparing `tmp/tibanna_ff-1.3.3.tar.gz` & `tmp/tibanna_ff-1.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibanna_ff-1.3.3.tar", max compression
+gzip compressed data, was "tibanna_ff-1.4.0b0.tar", max compression
```

## Comparing `tibanna_ff-1.3.3.tar` & `tibanna_ff-1.4.0b0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1083 2020-02-12 17:25:26.338682 tibanna_ff-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0      290 2020-02-12 17:25:26.339062 tibanna_ff-1.3.3/README.md
--rw-r--r--   0        0        0     2166 2023-04-14 15:18:20.779999 tibanna_ff-1.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-12 17:25:26.388455 tibanna_ff-1.3.3/tibanna_4dn/__init__.py
--rw-r--r--   0        0        0     9943 2021-08-18 20:28:06.333123 tibanna_ff-1.3.3/tibanna_4dn/__main__.py
--rw-r--r--   0        0        0     2352 2022-07-28 15:27:13.955013 tibanna_ff-1.3.3/tibanna_4dn/core.py
--rw-r--r--   0        0        0      317 2021-07-19 16:31:16.918389 tibanna_ff-1.3.3/tibanna_4dn/iam_utils.py
--rw-r--r--   0        0        0      131 2021-09-22 18:05:42.578265 tibanna_ff-1.3.3/tibanna_4dn/lambdas/__init__.py
--rw-r--r--   0        0        0      447 2020-02-12 17:25:26.389426 tibanna_ff-1.3.3/tibanna_4dn/lambdas/check_task.py
--rw-r--r--   0        0        0      106 2023-04-14 15:18:20.781080 tibanna_ff-1.3.3/tibanna_4dn/lambdas/requirements.txt
--rw-r--r--   0        0        0      435 2020-02-12 17:25:26.389831 tibanna_ff-1.3.3/tibanna_4dn/lambdas/run_task.py
--rw-r--r--   0        0        0     1065 2022-07-28 15:27:13.969283 tibanna_ff-1.3.3/tibanna_4dn/lambdas/start_run.py
--rw-r--r--   0        0        0      230 2021-11-18 14:02:19.666429 tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_cost.py
--rw-r--r--   0        0        0     1251 2022-07-28 15:27:13.974943 tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     6067 2021-11-01 16:47:18.092418 tibanna_ff-1.3.3/tibanna_4dn/pony_utils.py
--rw-r--r--   0        0        0      934 2022-05-12 18:36:39.965873 tibanna_ff-1.3.3/tibanna_4dn/start_run.py
--rw-r--r--   0        0        0      318 2021-08-18 20:28:06.335284 tibanna_ff-1.3.3/tibanna_4dn/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-11-18 14:02:19.668068 tibanna_ff-1.3.3/tibanna_4dn/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1450 2021-07-19 16:31:16.926459 tibanna_ff-1.3.3/tibanna_4dn/update_ffmeta.py
--rw-r--r--   0        0        0      863 2022-09-21 14:52:08.834451 tibanna_ff-1.3.3/tibanna_4dn/vars.py
--rw-r--r--   0        0        0        0 2020-02-12 17:25:26.392374 tibanna_ff-1.3.3/tibanna_cgap/__init__.py
--rw-r--r--   0        0        0     9962 2022-05-12 18:36:39.978678 tibanna_ff-1.3.3/tibanna_cgap/__main__.py
--rw-r--r--   0        0        0      255 2020-02-12 17:25:26.392929 tibanna_ff-1.3.3/tibanna_cgap/check_task.py
--rw-r--r--   0        0        0     2769 2022-05-12 18:36:39.983996 tibanna_ff-1.3.3/tibanna_cgap/core.py
--rw-r--r--   0        0        0      300 2021-07-19 16:31:16.931753 tibanna_ff-1.3.3/tibanna_cgap/cw_utils.py
--rw-r--r--   0        0        0      318 2021-07-19 16:31:16.932909 tibanna_ff-1.3.3/tibanna_cgap/iam_utils.py
--rw-r--r--   0        0        0      132 2021-09-22 18:05:42.579587 tibanna_ff-1.3.3/tibanna_cgap/lambdas/__init__.py
--rw-r--r--   0        0        0      467 2020-02-12 17:25:26.393889 tibanna_ff-1.3.3/tibanna_cgap/lambdas/check_task.py
--rw-r--r--   0        0        0      106 2023-04-14 15:18:20.781386 tibanna_ff-1.3.3/tibanna_cgap/lambdas/requirements.txt
--rw-r--r--   0        0        0      436 2020-02-12 17:25:26.394271 tibanna_ff-1.3.3/tibanna_cgap/lambdas/run_task.py
--rw-r--r--   0        0        0     1068 2022-07-28 15:27:13.984898 tibanna_ff-1.3.3/tibanna_cgap/lambdas/start_run.py
--rw-r--r--   0        0        0      231 2021-11-18 14:02:19.688789 tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_cost.py
--rw-r--r--   0        0        0     1285 2022-07-28 15:27:13.990793 tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     1281 2022-05-12 18:36:39.995036 tibanna_ff-1.3.3/tibanna_cgap/start_run.py
--rw-r--r--   0        0        0      319 2021-08-18 20:28:06.339708 tibanna_ff-1.3.3/tibanna_cgap/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-09-22 18:05:42.586269 tibanna_ff-1.3.3/tibanna_cgap/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1098 2020-02-12 17:25:26.396103 tibanna_ff-1.3.3/tibanna_cgap/update_ffmeta.py
--rw-r--r--   0        0        0     1106 2022-09-21 14:52:08.841665 tibanna_ff-1.3.3/tibanna_cgap/vars.py
--rw-r--r--   0        0        0     6094 2021-11-01 16:47:18.100132 tibanna_ff-1.3.3/tibanna_cgap/zebra_utils.py
--rw-r--r--   0        0        0        0 2020-02-12 17:25:26.396782 tibanna_ff-1.3.3/tibanna_ffcommon/__init__.py
--rw-r--r--   0        0        0      504 2022-07-28 15:27:14.000802 tibanna_ff-1.3.3/tibanna_ffcommon/_version.py
--rw-r--r--   0        0        0      677 2021-07-19 16:31:16.941336 tibanna_ff-1.3.3/tibanna_ffcommon/config.py
--rw-r--r--   0        0        0     4090 2023-04-14 13:36:23.433794 tibanna_ff-1.3.3/tibanna_ffcommon/core.py
--rw-r--r--   0        0        0     3796 2021-07-19 16:31:16.949528 tibanna_ff-1.3.3/tibanna_ffcommon/exceptions.py
--rw-r--r--   0        0        0     2302 2021-07-19 16:31:16.949786 tibanna_ff-1.3.3/tibanna_ffcommon/extra_files.py
--rw-r--r--   0        0        0     2171 2021-07-19 16:31:16.950054 tibanna_ff-1.3.3/tibanna_ffcommon/file_format.py
--rw-r--r--   0        0        0     2019 2022-05-12 18:36:40.014086 tibanna_ff-1.3.3/tibanna_ffcommon/iam_utils.py
--rw-r--r--   0        0        0    16981 2023-04-14 13:36:23.434318 tibanna_ff-1.3.3/tibanna_ffcommon/input_files.py
--rw-r--r--   0        0        0    71687 2023-04-14 13:36:23.435112 tibanna_ff-1.3.3/tibanna_ffcommon/portal_utils.py
--rw-r--r--   0        0        0    22791 2023-04-14 13:36:23.435831 tibanna_ff-1.3.3/tibanna_ffcommon/qc.py
--rw-r--r--   0        0        0     3162 2021-08-18 20:28:06.348560 tibanna_ff-1.3.3/tibanna_ffcommon/stepfunction.py
--rw-r--r--   0        0        0     3252 2023-04-14 13:36:23.436171 tibanna_ff-1.3.3/tibanna_ffcommon/vars.py
--rw-r--r--   0        0        0     6499 2023-04-14 13:36:23.436523 tibanna_ff-1.3.3/tibanna_ffcommon/wfr.py
--rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 tibanna_ff-1.3.3/setup.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 tibanna_ff-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2021-09-09 16:55:28.100725 tibanna_ff-1.4.0b0/LICENSE.txt
+-rw-r--r--   0        0        0      290 2021-09-09 16:55:28.100977 tibanna_ff-1.4.0b0/README.md
+-rw-r--r--   0        0        0     2168 2023-05-11 16:13:57.299973 tibanna_ff-1.4.0b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.176651 tibanna_ff-1.4.0b0/tibanna_4dn/__init__.py
+-rw-r--r--   0        0        0     9943 2021-09-09 16:55:28.176936 tibanna_ff-1.4.0b0/tibanna_4dn/__main__.py
+-rw-r--r--   0        0        0     2352 2022-05-12 18:43:14.943285 tibanna_ff-1.4.0b0/tibanna_4dn/core.py
+-rw-r--r--   0        0        0      317 2021-09-09 16:55:28.177367 tibanna_ff-1.4.0b0/tibanna_4dn/iam_utils.py
+-rw-r--r--   0        0        0      131 2021-09-23 17:36:29.921830 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/__init__.py
+-rw-r--r--   0        0        0      447 2021-09-09 16:55:28.177955 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/check_task.py
+-rw-r--r--   0        0        0      106 2023-05-01 19:20:54.569511 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/requirements.txt
+-rw-r--r--   0        0        0      435 2021-09-09 16:55:28.178373 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/run_task.py
+-rw-r--r--   0        0        0     1065 2022-05-12 18:43:14.950624 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/start_run.py
+-rw-r--r--   0        0        0      230 2021-11-02 15:52:14.099351 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1251 2022-05-12 18:43:14.956966 tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     6067 2021-10-06 17:12:17.709226 tibanna_ff-1.4.0b0/tibanna_4dn/pony_utils.py
+-rw-r--r--   0        0        0      934 2022-02-02 21:42:36.484027 tibanna_ff-1.4.0b0/tibanna_4dn/start_run.py
+-rw-r--r--   0        0        0      318 2021-09-09 16:55:28.180862 tibanna_ff-1.4.0b0/tibanna_4dn/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-11-02 15:52:14.100504 tibanna_ff-1.4.0b0/tibanna_4dn/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1450 2021-09-09 16:55:28.181306 tibanna_ff-1.4.0b0/tibanna_4dn/update_ffmeta.py
+-rw-r--r--   0        0        0      863 2022-09-07 17:39:50.069810 tibanna_ff-1.4.0b0/tibanna_4dn/vars.py
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.181843 tibanna_ff-1.4.0b0/tibanna_cgap/__init__.py
+-rw-r--r--   0        0        0     9962 2022-02-02 21:42:36.485354 tibanna_ff-1.4.0b0/tibanna_cgap/__main__.py
+-rw-r--r--   0        0        0      255 2021-09-09 16:55:28.182378 tibanna_ff-1.4.0b0/tibanna_cgap/check_task.py
+-rw-r--r--   0        0        0     2769 2022-02-02 21:42:36.486858 tibanna_ff-1.4.0b0/tibanna_cgap/core.py
+-rw-r--r--   0        0        0      300 2021-09-09 16:55:28.182774 tibanna_ff-1.4.0b0/tibanna_cgap/cw_utils.py
+-rw-r--r--   0        0        0      318 2021-09-09 16:55:28.182976 tibanna_ff-1.4.0b0/tibanna_cgap/iam_utils.py
+-rw-r--r--   0        0        0      132 2021-09-16 20:24:20.855907 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/__init__.py
+-rw-r--r--   0        0        0      467 2021-09-09 16:55:28.183470 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/check_task.py
+-rw-r--r--   0        0        0      106 2023-05-01 19:20:54.570305 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/requirements.txt
+-rw-r--r--   0        0        0      436 2021-09-09 16:55:28.183912 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/run_task.py
+-rw-r--r--   0        0        0     1068 2022-05-12 18:43:14.968145 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/start_run.py
+-rw-r--r--   0        0        0      231 2021-11-02 15:52:14.104064 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1285 2022-05-12 18:43:14.977223 tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     1281 2022-02-02 21:42:36.490690 tibanna_ff-1.4.0b0/tibanna_cgap/start_run.py
+-rw-r--r--   0        0        0      319 2021-09-09 16:55:28.185766 tibanna_ff-1.4.0b0/tibanna_cgap/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-11-01 14:42:13.461080 tibanna_ff-1.4.0b0/tibanna_cgap/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1098 2021-09-09 16:55:28.186145 tibanna_ff-1.4.0b0/tibanna_cgap/update_ffmeta.py
+-rw-r--r--   0        0        0     1106 2022-09-07 17:39:50.071236 tibanna_ff-1.4.0b0/tibanna_cgap/vars.py
+-rw-r--r--   0        0        0     6094 2021-10-06 17:12:17.709135 tibanna_ff-1.4.0b0/tibanna_cgap/zebra_utils.py
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.186877 tibanna_ff-1.4.0b0/tibanna_ffcommon/__init__.py
+-rw-r--r--   0        0        0      504 2022-05-12 18:43:14.981898 tibanna_ff-1.4.0b0/tibanna_ffcommon/_version.py
+-rw-r--r--   0        0        0      677 2021-09-09 16:55:28.187272 tibanna_ff-1.4.0b0/tibanna_ffcommon/config.py
+-rw-r--r--   0        0        0     4090 2022-12-16 18:49:18.399580 tibanna_ff-1.4.0b0/tibanna_ffcommon/core.py
+-rw-r--r--   0        0        0     3905 2023-05-04 19:21:43.919773 tibanna_ff-1.4.0b0/tibanna_ffcommon/exceptions.py
+-rw-r--r--   0        0        0     2302 2021-09-09 16:55:28.188001 tibanna_ff-1.4.0b0/tibanna_ffcommon/extra_files.py
+-rw-r--r--   0        0        0     2171 2021-09-09 16:55:28.188228 tibanna_ff-1.4.0b0/tibanna_ffcommon/file_format.py
+-rw-r--r--   0        0        0     2570 2023-05-12 13:44:43.523168 tibanna_ff-1.4.0b0/tibanna_ffcommon/generic_qc_utils.py
+-rw-r--r--   0        0        0     2019 2022-02-02 21:42:36.495197 tibanna_ff-1.4.0b0/tibanna_ffcommon/iam_utils.py
+-rw-r--r--   0        0        0    16981 2023-05-01 19:20:54.571865 tibanna_ff-1.4.0b0/tibanna_ffcommon/input_files.py
+-rw-r--r--   0        0        0    75632 2023-05-12 15:05:19.988369 tibanna_ff-1.4.0b0/tibanna_ffcommon/portal_utils.py
+-rw-r--r--   0        0        0    22815 2023-05-08 18:31:51.928352 tibanna_ff-1.4.0b0/tibanna_ffcommon/qc.py
+-rw-r--r--   0        0        0     3162 2021-09-09 16:55:28.190327 tibanna_ff-1.4.0b0/tibanna_ffcommon/stepfunction.py
+-rw-r--r--   0        0        0     3535 2023-05-08 21:04:54.606843 tibanna_ff-1.4.0b0/tibanna_ffcommon/vars.py
+-rw-r--r--   0        0        0     6499 2023-05-01 19:20:54.579772 tibanna_ff-1.4.0b0/tibanna_ffcommon/wfr.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 tibanna_ff-1.4.0b0/PKG-INFO
```

### Comparing `tibanna_ff-1.3.3/LICENSE.txt` & `tibanna_ff-1.4.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/pyproject.toml` & `tibanna_ff-1.4.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibanna_ff"
-version = "1.3.3"
+version = "1.4.0b0"
 description = "Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tibanna"]
 homepage = "http://github.com/4dn-dcic/tibanna_ff"
 repository = "http://github.com/4dn-dcic/tibanna_ff.git"
```

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/__main__.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/core.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/lambdas/start_run.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/lambdas/update_ffmeta.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/pony_utils.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/pony_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/start_run.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/stepfunction_cost_updater.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/update_ffmeta.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_4dn/vars.py` & `tibanna_ff-1.4.0b0/tibanna_4dn/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/__main__.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/core.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/lambdas/start_run.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/lambdas/update_ffmeta.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/start_run.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/stepfunction_cost_updater.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/update_ffmeta.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/vars.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_cgap/zebra_utils.py` & `tibanna_ff-1.4.0b0/tibanna_cgap/zebra_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/config.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/config.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/core.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/exceptions.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     pass
 
 
 class MalFormattedWorkflowMetadataException(Exception):
     """There is an error with pony/zebra workflow metadata"""
     pass
 
+class GenericQcException(Exception):
+    """There is an error with the generic QC functionality"""
+    pass
+
 
 def exception_coordinator(lambda_name, metadata_only_func):
     '''
     friendly wrapper for your lambda functions, based on input_json / event comming in...
     1. Logs basic input for all functions
     2. if 'skip' key == 'lambda_name', skip the function
     3. catch exceptions raised by labmda, and if not in  list of ignored exceptions, added
```

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/extra_files.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/extra_files.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/file_format.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/file_format.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/iam_utils.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/iam_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/input_files.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/input_files.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/portal_utils.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/portal_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,23 @@
     AwsemPostRunJson
 )
 from tibanna.vars import (
     METRICS_URL,
     DYNAMODB_TABLE,
     DYNAMODB_KEYNAME,
 )
-from .vars import BUCKET_NAME
+from .vars import (
+    BUCKET_NAME,
+    OUTPUT_PROCESSED_FILE,
+    OUTPUT_REPORT_FILE,
+    OUTPUT_QC_FILE,
+    GENERIC_QC_FILE,
+    OUTPUT_TO_BE_EXTRA_INPUT_FILE,
+    INPUT_FILE
+)
 from .config import (
     higlass_config
 )
 from .file_format import (
     FormatExtensionMap,
     parse_formatstr,
     cmp_fileformat
@@ -54,30 +62,43 @@
 from .extra_files import (
     ExtraFiles,
     get_extra_file_key
 )
 from .qc import (
     QCArgumentsByTarget
 )
+from .generic_qc_utils import (
+    check_qc_workflow_args,
+    filter_workflow_args_by_property
+)
 from .exceptions import (
     TibannaStartException,
     FdnConnectionException,
     MalFormattedFFInputException,
-    MalFormattedWorkflowMetadataException
+    MalFormattedWorkflowMetadataException,
+    GenericQcException
 )
 from .vars import AWSF_IMAGE
 
 
 logger = create_logger(__name__)
 
 
 # temp, debugging
 import pkg_resources
 logger.debug(pkg_resources.get_distribution('dcicutils').version)
 
+OUTPUT_ARG_TYPE_LIST = [OUTPUT_PROCESSED_FILE,
+                        OUTPUT_REPORT_FILE,
+                        OUTPUT_QC_FILE,
+                        GENERIC_QC_FILE,
+                        OUTPUT_TO_BE_EXTRA_INPUT_FILE]
+
+# File types that are uploaded to the portal (and S3)
+PROCESSED_FILE_TYPES = [OUTPUT_PROCESSED_FILE, GENERIC_QC_FILE]
 
 class FFInputAbstract(SerializableObject):
     # the following attribute works as a cache for metadata -
     # do not modify or access it directly, but use self.get_metadata
     # instead
     _metadata = dict()
 
@@ -235,17 +256,17 @@
         args['dependency'] = self.dependency
 
         # output target
         args['output_target'] = dict()
         args['secondary_output_target'] = dict()
         for of in ff_meta.output_files:
             arg_name = of.get('workflow_argument_name')
-            if of.get('type') == 'Output processed file':
+            if of.get('type') in PROCESSED_FILE_TYPES:
                 args['output_target'][arg_name] = of.get('upload_key')
-            elif of.get('type') == 'Output to-be-extra-input file':
+            elif of.get('type') == OUTPUT_TO_BE_EXTRA_INPUT_FILE:
                 target_inf = ff_meta.input_files[0]  # assume only one input for now
                 target_key = self.output_target_for_input_extra(target_inf['value'], of)
                 args['output_target'][arg_name] = target_key
             else:  # output QC or report file
                 wf_of = [_ for _ in self.wf_meta.get('arguments') if _['workflow_argument_name'] == arg_name][0]
                 if wf_of.get('qc_zipped', False) and wf_of.get('qc_unzip_from_ec2', False):
                     if 'argument_to_be_attached_to' not in wf_of:
@@ -418,18 +439,14 @@
 
 
 class FourfrontStarterAbstract(object):
 
     InputClass = FFInputAbstract
     ProcessedFileMetadata = ProcessedFileMetadataAbstract
     WorkflowRunMetadata = WorkflowRunMetadataAbstract
-    output_arg_type_list = ['Output processed file',
-                            'Output report file',
-                            'Output QC file',
-                            'Output to-be-extra-input file']
 
     def __init__(self, **kwargs):
         self.inp = self.InputClass(**kwargs)
         self.pfs = dict()
         self.ff = None
 
     def run(self):
@@ -461,15 +478,15 @@
         return self.inp.wf_meta.get('arguments', [])
 
     def arg(self, argname):
         return [arg for arg in self.args if arg.get('workflow_argument_name') == argname][0]
 
     @property
     def output_args(self):
-        return [arg for arg in self.args if arg.get('argument_type') in self.output_arg_type_list]
+        return [arg for arg in self.args if arg.get('argument_type') in OUTPUT_ARG_TYPE_LIST]
 
     @property
     def output_argnames(self):
         return [arg.get('workflow_argument_name') for arg in self.output_args]
 
     # processed files-related functions
     def create_pfs(self):
@@ -517,15 +534,15 @@
         return pf_other_fields
 
     def pf(self, argname, **kwargs):
         if self.user_supplied_output_files(argname):
             res = self.get_meta(self.user_supplied_output_files(argname)[0]['uuid'])
             return self.ProcessedFileMetadata(**res)
         arg = self.arg(argname)
-        if arg.get('argument_type') != 'Output processed file':
+        if arg.get('argument_type') not in PROCESSED_FILE_TYPES:
             return None
         if 'argument_format' not in arg:
             raise Exception("file format for processed file must be provided")
         if 'secondary_file_formats' in arg:
             extra_files = self.pf_extra_files(arg.get('secondary_file_formats', []),
                                               arg.get('processed_extra_file_use_for', {}))
         else:
@@ -565,15 +582,15 @@
         ff_outfile_list = []
         for argname in self.output_argnames:
             ff_outfile_list.append(self.ff_outfile(argname))
         return ff_outfile_list
 
     def ff_outfile(self, argname):
         arg = self.arg(argname)
-        if arg.get('argument_type') == 'Output processed file':
+        if arg.get('argument_type') in PROCESSED_FILE_TYPES:
             if argname not in self.pfs:
                 raise Exception("processed file objects must be ready before creating ff_outfile")
             try:
                 resp = self.get_meta(self.pfs[argname].uuid)
             except Exception as e:
                 raise Exception("processed file must be posted before creating ff_outfile: %s" % str(e))
             return WorkflowRunOutputFiles(arg.get('workflow_argument_name'),
@@ -618,15 +635,15 @@
             logger.warning(str(e))
             pass
 
 
 class InputExtraArgumentInfo(SerializableObject):
     def __init__(self, argument_type, workflow_argument_name, argument_to_be_attached_to,
                  extra_file_use_for=None, **kwargs):
-        if argument_type != 'Output to-be-extra-input file':
+        if argument_type != OUTPUT_TO_BE_EXTRA_INPUT_FILE:
             raise Exception("InputExtraArgumentInfo is not Output to-be-extra-input file: %s" % argument_type)
         self.workflow_argument_name = workflow_argument_name
         self.argument_to_be_attached_to = argument_to_be_attached_to
         self.extra_file_use_for = extra_file_use_for
 
 
 class FourfrontUpdaterAbstract(object):
@@ -801,15 +818,15 @@
                 return argname
         return None
 
     def pf_uuids(self, argname):
         uuids = []
         for of in self.ff_output_files:
             if argname == of['workflow_argument_name']:
-                if of['type'] == 'Output processed file':
+                if of['type'] in PROCESSED_FILE_TYPES:
                     uuids.append(of['value'])
         return uuids
 
     def pf_extra_file(self, pf_uuid, file_format):
         for extra in self.pf(pf_uuid).extra_files:
             if cmp_fileformat(extra['file_format'], file_format):
                 return extra
@@ -865,15 +882,15 @@
         else:
             return self.workflow['arguments']
 
     @property
     def workflow_input_extra_arguments(self):
         """dictionary of InputExtraArgumentInfo object list as value and
         argument_to_be_attached_to as key"""
-        ie_args = [InputExtraArgumentInfo(**ie) for ie in self.workflow_arguments('Output to-be-extra-input file')]
+        ie_args = [InputExtraArgumentInfo(**ie) for ie in self.workflow_arguments(OUTPUT_TO_BE_EXTRA_INPUT_FILE)]
         ie_args_per_attach = dict()
         for iearg in ie_args:
             if iearg.argument_to_be_attached_to not in ie_args_per_attach:
                 ie_args_per_attach[iearg.argument_to_be_attached_to] = []
             ie_args_per_attach[iearg.argument_to_be_attached_to].append(iearg)
         return ie_args_per_attach
 
@@ -963,14 +980,19 @@
 
     def s3(self, argname):
         return s3Utils(self.bucket(argname), self.bucket(argname), self.bucket(argname))
 
     def read(self, argname):
         """This function is useful for reading md5 report of qc report"""
         return self.s3(argname).read_s3(self.file_key(argname)).decode('utf-8', 'backslashreplace')
+    
+    def read_json_from_s3(self, argname):
+        """This function is useful for reading generic QC files"""
+        file_content = self.s3(argname).read_s3(self.file_key(argname)).decode('utf-8')
+        return json.loads(file_content)
 
     def s3_file_size(self, argname, secondary_format=None):
         return self.s3(argname).get_file_size(self.file_key(argname, secondary_format=secondary_format),
                                               self.bucket(argname))
 
     # get file features
     def md5sum(self, argname=None, pf_uuid=None, secondary_key=None):
@@ -1064,15 +1086,15 @@
         else:
             raise Exception("Either argname or pf must be provided to get a file_key")
 
     def accessions(self, argname):
         accessions = []
         # argname is output
         v = self.ff_output_file(argname)
-        if v and v['type'] == 'Output processed file':
+        if v and v['type'] in PROCESSED_FILE_TYPES:
             file_name = v['upload_key'].split('/')[-1]
             accession = file_name.split('.')[0].strip('/')
             accessions.append(accession)
         # argname is input
         else:
             if argname not in self.awsem_input_files:
                 return []
@@ -1216,18 +1238,83 @@
                                                            hgcf['file_type'],
                                                            hgcf['data_type'],
                                                            ip.get('genome_assembly', None))
                 if higlass_uid:
                     self.update_patch_items(ip['uuid'], {'higlass_uid': higlass_uid})
             self.update_patch_items(ip['uuid'], {'extra_files': ip['extra_files']})
 
+
+    def update_generic_qc(self):
+
+        input_file_args = self.workflow_arguments([INPUT_FILE])
+        generic_qc_args = self.workflow_arguments([GENERIC_QC_FILE])
+
+        if len(generic_qc_args) == 0:
+            return
+        
+        # Basic sanity checks of the workflow arguments
+        check_qc_workflow_args(input_file_args, generic_qc_args)
+
+        ff_key = self.tibanna_settings.ff_keys
+        ff_env = self.tibanna_settings.env
+        
+        for input_file_arg in input_file_args:
+            # Get the associated QC args
+            input_wf_arg_name = input_file_arg['workflow_argument_name']
+            input_file_accession = self.accessions(input_wf_arg_name)[0]
+
+            qc_args = filter_workflow_args_by_property(generic_qc_args, "argument_to_be_attached_to", input_wf_arg_name)
+            if len(qc_args) == 0:
+                continue
+
+            qc_args_json = filter_workflow_args_by_property(qc_args, "qc_json", True) 
+            qc_arg_json = qc_args_json[0] # After running check_qc_workflow_args, we know that this contains exactly one element
+            qc_arg_json_name = qc_arg_json['workflow_argument_name']
+            try:
+                qc_json = self.read_json_from_s3(qc_arg_json_name)
+            except Exception as e:
+                logger.error(str(e))
+                raise GenericQcException(f"Could not get {qc_arg_json_name} from S3. Error: {str(e)}")
+
+            # Get the link to the zipped report. This will be added to the QualityMetricGeneric item
+            qc_args_zipped = filter_workflow_args_by_property(qc_args, "qc_zipped", True) # After running check_qc_workflow_args, we know that this contains zero or one elements
+            qc_arg_zipped = qc_args_zipped[0] if len(qc_args_zipped) == 1 else None
+            qc_arg_zipped_s3_url = f"https://{self.outbucket}.s3.amazonaws.com/{self.file_key(qc_arg_zipped['workflow_argument_name'])}" if qc_arg_zipped else None
+ 
+            # The folling will create a new QualityMetricGeneric item in the portal
+            try:
+                post_dict = qc_json
+                post_dict['url'] = qc_arg_zipped_s3_url
+                qmc_item = post_metadata(post_dict, "quality_metric_generic", key=ff_key, ff_env=ff_env)
+            except Exception as e:
+                raise GenericQcException(f"Could not post quality_metric_generic item for  {qc_arg_json_name}. The JSON was: {json.dumps(post_dict)}. Error: {str(e)}")
+
+            # This QualityMetricGeneric item will now be linked to the corresponding input file.
+            try:
+                input_file_metadata = self.get_metadata(input_file_accession)
+                input_file_quality_metrics = input_file_metadata.get('quality_metrics', [])
+                input_file_quality_metrics_uuids = map(lambda qm: qm['uuid'], input_file_quality_metrics)
+                input_file_quality_metrics_uuids.append(qmc_item['uuid'])
+                patch_dict = {
+                    'quality_metrics': input_file_quality_metrics_uuids
+                }
+                patch_metadata(patch_dict, input_file_accession, key=ff_key, ff_env=ff_env)
+            except Exception as e:
+                raise GenericQcException(f"Could not patch quality_metrics of file {input_file_accession}. Error: {str(e)}")
+
+
+
+
+
+
+
     # update functions for QC
     def update_qc(self):
         # all qc arguments in the workflow (could be more than one)
-        wf_qc_arguments = self.workflow_arguments('Output QC file')
+        wf_qc_arguments = self.workflow_arguments(OUTPUT_QC_FILE)
         # put all qc arguments into QCArgumentsByTarget class object to
         # cluster them by target (argument_to_be_attached_to).
         qca_by_target = QCArgumentsByTarget(wf_qc_arguments)
         # dictionary containing s3 keys for qc args
         qc_path_dict = {arg: self.file_key(arg) for arg in qca_by_target.qca_argname_list}
         # add this s3 key path info to the QCArgument objects in qca_by_target
         qca_by_target.add_paths(qc_path_dict, self.outbucket)
@@ -1361,15 +1448,15 @@
             yield qc_item
 
     # rna-strandedness (hardcode it for now - later we generalize along with md5)
     def update_rna_strandedness(self):
         if self.app_name != 'rna-strandedness':
             return
         report_arg = self.output_argnames[0]  # assume one output arg
-        if self.ff_output_file(report_arg)['type'] != 'Output report file':
+        if self.ff_output_file(report_arg)['type'] != OUTPUT_REPORT_FILE:
             return
         if self.status(report_arg) == 'FAILED':
             self.ff_meta.run_status = 'error'
             return
         sense, antisense = self.parse_rna_strandedness_report(self.read(report_arg))
         input_arg = 'fastq'
         input_meta = self.file_items(input_arg)[0]  # assume one input file
@@ -1389,15 +1476,15 @@
             return int(strandedness_array[0]), int(strandedness_array[1])
 
     # fastq_first_line
     def update_fastq_first_line(self):
         if self.app_name != 'fastq-first-line':
             return
         report_arg = self.output_argnames[0]  # assume one output arg
-        if self.ff_output_file(report_arg)['type'] != 'Output report file':
+        if self.ff_output_file(report_arg)['type'] != OUTPUT_REPORT_FILE:
             return
         if self.status(report_arg) == 'FAILED':
             self.ff_meta.run_status = 'error'
             return
         first_line = self.parse_fastq_first_line_report(self.read(report_arg))
         input_arg = 'fastq'
         input_meta = self.file_items(input_arg)[0]  # assume one input file
@@ -1416,15 +1503,15 @@
             return fastq_first_line_content[0]
 
     # bam restriction enzyme check
     def update_file_processed_format_re_check(self):
         if self.app_name != 're_checker_workflow':
             return
         report_arg = self.output_argnames[0]  # assume one output arg
-        if self.ff_output_file(report_arg)['type'] != 'Output report file':
+        if self.ff_output_file(report_arg)['type'] != OUTPUT_REPORT_FILE:
             return
         if self.status(report_arg) == 'FAILED':
             self.ff_meta.run_status = 'error'
             return
         percent = self.parse_re_check(self.read(report_arg))
         input_arg = 'bamfile'
         input_meta = self.file_items(input_arg)[0]  # assume one input file
@@ -1449,15 +1536,15 @@
     # md5 report
     def update_md5(self):
         logger.info("updating md5...")
         if self.app_name != 'md5':
             return
         md5_report_arg = self.output_argnames[0]  # assume one output arg
         logger.debug("md5 report arg = %s" % md5_report_arg)
-        if self.ff_output_file(md5_report_arg)['type'] != 'Output report file':
+        if self.ff_output_file(md5_report_arg)['type'] != OUTPUT_REPORT_FILE:
             return
         logger.debug("md5 report arg type = %s" % self.ff_output_file(md5_report_arg)['type'])
         logger.debug("md5 report arg status = %s" % self.status(md5_report_arg))
         logger.debug("self.bucket for md5 report arg = %s" % self.bucket(md5_report_arg))
         if self.status(md5_report_arg) == 'FAILED':
             self.ff_meta.run_status = 'error'
             return
@@ -1535,14 +1622,15 @@
         self.update_all_pfs()
         logger.info("updating report...")
         self.update_md5()
         self.update_rna_strandedness()
         self.update_fastq_first_line()
         self.update_file_processed_format_re_check()
         logger.info("updating qc...")
+        self.update_generic_qc()
         self.update_qc()
         self.update_input_extras()
         self.create_wfr_qc()
         logger.info("posting all...")
         self.post_all()
         logger.info("patching all...")
         self.patch_all()
```

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/qc.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/qc.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 from tibanna.base import (
     SerializableObject
 )
 from collections import namedtuple
 from .exceptions import (
     FdnConnectionException
 )
-from .vars import S3_ENCRYPT_KEY_ID
+from .vars import (
+    S3_ENCRYPT_KEY_ID,
+    OUTPUT_QC_FILE
+)
 
 
 class QCArgument(SerializableObject):
     """This is a class that represents a QC-type workflow argument which is a part of
     a workflow metadata
     """
     def __init__(self, argument_type, workflow_argument_name, argument_to_be_attached_to, qc_type=None,
                  qc_zipped=False, qc_html=False, qc_json=False, qc_table=False,
                  qc_zipped_html=None, qc_zipped_tables=None, qc_acl='public-read',
                  qc_unzip_from_ec2=False, **kwargs):
-        if argument_type != 'Output QC file':
+        if argument_type != OUTPUT_QC_FILE:
             raise Exception("QC Argument must be an Output QC file: %s" % argument_type)
         self.workflow_argument_name = workflow_argument_name
         self.argument_to_be_attached_to = argument_to_be_attached_to
         self.qc_type = qc_type  # qc metadata item type (e.g. quality_metric_fastqc)
         self.qc_zipped = qc_zipped
         self.qc_html = qc_html  # boolean, true if qc is unzipped html
         self.qc_json = qc_json  # boolean, true if qc is unzipped json
@@ -324,15 +327,15 @@
         which is a list of dictionaries. Ideally, wf_arguments should be pre-filtered
         to contain only 'Output QC file' type arguments,
         but if not, the filtering will be done here.
         """
         self.qca_by_target = dict()
         if wf_arguments:
             qca_list = [QCArgument(**arg) for arg in wf_arguments
-                         if arg['argument_type'] == 'Output QC file']
+                         if arg['argument_type'] == OUTPUT_QC_FILE]
             for arg in set([_.argument_to_be_attached_to for _ in qca_list]):
                 self.qca_by_target.update({arg: QCArgumentsPerTarget([_ for _ in qca_list if _.argument_to_be_attached_to == arg])})
 
     @property
     def qca_list(self):
         """generator all all QCArgument items (without going through QCArgumentsPerTarget)"""
         for arg in self.qca_by_target:
```

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/stepfunction.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/stepfunction.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/vars.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/vars.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,23 @@
 _BUCKET_NAME_PROCESSED_FILES = dict()
 _BUCKET_NAME_RAW_FILES = dict()
 _BUCKET_NAME_SYS = dict()
 _BUCKET_NAME_LOG = dict()
 _BUCKET_NAME_CWL = dict()
 
 
+# Workflow argument file types
+OUTPUT_PROCESSED_FILE = 'Output processed file'
+OUTPUT_REPORT_FILE = 'Output report file'
+OUTPUT_QC_FILE = 'Output QC file'
+GENERIC_QC_FILE = 'Generic QC file'
+OUTPUT_TO_BE_EXTRA_INPUT_FILE = 'Output to-be-extra-input file'
+INPUT_FILE = 'Input file'
+
+
 # Secure Tibanna AMI
 # Note that this means only these regions will work (replicate AMI in main account as needed)
 # Note additionally that these AMI's all must be configured to be launchable by our AWS
 # accounts
 AMI_PER_REGION = {
     'x86': {
         'us-east-1': 'ami-00ad035048da98fc2',
```

### Comparing `tibanna_ff-1.3.3/tibanna_ffcommon/wfr.py` & `tibanna_ff-1.4.0b0/tibanna_ffcommon/wfr.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-1.3.3/PKG-INFO` & `tibanna_ff-1.4.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibanna-ff
-Version: 1.3.3
+Version: 1.4.0b0
 Summary: Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.
 Home-page: http://github.com/4dn-dcic/tibanna_ff
 License: MIT
 Keywords: tibanna
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.9
```

