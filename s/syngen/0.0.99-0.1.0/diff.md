# Comparing `tmp/syngen-0.0.99.tar.gz` & `tmp/syngen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.99.tar", last modified: Tue May  9 12:36:19 2023, max compression
+gzip compressed data, was "syngen-0.1.0.tar", last modified: Fri May 12 13:36:02 2023, max compression
```

## Comparing `syngen-0.0.99.tar` & `syngen-0.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-09 12:34:38.000000 syngen-0.0.99/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-09 12:34:38.000000 syngen-0.0.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-09 12:34:38.000000 syngen-0.0.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-09 12:36:18.996407 syngen-0.0.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-05-09 12:34:38.000000 syngen-0.0.99/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-09 12:34:38.000000 syngen-0.0.99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-09 12:36:19.000407 syngen-0.0.99/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.980407 syngen-0.0.99/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.980407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.988407 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.992407 syngen-0.0.99/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7044 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    30363 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.996407 syngen-0.0.99/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-09 12:34:38.000000 syngen-0.0.99/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:36:18.984407 syngen-0.0.99/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:36:18.000000 syngen-0.0.99/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-12 13:34:41.000000 syngen-0.1.0/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-12 13:34:41.000000 syngen-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-12 13:34:41.000000 syngen-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-12 13:36:02.153201 syngen-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-12 13:34:41.000000 syngen-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-12 13:34:41.000000 syngen-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-12 13:36:02.153201 syngen-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.141201 syngen-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.141201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15901 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.99/LICENSE` & `syngen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/PKG-INFO` & `syngen-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.99
+Version: 0.1.0
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -87,15 +87,15 @@
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
-- <i>print_report</i> - whether to generate plots of accuracy report and sample report
+- <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
 - <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
@@ -129,15 +129,15 @@
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
-- <i>print_report</i> – whether to generate plots of accuracy report, sample report
+- <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
 - <i>metadata_path</i> – a path to metadata file to generate linked tables
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.99 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.0 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -42,60 +42,62 @@
 as a reference - table_name â required parameter for training of single
 table, an arbitrary string to name the directories - epochs â a number of
 training epochs. Since the early stopping mechanism is implemented the bigger
 value of epochs is the better - row_limit â a number of rows to train over. A
 number less than the original table length will randomly subset the specified
 number of rows - drop_null â whether to drop rows with at least one missing
 value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate plots of accuracy report
-and sample report - metadata_path â a path to the metadata file containing
-the metadata for linked tables - column_types - might include the section
-categorical which contains the listed columns defined as categorical by a user
-Requirements for parameters of training process: * source - data type - string
-* table_name - data type - string * epochs - data type - integer, must be equal
-to or more than 1, default value is 10 * row_limit - data type - integer *
-drop_null - data type - boolean, default value - False * batch_size - data type
-- integer, must be equal to or more than 1, default value - 32 * print_report -
-data type - boolean, default value is False * metadata_path - data type -
-string * column_types - data type - dictionary with the key categorical - the
-list of columns (data type - string) ### Inference (generation) You can
-customize the inference processes by calling for one table: ```bash infer --
-size INT \ --table_name STR \ --run_parallel BOOL \ --batch_size INT \ --
-random_seed INT \ --print_report BOOL ``` For linked tables you can simply
-call: ```bash infer --metadata_path PATH_TO_METADATA ``` The parameters which
-you can set up for generation process: - size - the desired number of rows to
-generate - table_name â required parameter for inference of single table, the
-name of the table, same as in training - run_parallel â whether to use
-multiprocessing (feasible for tables > 5000 rows) - batch_size â if
-specified, the generation is split into batches. This can save the RAM -
+can save the RAM - print_report - whether to generate accuracy and sampling
+reports. Please note that the sampling report is generated only if the
+`row_limit` parameter is set. - metadata_path â a path to the metadata file
+containing the metadata for linked tables - column_types - might include the
+section categorical which contains the listed columns defined as categorical by
+a user Requirements for parameters of training process: * source - data type -
+string * table_name - data type - string * epochs - data type - integer, must
+be equal to or more than 1, default value is 10 * row_limit - data type -
+integer * drop_null - data type - boolean, default value - False * batch_size -
+data type - integer, must be equal to or more than 1, default value - 32 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string * column_types - data type - dictionary with the key
+categorical - the list of columns (data type - string) ### Inference
+(generation) You can customize the inference processes by calling for one
+table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
+batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
+you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
+parameters which you can set up for generation process: - size - the desired
+number of rows to generate - table_name â required parameter for inference of
+single table, the name of the table, same as in training - run_parallel â
+whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
+â if specified, the generation is split into batches. This can save the RAM -
 random_seed â if specified, generates a reproducible result - print_report
