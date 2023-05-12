# Comparing `tmp/validmind-1.8.1.tar.gz` & `tmp/validmind-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validmind-1.8.1.tar", max compression
+gzip compressed data, was "validmind-1.9.0.tar", max compression
```

## Comparing `validmind-1.8.1.tar` & `validmind-1.9.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1295 2023-05-12 04:30:18.299285 validmind-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/__init__.py
--rw-r--r--   0        0        0    11353 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/api_client.py
--rw-r--r--   0        0        0     9190 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/client.py
--rw-r--r--   0        0        0      590 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/data_validation/__init__.py
--rw-r--r--   0        0        0    35109 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/data_validation/metrics.py
--rw-r--r--   0        0        0    24265 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/data_validation/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/datasets/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/datasets/classification/__init__.py
--rw-r--r--   0        0        0     1330 2023-05-12 04:30:18.299285 validmind-1.8.1/validmind/datasets/classification/customer_churn.py
--rw-r--r--   0        0        0   545707 2023-05-12 04:30:18.303285 validmind-1.8.1/validmind/datasets/classification/datasets/bank_customer_churn.csv
--rw-r--r--   0        0        0  2897191 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/classification/datasets/taiwan_credit.csv
--rw-r--r--   0        0        0     1280 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/classification/taiwan_credit.py
--rw-r--r--   0        0        0     1645 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/__init__.py
--rw-r--r--   0        0        0   107835 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates.csv
--rw-r--r--   0        0        0     2634 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
--rw-r--r--   0        0        0     2634 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
--rw-r--r--   0        0        0     2736 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
--rw-r--r--   0        0        0     3355 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
--rw-r--r--   0        0        0     3866 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
--rw-r--r--   0        0        0    11624 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
--rw-r--r--   0        0        0     4378 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/fred.py
--rw-r--r--   0        0        0     2346 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/lending_club.py
--rw-r--r--   0        0        0    40067 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
--rw-r--r--   0        0        0    48314 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
--rw-r--r--   0        0        0    40063 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
--rw-r--r--   0        0        0    48292 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
--rw-r--r--   0        0        0    60343 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
--rw-r--r--   0        0        0    10529 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_utils.py
--rw-r--r--   0        0        0     1290 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/__init__.py
--rw-r--r--   0        0        0     6749 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/sklearn/__init__.py
--rw-r--r--   0        0        0    13446 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/sklearn/metrics.py
--rw-r--r--   0        0        0    31402 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/sklearn/threshold_tests.py
--rw-r--r--   0        0        0        0 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/statsmodels/__init__.py
--rw-r--r--   0        0        0    28009 2023-05-12 04:30:18.323284 validmind-1.8.1/validmind/model_validation/statsmodels/metrics.py
--rw-r--r--   0        0        0     1317 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/model_validation/statsmodels/threshold_tests.py
--rw-r--r--   0        0        0     1657 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/model_validation/utils.py
--rw-r--r--   0        0        0     5251 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_plans/__init__.py
--rw-r--r--   0        0        0     1985 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_plans/binary_classifier.py
--rw-r--r--   0        0        0     2836 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_plans/statsmodels_timeseries.py
--rw-r--r--   0        0        0     1822 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_plans/tabular_datasets.py
--rw-r--r--   0        0        0     6821 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_plans/time_series.py
--rw-r--r--   0        0        0     1825 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_suites/__init__.py
--rw-r--r--   0        0        0     1000 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/test_suites/test_suites.py
--rw-r--r--   0        0        0     6465 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/utils.py
--rw-r--r--   0        0        0     1116 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/__init__.py
--rw-r--r--   0        0        0    10425 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/dataset.py
--rw-r--r--   0        0        0     8287 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/dataset_utils.py
--rw-r--r--   0        0        0      592 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/figure.py
--rw-r--r--   0        0        0     3674 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/metric.py
--rw-r--r--   0        0        0     1757 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/metric_result.py
--rw-r--r--   0        0        0     6530 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/model.py
--rw-r--r--   0        0        0     3721 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/plot_utils.py
--rw-r--r--   0        0        0     1518 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/result_summary.py
--rw-r--r--   0        0        0     2501 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/test_context.py
--rw-r--r--   0        0        0     9846 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/test_plan.py
--rw-r--r--   0        0        0    19074 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/test_plan_result.py
--rw-r--r--   0        0        0     1698 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/test_result.py
--rw-r--r--   0        0        0     1811 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/test_suite.py
--rw-r--r--   0        0        0     3621 2023-05-12 04:30:18.327284 validmind-1.8.1/validmind/vm_models/threshold_test.py
--rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1295 2023-05-12 07:24:11.424716 validmind-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1443 2023-05-12 07:24:11.424716 validmind-1.9.0/validmind/__init__.py
+-rw-r--r--   0        0        0    11353 2023-05-12 07:24:11.424716 validmind-1.9.0/validmind/api_client.py
+-rw-r--r--   0        0        0     9190 2023-05-12 07:24:11.424716 validmind-1.9.0/validmind/client.py
+-rw-r--r--   0        0        0      590 2023-05-12 07:24:11.424716 validmind-1.9.0/validmind/data_validation/__init__.py
+-rw-r--r--   0        0        0    35109 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/data_validation/metrics.py
+-rw-r--r--   0        0        0    24265 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/data_validation/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/datasets/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/datasets/classification/__init__.py
+-rw-r--r--   0        0        0     1330 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/datasets/classification/customer_churn.py
+-rw-r--r--   0        0        0   545707 2023-05-12 07:24:11.428716 validmind-1.9.0/validmind/datasets/classification/datasets/bank_customer_churn.csv
+-rw-r--r--   0        0        0  2897191 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/classification/datasets/taiwan_credit.csv
+-rw-r--r--   0        0        0     1280 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/classification/taiwan_credit.py
+-rw-r--r--   0        0        0     1645 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/__init__.py
+-rw-r--r--   0        0        0   107835 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates.csv
+-rw-r--r--   0        0        0     2634 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv
+-rw-r--r--   0        0        0     2634 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv
+-rw-r--r--   0        0        0     2736 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv
+-rw-r--r--   0        0        0     3355 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv
+-rw-r--r--   0        0        0     3866 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv
+-rw-r--r--   0        0        0    11624 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/datasets/lending_club_loan_rates.csv
+-rw-r--r--   0        0        0     4378 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/fred.py
+-rw-r--r--   0        0        0     2346 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/lending_club.py
+-rw-r--r--   0        0        0    40067 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl
+-rw-r--r--   0        0        0    48314 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl
+-rw-r--r--   0        0        0    40063 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl
+-rw-r--r--   0        0        0    48292 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl
+-rw-r--r--   0        0        0    60343 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl
+-rw-r--r--   0        0        0    10529 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_utils.py
+-rw-r--r--   0        0        0     1290 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/__init__.py
+-rw-r--r--   0        0        0     6749 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/sklearn/__init__.py
+-rw-r--r--   0        0        0    13446 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/sklearn/metrics.py
+-rw-r--r--   0        0        0    31402 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/sklearn/threshold_tests.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/statsmodels/__init__.py
+-rw-r--r--   0        0        0    28009 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/statsmodels/metrics.py
+-rw-r--r--   0        0        0     1317 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/statsmodels/threshold_tests.py
+-rw-r--r--   0        0        0     1657 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/model_validation/utils.py
+-rw-r--r--   0        0        0     5251 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_plans/__init__.py
+-rw-r--r--   0        0        0     1985 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_plans/binary_classifier.py
+-rw-r--r--   0        0        0     2836 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_plans/statsmodels_timeseries.py
+-rw-r--r--   0        0        0     1822 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_plans/tabular_datasets.py
+-rw-r--r--   0        0        0     6821 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_plans/time_series.py
+-rw-r--r--   0        0        0     1825 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_suites/__init__.py
+-rw-r--r--   0        0        0     1119 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/test_suites/test_suites.py
+-rw-r--r--   0        0        0     6465 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/utils.py
+-rw-r--r--   0        0        0     1116 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/__init__.py
+-rw-r--r--   0        0        0    10425 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/dataset.py
+-rw-r--r--   0        0        0     8287 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/dataset_utils.py
+-rw-r--r--   0        0        0      592 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/figure.py
+-rw-r--r--   0        0        0     3674 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/metric.py
+-rw-r--r--   0        0        0     1757 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/metric_result.py
+-rw-r--r--   0        0        0     6530 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/model.py
+-rw-r--r--   0        0        0     3721 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/plot_utils.py
+-rw-r--r--   0        0        0     1518 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/result_summary.py
+-rw-r--r--   0        0        0     2501 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/test_context.py
+-rw-r--r--   0        0        0    11386 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/test_plan.py
+-rw-r--r--   0        0        0    19100 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/test_plan_result.py
+-rw-r--r--   0        0        0     1698 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/test_result.py
+-rw-r--r--   0        0        0     4958 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/test_suite.py
+-rw-r--r--   0        0        0     3621 2023-05-12 07:24:11.448716 validmind-1.9.0/validmind/vm_models/threshold_test.py
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 validmind-1.9.0/PKG-INFO
```

### Comparing `validmind-1.8.1/pyproject.toml` & `validmind-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # include = [
 #   "validmind/**/*.c",
 #   "validmind/**/*.pyx",
 #   "validmind/**/*.pyd",
 #   "validmind/**/*.so",
 # ]
 name = "validmind"
