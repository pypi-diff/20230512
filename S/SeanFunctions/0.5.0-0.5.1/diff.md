# Comparing `tmp/SeanFunctions-0.5.0.tar.gz` & `tmp/SeanFunctions-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.5.0.tar", last modified: Tue May  9 21:50:05 2023, max compression
+gzip compressed data, was "SeanFunctions-0.5.1.tar", last modified: Thu May 11 22:10:06 2023, max compression
```

## Comparing `SeanFunctions-0.5.0.tar` & `SeanFunctions-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.133871 SeanFunctions-0.5.0/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/.gitignore
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.5.0/LICENSE
--rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/MANIFEST.in
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-09 21:50:05.133551 SeanFunctions-0.5.0/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.5.0/README.md
--rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-05-09 21:38:49.000000 SeanFunctions-0.5.0/pyproject.toml
--rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-05-09 21:50:05.133926 SeanFunctions-0.5.0/setup.cfg
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.128271 SeanFunctions-0.5.0/src/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.131547 SeanFunctions-0.5.0/src/SeanFunctions/
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.133200 SeanFunctions-0.5.0/src/SeanFunctions/Data/
--rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.5.0/src/SeanFunctions/__init__.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     4717 2023-04-19 13:48:50.000000 SeanFunctions-0.5.0/src/SeanFunctions/fitting.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)     9393 2023-04-14 16:08:58.000000 SeanFunctions-0.5.0/src/SeanFunctions/math.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)    12866 2023-05-09 21:48:13.000000 SeanFunctions-0.5.0/src/SeanFunctions/scattering.py
--rw-r--r--   0 seanfayfar   (501) staff       (20)      196 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions/version.py
-drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-09 21:50:05.132357 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/
--rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/PKG-INFO
--rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/SOURCES.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/dependency_links.txt
--rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-05-09 21:50:05.000000 SeanFunctions-0.5.0/src/SeanFunctions.egg-info/top_level.txt
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-11 22:10:06.468370 SeanFunctions-0.5.1/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      251 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/.gitignore
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1067 2022-12-13 21:48:22.000000 SeanFunctions-0.5.1/LICENSE
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       36 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/MANIFEST.in
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-11 22:10:06.468029 SeanFunctions-0.5.1/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      137 2022-12-13 21:48:22.000000 SeanFunctions-0.5.1/README.md
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     1097 2023-05-11 19:46:06.000000 SeanFunctions-0.5.1/pyproject.toml
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       38 2023-05-11 22:10:06.468441 SeanFunctions-0.5.1/setup.cfg
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-11 22:10:06.463124 SeanFunctions-0.5.1/src/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-11 22:10:06.465839 SeanFunctions-0.5.1/src/SeanFunctions/
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-11 22:10:06.467589 SeanFunctions-0.5.1/src/SeanFunctions/Data/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    19607 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    14621 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    15253 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       39 2023-01-14 21:57:03.000000 SeanFunctions-0.5.1/src/SeanFunctions/__init__.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     4717 2023-04-19 13:48:50.000000 SeanFunctions-0.5.1/src/SeanFunctions/fitting.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)     9393 2023-04-14 16:08:58.000000 SeanFunctions-0.5.1/src/SeanFunctions/math.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)    13911 2023-05-11 22:09:58.000000 SeanFunctions-0.5.1/src/SeanFunctions/scattering.py
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      216 2023-05-11 22:10:06.000000 SeanFunctions-0.5.1/src/SeanFunctions/version.py
+drwxr-xr-x   0 seanfayfar   (501) staff       (20)        0 2023-05-11 22:10:06.466591 SeanFunctions-0.5.1/src/SeanFunctions.egg-info/
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      665 2023-05-11 22:10:06.000000 SeanFunctions-0.5.1/src/SeanFunctions.egg-info/PKG-INFO
+-rw-r--r--   0 seanfayfar   (501) staff       (20)      532 2023-05-11 22:10:06.000000 SeanFunctions-0.5.1/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)        1 2023-05-11 22:10:06.000000 SeanFunctions-0.5.1/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 seanfayfar   (501) staff       (20)       14 2023-05-11 22:10:06.000000 SeanFunctions-0.5.1/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.5.0/LICENSE` & `SeanFunctions-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/PKG-INFO` & `SeanFunctions-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.5.0
+Version: 0.5.1
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.5.0/pyproject.toml` & `SeanFunctions-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SeanFunctions"
-version = "0.5.0"
+version = "0.5.1"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.5.1/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.5.1/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.5.1/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/fitting.py` & `SeanFunctions-0.5.1/src/SeanFunctions/fitting.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/math.py` & `SeanFunctions-0.5.1/src/SeanFunctions/math.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions/scattering.py` & `SeanFunctions-0.5.1/src/SeanFunctions/scattering.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pandas as pd
 import numpy as np
 import re
 import mendeleev as pTable
 from scipy.interpolate import interp1d
+from scipy import constants
 from matplotlib import pyplot as plt
 from .math import find_nearest, fourierbesseltransform
 # from importlib import resources
 # import io
 
 
 def atomic_form_factor_constants():
@@ -119,15 +120,15 @@
                                         'Scatt xs':np.float64,
                                         'Abs xs':np.float64})
     return nsl_DF
 
 
 class weight_RDF_for_scattering:
     
