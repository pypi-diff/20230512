# Comparing `tmp/OptiPRISMS-1.0.5.tar.gz` & `tmp/OptiPRISMS-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OptiPRISMS-1.0.5.tar", last modified: Fri Feb 24 08:50:18 2023, max compression
+gzip compressed data, was "OptiPRISMS-1.1.0.tar", last modified: Fri May 12 14:44:14 2023, max compression
```

## Comparing `OptiPRISMS-1.0.5.tar` & `OptiPRISMS-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:50:18.992442 OptiPRISMS-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-02-24 08:50:18.992442 OptiPRISMS-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 08:50:18.992442 OptiPRISMS-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:50:18.992442 OptiPRISMS-1.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/CfgGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/ComputeCostFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 08:50:18.992442 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-02-24 08:50:18.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-24 08:50:18.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 08:50:18.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-24 08:50:18.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 08:50:18.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/OptiPRISMS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/costFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-02-24 08:50:06.000000 OptiPRISMS-1.0.5/src/vtk_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/CfgGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/ComputeCostFunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:14.652600 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 14:44:14.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/OptiPRISMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/costFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/misor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-12 14:44:03.000000 OptiPRISMS-1.1.0/src/vtk_utils.py
```

### Comparing `OptiPRISMS-1.0.5/LICENSE` & `OptiPRISMS-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.0.5/PKG-INFO` & `OptiPRISMS-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OptiPRISMS
-Version: 1.0.5
-Summary: Identifies Crystal Plasticity (CP) parameters by inverse analyis based on CPFEM simulations performed using PRISMS-Plasticity
+Version: 1.1.0
+Summary: Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity
 Home-page: https://github.com/DorianDepriester/OptiPRISMS
 Author: Dorian Depriester
 Author-email: dorian.depriester@ensam.eu
 License: GNU Lesser General Public License v2.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# OptiPRISMS
+# OptiPRISMS ![PyPI - Downloads](https://img.shields.io/pypi/dm/OptiPRISMS) [![PyPI](https://img.shields.io/pypi/v/OptiPRISMS)](https://pypi.org/project/OptiPRISMS/) ![GitHub](https://img.shields.io/github/license/DorianDepriester/OptiPRISMS)
 
 Perform inverse analysis to retrieve Crystal Plasticity parameters used for CPFEM simulation through the PRISMS-Plasticity software [[1]](#prisms). This inverse analysis is done using data from in situ tensile tests and Scanning Electron Microscopy Digital Image Correlation (SEM-DIC).
 
 ## How it works
 
 This program will optimize CP parameters in order to minimize a given cost function.
 At each step of the optimization process, it will:
@@ -40,18 +40,30 @@
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Installation
+You can install the latest release of OptiPRISMS with pip:
+```bash
+pip install OptiPRISMS
+```
+Otherwise, you can install the development version from sources:
+```bash
+git clone https://github.com/DorianDepriester/OptiPRISMS.git
+cd OptiPRISMS
+pip install --editable .
+```
+
 ## Step-by-step method to run optimization
 
 1. Create template files. They consist in usual configuration files (see [here](https://github.com/prisms-center/plasticity/blob/master/docs/PRISMS_plasticity_user_manual_V1_4_0.pdf) for details), where every value you want to optimize is given a variable name. These names must be precessed by a dollar symbol (``$``, e.g. ``$a`` instead of ``a``).
-2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder.
+2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder).
 3. With Python3, run the `optimize` function from `OptiPRISMS` module. E.g.:
 ```python
 from OptiPRISMS import optimize
 res = optimize(config_file='myConfigFile.ini')
 ```
 4. Then, wait a couple of days (or weeks...).
 
@@ -76,21 +88,23 @@
 
 - **prm file**: path to the main parameter file template
 - **latent hardening ratio** : path to latent hardening ratio template
 - **path to prisms**: path to PRISMS-Plasticity executable file. This entry is not required if Slurm is used (see [\[Slurm\]] section).
 
 #### [Experimental Data]
 
-- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). OptiPRISM will automatically 
-append the step number and the CSV extension to this pattern. For instance,
+- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). 
+OptiPRISMS will automatically append the step number and the CSV extension to this pattern. For instance,
 if one wants to use files ``DIC_1.csv`` and ``DIC_2.csv``, this parameter should be
 set to ``DIC_``.