-version = "1.8.1"
+version = "1.9.0"
 
 [tool.poetry.dependencies]
 arch = "^5.4.0"
 click = "^8.0.4"
 dython = "^0.7.1"
 ipython = "^8.11.0"
 myst-parser = "^1.0.0"
```

### Comparing `validmind-1.8.1/validmind/__init__.py` & `validmind-1.9.0/validmind/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/api_client.py` & `validmind-1.9.0/validmind/api_client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/client.py` & `validmind-1.9.0/validmind/client.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/data_validation/__init__.py` & `validmind-1.9.0/validmind/data_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/data_validation/metrics.py` & `validmind-1.9.0/validmind/data_validation/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/data_validation/threshold_tests.py` & `validmind-1.9.0/validmind/data_validation/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/classification/__init__.py` & `validmind-1.9.0/validmind/datasets/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/classification/customer_churn.py` & `validmind-1.9.0/validmind/datasets/classification/customer_churn.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/classification/datasets/bank_customer_churn.csv` & `validmind-1.9.0/validmind/datasets/classification/datasets/bank_customer_churn.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/classification/datasets/taiwan_credit.csv` & `validmind-1.9.0/validmind/datasets/classification/datasets/taiwan_credit.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/classification/taiwan_credit.py` & `validmind-1.9.0/validmind/datasets/classification/taiwan_credit.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/__init__.py` & `validmind-1.9.0/validmind/datasets/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_1.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_2.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_3.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_4.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/fred_loan_rates_test_5.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/datasets/lending_club_loan_rates.csv` & `validmind-1.9.0/validmind/datasets/regression/datasets/lending_club_loan_rates.csv`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/fred.py` & `validmind-1.9.0/validmind/datasets/regression/fred.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/lending_club.py` & `validmind-1.9.0/validmind/datasets/regression/lending_club.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl` & `validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_1.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl` & `validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_2.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl` & `validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_3.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl` & `validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_4.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl` & `validmind-1.9.0/validmind/datasets/regression/models/fred_loan_rates_model_5.pkl`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_utils.py` & `validmind-1.9.0/validmind/model_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/__init__.py` & `validmind-1.9.0/validmind/model_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/model_metadata.py` & `validmind-1.9.0/validmind/model_validation/model_metadata.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/sklearn/metrics.py` & `validmind-1.9.0/validmind/model_validation/sklearn/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/sklearn/threshold_tests.py` & `validmind-1.9.0/validmind/model_validation/sklearn/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/statsmodels/metrics.py` & `validmind-1.9.0/validmind/model_validation/statsmodels/metrics.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/statsmodels/threshold_tests.py` & `validmind-1.9.0/validmind/model_validation/statsmodels/threshold_tests.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/model_validation/utils.py` & `validmind-1.9.0/validmind/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_plans/__init__.py` & `validmind-1.9.0/validmind/test_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_plans/binary_classifier.py` & `validmind-1.9.0/validmind/test_plans/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_plans/statsmodels_timeseries.py` & `validmind-1.9.0/validmind/test_plans/statsmodels_timeseries.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_plans/tabular_datasets.py` & `validmind-1.9.0/validmind/test_plans/tabular_datasets.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_plans/time_series.py` & `validmind-1.9.0/validmind/test_plans/time_series.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_suites/__init__.py` & `validmind-1.9.0/validmind/test_suites/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/test_suites/test_suites.py` & `validmind-1.9.0/validmind/test_suites/test_suites.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,41 +6,44 @@
 
 
 class TabularDataset(TestSuite):
     """
     Test suite for tabular datasets.
     """
 
