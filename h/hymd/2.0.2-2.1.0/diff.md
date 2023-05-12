# Comparing `tmp/hymd-2.0.2.tar.gz` & `tmp/hymd-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hymd-2.0.2.tar", last modified: Fri Apr 28 15:24:00 2023, max compression
+gzip compressed data, was "hymd-2.1.0.tar", last modified: Fri May 12 13:24:21 2023, max compression
```

## Comparing `hymd-2.0.2.tar` & `hymd-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.478704 hymd-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-28 15:17:50.000000 hymd-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-28 15:24:00.478704 hymd-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-28 15:17:50.000000 hymd-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/hymd/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/barostat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/barostat_scr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_angle_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_angle_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_bond_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_bond_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_dihedral_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/compute_dihedral_forces__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/dipole_reconstruction.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/dipole_reconstruction__double.f90
--rw-r--r--   0 runner    (1001) docker     (123)    46365 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    26666 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/gaussian_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    52393 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    50045 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 15:17:50.000000 hymd-2.0.2/hymd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/hymd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:24:00.000000 hymd-2.0.2/hymd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 15:17:50.000000 hymd-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:24:00.478704 hymd-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 15:17:50.000000 hymd-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:24:00.474704 hymd-2.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_configure_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_distribute_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_force.py
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)    33165 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_input_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-28 15:17:50.000000 hymd-2.0.2/test/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:21.691550 hymd-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-05-12 13:18:44.000000 hymd-2.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-12 13:24:21.691550 hymd-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-05-12 13:18:44.000000 hymd-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:21.691550 hymd-2.1.0/hymd/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/barostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/barostat_scr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_angle_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_angle_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_bond_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_bond_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_dihedral_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/compute_dihedral_forces__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/dipole_reconstruction.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/dipole_reconstruction__double.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    46365 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27522 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29848 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19583 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/gaussian_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16234 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52393 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54502 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/plumed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 13:18:44.000000 hymd-2.1.0/hymd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:21.691550 hymd-2.1.0/hymd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-12 13:24:21.000000 hymd-2.1.0/hymd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-12 13:24:21.000000 hymd-2.1.0/hymd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:24:21.000000 hymd-2.1.0/hymd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 13:24:21.000000 hymd-2.1.0/hymd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 13:24:21.000000 hymd-2.1.0/hymd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-12 13:18:44.000000 hymd-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:24:21.691550 hymd-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-12 13:18:44.000000 hymd-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:24:21.691550 hymd-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_configure_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_distribute_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33165 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_input_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_plumed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-05-12 13:18:44.000000 hymd-2.1.0/test/test_thermostat.py
```

### Comparing `hymd-2.0.2/LICENSE.txt` & `hymd-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/PKG-INFO` & `hymd-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 2.0.2
+Version: 2.1.0
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hymd Version: 2.0.2 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.1.0 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `hymd-2.0.2/README.md` & `hymd-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/barostat.py` & `hymd-2.1.0/hymd/barostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         # Total pressure across all ranks
         P = np.average(pressure[-3:-1])  # kJ/(mol nm^3)
         P = P * 16.61  # bar
 
         # scaling factor
         alpha = (
             1.0
-            - config.time_step
+            - (config.time_step * config.respa_inner)
             * config.n_b
             / config.tau_p
             * beta
             * (config.target_pressure.P_L - P)
         ) ** (1 / 3)
 
         # length scaling
@@ -274,30 +274,30 @@
         alphaL = 1.0
         alphaN = 1.0
 
         if config.target_pressure.P_L:
             # scaling factor
             alphaL = (
                 1.0
-                - config.time_step
+                - (config.time_step * config.respa_inner)
                 * config.n_b
                 / config.tau_p
                 * beta
                 * (config.target_pressure.P_L - PL)
             ) ** (1 / 3)
             # length scaling
             config.box_size[0:2] *= alphaL
 
             positions[:][0:2] *= alphaL
 
         if config.target_pressure.P_N:
             # scaling factor
             alphaN = (
                 1.0
-                - config.time_step
+                - (config.time_step * config.respa_inner)
                 * config.n_b
                 / config.tau_p
                 * beta
                 * (config.target_pressure.P_N - PN)
             ) ** (1 / 3)
             # length scaling
             config.box_size[2] *= alphaN
```

### Comparing `hymd-2.0.2/hymd/barostat_scr.py` & `hymd-2.1.0/hymd/barostat_scr.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,23 +102,23 @@
         noise_term = (
             np.sqrt(
                 2.0
                 * config.n_b
                 * config.gas_constant
                 * config.target_temperature
                 * beta
-                * config.time_step
+                * config.time_step * config.respa_inner
                 * config.n_b
                 / (V * config.tau_p)
             )
             * R
         )
         log_alpha = (
             -config.n_b
-            * config.time_step
+            * config.time_step * config.respa_inner
             * beta
             / config.tau_p
             * (config.target_pressure.P_L - P)
         )
         log_alpha = log_alpha + noise_term
         alpha = np.exp(log_alpha / 3.0)
 