+- **DIC time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. 
+If not set, they will be inferred from option `set Tabular Time Output Table` in prm file.
 - **tensile curve**: path to strain-stress values of tensile curve
-- **time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. If not set, they will 
-be inferred from option `set Tabular Time Output Table` in prm file.
+- **tensile direction** *(optional)*: Direction of measured stress and strain. It can be ``x`` or ``y``. 
+The default value is ``x``.  
 
 #### [Cost Function]
 
 - **weight on tensile curve**: weight to apply to the tensile curve in the overall cost function
 - **penalty**: penalty value to raise if the simulation fails
 - **weight by correlation coefficients**: if enabled, the kinematic cost function will weight the 
 displacement errors by the inverse of the correlation coefficients. The latter will
```

### Comparing `OptiPRISMS-1.0.5/README.md` & `OptiPRISMS-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OptiPRISMS
+# OptiPRISMS ![PyPI - Downloads](https://img.shields.io/pypi/dm/OptiPRISMS) [![PyPI](https://img.shields.io/pypi/v/OptiPRISMS)](https://pypi.org/project/OptiPRISMS/) ![GitHub](https://img.shields.io/github/license/DorianDepriester/OptiPRISMS)
 
 Perform inverse analysis to retrieve Crystal Plasticity parameters used for CPFEM simulation through the PRISMS-Plasticity software [[1]](#prisms). This inverse analysis is done using data from in situ tensile tests and Scanning Electron Microscopy Digital Image Correlation (SEM-DIC).
 
 ## How it works
 
 This program will optimize CP parameters in order to minimize a given cost function.
 At each step of the optimization process, it will:
@@ -29,18 +29,30 @@
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Installation
+You can install the latest release of OptiPRISMS with pip:
+```bash
+pip install OptiPRISMS
+```
+Otherwise, you can install the development version from sources:
+```bash
+git clone https://github.com/DorianDepriester/OptiPRISMS.git
+cd OptiPRISMS
+pip install --editable .
+```
+
 ## Step-by-step method to run optimization
 
 1. Create template files. They consist in usual configuration files (see [here](https://github.com/prisms-center/plasticity/blob/master/docs/PRISMS_plasticity_user_manual_V1_4_0.pdf) for details), where every value you want to optimize is given a variable name. These names must be precessed by a dollar symbol (``$``, e.g. ``$a`` instead of ``a``).
-2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder.
+2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder).
 3. With Python3, run the `optimize` function from `OptiPRISMS` module. E.g.:
 ```python
 from OptiPRISMS import optimize
 res = optimize(config_file='myConfigFile.ini')
 ```
 4. Then, wait a couple of days (or weeks...).
 
@@ -65,21 +77,23 @@
 
 - **prm file**: path to the main parameter file template
 - **latent hardening ratio** : path to latent hardening ratio template
 - **path to prisms**: path to PRISMS-Plasticity executable file. This entry is not required if Slurm is used (see [\[Slurm\]] section).
 
 #### [Experimental Data]
 
-- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). OptiPRISM will automatically 
-append the step number and the CSV extension to this pattern. For instance,
+- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). 
+OptiPRISMS will automatically append the step number and the CSV extension to this pattern. For instance,
 if one wants to use files ``DIC_1.csv`` and ``DIC_2.csv``, this parameter should be
 set to ``DIC_``.
+- **DIC time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. 
+If not set, they will be inferred from option `set Tabular Time Output Table` in prm file.
 - **tensile curve**: path to strain-stress values of tensile curve
