# Comparing `tmp/vivarium_public_health-0.9.8.tar.gz` & `tmp/vivarium_public_health-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vivarium_public_health-0.9.8.tar", last modified: Tue Mar 19 22:25:02 2019, max compression
+gzip compressed data, was "dist/vivarium_public_health-0.9.9.tar", last modified: Thu Mar 28 22:20:21 2019, max compression
```

## Comparing `vivarium_public_health-0.9.8.tar` & `vivarium_public_health-0.9.9.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)    35146 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/LICENSE.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      646 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/requirements-doc.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/util.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/testing.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment/healthcare_access.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      122 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment/mass_treatment_campaign.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       95 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment/base_treatment.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment/schedule.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/disease.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/metrics/disability.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       93 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/metrics/sample_history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       78 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/metrics/inspector.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/dataset_manager.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/risks.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/treatment.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population/add_new_birth_cohort.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population/mortality.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population/base_population.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population/data_transformations.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/metrics.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/risks/base_risk.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/risks/effect.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/risks/distributions.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/population.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/testing/
--rw-rw-r--   0 travis    (2000) travis    (2000)       90 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/testing/mock_artifact.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/testing/utils.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/docs/source/api_reference/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/disease/model.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/disease/transition.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/api_reference/disease/state.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5936 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/docs/source/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2827 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/treatment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9170 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/treatment/test_base_treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/treatment/test_schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/treatment/test_healthcare_access_module.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7165 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/metrics/test_disability.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21799 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/metrics/test_utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7376 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/population/test_data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5502 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/population/test_add_new_birth_cohort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/population/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11808 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/population/test_base_population.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/test_data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2205 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/test_base_risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6287 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/test_distributions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7529 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20366 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/risks/test_effect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      987 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/dataset_manager/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15064 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/dataset_manager/test_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   172261 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/dataset_manager/artifact.hdf
--rw-rw-r--   0 travis    (2000) travis    (2000)     8586 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/dataset_manager/test_hdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/dataset_manager/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/dataset_manager/test_dataset_manager.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/tests/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18145 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/disease/test_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5544 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/disease/test_special_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/disease/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/tests/test_utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4378 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/CHANGELOG.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      283 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3267 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/CODE_OF_CONDUCT.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/
--rw-rw-r--   0 travis    (2000) travis    (2000)      521 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/__about__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8062 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/healthcare_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/therapeutic_inertia.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4533 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4715 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/mass_treatment_campaign.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6017 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/base_treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/magic_wand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1289 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/utilities.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/mortality.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/utilities.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3589 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/sample_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2616 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/treatment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4085 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/disability.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/inspector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/
--rw-rw-r--   0 travis    (2000) travis    (2000)    14341 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/base_population.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3167 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/mortality.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19628 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7986 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/population/add_new_birth_cohorts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/interactive.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17837 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/data_transformations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/base_risk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      103 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/effect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5883 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/risks/distributions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/magic_wand_components.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10471 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3924 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/intervention.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14284 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/delay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2090 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/population.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13473 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/observer.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6919 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/hdf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8160 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/dataset_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      331 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9955 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/artifact.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/testing/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3813 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/testing/mock_artifact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/testing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      939 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/testing/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17569 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8247 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8114 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/special_disease.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8807 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3318 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/src/vivarium_public_health/disease/transition.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2019-03-19 22:25:02.000000 vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2019-03-19 22:17:00.000000 vivarium_public_health-0.9.8/CONTRIBUTING.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35146 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/LICENSE.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      646 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/requirements-doc.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      195 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      290 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       55 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/util.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/healthcare_access.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      122 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/mass_treatment_campaign.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       95 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/base_treatment.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       77 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment/schedule.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      126 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/disability.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       93 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/sample_history.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       78 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics/inspector.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/dataset_manager.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      192 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/treatment.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/add_new_birth_cohort.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/mortality.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/base_population.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      114 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population/data_transformations.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/metrics.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/base_risk.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/effect.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       88 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/risks/distributions.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      200 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/population.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       90 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/mock_artifact.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/testing/utils.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/model.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       81 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/transition.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/api_reference/disease/state.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5936 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/docs/source/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2827 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/treatment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9170 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_base_treatment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/treatment/test_healthcare_access_module.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7165 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/test_disability.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21799 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/metrics/test_utilities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/population/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7376 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_data_transformations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5502 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_add_new_birth_cohort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11808 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/population/test_base_population.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/risks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_data_transformations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2205 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_base_risk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6287 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_distributions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7529 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20366 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/risks/test_effect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      987 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/dataset_manager/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15064 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   172261 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/artifact.hdf
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8585 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_hdf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/dataset_manager/test_dataset_manager.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/tests/disease/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18145 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/test_disease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5544 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/test_special_disease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/disease/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1212 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/tests/test_utilities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4549 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CHANGELOG.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      283 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3267 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CODE_OF_CONDUCT.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      521 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/__about__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8062 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/healthcare_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1573 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/therapeutic_inertia.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4533 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4715 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/mass_treatment_campaign.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6017 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/base_treatment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1190 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/magic_wand.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1289 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/utilities.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3319 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/mortality.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3242 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/utilities.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3589 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/risk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      271 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2239 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/sample_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2616 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/treatment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4085 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disability.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      575 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/inspector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      313 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14341 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/base_population.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3167 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/mortality.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19770 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/data_transformations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7986 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/population/add_new_birth_cohorts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2091 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/interactive.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17827 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/data_transformations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4017 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/base_risk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      103 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2963 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/effect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5883 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/risks/distributions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/magic_wand_components.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10471 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/disease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3924 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/intervention.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14284 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/delay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2090 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/population.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13473 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/observer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6923 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/hdf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8160 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/dataset_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      331 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9955 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/artifact.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3813 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/mock_artifact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      939 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/testing/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17569 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/state.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      432 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8247 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8114 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/special_disease.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8807 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3318 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/src/vivarium_public_health/disease/transition.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       23 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2862 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5204 2019-03-28 22:20:21.000000 vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      844 2019-03-28 22:11:55.000000 vivarium_public_health-0.9.9/CONTRIBUTING.rst
```

### Comparing `vivarium_public_health-0.9.8/LICENSE.txt` & `vivarium_public_health-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/docs/Makefile` & `vivarium_public_health-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/docs/source/conf.py` & `vivarium_public_health-0.9.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/README.rst` & `vivarium_public_health-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/setup.py` & `vivarium_public_health-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/AUTHORS.rst` & `vivarium_public_health-0.9.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/treatment/test_base_treatment.py` & `vivarium_public_health-0.9.9/tests/treatment/test_base_treatment.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/treatment/test_schedule.py` & `vivarium_public_health-0.9.9/tests/treatment/test_schedule.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/treatment/test_healthcare_access_module.py` & `vivarium_public_health-0.9.9/tests/treatment/test_healthcare_access_module.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/metrics/test_disability.py` & `vivarium_public_health-0.9.9/tests/metrics/test_disability.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/metrics/test_utilities.py` & `vivarium_public_health-0.9.9/tests/metrics/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/population/test_data_transformations.py` & `vivarium_public_health-0.9.9/tests/population/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/population/test_add_new_birth_cohort.py` & `vivarium_public_health-0.9.9/tests/population/test_add_new_birth_cohort.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/population/test_base_population.py` & `vivarium_public_health-0.9.9/tests/population/test_base_population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/risks/test_data_transformations.py` & `vivarium_public_health-0.9.9/tests/risks/test_data_transformations.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/risks/test_base_risk.py` & `vivarium_public_health-0.9.9/tests/risks/test_base_risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/risks/test_distributions.py` & `vivarium_public_health-0.9.9/tests/risks/test_distributions.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/risks/conftest.py` & `vivarium_public_health-0.9.9/tests/risks/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/risks/test_effect.py` & `vivarium_public_health-0.9.9/tests/risks/test_effect.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/conftest.py` & `vivarium_public_health-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/dataset_manager/test_artifact.py` & `vivarium_public_health-0.9.9/tests/dataset_manager/test_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/dataset_manager/artifact.hdf` & `vivarium_public_health-0.9.9/tests/dataset_manager/artifact.hdf`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/dataset_manager/test_hdf.py` & `vivarium_public_health-0.9.9/tests/dataset_manager/test_hdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 from vivarium_public_health.dataset_manager import EntityKey, hdf
 
 
 @pytest.fixture
 def hdf_file_path(tmpdir):
     """This file contains the following:
-
     Object Tree:
         / (RootGroup) ''
         /cause (Group) ''
         /population (Group) ''
         /population/age_bins (Group) ''
         /population/age_bins/table (Table(23,), shuffle, zlib(9)) ''
         /population/structure (Group) ''
```