+    name = "tabular_dataset"
     required_context = ["dataset"]
 
     test_plans = [
         "tabular_dataset_description",
         "tabular_data_quality",
     ]
 
 
 class BinaryClassifierModelValidation(TestSuite):
     """
     Test suite for binary classification models.
     """
 
+    name = "binary_classifier_model_validation"
     required_context = ["model"]
 
     test_plans = [
         "binary_classifier_metrics",
         "binary_classifier_validation",
         "binary_classifier_model_diagnosis",
     ]
 
 
 class BinaryClassifierFullSuite(TestSuite):
     """
     Full test suite for binary classification models.
     """
 
+    name = "binary_classifier_full_suite"
     required_context = ["dataset", "model"]
 
     test_plans = [
         "tabular_dataset_description",
         "tabular_data_quality",
         "binary_classifier_metrics",
         "binary_classifier_validation",
```

### Comparing `validmind-1.8.1/validmind/utils.py` & `validmind-1.9.0/validmind/utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/__init__.py` & `validmind-1.9.0/validmind/vm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/dataset.py` & `validmind-1.9.0/validmind/vm_models/dataset.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/dataset_utils.py` & `validmind-1.9.0/validmind/vm_models/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/figure.py` & `validmind-1.9.0/validmind/vm_models/figure.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/metric.py` & `validmind-1.9.0/validmind/vm_models/metric.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/metric_result.py` & `validmind-1.9.0/validmind/vm_models/metric_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/model.py` & `validmind-1.9.0/validmind/vm_models/model.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/plot_utils.py` & `validmind-1.9.0/validmind/vm_models/plot_utils.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/result_summary.py` & `validmind-1.9.0/validmind/vm_models/result_summary.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/test_context.py` & `validmind-1.9.0/validmind/vm_models/test_context.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/test_plan.py` & `validmind-1.9.0/validmind/vm_models/test_plan.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """
 TestPlan class
 """
-import os
-
 from dataclasses import dataclass
 from typing import ClassVar, List
 
-from IPython.display import display, HTML
-from tqdm import tqdm
+import ipywidgets as widgets
+
+from IPython.display import display
 
 from ..utils import is_notebook
 from .dataset import Dataset
 from .model import Model
 from .test_context import TestContext
 from .test_plan_result import TestPlanResult
 from ..utils import clean_docstring
 
-VM_SUMMARIZE_TEST_PLANS = os.environ.get("VM_SUMMARIZE_TEST_PLANS", "True")
-
 
 @dataclass
 class TestPlan:
     """
     Base class for test plans. Test plans are used to define any
     arbitrary grouping of tests that will be run on a dataset or model.
     """
@@ -44,16 +41,21 @@
 
     # Model and corresponding datasets for model related tests
     model: Model = None
 
     # Multiple models for model comparison tests
     models: List[Model] = None
 
-    # tqdm progress bar
-    pbar: tqdm = None
+    # ipywidgets progress bar
+    pbar: widgets.IntProgress = None
+    pbar_description: widgets.Label = None
+    pbar_box: widgets.HBox = None
+
+    # Stores the HTML summary of the test plan
+    summary: str = None
 
     def __repr__(self):
         class_name = type(self).__name__
 
         if self.config is None:
             return f"{class_name}(test_context={self.test_context})"
 
@@ -114,174 +116,213 @@
         }
         """
         if self.config is None:
             return None
 
         return self.config.get(test_name, None)
 
-    def run(self, send=True):  # noqa C901 'TestPlan.run' is too complex
+    def _init_pbar(self, render_summary: bool = True, send: bool = True):
+        """
+        Initializes the progress bar elements
+        """
+        self.pbar = widgets.IntProgress(
+            value=0,
+            min=0,
+            max=len(self.tests) * 2 if send else len(self.results),  # tests and results
+            step=1,
+            bar_style="",
+            orientation="horizontal",
+        )
+        self.pbar_description = widgets.Label(value="Running test plan...")
+        # Display them in a horizontal box
+        self.pbar_box = widgets.HBox([self.pbar_description, self.pbar])
+
+        if render_summary:
+            display(self.pbar_box)
+
+    def run(  # noqa C901 'TestPlan.run' is too complex
+        self, render_summary: bool = True, send: bool = True
+    ):
         """
         Runs the test plan