-- **time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. If not set, they will 
-be inferred from option `set Tabular Time Output Table` in prm file.
+- **tensile direction** *(optional)*: Direction of measured stress and strain. It can be ``x`` or ``y``. 
+The default value is ``x``.  
 
 #### [Cost Function]
 
 - **weight on tensile curve**: weight to apply to the tensile curve in the overall cost function
 - **penalty**: penalty value to raise if the simulation fails
 - **weight by correlation coefficients**: if enabled, the kinematic cost function will weight the 
 displacement errors by the inverse of the correlation coefficients. The latter will
```

### Comparing `OptiPRISMS-1.0.5/setup.py` & `OptiPRISMS-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='OptiPRISMS',
-    version='1.0.5',
+    version='1.1.0',
     packages=[''],
     package_dir={'': 'src'},
     url='https://github.com/DorianDepriester/OptiPRISMS',
     license='GNU Lesser General Public License v2.1',
     author='Dorian Depriester',
     author_email='dorian.depriester@ensam.eu',
-    description='Identifies Crystal Plasticity (CP) parameters by inverse analyis based on CPFEM simulations performed using PRISMS-Plasticity',
+    description='Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'scipy',
         'numpy',
         'vtk',
         'pandas',
```

### Comparing `OptiPRISMS-1.0.5/src/CfgGenerator.py` & `OptiPRISMS-1.1.0/src/CfgGenerator.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.0.5/src/ComputeCostFunctions.py` & `OptiPRISMS-1.1.0/src/ComputeCostFunctions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import pandas as pd
 import configparser, itertools
 from costFunctions import kinematic_cost_function, static_cost_function, weighted_cost_function
 from triangulate import triangular_projection
 from vtk_utils import read_pvtu
 
 
 def unpack_str_list(list, dtype=float):
@@ -10,30 +11,30 @@
     
 
 def compute_kine_cost(result_folder, config):
     Expe_data = config['Experimental Data']
     cost_options = config['Cost Function']
     DIC_data = Expe_data['DIC data']
     
-    if config.has_option('Experimental Data', 'time steps'):
-        time_steps = unpack_str_list(Expe_data['time steps'], dtype=int)
+    if config.has_option('Experimental Data', 'DIC time steps'):
+        dic_time_steps = unpack_str_list(Expe_data['DIC time steps'], dtype=int)
     else:
         # Read time steps from prm file template
         prm_file = result_folder + ".prm"
         config_template = configparser.ConfigParser()
         with open(prm_file) as fp:
             config_template.read_file(itertools.chain(['[global]'], fp), source=prm_file)
         dt = float(config_template['global']['set Time increments'])
         output_table = unpack_str_list(config_template['global']['set Tabular Time Output Table'])
-        time_steps = np.array(output_table)/dt - 1
-        time_steps = time_steps.astype('int')
+        dic_time_steps = np.array(output_table)/dt - 1
+        dic_time_steps = dic_time_steps.astype('int')
 
     chi_u = 0
-    n_steps = len(time_steps)
-    for step, step_simu in enumerate(time_steps):
+    n_steps = len(dic_time_steps)
+    for step, step_simu in enumerate(dic_time_steps):
         pvtu_fname = "{}/solution-{:04}.pvtu".format(result_folder, step_simu)
         nodes, u_SIM = read_pvtu(pvtu_fname)
         if nodes is None:
             # It seems that the simulation has failed, raise penalty value
             chi_u = float(cost_options['penalty'])
             n_steps = 1
             break
@@ -57,28 +58,33 @@
                 C = None
             chi_u += kinematic_cost_function(u_SIM_tri, u_DIC[inside_mesh], weights=C)
 
     return chi_u/n_steps
 
 
 def compute_stat_cost(result_folder, config):
+    # Read data from experimental tensile curve
     tensileCurve = config['Experimental Data']['tensile curve']