-â whether to generate plots of accuracy report, sample report - metadata_path
-â a path to metadata file to generate linked tables Requirements for
-parameters of generation process: * size - data type - integer, must be equal
-to or more than 1, default value is 100 * table_name - data type - string *
-run_parallel - data type - boolean, default value is False * batch_size - data
-type - integer, must be equal to or more than 1 * random_seed - data type -
-integer, must be equal to or more than 0 * print_report - data type - boolean,
-default value is False * metadata_path - data type - string The metadata can
-contain any of the arguments above for each table. If so, the duplicated
-arguments from the CLI will be ignored. ### Linked tables generation To
-generate linked tables, you should provide metadata in yaml format. It is used
-to handle complex relations for any number of tables. You can also specify
-additional parameters needed for training and inference in the metadata file
-and in this case, they will be ignored in the CLI call. The yaml metadata file
-should match the following template: CUSTOMER: # Table name source: "./files/
-customer.csv" # Supported formats include local files in CSV, Avro formats
-train_settings: # Settings for training process epochs: 10 # Number of epochs
-if different from the default in the command line options drop_null: False #
-Drop rows with NULL values row_limit: None # Number of rows to train over. A
-number less than the original table length will randomly subset the specified
-rows number batch_size: 32 # If specified, the training is split into batches.
-This can save the RAM print_report: False # Turn on or turn off generation of
-the report column_types: categorical: # Force listed columns to have
-categorical type (use dictionary of values) - gender - marital_status
+â whether to generate accuracy and sampling reports. Please note that the
+sampling report is generated only if the row_limit parameter is set. -
+metadata_path â a path to metadata file to generate linked tables
+Requirements for parameters of generation process: * size - data type -
+integer, must be equal to or more than 1, default value is 100 * table_name -
+data type - string * run_parallel - data type - boolean, default value is False
+* batch_size - data type - integer, must be equal to or more than 1 *
+random_seed - data type - integer, must be equal to or more than 0 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string The metadata can contain any of the arguments above for each
+table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+tables generation To generate linked tables, you should provide metadata in
+yaml format. It is used to handle complex relations for any number of tables.
+You can also specify additional parameters needed for training and inference in
+the metadata file and in this case, they will be ignored in the CLI call. The
+yaml metadata file should match the following template: CUSTOMER: # Table name
+source: "./files/customer.csv" # Supported formats include local files in CSV,
+Avro formats train_settings: # Settings for training process epochs: 10 #
+Number of epochs if different from the default in the command line options
+drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
+to train over. A number less than the original table length will randomly
+subset the specified rows number batch_size: 32 # If specified, the training is
+split into batches. This can save the RAM print_report: False # Turn on or turn
+off generation of the report column_types: categorical: # Force listed columns
+to have categorical type (use dictionary of values) - gender - marital_status
 infer_settings: # Settings for infer process size: 100 # Size for generated
 data run_parallel: False # Turn on or turn off parallel training process
 print_report: False # Turn on or turn off generation of the report batch_size:
 None # If specified, the generation is split into batches. This can save the
 RAM random_seed: None # If specified, generates a reproducible result keys:
 PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
 type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
```

### Comparing `syngen-0.0.99/README.md` & `syngen-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
-- <i>print_report</i> - whether to generate plots of accuracy report and sample report
+- <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
 - <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
@@ -110,15 +110,15 @@
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
-- <i>print_report</i> – whether to generate plots of accuracy report, sample report
+- <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
 - <i>metadata_path</i> – a path to metadata file to generate linked tables
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
```

#### html2text {}

```diff
@@ -32,60 +32,62 @@
 as a reference - table_name â required parameter for training of single
 table, an arbitrary string to name the directories - epochs â a number of
 training epochs. Since the early stopping mechanism is implemented the bigger
 value of epochs is the better - row_limit â a number of rows to train over. A
 number less than the original table length will randomly subset the specified
 number of rows - drop_null â whether to drop rows with at least one missing
 value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate plots of accuracy report
-and sample report - metadata_path â a path to the metadata file containing
-the metadata for linked tables - column_types - might include the section
-categorical which contains the listed columns defined as categorical by a user
-Requirements for parameters of training process: * source - data type - string
-* table_name - data type - string * epochs - data type - integer, must be equal
-to or more than 1, default value is 10 * row_limit - data type - integer *
-drop_null - data type - boolean, default value - False * batch_size - data type
-- integer, must be equal to or more than 1, default value - 32 * print_report -
-data type - boolean, default value is False * metadata_path - data type -
-string * column_types - data type - dictionary with the key categorical - the
-list of columns (data type - string) ### Inference (generation) You can
-customize the inference processes by calling for one table: ```bash infer --
-size INT \ --table_name STR \ --run_parallel BOOL \ --batch_size INT \ --
-random_seed INT \ --print_report BOOL ``` For linked tables you can simply
-call: ```bash infer --metadata_path PATH_TO_METADATA ``` The parameters which
-you can set up for generation process: - size - the desired number of rows to
-generate - table_name â required parameter for inference of single table, the
-name of the table, same as in training - run_parallel â whether to use
-multiprocessing (feasible for tables > 5000 rows) - batch_size â if
-specified, the generation is split into batches. This can save the RAM -
+can save the RAM - print_report - whether to generate accuracy and sampling
+reports. Please note that the sampling report is generated only if the
+`row_limit` parameter is set. - metadata_path â a path to the metadata file
+containing the metadata for linked tables - column_types - might include the
+section categorical which contains the listed columns defined as categorical by
+a user Requirements for parameters of training process: * source - data type -
+string * table_name - data type - string * epochs - data type - integer, must
+be equal to or more than 1, default value is 10 * row_limit - data type -
+integer * drop_null - data type - boolean, default value - False * batch_size -
+data type - integer, must be equal to or more than 1, default value - 32 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string * column_types - data type - dictionary with the key
+categorical - the list of columns (data type - string) ### Inference
+(generation) You can customize the inference processes by calling for one
+table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
+batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
+you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
+parameters which you can set up for generation process: - size - the desired
+number of rows to generate - table_name â required parameter for inference of
+single table, the name of the table, same as in training - run_parallel â
+whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
+â if specified, the generation is split into batches. This can save the RAM -
 random_seed â if specified, generates a reproducible result - print_report