### Comparing `vivarium_public_health-0.9.8/tests/dataset_manager/test_dataset_manager.py` & `vivarium_public_health-0.9.9/tests/dataset_manager/test_dataset_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/disease/test_disease.py` & `vivarium_public_health-0.9.9/tests/disease/test_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/disease/test_special_disease.py` & `vivarium_public_health-0.9.9/tests/disease/test_special_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/tests/test_utilities.py` & `vivarium_public_health-0.9.9/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/CHANGELOG.rst` & `vivarium_public_health-0.9.9/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-**0.9.8 - 03/19/10**
+**0.9.9 - 03/28/19**
+
+ - Bugfix in data free risk components when using a covariate for coverage.
+ - Bugfix for simulations that start in a future year with extrapolate.
+
+**0.9.8 - 03/19/19**
 
  - Bugfix in mortality observer.
 
 **0.9.7 - 03/17/19**
 
  - Bugfixes in disease and treatment observers.
  - Remove unnecessary output metrics.
```

### Comparing `vivarium_public_health-0.9.8/PKG-INFO` & `vivarium_public_health-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium_public_health
-Version: 0.9.8
+Version: 0.9.9
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
 Author: The vivarium_public_health developers
 Author-email: vivarium.dev@gmail.com
 License: GNU GPLv3
 Description: Vivarium Public Health
         ======================