+    Exper_curve = np.loadtxt(tensileCurve)
+    elon_expe = Exper_curve[:, 0]
+    stress_expe = Exper_curve[:, 1]
+
+    # Fetch simulated tensile curve
+    if config.has_option('Experimental Data', 'tensile direction'):
+        tensile_dir = config['Experimental Data']['tensile direction'].lower()
+    else:
+        tensile_dir = 'x'
+    col_E = 'E' + 2 * tensile_dir
+    col_sigma = 'T' + 2 * tensile_dir
     try:
-        stressstrain = np.loadtxt(result_folder + '/stressstrain.txt', skiprows=1)
-        
-        # PRISMS-Plasticity returns the Green-Lagrangian strain
-        Exx = stressstrain[:, 0]
-        eps_xx_simu = -1+np.sqrt(1+2*Exx)   # Compute elongation from Exx
-        Sxx_simu = stressstrain[:, 6]
-    
-        # Read data from experimental tensile curve
-        Exper_curve = np.loadtxt(tensileCurve)
-        eps_xx_expe = Exper_curve[:, 0]
-        Sxx_expe = Exper_curve[:, 1]
-        return static_cost_function(eps_xx_expe, Sxx_expe, eps_xx_simu, Sxx_simu)
+        stressstrain = pd.read_csv(result_folder + '/stressstrain.txt', sep='\t')
+        gl_eps = stressstrain[col_E]
+        elon_simu = -1 + np.sqrt(1 + 2 * gl_eps)  # Compute elongation from Green-Lagrangian strain
+        stress_simu = stressstrain[col_sigma]
+        return static_cost_function(elon_expe, stress_expe, elon_simu, stress_simu)
     except FileNotFoundError:
         return float(config['Cost Function']['penalty'])
 
 
 def compute_weighted_cost(result_folder, config):
     # Compute cost functions
     chi_u = compute_kine_cost(result_folder, config)
```

### Comparing `OptiPRISMS-1.0.5/src/OptiPRISMS.egg-info/PKG-INFO` & `OptiPRISMS-1.1.0/src/OptiPRISMS.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OptiPRISMS
-Version: 1.0.5
-Summary: Identifies Crystal Plasticity (CP) parameters by inverse analyis based on CPFEM simulations performed using PRISMS-Plasticity
+Version: 1.1.0
+Summary: Identifies Crystal Plasticity (CP) parameters by inverse analysis based on CPFEM simulations performed using PRISMS-Plasticity
 Home-page: https://github.com/DorianDepriester/OptiPRISMS
 Author: Dorian Depriester
 Author-email: dorian.depriester@ensam.eu
 License: GNU Lesser General Public License v2.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# OptiPRISMS