@@ -217,24 +217,24 @@
             noise_term = (
                 np.sqrt(
                     4.0
                     * config.n_b
                     * config.gas_constant
                     * config.target_temperature
                     * beta
-                    * config.time_step
+                    * config.time_step * config.respa_inner
                     * config.n_b
                     / (3 * V * config.tau_p)
                 )
                 * Rxy
             )
             log_alpha = (
                 -2.0
                 * config.n_b
-                * config.time_step
+                * config.time_step * config.respa_inner
                 * beta
                 / (3 * config.tau_p)
                 * (
                     config.target_pressure.P_L
                     - PL
                     - config.surface_tension / config.box_size[2]
                 )
@@ -253,23 +253,23 @@
             noise_term = (
                 np.sqrt(
                     2.0
                     * config.n_b
                     * config.gas_constant
                     * config.target_temperature
                     * beta
-                    * config.time_step
+                    * config.time_step * config.respa_inner
                     * config.n_b
                     / (3 * V * config.tau_p)
                 )
                 * Rz
             )
             log_alpha = (
                 -config.n_b
-                * config.time_step
+                * config.time_step * config.respa_inner
                 * beta
                 / (3 * config.tau_p)
                 * (config.target_pressure.P_N - PN)
             )
             log_alpha = log_alpha + noise_term
             alpha = np.exp(
                 log_alpha / 1.0
```

### Comparing `hymd-2.0.2/hymd/compute_angle_forces.f90` & `hymd-2.1.0/hymd/compute_angle_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/compute_angle_forces__double.f90` & `hymd-2.1.0/hymd/compute_angle_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/compute_bond_forces.f90` & `hymd-2.1.0/hymd/compute_bond_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/compute_bond_forces__double.f90` & `hymd-2.1.0/hymd/compute_bond_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/compute_dihedral_forces.f90` & `hymd-2.1.0/hymd/compute_dihedral_forces.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/compute_dihedral_forces__double.f90` & `hymd-2.1.0/hymd/compute_dihedral_forces__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/configure_runtime.py` & `hymd-2.1.0/hymd/configure_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Parses command line arguments to HyMD
 """
-from argparse import ArgumentParser
+import argparse
 import os
 import sys
 import numpy as np
 import atexit
 import cProfile
 import logging
 import pstats
@@ -26,15 +26,15 @@
     Returns
     -------
     args : argparse.Namespace
         Namespace containing command line arguments.
     config : hymd.input_parser.Config
         Parsed configuration object.
     """
-    ap = ArgumentParser()
+    ap = argparse.ArgumentParser()
 
     ap.add_argument(
         "-v",
         "--verbose",
         default=1,
         type=int,
         nargs="?",
@@ -123,15 +123,29 @@
     )
     ap.add_argument(
         "--logfile",
         default="sim.log",
         help="Redirect event logging to specified file",
     )
     ap.add_argument(
-        "-p", "--topol", default=None, help="Gmx-like topology file in toml format"
+        "--plumed", 
+        type=extant_file,
+        help="PLUMED input file",
+    )
+    ap.add_argument(
+        "--plumed-outfile",
+        default="plumed.out",
+        help="PLUMED input file",
+    )
+    ap.add_argument(
+        "-p",
+        "--topol",
+        default=None,
+        type=extant_file,
+        help="Gmx-like topology file in toml format"
     )
     ap.add_argument("config", help="Config .py or .toml input configuration script")
     ap.add_argument("input", help="input.hdf5")
     args = ap.parse_args(args_in)
 
     if comm.Get_rank() == 0:
         os.makedirs(args.destdir, exist_ok=True)
@@ -212,7 +226,20 @@
         Logger.rank0.log(logging.INFO, str(config))
     except ValueError as ve:
         raise ValueError(
             f"Unable to parse configuration file {args.config}"
             f"\n\ntoml parse traceback:" + repr(ve)
         )
     return args, config, prng, topol
+
+
+def extant_file(x):
+    """
+    'Type' for argparse - checks that file exists but does not open.
+    From https://stackoverflow.com/a/11541495
+    """
+    if not os.path.exists(x):
+        # Argparse uses the ArgumentTypeError to give a rejection message like:
+        # error: argument input: x does not exist
+        raise argparse.ArgumentTypeError("{0} does not exist".format(x))
+    return x
+
```

### Comparing `hymd-2.0.2/hymd/dipole_reconstruction.f90` & `hymd-2.1.0/hymd/dipole_reconstruction.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/dipole_reconstruction__double.f90` & `hymd-2.1.0/hymd/dipole_reconstruction__double.f90`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/field.py` & `hymd-2.1.0/hymd/field.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/file_io.py` & `hymd-2.1.0/hymd/file_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,14 +129,15 @@
     bonds_2_atom1,
     bonds_2_atom2,
     molecules=None,
     velocity_out=False,
     force_out=False,
     charges=False,
     dielectrics=False,
+    plumed_out=False,
     comm=MPI.COMM_WORLD,
 ):
     """Outputs all static time-independent quantities to the HDF5 output file
 
     Parameters
     ----------
     h5md : OutDataset
@@ -165,14 +166,16 @@
         If :code:`True`, velocities are written to output HDF5 file.
     force_out : bool, optional
         If :code:`True`, forces are written to output HDF5 file.
     charges : (N,) numpy.ndarray
         Array of particle charge values for :code:`N` particles.
     dielectrics : (N,) numpy.ndarray
         Array of particle relative dielectric values for :code:`N` particles.
+    plumed_out : bool, optional
+        If :code:`True`, PLUMED bias is written to output HDF5 file.
     comm : mpi4py.Comm
         MPI communicator to use for rank commuication.
 
     See also
     --------
     prepare_bonds :
         Constructs two-, three-, and four-particle bonds from toplogy input
@@ -387,15 +390,23 @@
             "field_q_energy",
             h5md.observables,
             n_frames,
             (1,),
             dtype,
             units="kJ mol-1",  # noqa: E501
         )  # <-------- xinmeng
-
+    if plumed_out is not False:
+        (
+            _,
+            h5md.plumed_bias_step,
+            h5md.plumed_bias_time,
+            h5md.plumed_bias,
+        ) = setup_time_dependent_element(
+            "plumed_bias", h5md.observables, n_frames, (1,), dtype, units="kJ mol-1"  # noqa: E501
+        )
     (
         _,
         h5md.total_momentum_step,
         h5md.total_momentum_time,
         h5md.total_momentum,
     ) = setup_time_dependent_element(  # noqa: E501
         "total_momentum",
@@ -538,19 +549,21 @@
     pressure,
     kinetic_energy,
     bond2_energy,
     bond3_energy,
     bond4_energy,
     field_energy,
     field_q_energy,
+    plumed_bias,
     time_step,
     config,
     velocity_out=False,
     force_out=False,
     charge_out=False,
+    plumed_out=False,
     dump_per_particle=False,
     comm=MPI.COMM_WORLD,
 ):
     """Writes time-step data to HDF5 output file
 
     Handles all quantities which change during simulation, as opposed to
     static quanitities (see :code:`store_static`).
@@ -581,27 +594,31 @@
         Calculated instantaneous harmonic two-particle bond energy.
     bond3_energy : float
         Calculated instantaneous harmonic angular three-particle bond energy.
     bond4_energy : float
         Calculated instantaneous dihedral four-particle torsion energy.
     field_energy : float
         Calculated instantaneous particle-field energy.
-    field_energy_q : float
+    field_q_energy : float
         Calculated instantaneous electrostatic energy.
+    plumed_bias : float
+        PLUMED instantaneous bias energy.
     time_step : float
         Value of the time step.
     config : Config
         Configuration object.
     velocity_out : bool, optional
         If :code:`True`, velocities are written to output HDF5 file.
     force_out : bool, optional
         If :code:`True`, forces are written to output HDF5 file.
     charge_out : bool, optional
         If :code:`True`, electrostatic energies are written to the output
         HDF5 file.
+    plumed_out : bool, optional
+        If :code:`True`, PLUMED bias is written to the output HDF5 file.
     dump_per_particle : bool, optional
         If :code:`True`, all quantities are written **per particle**.
     comm : mpi4py.Comm
         MPI communicator to use for rank commuication.
 
     See also
     --------
@@ -651,24 +668,29 @@
         h5md.velocities_time[frame] = step * time_step
     if force_out:
         h5md.forces_step[frame] = step
         h5md.forces_time[frame] = step * time_step
     if charge_out:
         h5md.field_q_energy_step[frame] = step
         h5md.field_q_energy_time[frame] = step * time_step
+    if plumed_out:
+        h5md.plumed_bias_step[frame] = step
+        h5md.plumed_bias_time[frame] = step * time_step
 
     ind_sort = np.argsort(indices)
     h5md.positions[frame, indices[ind_sort]] = positions[ind_sort]
 
     if velocity_out:
         h5md.velocities[frame, indices[ind_sort]] = velocities[ind_sort]
     if force_out:
         h5md.forces[frame, indices[ind_sort]] = forces[ind_sort]
     if charge_out:
         h5md.field_q_energy[frame] = field_q_energy
+    if plumed_out:
+        h5md.plumed_bias[frame] = plumed_bias
 
     potential_energy = (
         bond2_energy + bond3_energy + bond4_energy + field_energy + field_q_energy
     )
 
     total_momentum = config.mass * comm.allreduce(np.sum(velocities, axis=0), MPI.SUM)
     angular_momentum = config.mass * comm.allreduce(
@@ -701,33 +723,33 @@
         "kin E",
         "pot E",
         "field E",
         "elec E",
         "bond E",
         "ang E",
         "dih E",
+        "bias E",
         "Px",
         "Py",
         "Pz",
         "ΔH" if config.target_temperature else "ΔE",
     ]
     fmt_ = np.array(fmt_)
 
     # create mask to show only energies != 0
-    en_array = np.array(
-        [
-            field_energy,
-            field_q_energy,
-            bond2_energy,
-            bond3_energy,
-            bond4_energy,
-        ]
-    )
+    en_array = np.array([
+        field_energy,
+        field_q_energy,
+        bond2_energy,
+        bond3_energy,
+        bond4_energy,
+        plumed_bias,
+    ])
     mask = np.full_like(fmt_, True, dtype=bool)
-    mask[range(6, 11)] = en_array != 0.0
+    mask[range(6,12)] = en_array != 0.
 
     header_ = fmt_[mask].shape[0] * "{:>13}"
     if config.initial_energy is None:
         fmt_[-1] = ""
 
     divide_by = 1.0
     if dump_per_particle:
@@ -754,14 +776,15 @@
         kinetic_energy / divide_by,
         potential_energy / divide_by,
         field_energy / divide_by,
         field_q_energy / divide_by,
         bond2_energy / divide_by,
         bond3_energy / divide_by,
         bond4_energy / divide_by,
+        plumed_bias / divide_by,
         total_momentum[0] / divide_by,
         total_momentum[1] / divide_by,
         total_momentum[2] / divide_by,
         H_tilde / divide_by,
     ]
     data = data_fmt.format(*[val for i, val in enumerate(all_data) if mask[i]])
     Logger.rank0.log(logging.INFO, ("\n" + header + "\n" + data))
```

### Comparing `hymd-2.0.2/hymd/force.py` & `hymd-2.1.0/hymd/force.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/gaussian_core.py` & `hymd-2.1.0/hymd/gaussian_core.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/hamiltonian.py` & `hymd-2.1.0/hymd/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/input_parser.py` & `hymd-2.1.0/hymd/input_parser.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/integrator.py` & `hymd-2.1.0/hymd/integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/logger.py` & `hymd-2.1.0/hymd/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -190,37 +190,38 @@
     / / / /_  __/ / /__  _________ _____ ______   /  |/  / __ \
    / /_/ / / / / / / _ \/ ___/ __ `/ __ `/ ___/  / /|_/ / / / /
   / __  / /_/ / / /  __/ /  / /_/ / /_/ (__  )  / /  / / /_/ / 
  /_/ /_/\__, /_/_/\___/_/   \__,_/\__,_/____/  /_/  /_/_____/  
        /____/ 
     """
 
-    refs_set1 = """
+    refs_set = """
  
  [1] Ledum, M.; Sen, S.; Li, X.; Carrer, M.; Feng Y.; Cascella, M.; Bore, S. L. 
- HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter. ChemRxiv 2021
+ HylleraasMD: A Domain Decomposition-Based Hybrid Particle-Field Software for Multi-Scale Simulations of Soft Matter.
+ J. Chem. Theory Comput. 2023.
 
  [2] Ledum, M.; Carrer, M.; Sen, S.; Li, X.; Cascella, M.; Bore, S. L. 
  HyMD: Massively parallel hybrid particle-field molecular dynamics in Python.
+ J. Open Source Softw. 8(84), 4149, 2023.
  
- [3] Bore, S. L.; Cascella, M. 
- Hamiltonian and alias-free hybrid particle–field molecular dynamics. J. Chem. Phys. 2020, 153, 094106.
+ [3] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. 
+ Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble.
+ J Chem Inf Model 2023, 63(7), 1549-9596.
+
+ [4] Bore, S. L.; Cascella, M. 
+ Hamiltonian and alias-free hybrid particle–field molecular dynamics.
+ J. Chem. Phys. 2020, 153, 094106.
 
- [4] Pippig, M. PFFT: An extension of FFTW to massively parallel architectures. SIAM J. Sci. Comput. 2013, 35, C213–C236.
-"""
-    refs_set2 = """
+ [5] Pippig, M. PFFT: An extension of FFTW to massively parallel architectures.
+ SIAM J. Sci. Comput. 2013, 35, C213–C236.
 
- [5] Sen, S.; Ledum, M.; Bore, S. L.; Cascella, M. 
- Soft Matter under Pressure: Pushing Particle–Field Molecular Dynamics to the Isobaric Ensemble. ChemRxiv 2023
 """
 
     version = f"Version {get_version()}"
     header = banner
     header += version.center(56) + "\n\n"
     #header += " Please read and cite the references below:"
     header += " PLEASE READ AND CITE THE REFERENCES BELOW:"
-    header += refs_set1
-    #header += " \n\n For constant pressure (NPT) simulations, please cite:"
-    header += " \n\n FOR CONSTANT PRESSURE (NPT) SIMULATIONS, PLEASE CITE:"
-    header += refs_set2
+    header += refs_set
 
     return header
```

### Comparing `hymd-2.0.2/hymd/main.py` & `hymd-2.1.0/hymd/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     csvr_thermostat,
     cancel_com_momentum,
     generate_initial_velocities,
 )
 from .force import dipole_forces_redistribution, prepare_bonds
 from .integrator import integrate_velocity, integrate_position
 from .pressure import comp_pressure
+from .plumed import PlumedBias
 
 
 def main():
     """Main simulation driver
 
     Initializes structure, topology, and simulation configuration and iterates
     the molecular dynamics loop.
@@ -173,14 +174,15 @@
 
     bond_forces = np.zeros_like(positions)
     angle_forces = np.zeros_like(positions)
     dihedral_forces = np.zeros_like(positions)
     reconstructed_forces = np.zeros_like(positions)
     field_forces = np.zeros_like(positions)
     elec_forces = np.zeros_like(positions)
+    plumed_forces = np.zeros_like(positions)
 
     positions = np.mod(positions, config.box_size[None, :])
 
     # Initialize dipoles, populate them if protein_flag == True
     if args.disable_dipole:
         dipole_flag = 0
     else:
@@ -194,14 +196,15 @@
     # Initialize energies
     field_energy = 0.0
     bond_energy = 0.0
     angle_energy = 0.0
     dihedral_energy = 0.0
     kinetic_energy = 0.0
     field_q_energy = 0.0
+    plumed_bias = 0.0
 
     # more initialization
     bond_pr_ = np.zeros(3, dtype=dtype)
     angle_pr_ = np.zeros(3, dtype=dtype)
 
     hamiltonian = get_hamiltonian(config)
 
@@ -257,14 +260,16 @@
     ]
 
     if charges_flag:
         args_in.append(charges)
         args_in.append(elec_forces)
     if dielectric_flag:
         args_in.append(dielectric_sorted)
+    if args.plumed:
+        args_in.append(plumed_forces)
 
     if config.domain_decomposition:
         (
             positions,
             velocities,
             indices,
             bond_forces,
@@ -286,14 +291,16 @@
         )
 
         if charges_flag:
             charges = optional.pop(0)
             elec_forces = optional.pop(0)
         if dielectric_flag:
             dielectric_sorted = optional.pop(0)
+        if args.plumed:
+            plumed_forces = optional.pop(0)
         if molecules_flag:
             bonds = optional.pop(0)
             molecules = optional.pop(0)
 
         # rebuild args_in to point to correct arrays
         args_in = [
             velocities,
@@ -308,14 +315,16 @@
         ]
 
         if charges_flag:
             args_in.append(charges)
             args_in.append(elec_forces)
         if dielectric_flag:
             args_in.append(dielectric_sorted)
+        if args.plumed:
+            args_in.append(plumed_forces)
 
     if not args.disable_field:
         layouts = [
             pm.decompose(positions[types == t]) for t in range(config.n_types)
         ]  # noqa: E501
         update_field(
             phi,
@@ -601,14 +610,15 @@
         bonds_2_atom1,
         bonds_2_atom2,
         molecules=molecules if molecules_flag else None,
         velocity_out=args.velocity_output,
         force_out=args.force_output,
         charges=charges if charges_flag else False,
         dielectrics=dielectric_sorted if dielectric_flag else False,
+        plumed_out=True if args.plumed else False,
         comm=comm,
     )
 
     if config.n_print > 0:
         step = 0
         frame = 0
         if not args.disable_field:
@@ -665,14 +675,55 @@
             + bond_forces
             + angle_forces
             + dihedral_forces
             + reconstructed_forces
         )
         if charges_flag:
             forces_out += elec_forces
+
+    # initialize PLUMED and get initial forces and bias
+    if args.plumed:
+        plumed = PlumedBias(
+            config, 
+            args.plumed, 
+            args.plumed_outfile, 
+            comm=comm,
+            verbose=args.verbose
+        )
+
+        current_forces = (bond_forces + angle_forces + dihedral_forces
+                        + field_forces + reconstructed_forces)
+        if charges_flag:
+            current_forces += elec_forces
+
+        # pass info and check if PLUMED also needs the energy
+        needs_energy = plumed.prepare(
+            0,
+            current_forces,
+            positions,
+            indices,
+            config,
+            (
+                np.zeros_like(indices, dtype=np.double) 
+                if not charges_flag else charges
+            )
+        )
+
+        # PLUMED likes the energy per rank
+        poteng = (field_energy + bond_energy + angle_energy
+                 + dihedral_energy + field_q_energy) / size
+
+        # get the forces and bias from PLUMED
+        plumed_forces, plumed_bias = plumed.calc(current_forces, poteng)
+
+    # log after PLUMED forces and bias have been calculated
+    if config.n_print > 0:
+        if args.plumed:
+            forces_out += plumed_forces
+
         store_data(
             out_dataset,
             step,
             frame,
             indices,
             positions,
             velocities,
@@ -682,19 +733,21 @@
             pressure,
             kinetic_energy,
             bond_energy,
             angle_energy,
             dihedral_energy,
             field_energy,
             field_q_energy,
+            plumed_bias,
             config.time_step,
             config,
             velocity_out=args.velocity_output,
             force_out=args.force_output,
             charge_out=charges_flag,
+            plumed_out=True if args.plumed else False,
             dump_per_particle=args.dump_per_particle,
             comm=comm,
         )
 
     if rank == 0:
         loop_start_time = datetime.datetime.now()
         last_step_time = datetime.datetime.now()
@@ -740,15 +793,19 @@
 
         # Initial outer rRESPA velocity step
         velocities = integrate_velocity(
             velocities,
             field_forces / config.mass,
             config.respa_inner * config.time_step,
         )
-
+        if args.plumed:
+            velocities = integrate_velocity(
+                velocities, plumed_forces / config.mass,
+                config.respa_inner * config.time_step,
+            )
         if charges_flag and (
             config.coulombtype == "PIC_Spectral"
             or config.coulombtype == "PIC_Spectral_GPE"
         ):
             velocities = integrate_velocity(
                 velocities,
                 elec_forces / config.mass,
@@ -893,14 +950,24 @@
                     psi,
                     Vbar_elec,
                     Vbar_elec_fourier,
                     force_mesh_elec,
                     force_mesh_elec_fourier,
                 ) = coulomb_list
 
+        # Only compute and keep the molecular bond energy from the last rRESPA
+        # inner step
+        if molecules_flag:
+            if not args.disable_bonds:
+                bond_energy = comm.allreduce(bond_energy_, MPI.SUM)
+            if not args.disable_angle_bonds:
+                angle_energy = comm.allreduce(angle_energy_, MPI.SUM)
+            if not args.disable_dihedrals:
+                dihedral_energy = comm.allreduce(dihedral_energy_, MPI.SUM)
+
         # Update slow forces
         if not args.disable_field:
             layouts = [
                 pm.decompose(positions[types == t])
                 for t in range(config.n_types)  # noqa: E501
             ]
             update_field(
@@ -1015,21 +1082,72 @@
                     bonds_4_atom2,
                     bonds_4_atom3,
                     bonds_4_atom4,
                     bonds_4_type,
                     bonds_4_last,
                 )
 
+        if args.plumed:
+            current_forces = (bond_forces + angle_forces + dihedral_forces
+                            + field_forces + reconstructed_forces)
+            if charges_flag:
+                current_forces += elec_forces
+
+            # pass info and check if PLUMED also needs the energy
+            needs_energy = plumed.prepare(
+                step,
+                current_forces,
+                positions,
+                indices,
+                config,
+                (
+                    np.zeros_like(indices, dtype=np.double) 
+                    if not charges_flag else charges
+                )
+            )
+
+            if needs_energy:
+                if not args.disable_field:
+                    (
+                        field_energy, kinetic_energy,
+                    ) = compute_field_and_kinetic_energy(
+                        phi, velocities, hamiltonian, positions, types, v_ext,
+                        config, layouts, comm=comm,
+                    )
+
+                    if charges_flag and config.coulombtype == "PIC_Spectral":
+                        field_q_energy = compute_field_energy_q(
+                            config, phi_q_fourier, elec_energy_field,
+                            field_q_energy, comm=comm,
+                        )
+                else:
+                    field_energy = 0.0
+                    field_q_energy = 0.0
+
+                # PLUMED likes the energy per rank
+                poteng = (field_energy + bond_energy + angle_energy
+                         + dihedral_energy + field_q_energy) / size
+            else:
+                poteng = 0.0
+
+            # get the forces and bias from PLUMED
+            plumed_forces, plumed_bias = plumed.calc(current_forces, poteng)
+
         # Second rRESPA velocity step
         velocities = integrate_velocity(
             velocities,
             field_forces / config.mass,
             config.respa_inner * config.time_step,
         )
 
+        if args.plumed:
+            velocities = integrate_velocity(
+                velocities, plumed_forces / config.mass,
+                config.respa_inner * config.time_step,
+            )
         if charges_flag and (
             config.coulombtype == "PIC_Spectral"
             or config.coulombtype == "PIC_Spectral_GPE"
         ):
             velocities = integrate_velocity(
                 velocities,
                 elec_forces / config.mass,
@@ -1038,30 +1156,22 @@
         if protein_flag and not args.disable_dipole:
             velocities = integrate_velocity(
                 velocities,
                 reconstructed_forces / config.mass,
                 config.respa_inner * config.time_step,
             )
 
-        # Only compute and keep the molecular bond energy from the last rRESPA
-        # inner step
-        if molecules_flag:
-            if not args.disable_bonds:
-                bond_energy = comm.allreduce(bond_energy_, MPI.SUM)
-            if not args.disable_angle_bonds:
-                angle_energy = comm.allreduce(angle_energy_, MPI.SUM)
-            if not args.disable_dihedrals:
-                dihedral_energy = comm.allreduce(dihedral_energy_, MPI.SUM)
-
         if config.domain_decomposition:
             if np.mod(step, config.domain_decomposition) == 0:
                 positions = np.ascontiguousarray(positions)
                 bond_forces = np.ascontiguousarray(bond_forces)
                 angle_forces = np.ascontiguousarray(angle_forces)
                 dihedral_forces = np.ascontiguousarray(dihedral_forces)
+                if args.plumed:
+                    plumed_forces = np.ascontiguousarray(plumed_forces)
 
                 (
                     positions,
                     velocities,
                     indices,
                     bond_forces,
                     angle_forces,
@@ -1082,14 +1192,16 @@
                 )
 
                 if charges_flag:
                     charges = optional.pop(0)
                     elec_forces = optional.pop(0)
                 if dielectric_flag:
                     dielectric_sorted = optional.pop(0)
+                if args.plumed:
+                    plumed_forces = optional.pop(0)
                 if molecules_flag:
                     bonds = optional.pop(0)
                     molecules = optional.pop(0)
 
                 # rebuild args_in to point to correct arrays
                 args_in = [
                     velocities,
@@ -1104,14 +1216,16 @@
                 ]
 
                 if charges_flag:
                     args_in.append(charges)
                     args_in.append(elec_forces)
                 if dielectric_flag:
                     args_in.append(dielectric_sorted)
+                if args.plumed:
+                    args_in.append(plumed_forces)
 
                 positions = np.asfortranarray(positions)
                 bond_forces = np.asfortranarray(bond_forces)
                 angle_forces = np.asfortranarray(angle_forces)
                 dihedral_forces = np.asfortranarray(dihedral_forces)
 
                 layouts = [
@@ -1281,14 +1395,16 @@
                     + bond_forces
                     + angle_forces
                     + dihedral_forces
                     + reconstructed_forces
                 )
                 if charges_flag:
                     forces_out += elec_forces
+                if args.plumed:
+                    forces_out += plumed_forces
                 store_data(
                     out_dataset,
                     step,
                     frame,
                     indices,
                     positions,
                     velocities,
@@ -1298,19 +1414,21 @@
                     pressure,
                     kinetic_energy,
                     bond_energy,
                     angle_energy,
                     dihedral_energy,
                     field_energy,
                     field_q_energy,
+                    plumed_bias,
                     config.respa_inner * config.time_step,
                     config,
                     velocity_out=args.velocity_output,
                     force_out=args.force_output,
                     charge_out=charges_flag,
+                    plumed_out=True if args.plumed else False,
                     dump_per_particle=args.dump_per_particle,
                     comm=comm,
                 )
                 if np.mod(step, config.n_print * config.n_flush) == 0:
                     out_dataset.flush()
         last_step_time = current_step_time
 
@@ -1454,14 +1572,16 @@
             + bond_forces
             + angle_forces
             + dihedral_forces
             + reconstructed_forces
         )
         if charges_flag:
             forces_out += elec_forces
+        if args.plumed:
+            forces_out += plumed_forces
         store_data(
             out_dataset,
             step,
             frame,
             indices,
             positions,
             velocities,
@@ -1471,17 +1591,21 @@
             pressure,
             kinetic_energy,
             bond_energy,
             angle_energy,
             dihedral_energy,
             field_energy,
             field_q_energy,
+            plumed_bias,
             config.respa_inner * config.time_step,
             config,
             velocity_out=args.velocity_output,
             force_out=args.force_output,
             charge_out=charges_flag,
+            plumed_out=True if args.plumed else False,
             dump_per_particle=args.dump_per_particle,
             comm=comm,
         )
 
     out_dataset.close_file()
+    if args.plumed:
+        plumed.finalize()
```

### Comparing `hymd-2.0.2/hymd/pressure.py` & `hymd-2.1.0/hymd/pressure.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd/thermostat.py` & `hymd-2.1.0/hymd/thermostat.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/hymd.egg-info/PKG-INFO` & `hymd-2.1.0/hymd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hymd
-Version: 2.0.2
+Version: 2.1.0
 Summary: Massively parallel hybrid particle-field MD
 Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum
 Author-email: morten.ledum@gmail.com
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hymd Version: 2.0.2 Summary: Massively parallel
+Metadata-Version: 2.1 Name: hymd Version: 2.1.0 Summary: Massively parallel
 hybrid particle-field MD Home-page: https://github.com/Cascella-Group-UiO/HyMD
 Author: Morten Ledum Author-email: morten.ledum@gmail.com License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Intended Audience :: Science/Research Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
```

### Comparing `hymd-2.0.2/hymd.egg-info/SOURCES.txt` & `hymd-2.1.0/hymd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 hymd/force.py
 hymd/gaussian_core.py
 hymd/hamiltonian.py
 hymd/input_parser.py
 hymd/integrator.py
 hymd/logger.py
 hymd/main.py
+hymd/plumed.py
 hymd/pressure.py
 hymd/thermostat.py
 hymd/version.py
 hymd.egg-info/PKG-INFO
 hymd.egg-info/SOURCES.txt
 hymd.egg-info/dependency_links.txt
 hymd.egg-info/requires.txt
@@ -37,8 +38,9 @@
 test/test_field.py
 test/test_file_io.py
 test/test_force.py
 test/test_hamiltonian.py
 test/test_input_parser.py
 test/test_integrator.py
 test/test_logger.py
+test/test_plumed.py
 test/test_thermostat.py
```

### Comparing `hymd-2.0.2/setup.py` & `hymd-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_distribute_input.py` & `hymd-2.1.0/test/test_distribute_input.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_field.py` & `hymd-2.1.0/test/test_field.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_file_io.py` & `hymd-2.1.0/test/test_file_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,26 +159,27 @@
         bonds_4_atom1, bonds_4_atom2, bonds_4_atom3, bonds_4_atom4,
         bonds_4_coeff, bonds_4_type, bonds_4_last,
     ) = bonds_prep
 
 
     store_static(
         out, rank_range, names_, types_, indices_, config, bonds_2_atom1,
-        bonds_2_atom2, molecules=molecules_
+        bonds_2_atom2, molecules=molecules_, charges=True, plumed_out=True
     )
 
     groups = ['connectivity', 'h5md', 'observables', 'parameters', 'particles']
     assert all((k in out.file.keys()) for k in groups)
     groups = ['box', 'mass', 'position', 'species']
     assert all((k in out.file['particles/all']) for k in groups)
     groups = [
         'angle_energy', 'angular_momentum', 'bond_energy', 
         'dihedral_energy', 'field_energy', 'kinetic_energy', 
         'potential_energy', 'temperature', 'thermostat_work', 
-        'torque', 'total_energy', 'total_momentum'
+        'torque', 'total_energy', 'total_momentum', 'field_q_energy',
+        'plumed_bias'
     ]
     assert all((k in out.file['observables']) for k in groups)
     assert 'vmd_structure' in out.file['parameters'].keys()
 
     out.close_file()
 
 
@@ -238,22 +239,23 @@
         bonds_4_coeff, bonds_4_type, bonds_4_last,
     ) = bonds_prep
 
 
     # call it to prepare OutDataset
     store_static(
         out, rank_range, names_, types_, indices_, config, bonds_2_atom1,
-        bonds_2_atom2, molecules=molecules_
+        bonds_2_atom2, molecules=molecules_, charges=True, plumed_out=True
     )
 
     forces = np.copy(positions_)
 
     store_data(
         out, 0, 0, indices_, positions_, velocities_, forces,
-        box_size, 300., 1., 1., 2., 3., 4., 5., 6., 0.02, config
+        box_size, 300., 1., 1., 2., 3., 4., 5., 6., 7., 0.02, config,
+        charge_out=True, plumed_out=True
     )
 
     outdataset_step = [
         out.positions_step,
         out.total_energy_step,
         out.potential_energy_step,
         out.kinetc_energy_step,
@@ -282,24 +284,25 @@
         out.torque_time,
         out.temperature_time,
         out.thermostat_work_time,
     ]
 
     for dset in outdataset_step:
         assert isinstance(dset, h5py.Dataset)
-        print(dset)
         assert dset[0] == 0
 
     for dset in outdataset_time:
         assert isinstance(dset, h5py.Dataset)
         assert dset[0] == 0
 
     assert out.potential_energy[0] == pytest.approx(20.)
     assert out.kinetc_energy[0] == pytest.approx(1.)
     assert out.temperature[0] == pytest.approx(300.)
     assert out.pressure[0] == pytest.approx(1.)
     assert out.bond_energy[0] == pytest.approx(2.)
     assert out.angle_energy[0] == pytest.approx(3.)
     assert out.dihedral_energy[0] == pytest.approx(4.)
     assert out.field_energy[0] == pytest.approx(5.)
+    assert out.field_q_energy[0] == pytest.approx(6.)
+    assert out.plumed_bias[0] == pytest.approx(7.)
 
     out.close_file()
```

### Comparing `hymd-2.0.2/test/test_force.py` & `hymd-2.1.0/test/test_force.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_hamiltonian.py` & `hymd-2.1.0/test/test_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_input_parser.py` & `hymd-2.1.0/test/test_input_parser.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_integrator.py` & `hymd-2.1.0/test/test_integrator.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_logger.py` & `hymd-2.1.0/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `hymd-2.0.2/test/test_thermostat.py` & `hymd-2.1.0/test/test_thermostat.py`

 * *Files identical despite different names*