```

### Comparing `vivarium_public_health-0.9.8/CODE_OF_CONDUCT.rst` & `vivarium_public_health-0.9.9/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/__about__.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/__about__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,14 @@
     "__email__", "__license__", "__copyright__",
 ]
 
 __title__ = "vivarium_public_health"
 __summary__ = "Components for modelling diseases, risks, and interventions with ``vivarium``"
 __uri__ = "https://github.com/ihmeuw/vivarium_public_health"
 
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 __author__ = "The vivarium_public_health developers"
 __email__ = "vivarium.dev@gmail.com"
 
 __license__ = "GNU GPLv3"
 __copyright__ = f"Copyright 2016-2018 {__author__}"
```

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/healthcare_access.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/healthcare_access.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/therapeutic_inertia.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/therapeutic_inertia.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/schedule.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/schedule.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/mass_treatment_campaign.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/mass_treatment_campaign.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/base_treatment.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/base_treatment.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/treatment/magic_wand.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/treatment/magic_wand.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/utilities.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/mortality.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/disease.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/utilities.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/risk.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/sample_history.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/sample_history.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/treatment.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/treatment.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/disability.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/disability.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/metrics/inspector.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/metrics/inspector.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/population/base_population.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/population/base_population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/population/mortality.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/population/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/population/data_transformations.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/population/data_transformations.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,19 +371,23 @@
 
     initial_population_size = builder.configuration.population.population_size
     population_data = population_data.groupby(['year_start'])['value'].sum()
     birth_data = (birth_data[birth_data.parameter == 'mean_value']
                   .drop('parameter', 'columns')
                   .groupby(['year_start'])['value'].sum())
 
+    start_year = builder.configuration.time.start.year
+    if builder.configuration.interpolation.extrapolate and start_year > birth_data.index.max():
+        start_year = birth_data.index.max()
+
     if not builder.configuration.fertility.time_dependent_live_births:
-        birth_data = birth_data.at[builder.configuration.time.start.year]
+        birth_data = birth_data.at[start_year]
 
     if not builder.configuration.fertility.time_dependent_population_fraction:
-        population_data = population_data.at[builder.configuration.time.start.year]
+        population_data = population_data.at[start_year]
 
     live_birth_rate = initial_population_size / population_data * birth_data
 
     if isinstance(live_birth_rate, (int, float)):
         live_birth_rate = pd.Series(live_birth_rate, index=pd.RangeIndex(builder.configuration.time.start.year,
                                                                          builder.configuration.time.end.year + 1,
                                                                          name='year'))
```

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/population/add_new_birth_cohorts.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/population/add_new_birth_cohorts.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/interactive.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/interactive.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/risks/data_transformations.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/data_transformations.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     risk_config = builder.configuration[risk.name]
     exposure_source = risk_config['exposure']
 
     if exposure_source == 'data':
         exposure_data = builder.data.load(f'{risk}.exposure')
     else:
         if isinstance(exposure_source, str):  # Build from covariate