-â whether to generate plots of accuracy report, sample report - metadata_path
-â a path to metadata file to generate linked tables Requirements for
-parameters of generation process: * size - data type - integer, must be equal
-to or more than 1, default value is 100 * table_name - data type - string *
-run_parallel - data type - boolean, default value is False * batch_size - data
-type - integer, must be equal to or more than 1 * random_seed - data type -
-integer, must be equal to or more than 0 * print_report - data type - boolean,
-default value is False * metadata_path - data type - string The metadata can
-contain any of the arguments above for each table. If so, the duplicated
-arguments from the CLI will be ignored. ### Linked tables generation To
-generate linked tables, you should provide metadata in yaml format. It is used
-to handle complex relations for any number of tables. You can also specify
-additional parameters needed for training and inference in the metadata file
-and in this case, they will be ignored in the CLI call. The yaml metadata file
-should match the following template: CUSTOMER: # Table name source: "./files/
-customer.csv" # Supported formats include local files in CSV, Avro formats
-train_settings: # Settings for training process epochs: 10 # Number of epochs
-if different from the default in the command line options drop_null: False #
-Drop rows with NULL values row_limit: None # Number of rows to train over. A
-number less than the original table length will randomly subset the specified
-rows number batch_size: 32 # If specified, the training is split into batches.
-This can save the RAM print_report: False # Turn on or turn off generation of
-the report column_types: categorical: # Force listed columns to have
-categorical type (use dictionary of values) - gender - marital_status
+â whether to generate accuracy and sampling reports. Please note that the
+sampling report is generated only if the row_limit parameter is set. -
+metadata_path â a path to metadata file to generate linked tables
+Requirements for parameters of generation process: * size - data type -
+integer, must be equal to or more than 1, default value is 100 * table_name -
+data type - string * run_parallel - data type - boolean, default value is False
+* batch_size - data type - integer, must be equal to or more than 1 *
+random_seed - data type - integer, must be equal to or more than 0 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string The metadata can contain any of the arguments above for each
+table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+tables generation To generate linked tables, you should provide metadata in
+yaml format. It is used to handle complex relations for any number of tables.
+You can also specify additional parameters needed for training and inference in
+the metadata file and in this case, they will be ignored in the CLI call. The
+yaml metadata file should match the following template: CUSTOMER: # Table name
+source: "./files/customer.csv" # Supported formats include local files in CSV,
+Avro formats train_settings: # Settings for training process epochs: 10 #
+Number of epochs if different from the default in the command line options
+drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
+to train over. A number less than the original table length will randomly
+subset the specified rows number batch_size: 32 # If specified, the training is
+split into batches. This can save the RAM print_report: False # Turn on or turn
+off generation of the report column_types: categorical: # Force listed columns
+to have categorical type (use dictionary of values) - gender - marital_status
 infer_settings: # Settings for infer process size: 100 # Size for generated
 data run_parallel: False # Turn on or turn off parallel training process
 print_report: False # Turn on or turn off generation of the report batch_size:
 None # If specified, the generation is split into batches. This can save the
 RAM random_seed: None # If specified, generates a reproducible result keys:
 PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
 type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
```

### Comparing `syngen-0.0.99/setup.cfg` & `syngen-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/infer.py` & `syngen-0.1.0/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/config/configurations.py` & `syngen-0.1.0/src/syngen/ml/config/configurations.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     """
     The configuration class to set up the work of train process
     """
     source: Optional[str]
     epochs: int
     drop_null: bool
     row_limit: Optional[int]
-    random_state: Optional[int]
     table_name: Optional[str]
     metadata_path: Optional[str]
     print_report: bool
     batch_size: int
     paths: Dict = field(init=False)
     row_subset: int = field(init=False)
     schema: Dict = field(init=False)
     slugify_table_name: str = field(init=False)
 
     def __post_init__(self):
         self.paths = self._set_paths()
         self._prepare_dirs()
+
+    def preprocess_data(self):
         data, self.schema = self._extract_data()