-    def __init__(self,RDF_DataFrame,composition,cutoffR=None,isotopeDict=None):
+    def __init__(self,RDF_DataFrame,composition,cutoffR=None,isotopeDict=None,ionsDict=None):
         '''
         Converts molecular dynamics partial RDFs into weighted g(r) and S(Q) for neutron and X-ray scattering.
         The input RDF must be a Pandas DataFrame with the column names as the atomic pairs such as "F-F" or "Na-Cl".
 
         Parameters
         ---------
         RDF_DataFrame : DataFrame
@@ -143,14 +144,19 @@
 
         isotopeDict : dict, optional
                     Add the isotopes of each atom as a Python dictionary.
                     The dict must start with the atom then include isotopes.
                     The total must sum to 1.
                     Ex: {'Li':{'7Li':0.9,'6Li':0.1}}
 
+        ionsDict : dict, optional
+                Add the ionic charge for the form factors rather than 
+                the atomic form factors.
+                Ex: {'Li':'1+','Be':'2+','F':'1-'}
+
         Returns
         --------
         compositionTable : DataFrame
                         DateFrame containing the composition, b, and f(Q) values
 
         partialRDF : DataFrame
 
@@ -186,23 +192,28 @@
                         bValue += isotopeDict[atoms][isotope] * neutronScatteringLengths.loc[neutronScatteringLengths['Isotope'].str.fullmatch(isotope)]['Coh b'].values[0].real
                     bArr.append(bValue)
                 else:
                     bArr.append(neutronScatteringLengths.loc[neutronScatteringLengths['Isotope'].str.fullmatch(atoms)]['Coh b'].values[0].real)
         else:
             bArr = [neutronScatteringLengths.loc[neutronScatteringLengths['Isotope'].str.fullmatch(atomArr[i])]['Coh b'].values[0].real for i in range(len(atomArr))]
         
-        
         QArr, SofQ = fourierbesseltransform(RDF_DataFrame.iloc[:,0],RDF_DataFrame.iloc[:,1]-1,unpack=True)
         QArrInterp = np.linspace(QArr[0],QArr[-1],len(QArr)*10)
+
+        if ionsDict is not None:
+            affArr = [atomic_form_factor(atomArr[i]+ionsDict[atomArr[i]],QArrInterp) for i in range(len(atomArr))]
+        else:
+            affArr = [atomic_form_factor(atomArr[i],QArrInterp) for i in range(len(atomArr))]
+        
         
         self.compositionTable = pd.DataFrame({
                                         'conc':concArr/np.sum(concArr),
                                         'amu':[pTable.element(atomArr[i]).atomic_weight for i in range(len(atomArr))],
                                         'b':bArr,
-                                        'aff':[atomic_form_factor(atomArr[i],QArrInterp) for i in range(len(atomArr))]
+                                        'aff':affArr
                                                 },
                                             index=atomArr)
         
         # First Fourier transform the partial RDFs to partial SofQs
         totalUnweightedSofQ = 0
         self.unweightedSofQ = pd.DataFrame()
         # self.unweightedSofQ_nointerp = pd.DataFrame()
@@ -264,16 +275,17 @@
             totalSofQ += self.SofQXray[column]
         self.SofQXray['Total'] = totalSofQ
         
         # X-ray gofr
         self.gofrXray = pd.DataFrame()
         # self.gofrXray['r'] = RDF_DataFrame.iloc[:,0]
         totalgofr = 0
+        cutAt100InvAng = find_nearest(self.SofQXray['Q'],100)[0]
         for column in RDF_DataFrame.keys()[1:]:
-            r, gofr = fourierbesseltransform(self.SofQXray['Q'].iloc[::10].to_numpy(),self.SofQXray[column].iloc[::10].to_numpy(),unpack=True)
+            r, gofr = fourierbesseltransform(self.SofQXray['Q'].iloc[:cutAt100InvAng:10].to_numpy(),self.SofQXray[column].iloc[:cutAt100InvAng:10].to_numpy(),unpack=True)
             self.gofrXray['r'] = r
             self.gofrXray[column] = gofr * 2 / np.pi
             totalgofr += gofr * 2 / np.pi
         self.gofrXray['Total'] = totalgofr
         
         
         
@@ -299,8 +311,25 @@
         return ax
     
     def plot_gofrXray(self,axes=None,**kwargs):
         ax = plt.axes(axes)
         ax.plot(self.gofrXray['r'],self.gofrXray['Total'],'k-',lw=2,label='Total',**kwargs)
         for column in self.gofrXray.keys()[1:-1]:
             ax.plot(self.gofrXray['r'],self.gofrXray[column],'-',lw=1,label=column,**kwargs)
-        return ax
+        return ax
+    
+    def calc_num_density(self,density):
+        '''
+        Calculates the number density (in num per Ang^3) using the 
+        chemical formula and input density.
+
+        Inputs
+        ------
+        density : float
+                The density of the material at the desired temperature.
+
+        Returns
+        -------
+        num_density : float
+        '''
+        num_density = constants.Avogadro/10**24 * density / np.sum([self.compositionTable.conc * self.compositionTable.amu])
+        return num_density
```

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions.egg-info/PKG-INFO` & `SeanFunctions-0.5.1/src/SeanFunctions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeanFunctions
-Version: 0.5.0
+Version: 0.5.1
 Summary: Collection of useful python functions
 Author-email: Sean Fayfar <sfayfar@gmail.com>
 Project-URL: Homepage, https://github.mit.edu/sfayfar/SeanFunctions
 Project-URL: Bug Tracker, https://github.mit.edu/sfayfar/SeanFunctions/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SeanFunctions-0.5.0/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.5.1/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

