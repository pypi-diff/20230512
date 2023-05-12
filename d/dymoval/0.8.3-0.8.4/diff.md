# Comparing `tmp/dymoval-0.8.3.tar.gz` & `tmp/dymoval-0.8.4.tar.gz`

## Comparing `dymoval-0.8.3.tar` & `dymoval-0.8.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0   440916 2020-02-02 00:00:00.000000 dymoval-0.8.3/conda-lock.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 dymoval-0.8.3/coverage.svg
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 dymoval-0.8.3/environment.yml
--rw-r--r--   0        0        0    45390 2020-02-02 00:00:00.000000 dymoval-0.8.3/pip_freeze.txt
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/make.bat
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/api.rst
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/conf.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started.rst
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/index.rst
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/installation.rst
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/integration.rst
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/reference.rst
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/api_index/api.rst
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/Composition.svg
--rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/DymovalLogo.svg
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/DymovalLogo_Layer 2_Small.svg
--rw-r--r--   0        0        0    14905 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/DymovalNutshell.svg
--rw-r--r--   0        0        0   296183 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/ModelValidation.svg
--rw-r--r--   0        0        0   304653 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/figures/ModelValidationDymoval.svg
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/create_dataset.rst
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/doe.rst
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/model_validation.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/more_on_model_validation.rst
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/simulate_model.rst
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/tutorial.rst
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/getting_started_index/validation_session.rst
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/reference_index/dataset.rst
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dymoval-0.8.3/docs/source/reference_index/validation.rst
--rw-r--r--   0        0        0    65913 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/DCMotor.fmu
--rw-r--r--   0        0        0  1136010 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/DCMotor.svg
--rw-r--r--   0        0        0   963816 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/DCMotorLogs.h5
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/DCMotorModel.py
--rw-r--r--   0        0        0     6733 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/test_manual.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/test_plots_manual.py
--rw-r--r--   0        0        0  1022504 2020-02-02 00:00:00.000000 dymoval-0.8.3/scripts/tutorial.ipynb
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/dymoval/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/dymoval/config.py
--rw-r--r--   0        0        0   112814 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/dymoval/dataset.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/dymoval/utils.py
--rw-r--r--   0        0        0    32802 2020-02-02 00:00:00.000000 dymoval-0.8.3/src/dymoval/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/fixture_data.py
--rw-r--r--   0        0        0    54387 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/test_dataset.py
--rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/test_initializers.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/test_utils.py
--rw-r--r--   0        0        0    26477 2020-02-02 00:00:00.000000 dymoval-0.8.3/tests/test_validation.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dymoval-0.8.3/.gitignore
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 dymoval-0.8.3/LICENSE
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 dymoval-0.8.3/README.md
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dymoval-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 dymoval-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 dymoval-0.8.4/coverage.svg
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 dymoval-0.8.4/environment.yml
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 dymoval-0.8.4/environment_locked_py310.yml
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 dymoval-0.8.4/pip_freeze_py310.txt
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 dymoval-0.8.4/conda/meta.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/make.bat
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/api.rst
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/conf.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started.rst
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/index.rst
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/installation.rst
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/integration.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/reference.rst
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/api_index/api.rst
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/Composition.svg
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/DymovalLogo.svg
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/DymovalLogo_Layer 2_Small.svg
+-rw-r--r--   0        0        0    14905 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/DymovalNutshell.svg
+-rw-r--r--   0        0        0   296183 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/ModelValidation.svg
+-rw-r--r--   0        0        0   304653 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/figures/ModelValidationDymoval.svg
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/create_dataset.rst
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/doe.rst
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/model_validation.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/more_on_model_validation.rst
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/simulate_model.rst
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/tutorial.rst
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/getting_started_index/validation_session.rst
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/reference_index/dataset.rst
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 dymoval-0.8.4/docs/source/reference_index/validation.rst
+-rw-r--r--   0        0        0    65913 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/DCMotor.fmu
+-rw-r--r--   0        0        0  1136010 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/DCMotor.svg
+-rw-r--r--   0        0        0   963816 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/DCMotorLogs.h5
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/DCMotorModel.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/test_manual.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/test_plots_manual.py
+-rw-r--r--   0        0        0  1022504 2020-02-02 00:00:00.000000 dymoval-0.8.4/scripts/tutorial.ipynb
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/dymoval/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/dymoval/config.py
+-rw-r--r--   0        0        0   112849 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/dymoval/dataset.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/dymoval/utils.py
+-rw-r--r--   0        0        0    32835 2020-02-02 00:00:00.000000 dymoval-0.8.4/src/dymoval/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/fixture_data.py
+-rw-r--r--   0        0        0    54387 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/test_dataset.py
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/test_initializers.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/test_utils.py
+-rw-r--r--   0        0        0    26580 2020-02-02 00:00:00.000000 dymoval-0.8.4/tests/test_validation.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dymoval-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 dymoval-0.8.4/LICENSE
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 dymoval-0.8.4/README.md
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 dymoval-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 dymoval-0.8.4/PKG-INFO
```

### Comparing `dymoval-0.8.3/coverage.svg` & `dymoval-0.8.4/coverage.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/Makefile` & `dymoval-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/make.bat` & `dymoval-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/conf.py` & `dymoval-0.8.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/index.rst` & `dymoval-0.8.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/installation.rst` & `dymoval-0.8.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/integration.rst` & `dymoval-0.8.4/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/reference.rst` & `dymoval-0.8.4/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/Composition.svg` & `dymoval-0.8.4/docs/source/figures/Composition.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/DymovalLogo.svg` & `dymoval-0.8.4/docs/source/figures/DymovalLogo.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/DymovalLogo_Layer 2_Small.svg` & `dymoval-0.8.4/docs/source/figures/DymovalLogo_Layer 2_Small.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/DymovalNutshell.svg` & `dymoval-0.8.4/docs/source/figures/DymovalNutshell.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/ModelValidation.svg` & `dymoval-0.8.4/docs/source/figures/ModelValidation.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/figures/ModelValidationDymoval.svg` & `dymoval-0.8.4/docs/source/figures/ModelValidationDymoval.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/getting_started_index/create_dataset.rst` & `dymoval-0.8.4/docs/source/getting_started_index/create_dataset.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/getting_started_index/doe.rst` & `dymoval-0.8.4/docs/source/getting_started_index/doe.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/getting_started_index/model_validation.rst` & `dymoval-0.8.4/docs/source/getting_started_index/model_validation.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/getting_started_index/simulate_model.rst` & `dymoval-0.8.4/docs/source/getting_started_index/simulate_model.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/getting_started_index/validation_session.rst` & `dymoval-0.8.4/docs/source/getting_started_index/validation_session.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/reference_index/dataset.rst` & `dymoval-0.8.4/docs/source/reference_index/dataset.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/docs/source/reference_index/validation.rst` & `dymoval-0.8.4/docs/source/reference_index/validation.rst`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/DCMotor.fmu` & `dymoval-0.8.4/scripts/DCMotor.fmu`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/DCMotor.svg` & `dymoval-0.8.4/scripts/DCMotor.svg`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/DCMotorLogs.h5` & `dymoval-0.8.4/scripts/DCMotorLogs.h5`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/DCMotorModel.py` & `dymoval-0.8.4/scripts/DCMotorModel.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/test_manual.py` & `dymoval-0.8.4/scripts/test_manual.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # ===========================================================================
 
 from copy import deepcopy
 import dymoval as dmv
 import numpy as np
 import matplotlib.pyplot as plt
 