-            cat1 = builder.data.load(f'covariate.{exposure_source}.estimate')
+            cat1 = builder.data.load(f'{exposure_source}.estimate')
             # TODO: Generate a draw.
             cat1 = cat1[cat1['parameter'] == 'mean_value']
             cat1['parameter'] = 'cat1'
         else:  # We have a numerical value
             cat1 = builder.data.load('population.demographic_dimensions')
             cat1['parameter'] = 'cat1'
             cat1['value'] = float(exposure_source)
```

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/risks/base_risk.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/base_risk.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/risks/effect.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/effect.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/risks/distributions.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/risks/distributions.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/magic_wand_components.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/magic_wand_components.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/disease.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/intervention.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/intervention.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/delay.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/delay.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/population.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/population.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/mslt/observer.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/mslt/observer.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/hdf.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/hdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,27 +13,26 @@
     from vivarium_public_health.dataset_manager import EntityKey
 
 DEFAULT_COLUMNS = {"location", "draw"}
 
 
 def touch(path: str):
     """Creates an hdf file or wipes an existing file if necessary.
-
     If the given path is proper to create a hdf file, it creates a new hdf file.
 
     Parameters
     ----------
     path :
         The string path to the hdf file.
 
     Raises
     ------
     ValueError
-        If the non-proper path is given to create a hdf file."""
-
+        If the non-proper path is given to create a hdf file.
+    """
     path = Path(path)
     if not path.suffix == '.hdf':
         raise ValueError(f'You provided path: {str(path)} not valid for creating hdf file.')
 
     with tables.open_file(str(path), mode='w'):
         pass
 
@@ -91,14 +90,15 @@
 def remove(path: str, entity_key: 'EntityKey'):
     """Removes a piece of data from an hdf file.
 
     Parameters
     ----------
     path :
         The path to the hdf file to remove the data from.
+
     entity_key :
         A representation of the internal hdf path where the data is located.
     """
     with tables.open_file(path, mode='a') as file:
         file.remove_node(entity_key.path, recursive=True)
```

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/dataset_manager.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/dataset_manager/artifact.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/dataset_manager/artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/testing/mock_artifact.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/testing/mock_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/testing/utils.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/testing/utils.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/disease/state.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/state.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/disease/models.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/models.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/disease/special_disease.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/special_disease.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/disease/model.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/model.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health/disease/transition.py` & `vivarium_public_health-0.9.9/src/vivarium_public_health/disease/transition.py`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/PKG-INFO` & `vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-public-health
-Version: 0.9.8
+Version: 0.9.9
 Summary: Components for modelling diseases, risks, and interventions with ``vivarium``
 Home-page: https://github.com/ihmeuw/vivarium_public_health
 Author: The vivarium_public_health developers
 Author-email: vivarium.dev@gmail.com
 License: GNU GPLv3
 Description: Vivarium Public Health
         ======================
```

### Comparing `vivarium_public_health-0.9.8/src/vivarium_public_health.egg-info/SOURCES.txt` & `vivarium_public_health-0.9.9/src/vivarium_public_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium_public_health-0.9.8/CONTRIBUTING.rst` & `vivarium_public_health-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