-        self._prepare_data(data, self.random_state)
+        self._prepare_data(data)
         self._set_batch_size()
 
     def to_dict(self) -> Dict:
         """
         Return the values of the settings of training process
         """
         return {
@@ -102,29 +103,29 @@
         Extract data and schema necessary for training process
         """
         data, schema = self._load_source()
         data, dropped_columns = self._remove_empty_columns(data)
         schema = self._mark_removed_columns(data, schema, dropped_columns)
         return data, schema
 
-    def _preprocess_data(self, data: pd.DataFrame, random_state) -> pd.DataFrame:
+    def _preprocess_data(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Preprocess data and set the parameter "row_subset" for training process
         """
         if self.drop_null:
             if not data.dropna().empty:
                 data = data.dropna()
             else:
                 logger.warning("The specified 'drop_null' argument results in the empty dataframe, "
                                "so it will be ignored")
 
         if self.row_limit:
             self.row_subset = min(self.row_limit, len(data))
 
-            data = data.sample(n=self.row_subset, random_state=random_state)
+            data = data.sample(n=self.row_subset)
 
             if len(data) < 100:
                 logger.warning("The input table is too small to provide any meaningful results. "
                                "Please consider 1) disable drop_null argument, 2) provide bigger table")
             elif len(data) < 500:
                 logger.warning(
                     f"The amount of data is {len(data)} rows. It seems that it isn't enough to supply "
@@ -135,19 +136,19 @@
 
         self.row_subset = len(data)
         return data
 
     def _save_input_data(self, data: pd.DataFrame):
         DataLoader(self.paths["input_data_path"]).save_data(self.paths["input_data_path"], data)
 
-    def _prepare_data(self, data: pd.DataFrame, random_state):
+    def _prepare_data(self, data: pd.DataFrame):
         """
         Preprocess and save data necessary for training process
         """
-        data = self._preprocess_data(data, random_state)
+        data = self._preprocess_data(data)
         self._save_input_data(data)
 
     @slugify_attribute(table_name="slugify_table_name")
     def _set_paths(self) -> Dict:
         """
         Create the paths which used in training process
         """
```

### Comparing `syngen-0.0.99/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.0/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.0/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.0/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     BivariateMetric,
     JensenShannonDistance,
     Correlations,
     Clustering,
     Utility
 )
 from syngen.ml.metrics.utils import transform_to_base64
-from syngen.ml.data_loaders import BinaryLoader
+from syngen.ml.utils import fetch_training_config
+
 
 
 class BaseTest(ABC):
     def __init__(
             self,
             original: pd.DataFrame,
             synthetic: pd.DataFrame,
@@ -54,21 +55,14 @@
 
     def _remove_artifacts(self):
         """
         Remove artifacts after creating Accuracy report
         """
         shutil.rmtree(self.draws_path)
 
-    def _fetch_training_config(self):
-        """
-        Fetch the parameters of the training configuration
-        """
-        training_config, _ = BinaryLoader().load_data(self.paths["train_config_pickle_path"])
-        return training_config
-
 
 class AccuracyTest(BaseTest):
     def __init__(
             self,
             original: pd.DataFrame,
             synthetic: pd.DataFrame,
             paths: dict,
@@ -122,15 +116,15 @@
                                clusters_barplot=transform_to_base64(f"{draws_acc_path}/clusters_barplot.svg"),
                                clustering_value=clustering_result,
                                bi_imgs=bi_images,
                                utility_barplot=transform_to_base64(f"{draws_acc_path}/utility_barplot.svg"),
                                utility_table=utility_result.to_html(),
                                is_data_available=False if utility_result.empty else True,
                                table_name=self.table_name,
-                               training_config=self._fetch_training_config(),
+                               training_config=fetch_training_config(self.paths["train_config_pickle_path"]).to_dict(),
                                inference_config=self.config,
                                time=datetime.now().strftime("%H:%M:%S %d/%m/%Y")
                                )
 
         with open(f"{self.paths['draws_path']}/accuracy_report.html", 'w', encoding="utf-8") as f:
             f.write(html)
```

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/metrics/utils.py` & `syngen-0.1.0/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.0/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.0/src/syngen/ml/strategies/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 import os
 import traceback
-import random
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 from loguru import logger
 from syngen.ml.train_chain import RootHandler
 from syngen.ml.reporters import (
     Report,
     AccuracyReporter,
@@ -19,16 +18,14 @@
     LongTextsHandler,
     VaeTrainHandler,
     VaeInferHandler
 )
 from syngen.ml.vae import VanillaVAEWrapper
 from syngen.ml.data_loaders import BinaryLoader
 
-RANDOM_STATE = random.randint(0, 2 ** 32 - 1)
-
 class Strategy(ABC):
     """
     Abstract class for the strategies of training or infer process
     """
     def __init__(self):
         self.handler = None
         self.config = None
@@ -69,23 +66,24 @@
 class TrainStrategy(Strategy, ABC):
     """
     Class of the strategies of training process
     """
     def _save_training_config(self):
         BinaryLoader().save_data(
             path=self.config.paths["train_config_pickle_path"],
-            data=self.config.to_dict()
+            data=self.config
         )
 
     def set_config(self, **kwargs):
         """
         Set up configuration for training process
         """
         configuration = TrainConfig(**kwargs)
         self.config = configuration
+        self.config.preprocess_data()
         self._save_training_config()
         return self
 
     def add_handler(self):
         """
         Set up the handler which used in training process
         """
@@ -141,16 +139,15 @@
             source=kwargs["source"],
             epochs=kwargs["epochs"],
             drop_null=kwargs["drop_null"],
             row_limit=kwargs["row_limit"],
             table_name=kwargs["table_name"],
             metadata_path=kwargs["metadata_path"],
             print_report=kwargs["print_report"],
-            batch_size=kwargs["batch_size"],
-            random_state=RANDOM_STATE
+            batch_size=kwargs["batch_size"]
         )
 
         self.add_reporters().\
             set_metadata(kwargs["metadata"]).\
             add_handler()
 
         try:
```

### Comparing `syngen-0.0.99/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.0/src/syngen/ml/train_chain/train_chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import random
 from typing import Tuple, Optional, Dict, List
 from abc import ABC, abstractmethod
 import os
 import math
+import uuid
+from ulid import ULID
+from uuid import UUID
 from dataclasses import dataclass, field
 
 import pandas as pd
 import numpy as np
 from loguru import logger
 from numpy.random import seed, choice
 from pathos.multiprocessing import ProcessingPool
@@ -223,21 +227,66 @@
         return is_pk
 
     def _concat_slices_with_unique_pk(self, df_slices: list):
         if self.metadata and self.table_name in self.metadata:
             config_of_keys = self.metadata.get(self.table_name).get("keys", {})
             for key in config_of_keys.keys():
                 column = config_of_keys.get(key).get("columns")[0]
-                if config_of_keys.get(key).get("type") == "PK" and not isinstance(df_slices[0][column][0], str):
+                if config_of_keys.get(key).get("type") == "PK" and not isinstance(df_slices[0][column][0], (str, UUID, ULID)):
                     cumm_len = 0
                     for i, frame in enumerate(df_slices):
                         frame[column] = frame[column].map(lambda pk_val: pk_val + cumm_len)
                         cumm_len += len(frame)
         return pd.concat(df_slices, ignore_index=True)
 
+    def _generate_uuids(self, version: int, size: int):
+        ulid = ULID()
+        generated_uuid_column = []
+        for i in range(size):
+            if version != "ulid":
+                generated_uuid_column.append(uuid.UUID(int=random.getrandbits(128), version=int(version)))
+            else:
+                generated_uuid_column.append(ulid.generate())
+        return generated_uuid_column
+
+    def generate_vae(self, size, data, schema):
+        self.vae = self.create_wrapper(
+            self.wrapper_name,
+            data,
+            schema,
+            metadata={"table_name": self.table_name},
+            table_name=self.table_name,
+            paths=self.paths,
+            batch_size=self.batch_size,
+            process="infer"
+        )
+        self.vae.load_state(self.paths["state_path"])
+        synthetic_infer = self.vae.predict_sampled_df(size)
+        return synthetic_infer
+
+    def generate_long_texts(self, size, synthetic_infer):
+        with open(f'{self.paths["path_to_no_ml"]}', "rb") as file:
+            features = dill.load(file)
+        for col in features.keys():
+            kde = features[col]["kde"]
+            text_structures = np.maximum(kde.resample(size).astype('int32'), 0)
+            indexes = features[col]["indexes"]
+            counts = features[col]["counts"]
+            generated_column = [" ".join([self.synth_word(s, indexes, counts) for s in
+                                          np.maximum(np.random.normal(i / j, 1, j).astype('int32'), 2)])
+                                for i, j in zip(*text_structures)]
+            synthetic_infer[col] = generated_column
+        return synthetic_infer
+
+    def generate_uuid(self, size, dataset, uuid_columns, synthetic_infer):
+        uuid_columns_types = dataset.uuid_columns_types
+        for col in uuid_columns:
+            synthetic_infer[col] = self._generate_uuids(uuid_columns_types[col], size)
+        return synthetic_infer
+
     def run_separate(self, params: Tuple):
         i, size = params
 
         if self.random_seed:
             seed(self.random_seeds_list[i])
 
         input_data_existed = DataLoader(self.paths["input_data_path"]).has_existed_path
@@ -246,38 +295,22 @@
             data, schema = DataLoader(self.paths["input_data_path"]).load_data()
         else:
             data = pd.DataFrame()
             schema = None
 
         synthetic_infer = pd.DataFrame()
         if self.has_vae:
-            self.vae = self.create_wrapper(
-                self.wrapper_name,
-                data,
-                schema,
-                metadata={"table_name": self.table_name},
-                table_name=self.table_name,
-                paths=self.paths,
-                batch_size=self.batch_size,
-                process="infer"
-            )
-            self.vae.load_state(self.paths["state_path"])
-            synthetic_infer = self.vae.predict_sampled_df(size)
+            synthetic_infer = self.generate_vae(size, data, schema)
         if self.has_no_ml:
-            with open(f'{self.paths["path_to_no_ml"]}', "rb") as file:
-                features = dill.load(file)
-            for col in features.keys():
-                kde = features[col]["kde"]
-                text_structures = np.maximum(kde.resample(size).astype('int32'), 0)
-                indexes = features[col]["indexes"]
-                counts = features[col]["counts"]
-                generated_column = [" ".join([self.synth_word(s, indexes, counts) for s in
-                                              np.maximum(np.random.normal(i / j, 1, j).astype('int32'), 2)])
-                                    for i, j in zip(*text_structures)]
-                synthetic_infer[col] = generated_column
+            synthetic_infer = self.generate_long_texts(size, synthetic_infer)
+
+        dataset = fetch_dataset(self.paths["dataset_pickle_path"])
+        uuid_columns = dataset.uuid_columns
+        if uuid_columns:
+            synthetic_infer = self.generate_uuid(size, dataset, uuid_columns, synthetic_infer)
 
         return synthetic_infer
 
     @staticmethod
     def split_by_batches(size, nodes):
         quote = int(size / nodes)
         data = [quote] * nodes
@@ -314,15 +347,15 @@
             fk_pdf = np.maximum(kde.evaluate(numeric_pk), 1e-12)
             synth_fk = np.random.choice(pk, size=size, p=fk_pdf / sum(fk_pdf), replace=True)
             synth_fk = pd.DataFrame({fk_label: synth_fk}).reset_index(drop=True)
 
         except FileNotFoundError:
             logger.warning(f"The mapper for the {fk_label} text key is not found. Making simple sampling")
             synth_fk = pk.sample(size, replace=True).reset_index(drop=True)
-            synth_fk.rename(fk_label, inplace=True)
+            synth_fk = synth_fk.rename(fk_label)
 
         return synth_fk
 
     @staticmethod
     @slugify_parameters()
     def _set_pk_path(pk_table) -> str:
         """
@@ -340,30 +373,31 @@
     def generate_keys(self, generated, size, metadata, table_name):
         metadata_of_table = metadata.get(table_name)
         if "keys" not in metadata_of_table:
             return None
         config_of_keys = metadata_of_table.get("keys")
         for key in config_of_keys.keys():
             if config_of_keys.get(key).get("type") == "FK":
+                fk_column_name = config_of_keys.get(key).get("columns")[0]
                 pk_table = config_of_keys.get(key).get("references").get("table")
                 pk_path = self._set_pk_path(pk_table=pk_table)
                 pk_table_data, pk_table_schema = DataLoader(pk_path).load_data()
                 pk_column_label = config_of_keys.get(key).get("references").get("columns")[0]
                 logger.info(f"The {pk_column_label} assigned as a foreign_key feature")
 
-                synth_fk = self.kde_gen(pk_table_data, pk_column_label, size, config_of_keys.get(key).get("columns")[0])
+                synth_fk = self.kde_gen(pk_table_data, pk_column_label, size, fk_column_name)
                 generated = generated.reset_index(drop=True)
 
                 null_column_name = f"{key}_null"
                 if null_column_name in generated.columns:
                     not_null_column_mask = generated[null_column_name].astype("float64") <= 0.5
                     synth_fk = synth_fk.where(not_null_column_mask, np.nan)
                     generated = generated.drop(null_column_name, axis=1)
 
-                generated = pd.concat([generated, synth_fk], axis=1)
+                generated[fk_column_name] = synth_fk
         return generated
 
     def handle(
             self,
             **kwargs
     ):
         self._prepare_dir()
```

### Comparing `syngen-0.0.99/src/syngen/ml/utils/utils.py` & `syngen-0.1.0/src/syngen/ml/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pickle
 from datetime import datetime, timedelta
 
 import pandas as pd
 import numpy as np
 from slugify import slugify
 from loguru import logger
+import pickle as pkl
 
 
 def get_date_columns(df: pd.DataFrame, str_columns: List[str]):
     # TODO: extend pattern to more formats
     # pattern = r'\d{2}(\.|/|\-)\d{2}(\.|/|\-)(\d{2}|\d{4})'
     # pattern = r"\s{0,1}\d+[-/\\:]\s{0,1}\d+[-/\\:]\s{0,1}\d+"
 
@@ -184,7 +185,14 @@
     Check if features are assigned in the dataset
     """
     features = fetch_dataset(dataset_pickle_path).features
     if len(features) == 0:
         logger.info("No features to train VAE on")
         return False
     return True
+
+def fetch_training_config(train_config_pickle_path):
+    """
+    Fetch the parameters of the training configuration
+    """
+    with open(train_config_pickle_path, "rb") as f:
+        return pkl.load(f)
```

### Comparing `syngen-0.0.99/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.0/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.0/src/syngen/ml/vae/models/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Dict, Optional, List, Tuple
 from dataclasses import dataclass, field
 import pickle
+from uuid import UUID
+from datetime import datetime
+import base32_crockford
 
 from loguru import logger
 import numpy as np
 import dill
 import pandas as pd
 from scipy.stats import gaussian_kde
 
@@ -111,15 +114,17 @@
         Set up list of data types of primary and unique keys
         """
         self.pk_uq_keys_types = {}
         for key_name, config in pk_uq_keys_mapping.items():
             key_columns = config.get("columns")
             for column in key_columns:
                 column_type = \
-                    str if column in (self.str_columns | self.categ_columns | self.date_columns | self.long_text_columns) \
+                    str if column in (
+                        self.str_columns | self.categ_columns | self.date_columns | self.long_text_columns | self.uuid_columns
+                    ) \
                     else float
                 self.pk_uq_keys_types[column] = column_type
 
     def __map_text_pk(self):
         for pk, pk_type in self.pk_uq_keys_types.items():
             if pk_type is str:
                 mapper = {k: n for n, k in enumerate(self.df[pk])}
@@ -267,54 +272,111 @@
             [
                 col for col in df.columns
                 if df[col].dropna().nunique() <= 50 and col not in self.binary_columns
             ]
         )
         self.categ_columns.update(defined_columns)
 
+    def _select_str_columns(self, df):
+        if self.schema.get("format", "") == "CSV":
+            data_subset = df.select_dtypes(include=[pd.StringDtype(), "object"])
+        else:
+            text_columns = [
+                col for col, data_type in self.schema.get("fields", {}).items()
+                if data_type == "string"
+            ]
+            data_subset = df[text_columns]
+        return data_subset
+
     def _set_categorical_columns(self, df: pd.DataFrame, schema: Dict):
         """
         Set up the list of categorical columns
         """
         self._fetch_categorical_columns()
         self._define_categorical_columns(df)
         self._check_if_column_categorical(schema=schema)
 
     def _set_long_text_columns(self, df: pd.DataFrame):
         """
         Set up the list of columns with long texts (> 200 symbols)
         """
-        if self.schema.get("format", "") == "CSV":
-            data_subset = df.select_dtypes(include=[pd.StringDtype(), "object"])
-        else:
-            text_columns = [
-                col for col, data_type in self.schema.get("fields", {}).items()
-                if data_type == "string"
-            ]
-            data_subset = df[text_columns]
+        data_subset = self._select_str_columns(df)
+
         self.long_text_columns = set()
         if not data_subset.empty:
             data_subset = data_subset.loc[:, data_subset.apply(lambda x: (x.str.len() > 200).any())]
             self.long_text_columns = set(data_subset.columns)
             self.long_text_columns -= self.categ_columns
             if self.long_text_columns:
                 logger.info(
                     f"Please note that the columns - {self.long_text_columns} contain long texts (> 200 symbols). "
                     f"Such texts' handling consumes significant resources and results in poor quality content, "
                     f"therefore this column(-s) will be generated using a simplified statistical approach")
 
+    def _is_valid_ulid(self, uuid):
+        """
+        Check if uuid_to_test is a valid ULID (https://github.com/ulid/spec)
+        """
+        ulid_timestamp = uuid[:10]
+        try:
+            assert len(uuid) == 26
+            ulid_timestamp_int = base32_crockford.decode(ulid_timestamp)
+            datetime.fromtimestamp(ulid_timestamp_int / 1000.0)
+            return "ulid"
+        except:
+            return
+
+    def _is_valid_uuid(self, x):
+        """
+        Check if uuid_to_test is a valid UUID
+        """
+        result = []
+        for i in x:
+            for v in [1, 2, 3, 4, 5]:
+                try:
+                    uuid_obj = UUID(i, version=v)
+                    if str(uuid_obj) == i or str(uuid_obj).replace("-", "") == i:
+                        result.append(v)
+                except ValueError:
+                    continue
+            result.append(self._is_valid_ulid(i))
+        # returning the mode of the list, i.e. the most frequent element
+        if result:
+            return max(set(result), key=result.count)
+        else:
+            return 0
+
+    def _set_uuid_columns(self, df: pd.DataFrame):
+        """
+        Set up the list of columns with uuid
+        """
+
+        data_subset = self._select_str_columns(df)
+
+        self.uuid_columns = {}
+        self.uuid_columns_types = {}
+        if not data_subset.empty:
+            data_subset = data_subset.dropna().apply(self._is_valid_uuid)
+            self.uuid_columns_types = dict(data_subset[data_subset.isin([1, 2, 3, 4, 5, "ulid"])])
+            self.uuid_columns = set(self.uuid_columns_types.keys())
+            if self.uuid_columns:
+                logger.info(
+                    f"The columns - {self.uuid_columns} contain UUIDs")
+
+
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
         """
         if check_object_on_float:
             columns_nan_labels = get_nan_labels(df)
             df = nan_labels_to_float(df, columns_nan_labels)
 
+        self._set_uuid_columns(df)
         self._set_binary_columns(df)
         self._set_categorical_columns(df, schema)
         self._set_long_text_columns(df)
         tmp_df = get_tmp_df(df)
         self.float_columns = set(tmp_df.select_dtypes(include=["float", "float64"]).columns)
         self.int_columns = set(tmp_df.select_dtypes(include=["int", "int64"]).columns)
 
@@ -323,20 +385,22 @@
             if all(x.is_integer() for x in tmp_df[col]):
                 float_to_int_cols.add(col)
 
         self.int_columns = (self.int_columns | float_to_int_cols) - (self.categ_columns | self.binary_columns)
         self.float_columns = self.float_columns - self.categ_columns - self.int_columns - self.binary_columns
         self.str_columns = \
             set(tmp_df.columns) - self.float_columns - self.categ_columns - \
-            self.int_columns - self.binary_columns - self.long_text_columns
+            self.int_columns - self.binary_columns - self.long_text_columns - set(self.uuid_columns)
         self.categ_columns -= self.long_text_columns
         self.date_columns = \
             get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
             self.binary_columns - self.long_text_columns
         self.str_columns -= self.date_columns
+        self.uuid_columns = self.uuid_columns - self.categ_columns - self.binary_columns
+        self.uuid_columns_types = {k: v for k, v in self.uuid_columns_types.items() if k in self.uuid_columns}
 
     def _avro_data_pipeline(self, df, schema):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table in Avro format is present
         """
         logger.info(f"The schema of table - {self.table_name} was received")
@@ -351,29 +415,31 @@
         self.categ_columns -= self.long_text_columns
         self.str_columns = \
             self.str_columns - self.categ_columns - self.int_columns - self.binary_columns - self.long_text_columns
         self.date_columns = \
             get_date_columns(df, list(self.str_columns)) - self.categ_columns - \
             self.binary_columns - self.long_text_columns
         self.str_columns -= self.date_columns
+        self.long_text_columns -= self.uuid_columns
 
     def __data_pipeline(self, df: pd.DataFrame, schema: Optional[Dict]):
         if schema.get("format") == "CSV":
             self._general_data_pipeline(df, schema)
         elif schema.get("format") == 'Avro':
             schema = self._update_schema(schema, df)
             self._avro_data_pipeline(df, schema.get("fields"))
 
         assert len(self.str_columns) + \
                len(self.float_columns) + \
                len(self.int_columns) + \
                len(self.date_columns) + \
                len(self.categ_columns) + \
                len(self.binary_columns) + \
-               len(self.long_text_columns) == len(df.columns), "According to number of columns with defined types, " \
+               len(self.long_text_columns) + \
+               len(self.uuid_columns) == len(df.columns), "According to number of columns with defined types, " \
                                                                "column types are not identified correctly"
 
         logger.debug(
             f"Count of string columns: {len(self.str_columns)}; "
             + f"Count of float columns: {len(self.float_columns)}; "
             + f"Count of int columns: {len(self.int_columns)}; "
             + f"Count of categorical columns: {len(self.categ_columns)}; "
@@ -555,15 +621,16 @@
                         pk_table=correspondent_pk_table,
                         pk_column=correspondent_pk_col,
                         fk_column=fk_column
                     )
                     if mapper is None:
                         continue
                     fk_column_values = fk_column_values.map(mapper)
-                kde = gaussian_kde(fk_column_values)
+                noise_to_prevent_singularity = np.random.normal(0, 0.0001, len(fk_column_values))
+                kde = gaussian_kde(fk_column_values + noise_to_prevent_singularity)
                 self._save_kde_artifacts(kde=kde, fk_kde_path=self.fk_kde_path, fk_column=fk_column)
 
     def __drop_fk_columns(self):
         """
         Drop columns in dataframe which defined as foreign key
         """
         for fk in self.foreign_keys_list:
```

### Comparing `syngen-0.0.99/src/syngen/ml/vae/models/features.py` & `syngen-0.1.0/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/vae/models/model.py` & `syngen-0.1.0/src/syngen/ml/vae/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
             log_likelihoods = self.latent_model.score_samples(latent_sample)
             sliced_latent_sample.append(pop_npoints(latent_sample, log_likelihoods))
 
         synthetic_prediction = self.generator_model.predict(sliced_latent_sample)
         return self.dataset.inverse_transform(synthetic_prediction)
 
     def __check_pk_numeric_convertability(self, column, key_type):
-        if key_type is str and column not in self.dataset.long_text_columns:
+        if key_type is str and column not in self.dataset.long_text_columns | self.dataset.uuid_columns:
             return self.inverse_transformed_df[column].dropna().str.isnumeric().all()
         else:
             return False
 
     def __make_pk_uq_unique(self, pk_uq_keys_mapping):
         for key_name, config in pk_uq_keys_mapping.items():
             key_columns = config.get("columns")
```

### Comparing `syngen-0.0.99/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.0/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.0/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/ml/worker/worker.py` & `syngen-0.1.0/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen/train.py` & `syngen-0.1.0/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.99/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.0/src/syngen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.99
+Version: 0.1.0
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -87,15 +87,15 @@
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
-- <i>print_report</i> - whether to generate plots of accuracy report and sample report
+- <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
 - <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
@@ -129,15 +129,15 @@
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
-- <i>print_report</i> – whether to generate plots of accuracy report, sample report
+- <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
 - <i>metadata_path</i> – a path to metadata file to generate linked tables
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.99 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.0 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -42,60 +42,62 @@
 as a reference - table_name â required parameter for training of single
 table, an arbitrary string to name the directories - epochs â a number of
 training epochs. Since the early stopping mechanism is implemented the bigger
 value of epochs is the better - row_limit â a number of rows to train over. A
 number less than the original table length will randomly subset the specified
 number of rows - drop_null â whether to drop rows with at least one missing
 value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate plots of accuracy report
-and sample report - metadata_path â a path to the metadata file containing
-the metadata for linked tables - column_types - might include the section
-categorical which contains the listed columns defined as categorical by a user
-Requirements for parameters of training process: * source - data type - string
-* table_name - data type - string * epochs - data type - integer, must be equal
-to or more than 1, default value is 10 * row_limit - data type - integer *
-drop_null - data type - boolean, default value - False * batch_size - data type
-- integer, must be equal to or more than 1, default value - 32 * print_report -
-data type - boolean, default value is False * metadata_path - data type -
-string * column_types - data type - dictionary with the key categorical - the
-list of columns (data type - string) ### Inference (generation) You can
-customize the inference processes by calling for one table: ```bash infer --
-size INT \ --table_name STR \ --run_parallel BOOL \ --batch_size INT \ --
-random_seed INT \ --print_report BOOL ``` For linked tables you can simply
-call: ```bash infer --metadata_path PATH_TO_METADATA ``` The parameters which
-you can set up for generation process: - size - the desired number of rows to
-generate - table_name â required parameter for inference of single table, the
-name of the table, same as in training - run_parallel â whether to use
-multiprocessing (feasible for tables > 5000 rows) - batch_size â if
-specified, the generation is split into batches. This can save the RAM -
+can save the RAM - print_report - whether to generate accuracy and sampling
+reports. Please note that the sampling report is generated only if the
+`row_limit` parameter is set. - metadata_path â a path to the metadata file
+containing the metadata for linked tables - column_types - might include the
+section categorical which contains the listed columns defined as categorical by
+a user Requirements for parameters of training process: * source - data type -
+string * table_name - data type - string * epochs - data type - integer, must
+be equal to or more than 1, default value is 10 * row_limit - data type -
+integer * drop_null - data type - boolean, default value - False * batch_size -
+data type - integer, must be equal to or more than 1, default value - 32 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string * column_types - data type - dictionary with the key
+categorical - the list of columns (data type - string) ### Inference
+(generation) You can customize the inference processes by calling for one
+table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
+batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
+you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
+parameters which you can set up for generation process: - size - the desired
+number of rows to generate - table_name â required parameter for inference of
+single table, the name of the table, same as in training - run_parallel â
+whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
+â if specified, the generation is split into batches. This can save the RAM -
 random_seed â if specified, generates a reproducible result - print_report
-â whether to generate plots of accuracy report, sample report - metadata_path
-â a path to metadata file to generate linked tables Requirements for
-parameters of generation process: * size - data type - integer, must be equal
-to or more than 1, default value is 100 * table_name - data type - string *
-run_parallel - data type - boolean, default value is False * batch_size - data
-type - integer, must be equal to or more than 1 * random_seed - data type -
-integer, must be equal to or more than 0 * print_report - data type - boolean,
-default value is False * metadata_path - data type - string The metadata can
-contain any of the arguments above for each table. If so, the duplicated
-arguments from the CLI will be ignored. ### Linked tables generation To
-generate linked tables, you should provide metadata in yaml format. It is used
-to handle complex relations for any number of tables. You can also specify
-additional parameters needed for training and inference in the metadata file
-and in this case, they will be ignored in the CLI call. The yaml metadata file
-should match the following template: CUSTOMER: # Table name source: "./files/
-customer.csv" # Supported formats include local files in CSV, Avro formats
-train_settings: # Settings for training process epochs: 10 # Number of epochs
-if different from the default in the command line options drop_null: False #
-Drop rows with NULL values row_limit: None # Number of rows to train over. A
-number less than the original table length will randomly subset the specified
-rows number batch_size: 32 # If specified, the training is split into batches.
-This can save the RAM print_report: False # Turn on or turn off generation of
-the report column_types: categorical: # Force listed columns to have
-categorical type (use dictionary of values) - gender - marital_status
+â whether to generate accuracy and sampling reports. Please note that the
+sampling report is generated only if the row_limit parameter is set. -
+metadata_path â a path to metadata file to generate linked tables
+Requirements for parameters of generation process: * size - data type -
+integer, must be equal to or more than 1, default value is 100 * table_name -
+data type - string * run_parallel - data type - boolean, default value is False
+* batch_size - data type - integer, must be equal to or more than 1 *
+random_seed - data type - integer, must be equal to or more than 0 *
+print_report - data type - boolean, default value is False * metadata_path -
+data type - string The metadata can contain any of the arguments above for each
+table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
+tables generation To generate linked tables, you should provide metadata in
+yaml format. It is used to handle complex relations for any number of tables.
+You can also specify additional parameters needed for training and inference in
+the metadata file and in this case, they will be ignored in the CLI call. The
+yaml metadata file should match the following template: CUSTOMER: # Table name
+source: "./files/customer.csv" # Supported formats include local files in CSV,
+Avro formats train_settings: # Settings for training process epochs: 10 #
+Number of epochs if different from the default in the command line options
+drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
+to train over. A number less than the original table length will randomly
+subset the specified rows number batch_size: 32 # If specified, the training is
+split into batches. This can save the RAM print_report: False # Turn on or turn
+off generation of the report column_types: categorical: # Force listed columns
+to have categorical type (use dictionary of values) - gender - marital_status
 infer_settings: # Settings for infer process size: 100 # Size for generated
 data run_parallel: False # Turn on or turn off parallel training process
 print_report: False # Turn on or turn off generation of the report batch_size:
 None # If specified, the generation is split into batches. This can save the
 RAM random_seed: None # If specified, generates a reproducible result keys:
 PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
 type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
```

### Comparing `syngen-0.0.99/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.0/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