+
+        Args:
+            render_summary: Defaults to True. Whether to render the summary of the test
+                plan. When it's False, this allows test suites to collect the results of
+                sub test plans and render them all at once with widgets
+            send: Whether to send the results to the backend
+
+        Returns:
+            None
         """
         self.results = []  # Empty the results cache on every run
 
         if self.test_context is None:
             self.test_context = TestContext(
                 dataset=self.dataset,
                 model=self.model,
                 models=self.models,
             )
 
         if self.pbar is None:
-            self.pbar = tqdm(
-                total=len(self.tests),
-                desc=f"Running test plan: '{self.name}'",
-                leave=False,
-            )
-        else:
-            # if already initiated (meaning we are in a sub test plan), reset it
-            self.pbar.reset(total=len(self.tests))
-            self.pbar.set_description(f"Running sub test plan: '{self.name}'")
+            self._init_pbar(render_summary=render_summary, send=send)
 
         for test in self.tests:
             # TODO: we need to unify key/name for any object
             if hasattr(test, "key"):
                 test_name = test.key
             elif hasattr(test, "name"):
                 test_name = test.name
 
             test_params = self.get_config_params_for_test(test_name)
             test_instance = test(self.test_context, params=test_params)
 
-            self.pbar.set_description(f"Running {test.test_type}: {test_instance.name}")
+            self.pbar_description.value = (
+                f"Running {test.test_type}: {test_instance.name}"
+            )
 
             result = test_instance.run()
 
             if result is None:
-                self.pbar.set_description("Test returned None, skipping...")
-                self.pbar.update(1)
+                self.pbar_description.value = "Test returned None, skipping..."
+                self.pbar.value += 1
                 continue
 
             if not isinstance(result, TestPlanResult):
                 raise ValueError(
                     f"'{test_instance.name}' must return an instance of TestPlanResult Base Class"
                 )
 
             self.results.append(result)
-            self.pbar.update(1)
-
-        # Set the progress bar to 100% if it's not already
-        self.pbar.update(self.pbar.total - self.pbar.n)
+            self.pbar.value += 1
 
         if send:
             self.log_results()
 
+        # TODO: remove
         for test_plan in self.test_plans:
             test_plan_instance = test_plan(
                 config=self.config,
                 test_context=self.test_context,
-                pbar=self.pbar,
+                # pbar=self.pbar,
             )
             test_plan_instance.run(send=send)
 
             # Build up the subtest plan instances so we can log them
             if self._test_plan_instances is None:
                 self._test_plan_instances = []
 
             self._test_plan_instances.append(test_plan_instance)
 
-        self.pbar.close()
-
-        if VM_SUMMARIZE_TEST_PLANS == "True":
-            self.summarize()
+        self.summarize(render_summary)
 
     def log_results(self):
         """Logs the results of the test plan to ValidMind
 
         This method will be called after the test plan has been run and all results have been
         collected. This method will log the results to ValidMind.
         """
-        self.pbar.reset(total=len(self.results))
-        self.pbar.set_description(
-            f"Sending results of test plan execution '{self.name}' to ValidMind..."
+        self.pbar_description.value = (
+            f"Sending results of test plan '{self.name}' to ValidMind..."
         )
 
         for result in self.results:
-            self.pbar.set_description(f"Logging result: {result}")
+            self.pbar_description.value = f"Logging result: {result.result_id}"
 
             try:
                 result.log()
             except Exception as e:
                 self.pbar.set_description(
                     f"Failed to log result: {result} for test plan result '{str(result)}'"
                 )
                 print(e)
                 raise e
 
-            self.pbar.update(1)
+            self.pbar.value += 1
 
-    def _results_title(self, html: str = "") -> str:
+    def _results_title(self) -> str:
         """
         Builds the title for the results of the test plan
         """
-        html += f"<h2>Results for <i>{self.title()}</i> Test Plan:</h2><hr>"
-
-        return html
+        return f"<h2>Results for <i>{self.title()}</i> Test Plan:</h2><hr>"
 
-    def _results_description(self, html: str = "") -> str:
+    def _results_description(self) -> str:
         """
         Builds the description for the results of the test plan. Subclasses
         should override this method to provide an appropriate description
         """
-        html += f'<div class="result">{clean_docstring(self.description())}</div>'
-        return html
+        return f'<div class="result">{clean_docstring(self.description())}</div>'
 
-    def _results_summary(self, html: str = "") -> str:
+    def _results_summary(self) -> str:
         """
         Builds a summary of the results for each of the tests in the test plan
         """
+        accordions = []
         for result in self.results:
             result_html = result._to_html()
             if result_html:
-                html += f'<div class="result">{result_html}</div>'
+                accordions.append(
+                    widgets.HTML(value=f'<div class="result">{result_html}</div>')
+                )
 
-        return html
+        return accordions
 
-    def summarize(self):
+    def summarize(self, render_summary: bool = True):
         """Summarizes the results of the test plan
 
         This method will be called after the test plan has been run and all results have been
         logged to ValidMind. It will summarize the results of the test plan by creating an
         html table with the results of each test. This html table will be displayed in an
         VS Code, Jupyter or other notebook environment.
         """
         if not is_notebook():
             return
 
         if len(self.results) == 0:
             return
 
-        html = ""
-        html = self._results_title(html)
-        html = self._results_description(html)
-        html = self._results_summary(html)
+        vbox_children = []
+
+        # Only show the title if we are rendering the summary here
+        if render_summary:
+            vbox_children.append(widgets.HTML(value=self._results_title()))
+
+        vbox_children.append(widgets.HTML(value=self._results_description()))
 
-        html += """
+        accordion_contents = self._results_summary()
+        accordion_widget = widgets.Accordion(children=accordion_contents)
+        for i, _ in enumerate(accordion_widget.children):
+            result_id = self.results[i].result_id
+            title = f'{result_id.title().replace("_", " ")} ({result_id})'
+            accordion_widget.set_title(i, title)
+
+        vbox_children.append(accordion_widget)
+
+        style_footer = widgets.HTML(
+            value="""
         <style>
             .result {
                 margin: 10px 0;
                 padding: 10px;
                 background-color: #f1f1f1;
                 border: 1px solid #ccc;
                 border-radius: 5px;
             }
         </style>
         """
+        )
+
+        # Don't duplicate the footer if we are not rendering the summary here
+        if render_summary:
+            vbox_children.append(style_footer)
+
+        self.summary = widgets.VBox(vbox_children)
 
