# Comparing `tmp/prosimos-0.1.0.tar.gz` & `tmp/prosimos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosimos-0.1.0.tar", max compression
+gzip compressed data, was "prosimos-0.1.1.tar", max compression
```

## Comparing `prosimos-0.1.0.tar` & `prosimos-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,31 @@
--rw-r--r--   0        0        0    14755 2023-05-10 17:42:38.843014 prosimos-0.1.0/README.md
--rw-r--r--   0        0        0     3569 2023-05-10 15:57:02.367000 prosimos-0.1.0/cli/diff_res_bpsim.py
--rw-r--r--   0        0        0      543 2023-05-11 10:35:58.680493 prosimos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    15464 1970-01-01 00:00:00.000000 prosimos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    14755 2023-05-10 17:42:38.843014 prosimos-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 14:42:49.012095 prosimos-0.1.1/bpdfr_discovery/__init__.py
+-rw-r--r--   0        0        0     3478 2022-07-21 14:22:08.274751 prosimos-0.1.1/bpdfr_discovery/emd_metric.py
+-rw-r--r--   0        0        0      489 2022-09-05 08:40:55.010781 prosimos-0.1.1/bpdfr_discovery/exceptions.py
+-rw-r--r--   0        0        0     7248 2022-07-21 14:22:08.275184 prosimos-0.1.1/bpdfr_discovery/inter_arrival_cases_discovery.py
+-rw-r--r--   0        0        0     5645 2022-07-21 14:22:08.276118 prosimos-0.1.1/bpdfr_discovery/log_comparison_metrics.py
+-rw-r--r--   0        0        0    44123 2023-05-09 14:35:14.254459 prosimos-0.1.1/bpdfr_discovery/log_parser.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:42:35.119495 prosimos-0.1.1/bpdfr_simulation_engine/__init__.py
+-rw-r--r--   0        0        0    44607 2023-05-02 17:28:05.583852 prosimos-0.1.1/bpdfr_simulation_engine/batch_processing.py
+-rw-r--r--   0        0        0     4413 2023-02-17 14:22:25.708112 prosimos-0.1.1/bpdfr_simulation_engine/batch_processing_parser.py
+-rw-r--r--   0        0        0     2656 2023-02-17 14:22:25.709747 prosimos-0.1.1/bpdfr_simulation_engine/case_attributes.py
+-rw-r--r--   0        0        0    48500 2023-05-09 14:35:14.255329 prosimos-0.1.1/bpdfr_simulation_engine/control_flow_manager.py
+-rw-r--r--   0        0        0      487 2023-01-16 17:13:52.476673 prosimos-0.1.1/bpdfr_simulation_engine/exceptions.py
+-rw-r--r--   0        0        0     7355 2023-02-17 14:22:25.711906 prosimos-0.1.1/bpdfr_simulation_engine/execution_info.py
+-rw-r--r--   0        0        0     1109 2023-01-16 17:13:52.479840 prosimos-0.1.1/bpdfr_simulation_engine/file_manager.py
+-rw-r--r--   0        0        0     3177 2023-02-17 14:22:25.712748 prosimos-0.1.1/bpdfr_simulation_engine/prioritisation.py
+-rw-r--r--   0        0        0     1360 2023-03-01 10:12:00.187887 prosimos-0.1.1/bpdfr_simulation_engine/prioritisation_parser.py
+-rw-r--r--   0        0        0     3009 2023-02-17 14:22:25.714177 prosimos-0.1.1/bpdfr_simulation_engine/prioritisation_rules.py
+-rw-r--r--   0        0        0     8585 2023-05-09 14:34:59.262677 prosimos-0.1.1/bpdfr_simulation_engine/probability_distributions.py
+-rw-r--r--   0        0        0    41729 2023-03-01 09:12:49.498726 prosimos-0.1.1/bpdfr_simulation_engine/resource_calendar.py
+-rw-r--r--   0        0        0      467 2022-06-22 13:20:27.228747 prosimos-0.1.1/bpdfr_simulation_engine/resource_profile.py
+-rw-r--r--   0        0        0    28723 2023-05-09 14:34:59.263525 prosimos-0.1.1/bpdfr_simulation_engine/simulation_engine.py
+-rw-r--r--   0        0        0    22178 2023-05-09 14:34:59.264595 prosimos-0.1.1/bpdfr_simulation_engine/simulation_properties_parser.py
+-rw-r--r--   0        0        0     6298 2023-02-17 14:22:25.717592 prosimos-0.1.1/bpdfr_simulation_engine/simulation_queues_ds.py
+-rw-r--r--   0        0        0     6078 2023-05-09 14:34:59.265754 prosimos-0.1.1/bpdfr_simulation_engine/simulation_setup.py
+-rw-r--r--   0        0        0    15595 2022-09-05 08:40:55.012228 prosimos-0.1.1/bpdfr_simulation_engine/simulation_stats.py
+-rw-r--r--   0        0        0    14217 2022-10-24 15:14:16.638398 prosimos-0.1.1/bpdfr_simulation_engine/simulation_stats_calculator.py
+-rw-r--r--   0        0        0     1729 2023-01-16 17:13:52.540574 prosimos-0.1.1/bpdfr_simulation_engine/weekday_helper.py
+-rw-r--r--   0        0        0     3569 2023-05-10 15:57:02.367000 prosimos-0.1.1/cli/diff_res_bpsim.py
+-rw-r--r--   0        0        0      627 2023-05-12 14:45:52.332657 prosimos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15464 1970-01-01 00:00:00.000000 prosimos-0.1.1/PKG-INFO
```

### Comparing `prosimos-0.1.0/README.md` & `prosimos-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.0/cli/diff_res_bpsim.py` & `prosimos-0.1.1/cli/diff_res_bpsim.py`

 * *Files identical despite different names*

### Comparing `prosimos-0.1.0/pyproject.toml` & `prosimos-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "prosimos"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Iryna Halenok, Orlenys López Pintado"]
 readme = "README.md"
-packages = [{include = "cli"}]
+packages = [
+    {include = "cli"},
+    {include = "bpdfr_simulation_engine"},
+    {include = "bpdfr_discovery"}
+]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 click = "^8.1.3"
 numpy = "^1.24.3"
 pandas = "^2.0.1"
 python-dateutil = "^2.8.2"
```

### Comparing `prosimos-0.1.0/PKG-INFO` & `prosimos-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosimos
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Iryna Halenok, Orlenys López Pintado
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