+# OptiPRISMS ![PyPI - Downloads](https://img.shields.io/pypi/dm/OptiPRISMS) [![PyPI](https://img.shields.io/pypi/v/OptiPRISMS)](https://pypi.org/project/OptiPRISMS/) ![GitHub](https://img.shields.io/github/license/DorianDepriester/OptiPRISMS)
 
 Perform inverse analysis to retrieve Crystal Plasticity parameters used for CPFEM simulation through the PRISMS-Plasticity software [[1]](#prisms). This inverse analysis is done using data from in situ tensile tests and Scanning Electron Microscopy Digital Image Correlation (SEM-DIC).
 
 ## How it works
 
 This program will optimize CP parameters in order to minimize a given cost function.
 At each step of the optimization process, it will:
@@ -40,18 +40,30 @@
 Each of these files must have tabular data, ordered this way:
 1. x coordinates of DIC points where DIC measurements are performed,
 2. y coordinates of DIC points where DIC measurements are performed,
 3. x displacements,
 4. y displacements,
 5. correlation coefficients (optional, see [Cost Function](#cost-function) section)
 
+## Installation
+You can install the latest release of OptiPRISMS with pip:
+```bash
+pip install OptiPRISMS
+```
+Otherwise, you can install the development version from sources:
+```bash
+git clone https://github.com/DorianDepriester/OptiPRISMS.git
+cd OptiPRISMS
+pip install --editable .
+```
+
 ## Step-by-step method to run optimization
 
 1. Create template files. They consist in usual configuration files (see [here](https://github.com/prisms-center/plasticity/blob/master/docs/PRISMS_plasticity_user_manual_V1_4_0.pdf) for details), where every value you want to optimize is given a variable name. These names must be precessed by a dollar symbol (``$``, e.g. ``$a`` instead of ``a``).
-2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder.
+2. Edit the configuration file to tune optimization-related parameters (see below for details or check out the [example](https://github.com/DorianDepriester/OptiPRISMS/tree/main/example) folder).
 3. With Python3, run the `optimize` function from `OptiPRISMS` module. E.g.:
 ```python
 from OptiPRISMS import optimize
 res = optimize(config_file='myConfigFile.ini')
 ```
 4. Then, wait a couple of days (or weeks...).
 
@@ -76,21 +88,23 @@
 
 - **prm file**: path to the main parameter file template
 - **latent hardening ratio** : path to latent hardening ratio template
 - **path to prisms**: path to PRISMS-Plasticity executable file. This entry is not required if Slurm is used (see [\[Slurm\]] section).
 
 #### [Experimental Data]
 
-- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). OptiPRISM will automatically 
-append the step number and the CSV extension to this pattern. For instance,
+- **DIC data**: pattern describing the path to CSV files with DIC measurements (without step number nor extension). 
+OptiPRISMS will automatically append the step number and the CSV extension to this pattern. For instance,
 if one wants to use files ``DIC_1.csv`` and ``DIC_2.csv``, this parameter should be
 set to ``DIC_``.
+- **DIC time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. 
+If not set, they will be inferred from option `set Tabular Time Output Table` in prm file.
 - **tensile curve**: path to strain-stress values of tensile curve
-- **time steps** *(optional)*: increment numbers corresponding to each step of DIC measurements. If not set, they will 
-be inferred from option `set Tabular Time Output Table` in prm file.
+- **tensile direction** *(optional)*: Direction of measured stress and strain. It can be ``x`` or ``y``. 
+The default value is ``x``.  
 
 #### [Cost Function]
 
 - **weight on tensile curve**: weight to apply to the tensile curve in the overall cost function
 - **penalty**: penalty value to raise if the simulation fails
 - **weight by correlation coefficients**: if enabled, the kinematic cost function will weight the 
 displacement errors by the inverse of the correlation coefficients. The latter will
```

### Comparing `OptiPRISMS-1.0.5/src/OptiPRISMS.py` & `OptiPRISMS-1.1.0/src/OptiPRISMS.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 
 import numpy as np
 import pandas as pd
 
 from CfgGenerator import CfgGenerator
 from ComputeCostFunctions import compute_weighted_cost, unpack_str_list
 
+file_dir = os.path.dirname(__file__)
+version = '1.1.0'
+
 
 def parse_optional_param(config, section):
     if config.has_section(section):
         options = dict(config[section])
         for key, value in options.items():
             if key in ['forward', 'verbose', 'loginfo', 'time']:
                 options[key] = config.getboolean(section, key)
@@ -47,14 +50,24 @@
         else:
             try:
                 shutil.rmtree(path)
             except OSError as e:
                 print("Error: %s - %s." % (e.filename, e.strerror))
 
 
+def print_separator():
+    print('-------------------------------------------------------')
+
+
+def print_title(title):
+    print_separator()
+    print(title)
+    print_separator()
+
+
 def optimize(config_file='Config.ini'):
     """
     Run optimization loops.
     
     Parameters
     ----------
     config_file : string, optional
@@ -66,14 +79,30 @@
         Results from optimization.
     """
 
     # Read optimizer options from config file
     config = configparser.ConfigParser()
     config.read(config_file)
 
+    # Print splash screen
+    relative_path = "splash.txt"
+    full_path = os.path.join(file_dir, relative_path)
+    with open(full_path, 'r') as f:
+        print(f.read())
+    print('Version {}'.format(version))
+
+    # Print optimization options
+    print('')
+    print_title('Optimization options read from {}:'.format(config_file))
+    for each_section in config.sections():
+        print('[ {} ]'.format(each_section))
+        for (each_key, each_val) in config.items(each_section):
+            print('{}:{}'.format(each_key, each_val))
+        print_separator()
+
     # Infer the number of investigated parameters from the initial guess
     x0 = np.array([float(i) for i in config['Initial Guess'].values()])
 
     # Load bounds and check consistency with the initial guess
     lb, ub = read_bounds(config)
     error_msg = 'The size of the {} bounds must be the same as the number of values in initial guess.'
     if len(lb) != len(x0):
@@ -95,15 +124,17 @@
         kwargs['parallel'] = parse_optional_param(config, 'Minimize parallel')
         module = importlib.import_module('optimparallel')
         minimizer = module.minimize_parallel
     else:
         module = importlib.import_module('scipy.optimize')
         minimizer = module.minimize
 
+    print('Launch optimization...')
     res = minimizer(run_and_compare, x0n, **kwargs)
+    print("...Done!")
 
     # Restore the optimized parameters into un-normalized form
     k = ub - lb
     inv = 1 / k
     res.x = lb + res.x * k
     res.jac = res.jac * inv
```

### Comparing `OptiPRISMS-1.0.5/src/costFunctions.py` & `OptiPRISMS-1.1.0/src/costFunctions.py`

 * *Files identical despite different names*

### Comparing `OptiPRISMS-1.0.5/src/vtk_utils.py` & `OptiPRISMS-1.1.0/src/vtk_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -100,9 +100,40 @@
     mesh_new.PointData.append(u_sim_tri, "U (FEM)")
     mesh_new.PointData.append(u_dic_tri, "U (DIC)")
     mesh_new.PointData.append(delta_u, "Displacement error")
     mesh_new.PointData.append(c_tri, "Correlation coefficient")
     writer = vtk.vtkXMLUnstructuredGridWriter()
     writer.SetFileName("Displacement_error_{}.vtu".format(step))
     writer.SetInputData(mesh_new.VTKObject)
-    writer.Write()    
+    writer.Write()
+
+
+def create_vtu_from_field(mesh_vtk, locations, field, output_filename, field_name='My field'):
+    # Read mesh file and get node coordinates
+    reader = vtk.vtkGenericDataObjectReader()
+    reader.SetFileName(mesh_vtk)
+    reader.Update()
+    mesh = reader.GetOutput()
+    mesh_new = dsa.WrapDataObject(mesh)
+    points_mesh = vtk_to_numpy(mesh_new.GetPoints())
+
+    # Only keep nodes at the surface of interest
+    on_surface = points_mesh[:, 2] == 0.
+    point_mesh_surf = points_mesh[on_surface, :2]
+
+    # The field will be NaN everywhere, except on the surface of interest
+    n_pts = len(points_mesh)
+    if len(field.shape) == 1:
+        field = field[:, np.newaxis]
+    ndim = field.shape[1]
+    new_field = np.ones(shape=(n_pts, ndim)) * np.nan
+
+    # Map the given field onto the mesh
+    new_field[on_surface, :], _ = triangular_projection(locations, field, point_mesh_surf)
+
+    # Save displacement fields in vtu file
+    mesh_new.PointData.append(new_field, field_name)
+    writer = vtk.vtkXMLUnstructuredGridWriter()
+    writer.SetFileName(output_filename)
+    writer.SetInputData(mesh_new.VTKObject)
+    writer.Write()
```