-        display(HTML(html))
+        if render_summary:
+            display(self.summary)
 
     def _get_all_subtest_plan_results(self) -> List[TestPlanResult]:
         """
         Recursively gets all sub test plan results since a test plan
         can have sub test plans which can have sub test plans and so on.
         """
         results = []
```

### Comparing `validmind-1.8.1/validmind/vm_models/test_plan_result.py` & `validmind-1.9.0/validmind/vm_models/test_plan_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 
 @dataclass
 class TestPlanDatasetResult(TestPlanResult):
     """
     Result wrapper for datasets that run as part of a test plan
     """
 
+    result_id: str = None
     dataset: Dataset = None
 
     def __repr__(self) -> str:
         return f'TestPlanDatasetResult(result_id="{self.result_id}")'
 
     def _to_html(self):
         html = "<h4>Logged the following dataset to the ValidMind platform:</h4>"
```

### Comparing `validmind-1.8.1/validmind/vm_models/test_result.py` & `validmind-1.9.0/validmind/vm_models/test_result.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/validmind/vm_models/threshold_test.py` & `validmind-1.9.0/validmind/vm_models/threshold_test.py`

 * *Files identical despite different names*

### Comparing `validmind-1.8.1/PKG-INFO` & `validmind-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validmind
-Version: 1.8.1
+Version: 1.9.0
 Summary: ValidMind Developer Framework
 Author: Andres Rodriguez
 Author-email: andres@validmind.ai
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