-
 # ===========================================================================
 # Assume that we have some measurements from some experiment.
 # Unfortunately, there is some missing data and the signals are not even sampled
 # with the same sampling period.
 #
 # Simulate something with Simulink and export an FMU.
 #
@@ -27,14 +26,15 @@
 #                   "signal_unit": str | list[str]
 #                   "sampling_period": float
 #                   "time_unit": str
 #                     }
 # ===========================================================================
 # Create dymoval Dataset objects
 
+
 # %%
 plt.ion()
 # Let's create some Signal
 nan_intervals = np.empty(200)
 nan_intervals[:] = np.NaN
 
 # INPUT signals
@@ -51,14 +51,15 @@
             np.random.rand(30),
             nan_intervals,
         )
     ),
     np.hstack((np.random.rand(80), nan_intervals, np.random.rand(100))),
 ]
 
+# %%
 
 input_signal_units = ["m/s", "%", "°C"]
 #
 in_lst = []
 for ii, val in enumerate(input_signal_names):
     temp_in: dmv.Signal = {
         "name": val,
@@ -120,14 +121,15 @@
 
 # %% You can check if your Signal are in correct format through the function
 # dmv.validate_signals
 dmv.validate_signals(*signal_list)
 
 # ... and you can visually inspect them through the function dmv.plot_signals
 dmv.plot_signals(*signal_list)
+plt.pause(0.0001)
 
 # The signals to be included in a dataset must have the same sampling period,
 # so you may need to re-sample your signals.
 # Dymoval will try to fix the sampling period for you with
 # the function fix_sampling_period.
 # Such a function will tell you what signals were resampled and what not.
 
@@ -159,18 +161,20 @@
 # Once the dymoval Dataset is created, it is possible to handle with the NaN:s
 # in a number of ways
 ds = ds.remove_NaNs()
 
 # At this point we can visually inspect the resulting Dataset.
 # Note how the areas where the NaN:s have been replaced are shaded.
 ax = ds.plot()
+plt.pause(0.0001)
 
 # %% We can also inspect the Dataset coverage region
 
 ds.plot_coverage()
+plt.pause(0.0001)
 
 # Other methods of the class Dataset are self-explanatory.
 #
 #
 #
 # ===========================================================================
 # Validation Session
@@ -201,14 +205,15 @@
 # We use the ValidationSession's method append_simulation to append the simulation
 # results.
 vs = vs.append_simulation(sim1_name, sim1_labels, sim1_values)
 vs = vs.append_simulation(sim2_name, sim2_labels, sim2_values)
 
 # %% We can visually inspect the results...
 vs.plot_simulations()
+plt.pause(0.0001)
 
 # %% ... or we can get validation metrics
 
 vs.validation_results
 
 # %% At this point we can clear the simulations list
 vs.clear()
```

### Comparing `dymoval-0.8.3/scripts/test_plots_manual.py` & `dymoval-0.8.4/scripts/test_plots_manual.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/scripts/tutorial.ipynb` & `dymoval-0.8.4/scripts/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/src/dymoval/config.py` & `dymoval-0.8.4/src/dymoval/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "num_decimals": "NUM_DECIMALS",
     "color_map": "COLORMAP",
 }
 
 try:
     import tomllib
 except ModuleNotFoundError:
-    import tomli as tomllib  # type:ignore
+    import tomli as tomllib
 
 try:
     with open(
         pathlib.Path.home().joinpath(".dymoval/config.toml"), mode="rb"
     ) as fp:
         data = tomllib.load(fp)
     for k, val in data.items():
```

### Comparing `dymoval-0.8.3/src/dymoval/dataset.py` & `dymoval-0.8.4/src/dymoval/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,25 @@
 from matplotlib import pyplot as plt
 from scipy import io, fft
 from .config import *  # noqa
 from .utils import *  # noqa, Type
 from typing import TypedDict, Any, Literal
 from copy import deepcopy
 
+# %%
+a = 4
+b = 3
+
+
+# %%
+c = 9
+d = 69
+
+# %%
+
 
 class Signal(TypedDict):
     """
     :py:class:`Signals <dymoval.dataset.Signal>` are used to represent real-world measurements.
 
 
     They are used to instantiate :py:class:`Dataset <dymoval.dataset.Dataset>` objects.
@@ -231,15 +242,14 @@
         target_sampling_period: float | None = None,
         tin: float | None = None,
         tout: float | None = None,
         full_time_interval: bool = False,
         overlap: bool = False,
         verbosity: int = 0,
     ) -> None:
-
         # ==============================
         # Instance attributes
         # ==============================
         # Here are declared but they will be initialized
         # in the method _new_dataset_from_dataframe()
         self.name: str = "foo"
         self.dataset: pd.DataFrame = pd.DataFrame()
@@ -294,21 +304,19 @@
     #   Class methods
     # ==============================================
 
     def _shade_nans(
         self,
         axes: matplotlib.axes.Axes,
     ) -> None:
-
         # Function for cfiltering out only the signals present in the dataset
         # Note that only signals in the dataset can have NaN:s
         def filter_signals(
             avail_signals: list[str], ax: matplotlib.axes.Axes
         ) -> list[tuple[matplotlib.lines.Line2D, str]]:
-
             # Implementation
             lines, labels = ax.get_legend_handles_labels()
             lines_labels_all = list(zip(lines, labels))
             lines_labels_filt = []
             for line_label in lines_labels_all:
                 for s in available_signals:
                     if s in line_label[1]:  # check if s is in the legend
@@ -335,15 +343,14 @@
                     # Shade only if there is a non-empty interval
                     if not val.size == 0:
                         ax.axvspan(min(val), max(val), color=color, alpha=0.2)
 
     def _find_dataset_coverage(
         self,
     ) -> tuple[pd.Series, pd.DataFrame, pd.Series, pd.DataFrame]:
-
         df = self.dataset
         u_mean = df["INPUT"].mean(axis=0).round(NUM_DECIMALS)
         u_cov = df["INPUT"].cov().round(NUM_DECIMALS)
         y_mean = df["OUTPUT"].mean(axis=0).round(NUM_DECIMALS)
         y_cov = df["OUTPUT"].cov().round(NUM_DECIMALS)
 
         return u_mean, u_cov, y_mean, y_cov
@@ -389,16 +396,16 @@
         # Create a reference to self._nan_intervals
         NaN_intervals = self._nan_intervals
 
         for k in NaN_intervals.keys():
             for idx, nan_chunk in enumerate(NaN_intervals[k]):
                 nan_chunk_translated = nan_chunk - tin
                 NaN_intervals[k][idx] = np.round(
-                    nan_chunk_translated, NUM_DECIMALS  # noqa
-                )
+                    nan_chunk_translated, NUM_DECIMALS
+                )  # noqa
                 NaN_intervals[k][idx] = nan_chunk_translated[
                     nan_chunk_translated >= 0.0
                 ]
 
     def _new_dataset_from_dataframe(
         self,
         name: str,
@@ -408,15 +415,14 @@
         tin: float | None = None,
         tout: float | None = None,
         full_time_interval: bool = False,
         overlap: bool = False,
         verbosity: int = 0,
         _excluded_signals: list[str] = [],
     ) -> None:
-
         # ==============================================================
         # All the class attributes are defined and initialized here
         #
         # self.name
         # self.dataset
         # self.coverage
         # self.information_level
@@ -586,15 +592,14 @@
         target_sampling_period: float | None = None,
         tin: float | None = None,
         tout: float | None = None,
         full_time_interval: bool = False,
         overlap: bool = False,
         verbosity: int = 0,
     ) -> None:
-
         # Do not initialize any class attribute here!
         # All attributes are initialized in the _new_dataset_from_dataframe() method
 
         # Arguments validation
         validate_signals(*signal_list)
 
         # If the user pass a single signal as a str,
@@ -876,15 +881,14 @@
         linecolors_tpl: list[tuple[str, ...]],
         ylabels_tpl: list[tuple[str, ...]],
         labels_tpl: list[tuple[str, ...]],
         linestyles_tpl: list[tuple[str, ...]],
         alpha_fg: float,
         alpha_bg: float,
     ) -> matplotlib.figure.Figure:
-
         # This is the function who makes the actual plot once all the
         # parameters are set and passed
         # Adjust passed dataframe.
 
         # Initialize iteration
         fig = grid.figure
         if fig.get_axes():
@@ -1024,15 +1028,14 @@
                 f"{[s for s in excluded_signals]}"
             )
             print(f"actual sampling period = {target_sampling_period}")
 
         return resampled_signals, excluded_signals
 
     def _add_signals(self, kind: Signal_type, *signals: Signal) -> Dataset:
-
         # Validate the dymoval Signals
         validate_signals(*signals)
 
         # Target dataset
         ds = deepcopy(self)
 
         # Check if the sampling period is OK
@@ -2652,15 +2655,14 @@
 # Useful functions
 # ====================================================
 
 
 def _list_to_structured_list_of_tuple(
     tpl: list[tuple[str, ...]], lst: list[str]
 ) -> list[tuple[str, ...]]:
-
     # Convert a plain list to a list of tuple of a given structure, i.e.
     # Given tpl = [("a0","a1"),("b0",),("b1","a1","b0"),("a0","a1"),("b0",)]
     # and lst = ["u0", "u1", "u2", "u3", "u4", "u5", "u6", "u7" , "u8"]
     # it returns [("u0", "u1"), ("u2",), ("u3", "u4", "u5"), ("u6", "u7") , ("u8",)]
     R = []
     idx = 0
     for ii in [len(jj) for jj in tpl]:
```

### Comparing `dymoval-0.8.3/src/dymoval/utils.py` & `dymoval-0.8.4/src/dymoval/utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/src/dymoval/validation.py` & `dymoval-0.8.4/src/dymoval/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     )
     return r2  # type: ignore
 
 
 def _xcorr_norm_validation(
     Rxy: XCorrelation,
 ) -> XCorrelation:
-
     R = Rxy["values"]
 
     # MISO or SIMO case
     if R.ndim == 2:
         R = R[:, :, np.newaxis]
     # SISO case
     elif R.ndim == 1:
@@ -314,15 +313,14 @@
 
     def _append_validation_results(
         self,
         sim_name: str,
         l_norm: float | Literal["fro", "nuc"] | None = np.inf,
         matrix_norm: float | Literal["fro", "nuc"] | None = 2,
     ) -> None:
-
         # Extact dataset output values
         df_val = self.Dataset.dataset
         y_values = df_val["OUTPUT"].to_numpy()
 
         # Simulation results
         y_sim_values = self.simulations_results[sim_name].to_numpy()
 
@@ -343,15 +341,14 @@
                 "The simulations list looks empty. "
                 "Check the available simulation names with 'simulations_namess()'"
             )
 
     def _simulation_validation(
         self, sim_name: str, y_names: list[str], y_data: np.ndarray
     ) -> None:
-
         if len(y_names) != len(set(y_names)):
             raise ValueError("Signals name must be unique.")
         if (
             not self.simulations_results.empty
             and sim_name in self.simulations_names()
         ):
             raise ValueError(
@@ -814,17 +811,17 @@
         df_sim = pd.DataFrame(data=y_data, index=vs_temp.Dataset.dataset.index)
         multicols = list(zip([sim_name] * len(y_names), y_names, y_units))
         df_sim.columns = pd.MultiIndex.from_tuples(
             multicols, names=["sim_names", "signal_names", "units"]
         )
 
         # Concatenate df_sim with the current sim results
-        vs_temp.simulations_results = pd.concat(
-            [df_sim, vs_temp.simulations_results], axis=1
-        )
+        vs_temp.simulations_results = vs_temp.simulations_results.join(
+            df_sim, how="right"
+        ).rename_axis(df_sim.columns.names, axis=1)
 
         # Update residuals auto-correlation and cross-correlation attributes
         vs_temp._append_correlations_tensors(sim_name)
         vs_temp._append_validation_results(sim_name)
 
         return vs_temp
```

### Comparing `dymoval-0.8.3/tests/fixture_data.py` & `dymoval-0.8.4/tests/fixture_data.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/tests/test_dataset.py` & `dymoval-0.8.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/tests/test_initializers.py` & `dymoval-0.8.4/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/tests/test_utils.py` & `dymoval-0.8.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/tests/test_validation.py` & `dymoval-0.8.4/tests/test_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,16 +353,19 @@
     def test_plots(self, good_dataframe: pd.DataFrame, tmp_path: str) -> None:
         df, u_names, y_names, _, _, fixture = good_dataframe
         name_ds = "my_dataset"
         ds = dmv.dataset.Dataset(
             name_ds, df, u_names, y_names, full_time_interval=True
         )
 
+        print(ds.dataset)
+
         name_vs = "my_validation"
         vs = dmv.ValidationSession(name_vs, ds)
+        print(vs.simulations_results)
 
         # Add one model
         sim1_name = "Model 1"
         sim1_labels = ["my_y1", "my_y2"]  # The fixture has two outputs
         if fixture == "SISO" or fixture == "MISO":
             sim1_labels = [sim1_labels[0]]
         sim1_values = np.random.rand(
@@ -375,14 +378,15 @@
         sim2_labels = ["your_y1", "your_y2"]  # The fixture has two outputs
         if fixture == "SISO" or fixture == "MISO":
             sim2_labels = [sim2_labels[0]]
         sim2_values = vs.Dataset.dataset["OUTPUT"].values + np.random.rand(
             len(vs.Dataset.dataset["OUTPUT"].values), 1
         )
         vs = vs.append_simulation(sim2_name, sim2_labels, sim2_values)
+        print(vs.simulations_results)
 
         # =============================
         # plot simulations
         # =============================
         _ = vs.plot_simulations()
         plt.close("all")
```

### Comparing `dymoval-0.8.3/LICENSE` & `dymoval-0.8.4/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Volvo Autonomous Solutions (Official)
+Author: Ubaldo Tiberi.
+Copyright (c) 2018, Volvo Autonomous Solutions.
 All rights reserved.
-Author: Ubaldo Tiberi
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
 
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
```

### Comparing `dymoval-0.8.3/README.md` & `dymoval-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `dymoval-0.8.3/PKG-INFO` & `dymoval-0.8.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: dymoval
-Version: 0.8.3
+Version: 0.8.4
 Summary: Dymoval is a Python package for validating models and analyzing datasets.
 Project-URL: Homepage, https://github.com/VolvoGroup/dymoval
 Project-URL: Documentation, https://volvogroup.github.io/dymoval/
 Project-URL: Bug Tracker, https://github.com/VolvoGroup/dymoval/issues
 Author-email: Ubaldo Tiberi <ubaldo.tiberi@volvo.com>, Ubaldo Tiberi <ubaldo.tiberi@gmail.com>
 License: BSD 3-Clause License
         
-        Copyright (c) 2022, Volvo Autonomous Solutions (Official)
+        Author: Ubaldo Tiberi.
+        Copyright (c) 2018, Volvo Autonomous Solutions.
         All rights reserved.
-        Author: Ubaldo Tiberi
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
         
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
         AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
         IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
         DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
@@ -38,34 +38,35 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Keywords: data,data-analysis,dataset,model validation,modeling
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: black
-Requires-Dist: conda-lock
 Requires-Dist: control
-Requires-Dist: coverage
-Requires-Dist: flake8
-Requires-Dist: furo
 Requires-Dist: h5py
 Requires-Dist: matplotlib
-Requires-Dist: mypy
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathlib
-Requires-Dist: pytest
 Requires-Dist: scipy
-Requires-Dist: sphinx
-Requires-Dist: sphinx-autodoc-typehints
-Requires-Dist: sphinx-toolbox
 Requires-Dist: tomli
 Provides-Extra: build
 Requires-Dist: hatch; extra == 'build'
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: flake8; extra == 'dev'
+Requires-Dist: furo; extra == 'dev'
+Requires-Dist: grayskull; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: sphinx; extra == 'dev'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'dev'
+Requires-Dist: sphinx-toolbox; extra == 'dev'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://github.com/VolvoGroup/dymoval/blob/main/docs/source/figures/DymovalLogo.svg" data-canonical-src="[https://github.com/VolvoGroup/dymoval/blob/main/docs/source/figures/DymovalLogo.svg](https://github.com/VolvoGroup/dymoval/blob/main/docs/source/figures/DymovalLogo.svg)" width="800" class="center" />
```

