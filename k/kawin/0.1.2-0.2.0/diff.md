# Comparing `tmp/kawin-0.1.2.tar.gz` & `tmp/kawin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nury\Desktop\Projects\Precipitation Model\KWN-Precipitation MGI\dist\tmp8x4im5cd\kawin-0.1.2.tar", last modified: Wed Jun  1 14:41:44 2022, max compression
+gzip compressed data, was "kawin-0.2.0.tar", last modified: Fri May 12 03:08:57 2023, max compression
```

## Comparing `kawin-0.1.2.tar` & `kawin-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxrwx   0        0        0        0 2022-06-01 14:41:44.000000 kawin-0.1.2/
--rw-rw-rw-   0        0        0      265 2022-03-30 18:31:13.000000 kawin-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1251 2021-09-15 17:54:41.000000 kawin-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       52 2021-07-28 23:53:48.000000 kawin-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1325 2022-06-01 14:41:44.000000 kawin-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      501 2021-12-08 01:28:53.000000 kawin-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin/
--rw-rw-rw-   0        0        0     4880 2022-02-07 18:16:58.000000 kawin-0.1.2/kawin/EffectiveDiffusion.py
--rw-rw-rw-   0        0        0    26994 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/ElasticFactors.py
--rw-rw-rw-   0        0        0     7543 2021-09-23 20:33:56.000000 kawin-0.1.2/kawin/FreeEnergyHessian.py
--rw-rw-rw-   0        0        0     6858 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/GrainBoundaries.py
--rw-rw-rw-   0        0        0    71809 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/KWNBase.py
--rw-rw-rw-   0        0        0    45824 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/KWNEuler.py
--rw-rw-rw-   0        0        0    37390 2021-12-08 00:49:56.000000 kawin-0.1.2/kawin/LebedevNodes.py
--rw-rw-rw-   0        0        0     2644 2022-06-01 14:37:46.000000 kawin-0.1.2/kawin/LocalEquilibrium.py
--rw-rw-rw-   0        0        0    16600 2022-05-02 17:22:54.000000 kawin-0.1.2/kawin/Mobility.py
--rw-rw-rw-   0        0        0    25236 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/PopulationBalance.py
--rw-rw-rw-   0        0        0    13542 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/ShapeFactors.py
--rw-rw-rw-   0        0        0    67074 2022-02-07 18:16:58.000000 kawin-0.1.2/kawin/Surrogate.py
--rw-rw-rw-   0        0        0    70732 2022-06-01 14:19:22.000000 kawin-0.1.2/kawin/Thermodynamics.py
--rw-rw-rw-   0        0        0        0 2021-12-02 18:43:51.000000 kawin-0.1.2/kawin/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin/tests/
--rw-rw-rw-   0        0        0    51225 2021-11-12 18:59:45.000000 kawin-0.1.2/kawin/tests/datasets.py
--rw-rw-rw-   0        0        0     4185 2022-02-07 18:16:58.000000 kawin-0.1.2/kawin/tests/test_PBM.py
--rw-rw-rw-   0        0        0     7503 2021-11-09 21:44:02.000000 kawin-0.1.2/kawin/tests/test_extraFactors.py
--rw-rw-rw-   0        0        0    11006 2021-11-02 23:47:07.000000 kawin-0.1.2/kawin/tests/test_surrogate.py
--rw-rw-rw-   0        0        0    10536 2021-10-22 15:53:12.000000 kawin-0.1.2/kawin/tests/test_thermodynamics.py
-drwxrwxrwx   0        0        0        0 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/
--rw-rw-rw-   0        0        0     1325 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-06-01 14:41:44.000000 kawin-0.1.2/kawin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2021-08-04 00:31:08.000000 kawin-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-01 14:41:44.000000 kawin-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1602 2022-06-01 14:40:22.000000 kawin-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.980107 kawin-0.2.0/
+-rw-rw-rw-   0        0        0     1251 2022-08-31 21:05:28.000000 kawin-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       52 2022-08-31 21:05:28.000000 kawin-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1325 2023-05-12 03:08:57.979106 kawin-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2022-08-31 21:05:28.000000 kawin-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.937760 kawin-0.2.0/kawin/
+-rw-rw-rw-   0        0        0    35058 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Diffusion.py
+-rw-rw-rw-   0        0        0     4924 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/EffectiveDiffusion.py
+-rw-rw-rw-   0        0        0    35769 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/ElasticFactors.py
+-rw-rw-rw-   0        0        0     7543 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/FreeEnergyHessian.py
+-rw-rw-rw-   0        0        0     6858 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/GrainBoundaries.py
+-rw-rw-rw-   0        0        0    75858 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/KWNBase.py
+-rw-rw-rw-   0        0        0    52739 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/KWNEuler.py
+-rw-rw-rw-   0        0        0    37701 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/LebedevNodes.py
+-rw-rw-rw-   0        0        0     2644 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/LocalEquilibrium.py
+-rw-rw-rw-   0        0        0    17421 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Mobility.py
+-rw-rw-rw-   0        0        0    25704 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/PopulationBalance.py
+-rw-rw-rw-   0        0        0    13586 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/ShapeFactors.py
+-rw-rw-rw-   0        0        0    39544 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Strength.py
+-rw-rw-rw-   0        0        0    67348 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Surrogate.py
+-rw-rw-rw-   0        0        0    78335 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/Thermodynamics.py
+-rw-rw-rw-   0        0        0        0 2023-05-05 03:15:13.000000 kawin-0.2.0/kawin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.978107 kawin-0.2.0/kawin/tests/
+-rw-rw-rw-   0        0        0    71718 2022-11-02 19:07:56.000000 kawin-0.2.0/kawin/tests/datasets.py
+-rw-rw-rw-   0        0        0     4217 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_PBM.py
+-rw-rw-rw-   0        0        0     9266 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_diffusion.py
+-rw-rw-rw-   0        0        0     7503 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_extraFactors.py
+-rw-rw-rw-   0        0        0     8101 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_strength.py
+-rw-rw-rw-   0        0        0    11110 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_surrogate.py
+-rw-rw-rw-   0        0        0    14488 2023-05-12 03:03:30.000000 kawin-0.2.0/kawin/tests/test_thermodynamics.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:08:57.967637 kawin-0.2.0/kawin.egg-info/
+-rw-rw-rw-   0        0        0     1325 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      758 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 03:08:57.000000 kawin-0.2.0/kawin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2022-08-31 21:05:28.000000 kawin-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 03:08:57.980107 kawin-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1602 2022-11-02 19:07:56.000000 kawin-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kawin-0.1.2/LICENSE.txt` & `kawin-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kawin-0.1.2/PKG-INFO` & `kawin-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kawin
-Version: 0.1.2
+Version: 0.2.0
 Summary: Tool for simulating precipitation using the KWN model coupled with Calphad.
 Home-page: https://kawin.org/
 Author: Nicholas Ury
 Author-email: nury12n@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kawin-0.1.2/kawin/EffectiveDiffusion.py` & `kawin-0.2.0/kawin/EffectiveDiffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,21 +47,25 @@
         Returns
         -------
         Effective diffusion distance (eps) to be used as (eps*R) in the growth rate equation
         '''
         return np.interp(supersaturation, self.ohmInterp, self.effDiffInterp)
 
     def lambdaLow(self, supersaturation):
-        # Lambda when Q approaches 0
-        # This is done to prevent precision errors when multiplying exp*(1-erf)
+        '''
+        Lambda when Q approaches 0
+        This is done to prevent precision errors when multiplying exp*(1-erf)
+        '''
         return np.sqrt(supersaturation / 2)
 
     def lambdaHigh(self, supersaturation):
-        # Lambda when Q approaches 1
-        # This is done to prevent precision errors when multiplying exp*(1-erf)
+        '''
+        Lambda when Q approaches 1
+        This is done to prevent precision errors when multiplying exp*(1-erf)
+        '''
         return np.sqrt(3 / (2 * (1 - supersaturation)))
 
     def effectiveDiffusionDistanceApprox(self, supersaturation):
         '''
         Effective diffusion distance given supersaturation
         This gives a constant to be multiplied by the particle radius
```

### Comparing `kawin-0.1.2/kawin/ElasticFactors.py` & `kawin-0.2.0/kawin/ElasticFactors.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import itertools
 import matplotlib.pyplot as plt
 from kawin.LebedevNodes import loadPoints
+import copy
 
 class StrainEnergy:
     '''
     Defines class for calculating strain energy of a precipitate
 
     Ellipsoidal precipitates will use the Eshelby's tensor
     Spherical and Cuboidal precipitates will use the Khachaturyan's approximation
@@ -15,30 +16,34 @@
     ELLIPSE = 1
     CUBE = 2
     CONSTANT = 3
 
     def __init__(self):
         self.c = None
         self._c4 = np.zeros((3,3,3,3))
+        self.cPrec = None
+        self._c4Prec = np.zeros((3,3,3,3))
         self.eigstrain = np.zeros((3,3))
         self.appstress = np.zeros((3,3))
         self.appstrain = np.zeros((3,3))
         self.rotation = None
+        self.rotationPrec = None
 
         self.lebedevIntegration('high')
 
         self._strainEnergyGeneric = self._strainEnergyConstant
         self.type = self.CONSTANT
         self.r = np.zeros(3)
         self.oldr = np.zeros(3)
         self._prevEnergy = 0
 
         self._gElasticConstant = 0
 
         #Cached values for calculating equilibrium aspect ratio
+        self.ifmethod = 1
         self._aspectRatios = None
         self._normEnergies = None
         self._cachedRange = 5
         self._cachedIntervals = 100
 
     def setAspectRatioResolution(self, resolution = 0.01, cachedRange = 5):
         '''
@@ -49,21 +54,36 @@
 
         If aspect ratio does not vary much in a given system, then the default parameters may lead to poor
         prediction of the aspect ratios
 
         Parameters
         ----------
         resolution : float (optional)
-            Minimum distance between aspect ratios when calculating cache
+            Minimum distance between aspect ratios when calculating cache (default at 0.01)
         cachedRange : float (optional)
-            Range of aspect ratio to calculate strain energy when updated cache
+            Range of aspect ratio to calculate strain energy when updated cache (default at 5)
         '''
         self._cachedRange = cachedRange
         self._cachedIntervals = int(1 / resolution)
 
+    def setInterfacialEnergyMethod(self, method):
+        '''
+        Sets method for calculating interfacial energy as a function of aspect ratio
+
+        Parameters
+        ----------
+        method : str
+            'eqradius' - interfacial energy is determined using the equivalent spherical radius
+            'thermo' - interfacial energy is determined using dG/dSA (default)
+        '''
+        if method == 'eqradius':
+            self.ifmethod = 0
+        else:
+            self.ifmethod = 1
+
     def setSpherical(self):
         '''
         Assumes spherical geometry for strain energy calculation
         Uses Khachaturyan's approximation
         '''
         self._strainEnergyGeneric = self._strainEnergySphere
         self.type = self.SPHERE
@@ -78,14 +98,15 @@
 
     def setEllipsoidal(self):
         '''
         Assumes ellipsoidal geometry for strain energy calculation
         Uses Eshelby's tensor
         '''
         self._strainEnergyGeneric = self._strainEnergyEllipsoid
+        self._strainEnergyGeneric = self._strainEnergyBohm
         self.type = self.ELLIPSE
 
     def setConstantElasticEnergy(self, energy):
         '''
         If elastic strain energy is known to be a constant, this can be use to greatly
         simplify calculations
 
@@ -95,41 +116,146 @@
         '''
         self._gElasticConstant = energy
         self._strainEnergyGeneric = self._strainEnergyConstant
         self.type = self.CONSTANT
 
     def setElasticTensor(self, tensor):
         '''
+        Sets elastic tensor of matrix using 2nd rank tensor
+
+        Parameters
+        ----------
+        tensor : 6x6 array
+            2nd rank elastic tensor
+        '''
+        self.c = self._setElasticTensor(tensor)
+        self._c4 = self._convert2To4rankTensor(self.c)
+
+    def setElasticConstants(self, c11, c12, c44):
+        '''
+        Sets elastic tensor of matrix by elastic constants, assuming cubic symmetry
+
+        Parameters
+        ----------
+        c11 : float
+            Modulus for compression
+            c11 = E(1-nu) / (1+nu)(1-2nu)
+        c12 : float
+            Modulus for dilation (accounts for compression and Poisson's ratio)
+            c12 = E nu / (1+nu)(1-2nu)
+        c44 : float
+            Modulus for shear
+            c44 = (c11-c12)/2
+        '''
+        self.c = self._setElasticConstants(c11, c12, c44)
+        self._c4 = self._convert2To4rankTensor(self.c)
+
+    def setModuli(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
+        '''
+        Sets elastic tensor of matrix by 2 moduli
+
+        Parameters (only 2 has to be defined)
+        ----------
+        E : float
+            Elastic modulus
+        nu : float
+            Poisson's ratio
+        G : float
+            Shear modulus
+        lam : float
+            Lame's first parameter
+        K : float
+            Bulk modulus
+        M : float
+            P-wave modulus
+        '''
+        self.c = self._setModuli(E, nu, G, lam, K, M)
+        self._c4 = self._convert2To4rankTensor(self.c)
+
+    def setElasticTensorPrecipitate(self, tensor):
+        '''
+        Sets elastic tensor of precipitate using 2nd rank tensor
+
+        Parameters
+        ----------
+        tensor : 6x6 array
+            2nd rank elastic tensor
+        '''
+        self.cPrec = self._setElasticTensor(tensor)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
+
+    def setElasticConsantsPrecipitate(self, c11, c12, c44):
+        '''
+        Sets elastic tensor of precipitate by elastic constants, assuming cubic symmetry
+
+        Parameters
+        ----------
+        c11 : float
+            Modulus for compression
+            c11 = E(1-nu) / (1+nu)(1-2nu)
+        c12 : float
+            Modulus for dilation (accounts for compression and Poisson's ratio)
+            c12 = E nu / (1+nu)(1-2nu)
+        c44 : float
+            Modulus for shear
+            c44 = (c11-c12)/2
+        '''
+        self.cPrec = self._setElasticConstants(c11, c12, c44)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
+    
+    def setModuliPrecipitate(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
+        '''
+        Sets elastic tensor of precipitate by 2 moduli
+
+        Parameters (only 2 has to be defined)
+        ----------
+        E : float
+            Elastic modulus
+        nu : float
+            Poisson's ratio
+        G : float
+            Shear modulus
+        lam : float
+            Lame's first parameter
+        K : float
+            Bulk modulus
+        M : float
+            P-wave modulus
+        '''
+        self.cPrec = self._setModuli(E, nu, G, lam, K, M)
+        self._c4Prec = self._convert2To4rankTensor(self.cPrec)
+
+    def _setElasticTensor(self, tensor):
+        '''
         Inputs 6x6 elastic matrix
 
         Parameters
         ----------
         tensor : matrix of floats
             Must be 6x6
         '''
-        self.c = np.array(tensor)
-        self._setupElasticTensor()
+        return np.array(tensor)
 
-    def setElasticConstants(self, c11, c12, c44):
+    def _setElasticConstants(self, c11, c12, c44):
         '''
         Creates elastic tensor from c11, c12 and c44 constants assuming isotropic system
 
         Parameters
         ----------
         c11 : float
         c12 : float
         c44 : float
         '''
-        self.c = np.zeros((6, 6))
-        self.c[0,0], self.c[1,1], self.c[2,2] = c11, c11, c11
-        self.c[0,1], self.c[0,2], self.c[1,0], self.c[1,2], self.c[2,0], self.c[2,1] = c12, c12, c12, c12, c12, c12
-        self.c[3,3], self.c[4,4], self.c[5,5] = c44, c44, c44
-        self._setupElasticTensor()
+        c = np.zeros((6, 6))
+        c[0,0], c[1,1], c[2,2] = c11, c11, c11
+        c[0,1], c[0,2], c[1,0], c[1,2], c[2,0], c[2,1] = c12, c12, c12, c12, c12, c12
+        c[3,3], c[4,4], c[5,5] = c44, c44, c44
+        return c
 
-    def setModuli(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
+    def _setModuli(self, E = None, nu = None, G = None, lam = None, K = None, M = None):
         '''
         Set elastic tensor by defining at least two of the moduli
         Everything will be converted to E, nu and G
         If more than two parameters are defined, then the following priority will be used:
         E - Youngs modulus
         nu - Poisson's ratio
         G - shear modulus
@@ -192,44 +318,15 @@
                 G = 3*(M - K) / 4
                 nu = (3*K - M) / (3*K + M)
 
         s = np.zeros((6,6))
         s[0,0], s[1,1], s[2,2] = 1/E, 1/E, 1/E
         s[3,3], s[4,4], s[5,5] = 1/G, 1/G, 1/G
         s[0,1], s[0,2], s[1,0], s[1,2], s[2,0], s[2,1] = -nu/E, -nu/E, -nu/E, -nu/E, -nu/E, -nu/E
-        self.c = np.linalg.inv(s)
-
-        self._setupElasticTensor()
-
-    def _setupElasticTensor(self):
-        '''
-        Creates the 4th rank elastic tensor
-        This makes it easer to use np.tensordot for most calculations
-
-        This will also automatically calculate applied strain, in case the applied stress is
-        given before the elastic constants are
-        '''
-        vMap = {frozenset({0}): 0, frozenset({1}): 1, frozenset({2}): 2,
-                frozenset({1,2}): 3, frozenset({0,2}): 4, frozenset({0,1}): 5}
-
-        self._c4 = np.zeros((3,3,3,3))
-        for i, j, k, l in itertools.product(range(3), range(3), range(3), range(3)):
-            self._c4[i,j,k,l] = self.c[vMap[frozenset({i,j})], vMap[frozenset({k,l})]]
-
-        self.getAppliedStrain()
-
-        #Set type to something other than CONSTANT
-        #Since CONSTANT is the only method not requiring the elastic tensor,
-        #    we assume that the user is intending to calculate strain energy when inputting the tensor
-        if self.type == self.CONSTANT:
-            self.type = self.SPHERE
-
-        if self.rotation is not None:
-            self.appstrain = self._rotateRank2Tensor(self.appstrain)
-            self._c4 = self._rotateRank4Tensor(self._c4)
+        return np.linalg.inv(s)
 
     def setRotationMatrix(self, rot):
         '''
         Sets rotation matrix to be applied to the matrix
 
         This is for cases where the axes of the precipitate does not align with the axes of the matrix
         (e.g., the long/short axes of the precipitate is not parallel to the <100> directions of the matrix)
@@ -237,44 +334,16 @@
         Parameters
         ----------
         rot : matrix
             3x3 rotation matrix
         '''
         self.rotation = np.array(rot)
 
-        if self.c is not None:
-            self._c4 = self._rotateRank4Tensor(self._c4)
-
-    def _rotateRank2Tensor(self, tensor):
-        '''
-        Rotates a 2nd rank tensor
-        T_ij = r_il * r_jk * T_lk
-
-        Parameters
-        ----------
-        tensor : ndarray
-            2nd rank tensor to rotate (3x3 array)
-        '''
-        return np.tensordot(self.rotation,
-                np.tensordot(self.rotation, tensor, axes=(1,1)), axes=(1,1))
-
-    def _rotateRank4Tensor(self, tensor):
-        '''
-        Rotates a 4th rank tensor
-        T_ijkl = r_im * r_jn * r_ok * r_lp * T_mnop
-
-        Parameters
-        ----------
-        tensor : ndarray
-            4th rank tensor to rotate (3x3x3x3 array)
-        '''
-        return np.tensordot(self.rotation, 
-                np.tensordot(self.rotation, 
-                np.tensordot(self.rotation, 
-                np.tensordot(self.rotation, tensor, axes=(1,3)), axes=(1,3)), axes=(1,3)), axes=(1,3))
+    def setRotationPrecipitate(self, rot):
+        self.rotationPrec = np.array(rot)
 
     def setEigenstrain(self, strain):
         '''
         Sets eigenstrain of precipitate
 
         Parameters
         ----------
@@ -297,14 +366,15 @@
         #Else, assume it's a tensor
         else:
             self.eigstrain = strain
 
     def setAppliedStress(self, stress):
         '''
         Sets applied stress tensor
+        Axes of stress tensor should be the same as the matrix
 
         Parameters
         ----------
         stress : float, array or matrix
             float - assume stress is the same along all 3 axis
             array - each index corresponds to stress in a given axis
             matrix - full 2nd rank stress tensor
@@ -325,30 +395,167 @@
         #If array of length 3, then apply stress along each index to corresponding axis
         elif stress.ndim == 1:
             self.appstress = np.array([[stress[0], 0, 0], [0, stress[1], 0], [0, 0, stress[2]]])
         #Else, assume it's a tensor
         else:
             self.appstress = stress
 
-        if self.c is not None:
-            self.getAppliedStrain()
-
     def getAppliedStrain(self):
         '''
         Calculates applied strain tensor from applied stress tensor and elastic tensor
         '''
-        flatStress = np.array([self.appstress[0,0], self.appstress[1,1], self.appstress[2,2], \
-                                self.appstress[1,2], self.appstress[0,2], self.appstress[0,1]])
+        flatStress = self._convert2rankToVec(self.appstress)
         flatStrain = np.matmul(np.linalg.inv(self.c), flatStress)
-        self.appstrain = np.array([[flatStrain[0], flatStrain[5], flatStrain[4]], \
-                                    [flatStrain[5], flatStrain[1], flatStrain[3]], \
-                                    [flatStrain[3], flatStrain[4], flatStrain[2]]])
+        self.appstrain = self._convertVecTo2rankTensor(flatStrain)
 
-        if self.rotation is not None:
-            self.appstrain = self._rotateRank2Tensor(self.appstrain)
+    def setup(self):
+        '''
+        Sets up elastic constants
+        '''
+        #If no elastic tensor is given, then elastic energy will be constant at 0
+        if self.c is not None:
+            #Apply rotation on matrix phase if there is one
+            #Since applied stress tensor is aligned with matrix, rotate it too since calculations will be in reference to precipitate axes
+            if self.rotation is not None:
+                self._c4 = self._rotateRank4Tensor(self.rotation, self._c4)
+                self.c = self._convert4To2rankTensor(self._c4)
+                self.appstress = self._rotateRank2Tensor(self.rotation, self.appstress)
+
+            #If elastic constants for precipitate are not given, then assume they're the same as the matrix
+            #This will give the elastic energy equation from Wu et al, Journal of Phase Equilibria and Diffusion, 39, 2018
+            #Using a different elastic tensor for the precipitate will give energy from Bohm et al, Mechanics of Materials, 155, 2021
+            if self.cPrec is None:
+                self.cPrec = copy.copy(self.c)
+                self._c4Prec = copy.copy(self._c4)
+
+            if self.rotationPrec is not None:
+                self._c4Prec = self._rotateRank4Tensor(self.rotationPrec, self._c4Prec)
+                self.cPrec = self._convert4To2rankTensor(self._c4Prec)
+
+            self.getAppliedStrain()
+
+            #Set type to something other than CONSTANT
+            #Since CONSTANT is the only method not requiring the elastic tensor,
+            #    we assume that the user is intending to calculate strain energy when inputting the tensor
+            if self.type == self.CONSTANT:
+                self.type = self.SPHERE
+
+    #Utility functions for tensors
+    def _convert2To4rankTensor(self, c):
+        '''
+        Converts 2nd rank elastic tensor to 4th rank
+
+        Parameters
+        ----------
+        c : ndarray
+            2nd rank elastic tensor
+
+        Returns
+        -------
+        c4 : ndarray
+            4th rank elastic tensor
+        '''
+        vMap = {frozenset({0}): 0, frozenset({1}): 1, frozenset({2}): 2,
+                frozenset({1,2}): 3, frozenset({0,2}): 4, frozenset({0,1}): 5}
+
+        c4 = np.zeros((3,3,3,3))
+        for i, j, k, l in itertools.product(range(3), range(3), range(3), range(3)):
+            c4[i,j,k,l] = c[vMap[frozenset({i,j})], vMap[frozenset({k,l})]]
+        return c4
+
+    def _convert4To2rankTensor(self, c4):
+        '''
+        Converts 4th rank elastic tensor to 4nd rank
+
+        Parameters
+        ----------
+        c4 : ndarray
+            4th rank elastic tensor
+
+        Returns
+        -------
+        c : ndarray
+            2nd rank elastic tensor
+        '''
+        vMap = [[0,0], [1,1], [2,2], [1,2], [0,2], [0,1]]
+        c = np.zeros((6,6))
+        for i, j in itertools.product(range(6), range(6)):
+            c[i,j] = c4[vMap[i][0], vMap[i][1], vMap[j][0], vMap[j][1]]
+        return c
+
+    def _invert4rankTensor(self, c4):
+        '''
+        Inverts 4th rank tensor to give stiffness tensor
+
+        This is done by converting to 2nd rank, inverting, then converting back to 4th rank
+        '''
+        c = self._convert4To2rankTensor(c4)
+        return self._convert2To4rankTensor(np.linalg.inv(c))
+
+    def _convertVecTo2rankTensor(self, v):
+        '''
+        Converts strain/stress vector to 2nd rank tensor
+
+        Parameters
+        ----------
+        v : 1d array
+            Strain/stress vector
+
+        Returns
+        -------
+        e : ndarray
+            2nd rank elastic tensor
+        '''
+        return np.array([[v[0], v[5], v[4]], \
+                        [v[5], v[1], v[3]], \
+                        [v[3], v[4], v[2]]])
+
+    def _convert2rankToVec(self, c):
+        '''
+        Converts 2nd rank tensor to vector
+
+        Parameter
+        ---------
+        c : ndarray
+            3x3 tensor
+
+        Returns
+        -------
+        v : 1darray
+            Strain/stress vector
+        '''
+        return np.array([c[0,0], c[1,1], c[2,2], c[1,2], c[0,2], c[0,1]])
+
+    def _rotateRank2Tensor(self, rot, tensor):
+        '''
+        Rotates a 2nd rank tensor
+        T_ij = r_il * r_jk * T_lk
+
+        Parameters
+        ----------
+        tensor : ndarray
+            2nd rank tensor to rotate (3x3 array)
+        '''
+        return np.tensordot(rot,
+                np.tensordot(rot, tensor, axes=(1,1)), axes=(1,1))
+
+    def _rotateRank4Tensor(self, rot, tensor):
+        '''
+        Rotates a 4th rank tensor
+        T_ijkl = r_im * r_jn * r_ok * r_lp * T_mnop
+
+        Parameters
+        ----------
+        tensor : ndarray
+            4th rank tensor to rotate (3x3x3x3 array)
+        '''
+        return np.tensordot(rot, 
+                np.tensordot(rot, 
+                np.tensordot(rot, 
+                np.tensordot(rot, tensor, axes=(1,3)), axes=(1,3)), axes=(1,3)), axes=(1,3))
 
     def setIntegrationIntervals(self, phiInt, thetaInt, assumeSymmetric=True):
         '''
         Number of intervals to split domain along phi and theta for integration
 
         Parameters
         ----------
@@ -356,28 +563,22 @@
             Number of intervals to divide along phi
         thetaInt : int
             Number of intervals to divide along theta
         assumeSymmetric : bool (optional)
             If True (default), will only integrate Eshelby's tensor on a single quadrant and
             multiply the results by 8
         '''
-        #Integral should be symmetric per quadrant (need to check)
-        #Thus we only need to integrate along a single quadrant
-        if assumeSymmetric:
-            dphi = np.pi/2 / phiInt
-            dtheta = np.pi/2 / thetaInt
-            midPhi = np.linspace(dphi/2, np.pi/2 - dphi/2, phiInt)
-            midTheta = np.linspace(dtheta/2, np.pi/2 - dtheta/2, thetaInt)
-            self.dA = dtheta * dphi
-        else:
-            dphi = 2*np.pi / phiInt
-            dtheta = np.pi / thetaInt
-            midPhi = np.linspace(dphi/2, 2*np.pi-dphi/2, phiInt)
-            midTheta = np.linspace(dtheta/2, np.pi-dtheta/2, thetaInt)
-            self.dA = 1/8 * dtheta * dphi
+        #If assume symmetric, then only a single quadrant will be integrated over
+        phiRange = np.pi/2 if assumeSymmetric else 2*np.pi
+        thetaRange = np.pi/2 if assumeSymmetric else np.pi
+        dphi = phiRange / phiInt
+        dtheta = thetaRange / thetaInt
+        midPhi = np.linspace(dphi/2, phiRange - dphi/2, phiInt)
+        midTheta = np.linspace(dtheta/2, thetaRange - dtheta/2, thetaInt)
+        self.dA = dtheta*dphi if assumeSymmetric else 1/8 * dtheta*dphi
 
         #Cartesian product of phi and theta intervals
         self.midPhiGrid, self.midThetaGrid = np.meshgrid(midPhi, midTheta)
         self.midPhiGrid = self.midPhiGrid.ravel()
         self.midThetaGrid = self.midThetaGrid.ravel()
         self.midWeights = np.sin(self.midThetaGrid)
 
@@ -397,15 +598,14 @@
             order = 53
         elif order == 'mid':
             order = 83
         else:
             order = 131
 
         self.midPhiGrid, self.midThetaGrid, self.midWeights = loadPoints(order)
-
         self.dA = np.pi/2
 
     def _n(self, phi, theta):
         '''
         Unit normal vector of sphere
 
         Parameters
@@ -460,50 +660,97 @@
         #For summing over grid points (D_ijkl = ohm_ij * nProd_kln * endTerm_n)
         d = np.tensordot(ohm, np.multiply(nProd, endTerm * self.midWeights), axes=[[2], [2]])
 
         #Multiply by differential area and across the 8 quadrants
         return 8*d*self.dA
 
     def Dijkl(self):
+        '''
+        Dijkl term for Eshelby's theory
+        '''
         #return -np.product(self.r)/(4*np.pi) * self.sphericalIntegral(self.Dfunc)
         return -np.product(self.r)/(4*np.pi) * self.sphInt()
 
     def Sijmn(self, D):
         '''
         S_ijmn = -0.5 * C_lkmn * (D_iklj + D_jkli)
         '''
         S = -0.5 * np.tensordot(self._c4, D + np.transpose(D, (3,1,2,0)), axes=[[0,1],[2,1]])
         #The tensor product gives S_mnij so we'll need to transpose it
         return np.transpose(S, (2,3,0,1))
 
-    def _strainC(self, S, strain):
+    def _multiply(self, a, b):
         '''
-        ec_ij = S_ijkl * e_kl
+        Multiplies 2 tensors
+        4th x 2nd -> c_ij = a_ijkl * b_kl
+        4th x 4th -> c_ijkl = a_ijmn * b_mnkl
         '''
-        return np.tensordot(S, strain, axes=[[2,3],[0,1]])
-
-    def _stress(self, strain):
-        '''
-        sigma_ij = C_ijkl * e_kl
-        '''
-        return np.tensordot(self._c4, strain, axes = [[2,3], [0,1]])
+        return np.tensordot(a, b, axes=[[2,3], [0,1]])
 
     def _strainEnergy(self, stress, strain, V):
         '''
         u = -0.5 * V * sigma_ij * strain_ij
         '''
         return -0.5 * V * np.sum(stress * strain)
 
-    def _strainEnergyEllipsoid(self):
+    def _strainEnergyEllipsoidWithStress(self):
+        '''
+        Strain energy of ellipsoidal particle with applied stress
+        '''
         V = 4*np.pi/3 * np.product(self.r)
         S = self.Sijmn(self.Dijkl())
-        stress = self._stress(self._strainC(S, self.eigstrain) - self.eigstrain)
-        stress0 = self._stress(self._strainC(S, self.appstrain) - self.appstrain)
+        stress = self._multiply(self._c4, self._multiply(S, self.eigstrain) - self.eigstrain)
+        stress0 = self._multiply(self._c4, self._multiply(S, self.appstrain) - self.appstrain)
         return self._strainEnergy(stress - stress0, self.eigstrain - self.appstrain, V)
 
+    def _strainEnergyEllipsoid(self):
+        '''
+        Strain energy of ellipsoidal particle
+        '''
+        V = 4*np.pi/3 * np.product(self.r)
+        S = self.Sijmn(self.Dijkl())
+        stress = self._multiply(self._c4, self._multiply(S, self.eigstrain) - self.eigstrain)
+        return self._strainEnergy(stress, self.eigstrain, V)
+
+    def _strainEnergyEllipsoid2(self):
+        '''
+        Alternative method of strain energy on ellipsoidal particle using 2nd rank tensors
+        '''
+        V = 4*np.pi/3 * np.product(self.r)
+        S = self._convert4To2rankTensor(self.Sijmn(self.Dijkl()))
+        eigFlat = self._convert2rankToVec(self.eigstrain)
+        multTerm = np.matmul(self.c, S - np.eye(6))
+        return -0.5 * V * np.matmul(eigFlat, np.matmul(multTerm, eigFlat))
+
+    def _strainEnergyBohm(self):
+        '''
+        Strain energy of particle for when matrix and precipitate phases have different elastic tensors
+        '''
+        V = 4*np.pi/3 * np.product(self.r)
+        S = self.Sijmn(self.Dijkl())
+        #invTerm = np.linalg.tensorinv(self._multiply(self._c4Prec - self._c4, S) + self._c4)
+        invTerm = self._invert4rankTensor(self._multiply(self._c4Prec - self._c4, S) + self._c4)
+        multTerm = self._multiply(invTerm, self._c4Prec)
+        stressC = self._multiply(self._c4, self._multiply(self._multiply(S, multTerm), self.eigstrain))
+        stress0 = self._multiply(self._c4, self._multiply(multTerm, self.eigstrain))
+        return self._strainEnergy(stressC-stress0, self.eigstrain, V)
+
+    def _strainEnergyBohm2(self):
+        '''
+        Strain energy of particle for when matrix and precipitate phases have different elastic tensors using 2nd rank tensors
+        '''
+        V = 4*np.pi/3 * np.product(self.r)
+        S = self._convert4To2rankTensor(self.Sijmn(self.Dijkl()))
+        eigFlat = self._convert2rankToVec(self.eigstrain)
+        invTerm = np.linalg.inv(np.matmul(self.cPrec - self.c, S) + self.c)
+        multTerm = np.matmul(invTerm, self.cPrec)
+        stressC = np.matmul(self.c, np.matmul(np.matmul(S, multTerm), eigFlat))
+        stress0 = np.matmul(self.c, np.matmul(multTerm, eigFlat))
+        return -0.5 * V * np.matmul(eigFlat, stressC - stress0)
+
     def _Khachaturyan(self, I1, I2):
         '''
         Khachaturyan's approximation for strain energy of spherical and cuboidal precipitates
         '''
         V = 4*np.pi/3 * np.product(self.r)
         A1 = 2 * (self.c[0,0] - self.c[0,1]) / self.c[0,0]
         A1 -= 12 * (self.c[0,0] + 2 * self.c[0,1]) * (self.c[0,0] - self.c[0,1] - 2 * self.c[3,3]) / (self.c[0,0] * (self.c[0,0] + self.c[0,1] + 2*self.c[3,3])) * I1
@@ -580,36 +827,38 @@
         d = self.c[0,0]
         d += self._xi*(self.c[0,0] + self.c[0,1])*((n[0]*n[1])**2 + (n[0]*n[2])**2 + (n[1]*n[2])**2)
         d += self._xi**2 * (self.c[0,0] + 2*self.c[0,1] + self.c[3,3])*(n[0]*n[1]*n[2])**2
         return d
 
     @property
     def _xi(self):
+        '''
+        Needed for the Ohm term with cubic crystal symmetry
+        '''
         return (self.c[0,0] - self.c[0,1] - 2*self.c[3,3]) / self.c[3,3]
 
     #Equilibrium aspect ratios
     #Determined by minimum of strain energy + interfacial energy
     def eqAR_byGR(self, Rsph, gamma, shpFactor, a=1.001, b=100):
         '''
-        Golden ratio search
+        Equilibrium aspect ratio using golden ratio search
 
         Parameters
         ----------
         Rsph : float or array
             Equivalent spherical radius
         gamma : float
             Interfacial energy
         shpFactor : ShapeFactor object
         a, b : float
             Min and max bounds
             Default is 1.001 and 100
         '''
         normR = shpFactor._normalRadiiEquation
-        #interfacial = shpFactor._eqRadiusEquation
-        interfacial = shpFactor._thermoEquation
+        interfacial = shpFactor._thermoEquation if self.ifmethod == 1 else shpFactor._eqRadiusEquation
         if hasattr(Rsph, '__len__'):
             eqAR = np.ones(len(Rsph))
             for i in range(len(Rsph)):
                 eqAR[i] = self._GRsearch(Rsph[i], gamma, interfacial, normR, a, b)
         else:
             eqAR = self._GRsearch(Rsph, gamma, interfacial, normR, a, b)
 
@@ -660,27 +909,26 @@
         Clear cached calculations
         '''
         self._aspectRatios = None
         self._normEnergies = None
 
     def eqAR_bySearch(self, Rsph, gamma, shpFactor):
         '''
-        Cached search
+        Equilibrium aspect ratio by cached search
 
         Parameters
         ----------
         Rsph : float or array
             Equivalent spherical radius
         gamma : float
             Interfacial energy
         shpFactor : ShapeFactor object
         '''
         normR = shpFactor._normalRadiiEquation
-        #interfacial = shpFactor._eqRadiusEquation
-        interfacial = shpFactor._thermoEquation
+        interfacial = shpFactor._thermoEquation if self.ifmethod == 1 else shpFactor._eqRadiusEquation
         if hasattr(Rsph, '__len__'):
             eqAR = np.ones(len(Rsph))
             for i in range(len(Rsph)):
                 eqAR[i] = self._cachedSearch(Rsph[i], gamma, interfacial, normR)
         else:
             eqAR = self._cachedSearch(Rsph, gamma, interfacial, normR)
         return eqAR
```

### Comparing `kawin-0.1.2/kawin/FreeEnergyHessian.py` & `kawin-0.2.0/kawin/FreeEnergyHessian.py`

 * *Files identical despite different names*

### Comparing `kawin-0.1.2/kawin/GrainBoundaries.py` & `kawin-0.2.0/kawin/GrainBoundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             self.areaFactor = 4 * np.pi
             self.volumeFactor = 4 * np.pi / 3
         
         #Grain boundary area nucleation
         elif self.nucleationSiteType == self.GRAIN_BOUNDARIES:
             self.gbRemoval = np.pi * (1 - self.GBk**2)
             self.areaFactor = 4 * np.pi * (1 - self.GBk)
-            self.volumeFactor = (2 * np.pi / 3) * (2 - 3 * self.GBk + self.GBk**2)
+            self.volumeFactor = (2 * np.pi / 3) * (2 - 3 * self.GBk + self.GBk**3)
 
         #Grain edge nucleation
         elif self.nucleationSiteType == self.GRAIN_EDGES and self.GBk < np.sqrt(3) / 2:
             alpha = np.arcsin(1 / (2 * np.sqrt(1 - self.GBk**2)))
             beta = np.arccos(self.GBk / np.sqrt(3 * (1 - self.GBk**2)))
             self.gbRemoval = 3 * beta * (1 - self.GBk**2) - self.GBk * np.sqrt(3 - 4 * self.GBk**2)
             self.areaFactor = 12 * (np.pi / 2 - alpha - self.GBk * beta)
```

### Comparing `kawin-0.1.2/kawin/KWNBase.py` & `kawin-0.2.0/kawin/KWNBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     '''
     def __init__(self, t0, tf, steps, phases = ['beta'], linearTimeSpacing = False, elements = ['solute']):
         #Store input parameters
         self.initialSteps = int(steps)      #Initial number of steps for when model is reset
         self.steps = int(steps)             #This includes the number of steps added when adaptive time stepping is enabled
         self.t0 = t0
         self.tf = tf
-        self.phases = phases
+        self.phases = np.array(phases)
         self.linearTimeSpacing = linearTimeSpacing
 
         #Change t0 to finite value if logarithmic time spacing
         #New t0 will be tf / 1e6
         if self.t0 <= 0 and self.linearTimeSpacing == False:
             self.t0 = self.tf / 1e6
             print('Warning: Cannot use 0 as an initial time when using logarithmic time spacing')
@@ -109,30 +109,30 @@
         
         #Free energy parameters
         self.gamma = np.empty(len(self.phases), dtype=np.float32)
         self.dG = [None for i in self.phases]
         self.interfacialComposition = [None for i in self.phases]
 
         if self.numberOfElements == 1:
-            self._Beta = self._BetaBinary
+            self._Beta = self._BetaBinary1
         else:
             self._Beta = self._BetaMulti
             self._betaFuncs = [None for p in phases]
             self._defaultBeta = 20
         
     def phaseIndex(self, phase = None):
         '''
         Returns index of phase in list
 
         Parameters
         ----------
         phase : str (optional)
             Precipitate phase (defaults to None, which will return 0)
         '''
-        return 0 if phase is None else self.phases.index(phase)
+        return 0 if phase is None else np.where(self.phases == phase)[0][0]
         
     def reset(self):
         '''
         Resets simulation results
         This does not reset the model parameters, however, it will clear any stopping conditions
         '''
         self._resetArrays()
@@ -144,14 +144,27 @@
             self.setTemperature(self.Tparameters)
         elif len(self.Tparameters) == 2:
             self.setTemperatureArray(*self.Tparameters)
         elif self.Tparameters is not None:
             self.setNonIsothermalTemperature(self.Tparameters)
         
     def _resetArrays(self):
+        '''
+        Resets and initializes arrays for all variables
+            time
+            matrix composition, equilibrium composition
+            critial radius and nucleation barrier
+            average radius and aspect ratio
+            volume fraction
+            nucleation rate
+            precipitate density
+            driving force
+            beta
+            incubation time
+        '''
         self.steps = self.initialSteps
         self.time = np.linspace(self.t0, self.tf, self.steps) if self.linearTimeSpacing else np.logspace(np.log10(self.t0), np.log10(self.tf), self.steps)
 
         if self.numberOfElements == 1:
             self.xComp = np.zeros(self.steps)                                #Current composition of matrix phase
             self.xEqAlpha = np.zeros((len(self.phases), self.steps))         #Equilibrium composition of matrix phase with respect to each precipitate phase
             self.xEqBeta = np.zeros((len(self.phases), self.steps))          #Equilibrium composition of precipitate phases
@@ -164,15 +177,15 @@
         self.Gcrit = np.zeros((len(self.phases), self.steps))                #Height of nucleation barrier
         self.Rad = np.zeros((len(self.phases), self.steps))                  #Radius of particles formed at each time step
         self.avgR = np.zeros((len(self.phases), self.steps))                 #Average radius
         self.avgAR = np.zeros((len(self.phases), self.steps))                #Mean aspect ratio
         self.betaFrac = np.zeros((len(self.phases), self.steps))             #Fraction of precipitate
         
         self.nucRate = np.zeros((len(self.phases), self.steps))              #Nucleation rate
-        self.precipitateDensity = np.zeros((len(self.phases), self.steps))  #Number of nucleates
+        self.precipitateDensity = np.zeros((len(self.phases), self.steps))   #Number of nucleates
         
         self.dGs = np.zeros((len(self.phases), self.steps))                  #Driving force
         self.betas = np.zeros((len(self.phases), self.steps))                #Impingement rates (used for non-isothermal)
         self.incubationOffset = np.zeros(len(self.phases))                   #Offset for incubation time (for non-isothermal precipitation)
         self.incubationSum = np.zeros(len(self.phases))                      #Sum of incubation time
 
         self.prevFConc = np.zeros((2, len(self.phases), self.numberOfElements))    #Sum of precipitate composition for mass balance
@@ -225,16 +238,18 @@
                 filename = filename + '.csv'
             with open(filename, 'w', newline='') as f:
                 csv.writer(f).writerow(headers)
                 csv.writer(f).writerows(rows)
         else:
             if compressed:
                 np.savez_compressed(filename, **vDict)
+                #np.savez_compressed(filename, **vDict, allow_pickle=True)
             else:
                 np.savez(filename, **vDict)
+                #np.savez(filename, **vDict, allow_pickle=True)
 
     def load(filename):
         '''
         Loads data
 
         Parameters
         ----------
@@ -243,15 +258,15 @@
         Returns
         -------
         PrecipitateBase object
             Note: this will only contain model outputs which can be used for plotting
         '''
         setupVars = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements']
         if '.np' in filename.lower():
-            data = np.load(filename)
+            data = np.load(filename, allow_pickle=True)
             model = PrecipitateBase(data['t0'], data['tf'], data['steps'], data['phases'], data['linearTimeSpacing'], data['elements'])
             for d in data:
                 if d not in setupVars:
                     setattr(model, d, data[d])
         elif '.csv' in filename.lower():
             with open(filename, 'r') as csvFile:
                 data = csv.reader(csvFile, delimiter=',')
@@ -353,15 +368,16 @@
         Parameters
         ----------
         adaptive : bool (optional)
             Defaults to True
         '''
         if adaptive:
             self._timeIncrementCheck = self._checkDT
-            self._postTimeIncrementCheck = self._postCheckDT
+            #self._postTimeIncrementCheck = self._postCheckDT
+            self._postTimeIncrementCheck = self._noPostCheckDT
         else:
             self._timeIncrementCheck = self._noCheckDT
             self._postTimeIncrementCheck = self._noPostCheckDT
 
     def _calculateDT(self, i, fraction):
         '''
         Calculates DT as a fraction of the total simulation time
@@ -392,19 +408,23 @@
         self.maxRcritChange = 0.01
 
         self.checkNucleation = True
         self.maxNucleationRateChange = 0.5
         self.minNucleationRate = 1e-5
 
         self.checkVolumePre = True
-        self.checkVolumePost = True
+        self.checkVolumePost = False
         self.maxVolumeChange = 0.001
         
-        self.checkComposition = True
+        self.checkComposition = False
+        self.checkCompositionPre = False
         self.maxCompositionChange = 0.001
+        self.minComposition = 0
+
+        self.minNucleateDensity = 1e-5
 
     def setConstraints(self, **kwargs):
         '''
         Sets constraints
 
         TODO: the following constraints are not implemented
             maxDTFraction
@@ -427,24 +447,46 @@
         checkRcrit - checks maximum change in critical radius (False)
         maxRcritChange - maximum change in critical radius (as a fraction) per single time step (0.01)
 
         checkNucleation - checks maximum change in nucleation rate (True)
         maxNucleationRateChange - maximum change in nucleation rate (on log scale) per single time step (0.5)
         minNucleationRate - minimum nucleation rate to be considered for checking time intervals (1e-5)
 
-        checkVolumePre - checks maximum estimated volume change (True)
+        checkVolumePre - estimates maximum volume change (True)
         checkVolumePost - checks maximum calculated volume change (True)
         maxVolumeChange - maximum absolute value that volume fraction can change per single time step (0.001)
 
         checkComposition - checks maximum change in composition (True)
+        chekcCompositionPre - estimates maximum change in composition (False)
         maxCompositionChange - maximum change in composition in single time step (0.01)
+
+        minNucleateDensity - minimum nucleate density to consider nucleation to have occurred (1e-5)
         '''
         for key, value in kwargs.items():
             setattr(self, key, value)
         
+    def setBetaBinary(self, functionType = 1):
+        '''
+        Sets function for beta calculation in binary systems
+
+        If using a multicomponent system, this function will not do anything
+
+        Parameters
+        ----------
+        functionType : int
+            ID for function
+                1 for implementation seen in Perez et al, 2008 (default)
+                2 for implementation similar to multicomponent systems
+        '''
+        if self.numberOfElements == 1:
+            if functionType == 2:
+                self.beta = self._BetaBinary2
+            else:
+                self.beta = self._BetaBinary1
+
     def setInitialComposition(self, xInit):
         '''
         Parameters
         
         xInit : float or array
             Initial composition of parent matrix phase in atomic fraction
             Use float for binary system and array of solutes for multicomponent systems
@@ -853,14 +895,15 @@
         self.strainEnergy[index] = strainEnergy
         self.calculateAspectRatio[index] = calculateAspectRatio
 
     def _setupStrainEnergyFactors(self):
         #For each phase, the strain energy calculation will be set to assume
         # a spherical, cubic or ellipsoidal shape depending on the defined shape factors
         for i in range(len(self.phases)):
+            self.strainEnergy[i].setup()
             if self.strainEnergy[i].type != StrainEnergy.CONSTANT:
                 if self.shapeFactors[i].particleType == ShapeFactor.SPHERE:
                     self.strainEnergy[i].setSpherical()
                 elif self.shapeFactors[i].particleType == ShapeFactor.CUBIC:
                     self.strainEnergy[i].setCuboidal()
                 else:
                     self.strainEnergy[i].setEllipsoidal()
@@ -922,30 +965,37 @@
         This will be a positive value, so the function should ensure that the excess free energy to reduce the driving force
         
         If equilibrium cannot be solved, then the function should return (None, None) or (-1, -1)
         '''
         index = self.phaseIndex(phase)
         self.interfacialComposition[index] = composition
 
-    def setThermodynamics(self, therm, phase = None):
+    def setThermodynamics(self, therm, phase = None, removeCache = False, addDiffusivity = True):
         '''
         Parameters
         ----------
         therm : Thermodynamics class
         phase : str (optional)
             Phase to consider (defaults to first precipitate in list)
+        removeCache : bool (optional)
+            Will not cache equilibrium results if True (defaults to False)
+        addDiffusivity : bool (optional)
+            For binary systems, will add diffusivity functions from the database if present
+            Defaults to True
         '''
         index = self.phaseIndex(phase)
-        self.dG[index] = lambda x, T: therm.getDrivingForce(x, T, precPhase=phase)
+        self.dG[index] = lambda x, T, removeCache = removeCache: therm.getDrivingForce(x, T, precPhase=phase, training = removeCache)
         
         if self.numberOfElements == 1:
             self.interfacialComposition[index] = lambda x, T: therm.getInterfacialComposition(x, T, precPhase=phase)
+            if (therm.mobCallables is not None or therm.diffCallables is not None) and addDiffusivity:
+                self.Diffusivity = lambda x, T, removeCache = removeCache: therm.getInterdiffusivity(x, T, removeCache = removeCache)
         else:
-            self.interfacialComposition[index] = lambda x, T, dG, R, gExtra: therm.getGrowthAndInterfacialComposition(x, T, dG, R, gExtra, precPhase=phase)
-            self._betaFuncs[index] = lambda x, T: therm.impingementFactor(x, T, precPhase=phase)
+            self.interfacialComposition[index] = lambda x, T, dG, R, gExtra, removeCache = removeCache: therm.getGrowthAndInterfacialComposition(x, T, dG, R, gExtra, precPhase=phase, training = False)
+            self._betaFuncs[index] = lambda x, T, removeCache = removeCache: therm.impingementFactor(x, T, precPhase=phase, training = False)
 
     def setSurrogate(self, surr, phase = None):
         '''
         Parameters
         ----------
         surr : Surrogate class
         phase : str (optional)
@@ -1107,25 +1157,25 @@
         '''
         Prints various terms at step i
         '''
         if self.numberOfElements == 1:
             print('N\tTime (s)\tTemperature (K)\tMatrix Comp')
             print('{:.0f}\t{:.1e}\t\t{:.0f}\t\t{:.4f}\n'.format(i, self.time[i], self.T[i], 100*self.xComp[i]))
         else:
-            compStr = 'N\tTime (s)\tTemperature (K)'
-            compValStr = '{:.0f}\t{:.1e}\t\t{:.0f}\t'.format(i, self.time[i], self.T[i])
+            compStr = 'N\tTime (s)\tTemperature (K)\t'
+            compValStr = '{:.0f}\t{:.1e}\t\t{:.0f}\t\t'.format(i, self.time[i], self.T[i])
             for a in range(self.numberOfElements):
                 compStr += self.elements[a] + '\t'
                 compValStr += '{:.4f}\t'.format(100*self.xComp[i,a])
             compValStr += '\n'
             print(compStr)
             print(compValStr)
-        print('\tPhase\tPrec Density (#/m3)\tVolume Frac\tAvg Radius (m)')
+        print('\tPhase\tPrec Density (#/m3)\tVolume Frac\tAvg Radius (m)\tDriving Force (J/mol)')
         for p in range(len(self.phases)):
-            print('\t{}\t{:.3e}\t{:.4f}\t\t{:.4e}'.format(self.phases[p], self.precipitateDensity[p,i], 100*self.betaFrac[p,i], self.avgR[p,i]))
+            print('\t{}\t{:.3e}\t\t{:.4f}\t\t{:.4e}\t{:.4e}'.format(self.phases[p], self.precipitateDensity[p,i], 100*self.betaFrac[p,i], self.avgR[p,i], self.dGs[p,i]*self.VmBeta[p]))
         print('')
                 
     def solve(self, verbose = False, vIt = 1000):
         '''
         Solves the KWN model between initial and final time
         
         Note: _calculateNucleationRate, _calculatePSD and _printOutput will need to be implemented in the child classes
@@ -1215,15 +1265,15 @@
         self.dGs[p, i] -= self.strainEnergy[p].strainEnergy(self.shapeFactors[p].normalRadii(self.Rcrit[p, i-1]))
 
         if self.dGs[p, i] < 0:
             return self._noDrivingForce(p, i)
 
         #Only do this if there is some parent phase left (brute force solution for to avoid numerical errors)
         if self.betaFrac[p, i-1] < 1:
-            
+
             #Calculate critical radius
             #For bulk or dislocation nucleation sites, use previous critical radius to get aspect ratio
             if self.GB[p].nucleationSiteType == GBFactors.BULK or self.GB[p].nucleationSiteType == GBFactors.DISLOCATION:
                 self.Rcrit[p, i] = 2 * self.shapeFactors[p].thermoFactor(self.Rcrit[p, i-1]) * self.gamma[p] / self.dGs[p, i]
                 #self.Rcrit[p, i] = 2 * self.gamma[p] / self.dGs[p, i]
                 if self.Rcrit[p, i] < self.Rmin[p]:
                     self.Rcrit[p, i] = self.Rmin[p]
@@ -1237,20 +1287,22 @@
                     self.Rcrit[p, i] = self.Rmin[p]
                     
                 self.Gcrit[p, i] = self.GB[p].Gcrit(self.dGs[p, i], self.Rcrit[p, i])
 
             #Calculate nucleation rate
             Z = self._Zeldovich(p, i)
             self.betas[p,i] = self._Beta(p, i)
-                
+            if self.betas[p,i] == 0:
+                return self._noDrivingForce(p, i)
+
             #Incubation time, either isothermal or nonisothermal
             self.incubationSum[p] = self._incubation(Z, p, i)
             if self.incubationSum[p] > 1:
                 self.incubationSum[p] = 1
-            
+
             return Z * self.betas[p,i] * np.exp(-self.Gcrit[p, i] / (self.kB * self.T[i])) * self.incubationSum[p]
 
         else:
             return self._noDrivingForce(p, i)
             
     def _noCheckDT(self, i):
         '''
@@ -1276,32 +1328,51 @@
         '''
         pass
 
     def _noDrivingForce(self, p, i):
         '''
         Set everything to 0 if there is no driving force for precipitation
         '''
-        #self.dGs[p, i] = 0
         self.Rcrit[p, i] = 0
-        #self.incubationOffset[p] = self.time[i-1]
         self.incubationOffset[p] = np.amax([i-1, 0])
         return 0
 
     def _nucleateFreeEnergy(self, Rsph, p, i):
+        '''
+        Free energy change for a nucleate with radius of Rsph
+        '''
         volContribution = 4/3 * np.pi * Rsph**3 * (self.dGs[p,i] + self.strainEnergy[p].strainEnergy(self.shapeFactors[p].normalRadii(Rsph)))
         areaContribution = 4 * np.pi * self.gamma[p] * Rsph**2 * self.shapeFactors[p].thermoFactor(Rsph)
         return -volContribution + areaContribution
 
     def _Zeldovich(self, p, i):
+        '''
+        Zeldovich factor - probability that cluster at height of nucleation barrier will continue to grow
+        '''
         return np.sqrt(3 * self.GB[p].volumeFactor / (4 * np.pi)) * self.VmBeta[p] * np.sqrt(self.gamma[p] / (self.kB * self.T[i])) / (2 * np.pi * self.avo * self.Rcrit[p,i]**2)
         
-    def _BetaBinary(self, p, i):
-        return self.GB[p].areaFactor * self.Rcrit[p,i]**2 * self.xComp[0] * self.Diffusivity(self.xComp[i], self.T[i]) / self.aAlpha**4
+    def _BetaBinary1(self, p, i):
+        '''
+        Impingement rate for binary systems using Perez et al
+        '''
+        return self.GB[p].areaFactor * self.Rcrit[p,i]**2 * self.xComp[0] * self.Diffusivity(self.xComp[i-1], self.T[i]) / self.aAlpha**4
+
+    def _BetaBinary2(self, p, i):
+        '''
+        Impingement rate for binary systems taken from Thermocalc prisma documentation
+        This will follow the same equation as with _BetaMulti; however, some simplications can be made based off the summation contraint
+        '''
+        D = self.Diffusivity(self.xComp[i-1], self.T[i])
+        Dfactor = (self.xEqBeta[p,i-1] - self.xEqAlpha[p,i-1])**2 / (self.xEqAlpha[p,i-1]*D) + (self.xEqBeta[p,i-1] - self.xEqAlpha[p,i-1])**2 / ((1 - self.xEqAlpha[p,i-1])*D)
+        return self.GB[p].areaFactor * self.Rcrit[p,i]**2 * (1/Dfactor) / self.aAlpha**4
             
     def _BetaMulti(self, p, i):
+        '''
+        Impingement rate for multicomponent systems
+        '''
         if self._betaFuncs[p] is None:
             return self._defaultBeta
         else:
             beta = self._betaFuncs[p](self.xComp[i-1], self.T[i-1])
             if beta is None:
                 return self.betas[p,i-1]
             else:
@@ -1345,21 +1416,53 @@
                 tau = LHS[-1] / self.betas[p,i] - RHS[-1] / self.betas[p,i] + (self.time[i] - self.time[int(self.incubationOffset[p])])
         else:
             tau = self.time[int(self.incubationOffset[p]):-1][signChange][0] - self.time[int(self.incubationOffset[p])]
 
         return np.exp(-tau / (self.time[i] - self.time[int(self.incubationOffset[p])]))
 
     def _setNucleateRadius(self, i):
+        '''
+        Adds 1/2 * sqrt(kb T / pi gamma) to critical radius to ensure they grow when growth rates are calculated
+        '''
         for p in range(len(self.phases)):
             #If nucleates form, then calculate radius of precipitate
-            #Radius is set slightly larger so preciptate 
-            if self.nucRate[p,i]*(self.time[i]-self.time[i-1]) >= 1 and self.Rcrit[p, i] >= self.Rmin[p]:
+            #Radius is set slightly larger so precipitate 
+            if self.nucRate[p,i]*(self.time[i]-self.time[i-1]) >= self.minNucleateDensity and self.Rcrit[p, i] >= self.Rmin[p]:
                 self.Rad[p, i] = self.Rcrit[p, i] + 0.5 * np.sqrt(self.kB * self.T[i] / (np.pi * self.gamma[p]))
             else:
                 self.Rad[p, i] = 0
+
+    def getTimeAxis(self, timeUnits='s', bounds=None):
+        '''
+        Returns scaling factor, label and x-limits depending on units of time
+
+        Parameters
+        ----------
+        timeUnits : str
+            's' / 'sec' / 'seconds' - seconds
+            'min' / 'minutes' - minutes
+            'h' / 'hrs' / 'hours' - hours
+        '''
+        timeScale = 1
+        timeLabel = 'Time (s)'
+        if 'min' in timeUnits:
+            timeScale = 1/60
+            timeLabel = 'Time (min)'
+        if 'h' in timeUnits:
+            timeScale = 1/3600
+            timeLabel = 'Time (hrs)'
+
+        if bounds is None:
+            if self.t0 == 0:
+                bounds = [timeScale * 1e-5 * self.tf, timeScale * self.tf]
+            else:
+                bounds = [timeScale * self.t0, timeScale * self.tf]
+
+        return timeScale, timeLabel, bounds
+        
     
     def plot(self, axes, variable, bounds = None, timeUnits = 's', radius='spherical', *args, **kwargs):
         '''
         Plots model outputs
         
         Parameters
         ----------
@@ -1376,38 +1479,25 @@
                 Note: for multi-phase simulations, adding the word 'Total' will
                     sum the variable for all phases. Without the word 'Total', the variable
                     for each phase will be plotted separately
                     
         bounds : tuple (optional)
             Limits on the x-axis (float, float) or None (default, this will set bounds to (initial time, final time))
         timeUnits : str (optional)
-            Plot time dependent variables per seconds ('s'), minutes ('m') or hours ('h')
+            Plot time dependent variables per seconds ('s'), minutes ('min') or hours ('h')
         radius : str (optional)
             For non-spherical precipitates, plot the Average Radius by the -
                 Equivalent spherical radius ('spherical')
                 Short axis ('short')
                 Long axis ('long')
             Note: Total Average Radius and Volume Average Radius will still use the equivalent spherical radius
         *args, **kwargs - extra arguments for plotting
         '''
-        timeScale = 1
-        timeLabel = 'Time (s)'
-        if 'min' in timeUnits:
-            timeScale = 1/60
-            timeLabel = 'Time (min)'
-        if 'h' in timeUnits:
-            timeScale = 1/3600
-            timeLabel = 'Time (hrs)'
+        timeScale, timeLabel, bounds = self.getTimeAxis(timeUnits, bounds)
 
-        if bounds is None:
-            if self.t0 == 0:
-                bounds = [timeScale * 1e-5 * self.tf, timeScale * self.tf]
-            else:
-                bounds = [timeScale * self.t0, timeScale * self.tf]
-            
         axes.set_xlabel(timeLabel)
         axes.set_xlim(bounds)
 
         labels = {
             'Volume Fraction': 'Volume Fraction',
             'Total Volume Fraction': 'Volume Fraction',
             'Critical Radius': 'Critical Radius (m)',
```

### Comparing `kawin-0.1.2/kawin/KWNEuler.py` & `kawin-0.2.0/kawin/KWNEuler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from kawin.KWNBase import PrecipitateBase
 from kawin.PopulationBalance import PopulationBalanceModel
 from kawin.GrainBoundaries import GBFactors
 import copy
 import csv
 from itertools import zip_longest
+import time
 
 class PrecipitateModel (PrecipitateBase):
     '''
     Euler implementation of the KWN model designed for binary systems
 
     Parameters
     ----------
@@ -31,23 +32,30 @@
     '''
     def __init__(self, t0, tf, steps, phases = ['beta'], linearTimeSpacing = False, elements = ['solute']):
         #Initialize base class
         super().__init__(t0, tf, steps, phases, linearTimeSpacing, elements)
 
         if self.numberOfElements == 1:
             self._growthRate = self._growthRateBinary
-            self._Beta = self._BetaBinary
+            self._Beta = self._BetaBinary1
         else:
             self._growthRate = self._growthRateMulti
             self._Beta = self._BetaMulti
 
-        #Adaptive time stepping
-        self._postTimeIncrementCheck = self._noPostCheckDT
+        #Additional outputs
+        self.additionalFunctions = []
+        self.additionalFunctionNames = []
+        self.additionalOutputs = None
 
     def _resetArrays(self):
+        '''
+        Resets and initializes arrays for all variables
+
+        In addition to PrecipitateBase, the equilibrium aspect ratio area and population balance models are created here
+        '''
         super()._resetArrays()
         self.PBM = [PopulationBalanceModel() for p in self.phases]
 
         #Index of particle size classes which below, precipitates are unstable
         self.RdrivingForceIndex = np.zeros(len(self.phases), dtype=np.int32)
 
         #Aspect ratio
@@ -59,14 +67,17 @@
         '''
         super().reset()
 
         #Bounds of the bins in PSD
         for i in range(len(self.phases)):
             self.PBM[i].reset()
 
+        #Resets PSD outputs
+        self._setupAdditionalOutputs()
+
     def save(self, filename, compressed = False, toCSV = False):
         '''
         Save results into a numpy .npz format
 
         Parameters
         ----------
         filename : str
@@ -74,14 +85,18 @@
             If true, will save compressed .npz format
         toCSV : bool
             If true, wil save to .csv
         '''
         variables = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements', \
             'time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta']
         vDict = {v: getattr(self, v) for v in variables}
+        if self.additionalOutputs is not None:
+            vDict['additionalOutputs'] = self.additionalOutputs
+            if not toCSV:
+                vDict['additionalFunctionNames'] = self.additionalFunctionNames
         for p in range(len(self.phases)):
             vDict['PSDdata_'+self.phases[p]] = [self.PBM[p].min, self.PBM[p].max, self.PBM[p].bins]
             vDict['PSDsize_' + self.phases[p]] = self.PBM[p].PSDsize
             vDict['PSD_' + self.phases[p]] = self.PBM[p].PSD
             vDict['PSDbounds_' + self.phases[p]] = self.PBM[p].PSDbounds
             vDict['eqAspectRatio_' + self.phases[p]] = self.eqAspectRatio[p]
 
@@ -104,28 +119,35 @@
                         else:
                             headers.append(v + '_' + self.phases[i])
                 elif v == 'xEqAlpha' or v == 'xEqBeta':
                     for i in range(len(self.phases)):
                         for j in range(self.numberOfElements):
                             arrays.append(vDict[v][i,:,j])
                             headers.append(v + '_' + self.phases[i] + '_' + self.elements[j])
+                elif v == 'additionalOutputs':
+                    for i in range(len(self.phases)):
+                        for j in range(len(self.additionalFunctionNames)):
+                            arrays.append(vDict[v][i,:,j])
+                            headers.append(v + '_' + self.phases[i] + '_' + self.additionalFunctionNames[j])
                 else:
                     arrays.append(vDict[v])
                     headers.append(v)
             rows = zip_longest(*arrays, fillvalue='')
             if '.csv' not in filename.lower():
                 filename = filename + '.csv'
             with open(filename, 'w', newline='') as f:
                 csv.writer(f).writerow(headers)
                 csv.writer(f).writerows(rows)
         else:
             if compressed:
                 np.savez_compressed(filename, **vDict)
+                #np.savez_compressed(filename, **vDict, allow_pickle=True)
             else:
                 np.savez(filename, **vDict)
+                #np.savez(filename, **vDict, allow_pickle=True)
 
     def load(filename):
         '''
         Loads data
 
         Parameters
         ----------
@@ -134,15 +156,15 @@
         Returns
         -------
         PrecipitateModel object
             Note: this will only contain model outputs which can be used for plotting
         '''
         setupVars = ['t0', 'tf', 'steps', 'phases', 'linearTimeSpacing', 'elements']
         if '.np' in filename.lower():
-            data = np.load(filename)
+            data = np.load(filename, allow_pickle=True)
             
             #Input arbitrary values for PSD parameters (rMin, rMax, bins) since this will be changed shortly after
             model = PrecipitateModel(data['t0'], data['tf'], data['steps'], data['phases'], data['linearTimeSpacing'], data['elements'])
             for p in range(len(model.phases)):
                 PSDvars = ['PSDdata_' + model.phases[p], 'PSD_' + model.phases[p], 'PSDsize_' + model.phases[p], 'eqAspectRatio_' + model.phases[p], 'PSDbounds_' + model.phases[p]]
                 #For back compatibility
                 if PSDvars[0] not in data:
@@ -152,14 +174,18 @@
                 model.PBM[p].PSD = data[PSDvars[1]]
                 model.PBM[p].PSDsize = data[PSDvars[2]]
                 model.eqAspectRatio[p] = data[PSDvars[3]]
                 model.PBM[p].PSDbounds = data[PSDvars[4]]
             for d in data:
                 if d not in setupVars:
                     setattr(model, d, data[d])
+            if 'additionalOutputs' not in data:
+                model.additionalOutputs = None
+                model.additionalFunctions = []
+                model.additionalFunctionNames = []
         elif '.csv' in filename.lower():
             with open(filename, 'r') as csvFile:
                 data = csv.reader(csvFile, delimiter=',')
                 i = 0
                 headers = []
                 columns = {}
                 #Grab all columns
@@ -185,30 +211,33 @@
                     setupVars = np.concatenate((setupVars, PSDvars))
                     model.PBM[p] = PopulationBalanceModel(float(columns[PSDvars[0]][0]), float(columns[PSDvars[0]][1]), int(float(columns[PSDvars[0]][2])), True)
                     model.PBM[p].PSD = np.array(columns[PSDvars[1]], dtype='float')
                     model.PBM[p].PSDsize = np.array(columns[PSDvars[2]], dtype='float')
                     model.eqAspectRatio[p] = np.array(columns[PSDvars[3]], dtype='float')
                     model.PBM[p].PSDbounds = np.array(columns[PSDvars[4]], dtype='float')
 
-                restOfVariables = ['time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta']
+                restOfVariables = ['time', 'xComp', 'Rcrit', 'Gcrit', 'Rad', 'avgR', 'avgAR', 'betaFrac', 'nucRate', 'precipitateDensity', 'dGs', 'xEqAlpha', 'xEqBeta', 'additionalOutputs']
                 restOfColumns = {v: [] for v in restOfVariables}
+                additionalFunctionNames = []
                 for d in columns:
                     if d not in setupVars:
                         if d == 'time':
                             restOfColumns[d] = np.array(columns[d], dtype='float')
                         elif d == 'xComp':
                             if model.numberOfElements == 1:
                                 restOfColumns[d] = np.array(columns[d], dtype='float')
                             else:
                                 restOfColumns['xComp'].append(columns[d], dtype='float')
                         else:
                             selectedVar = ''
                             for r in restOfVariables:
                                 if r in d:
                                     selectedVar = r
+                            if selectedVar == 'additionalOutputs':
+                                additionalFunctionNames.append(d[18:])
                             restOfColumns[selectedVar].append(np.array(columns[d], dtype='float'))
                 for d in restOfColumns:
                     restOfColumns[d] = np.array(restOfColumns[d])
                     setattr(model, d, restOfColumns[d])
 
                 #For multicomponent systems, adjust as necessary such that number of elements will be the last axis
                 if model.numberOfElements > 1:
@@ -217,16 +246,36 @@
                         model.xEqAlpha = np.expand_dims(model.xEqAlpha, 0)
                         model.xEqBeta = np.expand_dims(model.xEqBeta, 0)
                     else:
                         model.xEqAlpha = np.reshape(model.xEqAlpha, ((len(model.phases), model.numberOfElements, len(model.time))))
                         model.xEqBeta = np.reshape(model.xEqBeta, ((len(model.phases), model.numberOfElements, len(model.time))))
                     model.xEqAlpha = np.transpose(model.xEqAlpha, (0, 2, 1))
                     model.xEqBeta = np.transpose(model.xEqBeta, (0, 2, 1))
+
+                #If additional outputs exists, then reshape array to (phase, iterations, functions)
+                if len(additionalFunctionNames) > 0:
+                    numberOfFunctions = int(len(additionalFunctionNames) / len(model.phases))
+                    model.additionalOutputs = np.reshape(model.additionalOutputs, (len(model.phases), numberOfFunctions, len(model.time)))
+                    model.additionalOutputs = np.transpose(model.additionalOutputs, (0, 2, 1))
+                    model.additionalFunctionNames = []
+                    for i in range(numberOfFunctions):
+                        model.additionalFunctionNames.append(additionalFunctionNames[i][len(model.phases[0])+1:])
+                    model.additionalFunctionNames = np.array(model.additionalFunctionNames)
+
         return model
 
+    def _divideTimestep(self, i, dt):
+        '''
+        Divides timestep at iteration i
+        '''
+        super()._divideTimestep(i, dt)
+
+        if len(self.additionalFunctions) > 0:
+            self.additionalOutputs = np.append(self.additionalOutputs, np.zeros((len(self.phases), 1, len(self.additionalFunctions))), axis=1)
+
     def setPBMParameters(self, cMin = 1e-10, cMax = 1e-9, bins = 150, minBins = 100, maxBins = 200, adaptive = True, phase = None):
         '''
         Sets population balance model parameters for each phase
 
         Parameters
         ----------
         cMin : float
@@ -263,14 +312,70 @@
             Array of data containing precipitate sizes
         phase : str (optional)
             Phase to consider (defaults to first precipitate in list)
         '''
         index = self.phaseIndex(phase)
         self.PBM[index].LoadDistribution(data)
 
+    def addAdditionalOutput(self, name, f):
+        '''
+        Creates output based off PSD
+
+        Parameters
+        ----------
+        name : str
+            Name of the function
+        f : function
+            Takes in model, phase index and iteration index and returns a value
+        '''
+        if name in self.additionalFunctionNames:
+            i = 1
+            name = name + '_{}'.format(i)
+            while name in self.additionalFunctionNames:
+                i += 1
+                name = name[:-2]
+                name = name + '_{}'.format(i)
+            print('Warning: Function \'{}\' has already been set, this function will be stored as \'{}\''.format(name[:-2], name))
+            
+        self.additionalFunctions.append(f)
+        self.additionalFunctionNames = np.append(self.additionalFunctionNames, name)
+
+    def _setupAdditionalOutputs(self):
+        '''
+        Function to setup PSD output arrays, will be used in setup and reset functions
+        '''
+        #Resets PSD outputs
+        if len(self.additionalFunctions) > 0:
+            self.additionalOutputs = np.zeros((len(self.phases), self.steps, len(self.additionalFunctions)))
+
+    def _calculateAdditionalOutputs(self, i):
+        '''
+        Calculates additional PSD functions
+        '''
+        for f in range(len(self.additionalFunctions)):
+            for p in range(len(self.phases)):
+                self.additionalOutputs[p, i, f] = self.additionalFunctions[f](self, p, i)
+
+    def getAdditionalOutput(self, name):
+        '''
+        Gets additional output by name
+
+        Parameters
+        ----------
+        name : str
+            Name of function used for the additional output
+
+        Returns
+        -------
+        (p, N) array for the output for each phase
+        '''
+        if name in self.additionalFunctionNames:
+            index, = np.where(self.additionalFunctionNames == name)
+            return self.additionalOutputs[:, :, index[0]]
+
     def particleRadius(self, phase = None):
         '''
         Returns PSD bounds of given phase
 
         Parameters
         ----------
         phase : str (optional)
@@ -345,16 +450,23 @@
                 self.PSDXalpha[p][:self.RdrivingForceIndex[p]+1] = self.PSDXalpha[p][self.RdrivingForceIndex[p]+1]
                 self.PSDXbeta[p][:self.RdrivingForceIndex[p]+1] = self.PSDXbeta[p][self.RdrivingForceIndex[p]+1]
             else:
                 self.PSDXalpha[p] = np.zeros(self.PBM[p].bins + 1)
                 self.PSDXbeta[p] = np.zeros(self.PBM[p].bins + 1)
             
     def setup(self):
+        '''
+        Sets up additional variables in addition to PrecipitateBase
+
+        Sets up additional outputs, population balance models, equilibrium aspect ratio and equilibrium compositions
+        '''
         super().setup()
 
+        self._setupAdditionalOutputs()
+
         #Equilibrium aspect ratio and PBM setup
         #If calculateAspectRatio is True, then use strain energy to calculate aspect ratio for each size class in PSD
         #Else, then use aspect ratio defined in shape factors
         self.eqAspectRatio = [None for p in range(len(self.phases))]
         for p in range(len(self.phases)):
             self.PBM[p].reset()
 
@@ -407,26 +519,29 @@
         #Backup variables in case size classes on PSD changes
         self.growthBackup = copy.copy(self.growth)
         self.PSDXalphaBackup = copy.copy(self.PSDXalpha)
         self.PSDXbetaBackup = copy.copy(self.PSDXbeta)
         self.eqAspectRatioBackup = copy.copy(self.eqAspectRatio)
         self.RdrivingForceIndexBackup = copy.copy(self.RdrivingForceIndex)
         self.RdrivingForceLimitBackup = copy.copy(self.RdrivingForceLimit)
-        
+
         postDTCheck = False
         while not postDTCheck:
             dt = self.time[i] - self.time[i-1]
             self._calculatePSD(i, dt)
             self._massBalance(i)
 
             if i < self.steps - 1:
                 postDTCheck = self._postTimeIncrementCheck(i)
             else:
                 postDTCheck = True
 
+        #Calculate additional PSD function
+        self._calculateAdditionalOutputs(i)
+
     def _noCheckDT(self, i):
         '''
         Function if adaptive time stepping is not used
         Will calculated growth rate since it is done in the _checkDT function (not a good way of doing this, but works for now)
         '''
         return
 
@@ -443,48 +558,79 @@
             else:
                 dtPBM = [dt]
             dt = np.amin(np.concatenate(([dt], dtPBM)))
             dtAll.append(dt)
 
         if i > 1:
             dtPrev = self.time[i-1] - self.time[i-2]
+        else:
+            dtPrev = dt
 
-            #Nucleation rate constraint
-            if self.checkNucleation:
-                dtNuc = dt * np.ones(len(self.phases)+1)
-                for p in range(len(self.phases)):
-                    if self.nucRate[p,i] > self.minNucleationRate and self.nucRate[p,i-1] > self.minNucleationRate and self.nucRate[p,i-1] != self.nucRate[p,i]:
-                        dtNuc[p] = self.maxNucleationRateChange * dtPrev / np.abs(np.log10(self.nucRate[p,i-1] / self.nucRate[p,i]))
-                dt = np.amin(dtNuc)
-                dtAll.append(dt)
+        #Nucleation rate constraint
+        if self.checkNucleation:
+            dtNuc = dt * np.ones(len(self.phases)+1)
+            for p in range(len(self.phases)):
+                if self.nucRate[p,i] > self.minNucleationRate and self.nucRate[p,i-1] > self.minNucleationRate and self.nucRate[p,i-1] != self.nucRate[p,i]:
+                    dtNuc[p] = self.maxNucleationRateChange * dtPrev / np.abs(np.log10(self.nucRate[p,i-1] / self.nucRate[p,i]))
+            dt = np.amin(dtNuc)
+            dtAll.append(dt)
 
-            #Temperature change constraint
-            if self.checkTemperature:
-                Tchange = self.T[i] - self.T[i-1]
-                dtTemp = dt
-                if Tchange > self.maxNonIsothermalDT:
-                    dtTemp = self.maxNonIsothermalDT * (self.time[i] - self.time[i-1]) / Tchange
-                    dt = np.amin([dt, dtTemp])
-
-            if self.checkRcrit:
-                dtRad = dt * np.ones(len(self.phases)+1)
-                if not all((self.Rcrit[:,i-1] == 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] == 0) & (self.dGs[:,i] <= 0)):
-                    indices = (self.Rcrit[:,i-1] > 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] != 0) & (self.dGs[:,i] > 0)
-                    dtRad[:-1][indices] = self.maxRcritChange * dtPrev / np.abs((self.Rcrit[:,i][indices] - self.Rcrit[:,i-1][indices]) / self.Rcrit[:,i-1][indices])
-                dt = np.amin(dtRad)
-                dtAll.append(dt)
+        #Temperature change constraint
+        if self.checkTemperature:
+            Tchange = self.T[i] - self.T[i-1]
+            dtTemp = dt
+            if Tchange > self.maxNonIsothermalDT:
+                dtTemp = self.maxNonIsothermalDT * (self.time[i] - self.time[i-1]) / Tchange
+                dt = np.amin([dt, dtTemp])
+
+        if self.checkRcrit:
+            dtRad = dt * np.ones(len(self.phases)+1)
+            if not all((self.Rcrit[:,i-1] == 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] == 0) & (self.dGs[:,i] <= 0)):
+                indices = (self.Rcrit[:,i-1] > 0) & (self.Rcrit[:,i] - self.Rcrit[:,i-1] != 0) & (self.dGs[:,i] > 0)
+                dtRad[:-1][indices] = self.maxRcritChange * dtPrev / np.abs((self.Rcrit[:,i][indices] - self.Rcrit[:,i-1][indices]) / self.Rcrit[:,i-1][indices])
+            dt = np.amin(dtRad)
+            dtAll.append(dt)
+
+        if self.checkVolumePre or self.checkCompositionPre:
+            dV = np.zeros(len(self.phases))
+            for p in range(len(self.phases)):
+                #Calculate estimate volume change based off growth rate and nucleated particles
+                #TODO: account for non-spherical precipitates
+                dVi = self.PBM[p].PSD * self.PBM[p].PSDsize**2 * 0.5 * (self.growth[p][1:] + self.growth[p][:-1])
+                dVi[dVi < 0] = 0
+                dV = self.VmAlpha / self.VmBeta[p] * (self.GB[p].areaFactor * np.sum(dVi) + self.GB[p].volumeFactor * self.nucRate[p,i] * self.Rad[p,i]**3)
 
             if self.checkVolumePre:
                 dtVol = dt * np.ones(len(self.phases) + 1)
-                if not all((self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)):
-                    indices = (self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)
-                    dtVol[:-1][indices] = self.maxVolumeChange / (10 * (4*np.pi*self.Rad[:,i][indices]**3*self.nucRate[:,i][indices]/3))
+                for p in range(len(self.phases)):
+                    if dV != 0:
+                        dtVol[p] = self.maxVolumeChange / (2 * np.abs(dV))
+                #if not all((self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)):
+                #    indices = (self.Rad[:,i]**3*self.nucRate[:,i] > 1e-30)
+                #    dtVol[:-1][indices] = self.maxVolumeChange / (10 * (4*np.pi*self.Rad[:,i][indices]**3*self.nucRate[:,i][indices]/3))
                 dt = np.amin(dtVol)
                 dtAll.append(dt)
 
+            if self.checkCompositionPre:
+                dtComp = dt * np.ones(self.numberOfElements + 1)
+                fvsum = np.sum(self.betaFrac[:,i-1])
+                xbavg = np.zeros(self.numberOfElements)
+                if self.numberOfElements == 1:
+                    xbavg[0] = 0 if fvsum == 0 else (self.xComp[0] - self.xComp[i-1] * (1 - fvsum)) / fvsum
+                    dxadt = (self.xComp[i-1] - xbavg) * np.sum(dV) / (1 - fvsum)
+                else:
+                    for e in range(self.numberOfElements):
+                        xbavg[e] = 0 if fvsum == 0 else (self.xComp[0,e] - self.xComp[i-1,e] * (1 - fvsum)) / fvsum
+                    dxadt = (self.xComp[i-1,:] - xbavg) * np.sum(dV) / (1 - fvsum)
+                dxadt[dxadt == 0] = self.maxCompositionChange / (2 * dt)
+                dtComp[:self.numberOfElements] = self.maxCompositionChange / (2 * dxadt)
+                    
+                dt = np.amin(dtComp)
+                dtAll.append(dt)
+
         #Minimum dt is the lower of the minimum allowed time increment or the time to the next pre-defined increment
         minDT = self._calculateDT(i-1, self.minDTFraction)
         dt = np.amax([dt, minDT])
 
         #Override time increment with the predefined time steps
         #This prevents the next time increment from becoming 0 or negative
         dt = np.amin([dt, self.time[i] - self.time[i-1]])
@@ -497,14 +643,16 @@
         '''
         Function if no adaptive time stepping is used, no need to do anything in this function
         '''
         return True
 
     def _postCheckDT(self, i):
         '''
+        CURRENTLY UNUSED AND MAY BE REMOVED LATER
+
         If adaptive time step is used, this checks new values at iteration i
         and compares with simulation contraints
 
         If contraints are not met, then remove current values and divide time step
         '''
         #Only perform checks in non-isothermal situations
         if np.abs(self.T[i] - self.T[i-1]) > 1:
@@ -520,17 +668,17 @@
             volChange[self.betaFrac[:,i] == 0] = 0
             volCheck = np.amax(volChange) < self.maxVolumeChange
         else:
             volCheck = True
 
         if self.checkComposition:
             if self.numberOfElements == 1:
-                compCheck = np.abs(self.xComp[i] - self.xComp[i-1]) < self.maxCompositionChange
+                compCheck = (np.abs(self.xComp[i] - self.xComp[i-1]) < self.maxCompositionChange) & (self.xComp[i] > 0)
             else:
-                compCheck = np.amax(np.abs(self.xComp[i,:] - self.xComp[i-1,:])) < self.maxCompositionChange
+                compCheck = (np.amax(np.abs(self.xComp[i,:] - self.xComp[i-1,:])) < self.maxCompositionChange) & (np.amin(self.xComp[i,:] > self.minComposition))
         else:
             compCheck = True
 
         checks = [volCheck, compCheck]
 
         #If any test fails, then reset iteration and divide time increment
         if not all(checks):
@@ -691,14 +839,15 @@
             if np.sum(fBeta) < 1:
                 self.xComp[i] = (self.xComp[0] - np.sum(fConc)) / (1 - np.sum(fBeta))
             else:
                 self.xComp[i] = 0
         else:
             if np.sum(fBeta) < 1:
                 self.xComp[i] = (self.xComp[0] - np.sum(fConc, axis=0)) / (1 - np.sum(fBeta))
+                self.xComp[i][self.xComp[i] < 0] = self.minComposition
             else:
                 self.xComp[i] = np.zeros(self.numberOfElements)
 
     def _singleGrowthBinary(self, i, p):
         '''
         Calculates growth rate for a single phase
         This is separated from _growthRateBinary since it's used in _calculatePSD
@@ -745,15 +894,15 @@
         Calculates growth rate for a single phase
         This is separated from _growthRateMulti since it's used in _calculatePSD
 
         This will also calculate the matrix/precipitate composition 
         for the radius in the PSD as well as equilibrium (infinite radius)
         '''
         growth, xAlpha, xBeta, xEqAlpha, xEqBeta = self.interfacialComposition[p](self.xComp[i-1], self.T[i], self.dGs[p,i-1] * self.VmBeta[p], self.PBM[p].PSDbounds, self.particleGibbs(phase=self.phases[p]))
-            
+
         #If two-phase equilibrium not found, two possibilities - precipitates are unstable or equilibrium calculations didn't converge
         if growth is None:
             #If driving force is negative, then precipitates are unstable
             if self.dGs[p,i] < 0:
                 #Completely reset the PBM, including bounds and number of bins
                 #In case nucleation occurs again, the PBM will be at a good length scale
                 self.PBM[p].reset()
@@ -781,15 +930,14 @@
     def _growthRateMulti(self, i):
         '''
         Determines current growth rate of all particle size classes in a multicomponent system
         '''
         growthRate = []
         for p in range(len(self.phases)):
             growthRate.append(self._singleGrowthMulti(i, p))
-
         self.growth = growthRate
 
     def plot(self, axes, variable, bounds = None, timeUnits = 's', radius='spherical', *args, **kwargs):
         '''
         Plots model outputs
         
         Parameters
```

### Comparing `kawin-0.1.2/kawin/LebedevNodes.py` & `kawin-0.2.0/kawin/LebedevNodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,27 @@
     ('D', 0.000189012564173, [0.04721844302802548, 1.5339564539800772, 0.9083862717504001], [0.6629509471710564, 0.9087154003228725, 1.5417426633033782]), \
     ('D', 0.00018994346378, [0.08997265710953405, 1.4944671446274873, 0.8676295668072698], [0.7051665794239899, 0.8690675011500809, 1.512525264138776]), \
     ('D', 0.000190452085683, [0.12882242002665842, 1.4520953569378034, 0.8266854191783667], [0.7482584375378902, 0.8302031182301477, 1.4832808075024158]), \
     ('D', 0.000190553449873, [0.043090374834379094, 1.5311012100198818, 0.8264346362389648], [0.7448244839219743, 0.8268273262435484, 1.541592714558998]) \
 ]
 
 def loadPoints(order):
+    '''
+    Load lebedov nodes of specific order
+
+    Parameters
+    ----------
+    order : int
+        Can be 53, 83 or 131
+        Determines the order of polynomial at which an exact integral solution can be found
+
+    Returns
+    -------
+    phi coordinates, theta coordinates, weights
+    '''
     if order == 53:
         node = q53
     elif order == 83:
         node = q83
     else:
         node = q131
```

### Comparing `kawin-0.1.2/kawin/LocalEquilibrium.py` & `kawin-0.2.0/kawin/LocalEquilibrium.py`

 * *Files identical despite different names*

### Comparing `kawin-0.1.2/kawin/Mobility.py` & `kawin-0.2.0/kawin/Mobility.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,18 +39,32 @@
         self.mob_site_fractions = {c: sorted([x for x in self.mobility_variables[c] if isinstance(x, v.SiteFraction)], key=str) for c in self.mobility}
         self.diff_site_fractions = {c: sorted([x for x in self.diffusivity_variables[c] if isinstance(x, v.SiteFraction)], key=str) for c in self.diffusivity}
         self.mob_state_variables = {c: sorted([x for x in self.mobility_variables[c] if not isinstance(x, v.SiteFraction)], key=str) for c in self.mobility}
         self.diff_state_variables = {c: sorted([x for x in self.diffusivity_variables[c] if not isinstance(x, v.SiteFraction)], key=str) for c in self.diffusivity}
 
     @property
     def mobility_variables(self):
+        '''
+        List of variables in the mobility functions
+
+        Returns
+        -------
+        dictionary {component name (str) : variables (list)}
+        '''
         return {c: sorted([x for x in self.mobility[c].free_symbols if isinstance(x, v.StateVariable)], key=str) for c in self.mobility}
 
     @property
     def diffusivity_variables(self):
+        '''
+        List of variables in the diffusivity functions
+
+        Returns
+        -------
+        dictionary {component name (str) : variables (list)}
+        '''
         return {c: sorted([x for x in self.diffusivity[c].free_symbols if isinstance(x, v.StateVariable)], key=str) for c in self.diffusivity}
 
     def build_phase(self, dbe):
         '''
         Builds free energy and mobility/diffusivity models as abstract syntax tree
 
         Parameters
@@ -106,47 +120,69 @@
                 mob[c.name] = (1 / (v.R * v.T)) * exp((self.mob_models['MF'][c.name] + self.mob_models['MQ'][c.name]) / (v.R * v.T))
                 setattr(self, 'mob_'+str(c.name).upper(), mob[c.name])
                 diff[c.name] = exp((self.mob_models['DF'][c.name] + self.mob_models['DQ'][c.name]) / (v.R * v.T))
                 setattr(self, 'diff_' + str(c.name).upper(), diff[c.name])
 
         return mob, diff
 
-def tracer_diffusivity(composition_set, mobility_callables = None, mobility_correction = None):
+def mobility_from_composition_set(composition_set, mobility_callables = None, mobility_correction = None):
     '''
-    Computers tracer diffusivity for given equilibrium results
-    D = MRT
+    Computes mobility from equilibrium results
 
     Parameters
     ----------
     composition_set : pycalphad.core.composition_set.CompositionSet
     mobility_callables : dict
         Pre-computed mobility callables for each element
     mobility_correction : dict (optional)
         Factor to multiply mobility by for each given element (defaults to 1)
 
     Returns
     -------
-    Array of floats of diffusivity for each element (alphabetical order)
+    Array for floats for mobility of each element (alphabetical order)
     '''
     if mobility_callables is None:
         raise ValueError('mobility_callables is required')
 
-    R = 8.314
-    T = composition_set.dof[composition_set.phase_record.state_variables.index(v.T)]
     elements = list(composition_set.phase_record.nonvacant_elements)
 
     #Set mobility correction if not set
     if mobility_correction is None:
         mobility_correction = {A: 1 for A in elements}
     else:
         for A in elements:
             if A not in mobility_correction:
                 mobility_correction[A] = 1
 
-    return R * T * np.array([mobility_correction[elements[A]] * mobility_callables[elements[A]](composition_set.dof) for A in range(len(elements))])
+    return np.array([mobility_correction[elements[A]] * mobility_callables[elements[A]](composition_set.dof) for A in range(len(elements))])
+    
+
+def tracer_diffusivity(composition_set, mobility_callables = None, mobility_correction = None):
+    '''
+    Computes tracer diffusivity for given equilibrium results
+    D = MRT
+
+    Parameters
+    ----------
+    composition_set : pycalphad.core.composition_set.CompositionSet
+    mobility_callables : dict
+        Pre-computed mobility callables for each element
+    mobility_correction : dict (optional)
+        Factor to multiply mobility by for each given element (defaults to 1)
+
+    Returns
+    -------
+    Array of floats of diffusivity for each element (alphabetical order)
+    '''
+    if mobility_callables is None:
+        raise ValueError('mobility_callables is required')
+
+    R = 8.314
+    T = composition_set.dof[composition_set.phase_record.state_variables.index(v.T)]
+    return R * T * mobility_from_composition_set(composition_set, mobility_callables, mobility_correction)
 
 def tracer_diffusivity_from_diff(composition_set, diffusivity_callables = None, diffusivity_correction = None):
     '''
     Tracer diffusivity from diffusivity callables
 
     This will just return the Da as an array
 
@@ -191,29 +227,19 @@
         Factor to multiply mobility by for each given element (defaults to 1)
 
     Returns
     -------
     Matrix of floats
         Each index along an axis correspond to elements in alphabetical order
     '''
-    if mobility_callables is None:
-        raise ValueError('mobility_callables is required')
-
     elements = list(composition_set.phase_record.nonvacant_elements)
     X = composition_set.X
 
-    #Set mobility correction if not set
-    if mobility_correction is None:
-        mobility_correction = {A: 1 for A in elements}
-    else:
-        for A in elements:
-            if A not in mobility_correction:
-                mobility_correction[A] = 1
-
-    mob = np.array([X[A] * mobility_correction[elements[A]] * mobility_callables[elements[A]](composition_set.dof) for A in range(len(elements))])
+    computedMob = mobility_from_composition_set(composition_set, mobility_callables, mobility_correction)
+    mob = np.array([X[A] * computedMob[A] for A in range(len(elements))])
 
     mobMatrix = np.zeros((len(elements), len(elements)))
     for a in range(len(elements)):
         for b in range(len(elements)):
             if a == b:
                 mobMatrix[a, b] = (1 - X[a]) * mob[b]
             else:
```

### Comparing `kawin-0.1.2/kawin/PopulationBalance.py` & `kawin-0.2.0/kawin/PopulationBalance.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,24 +57,14 @@
         self.max = self.originalMax
 
         self.originalBins = bins
         self.setBinConstraints(bins, minBins, maxBins)
         
         self.reset()
 
-        #Hidden variable for use in KWNEuler when determining composition assuming no diffusion in precipitate
-        #Represents d(PSD)/dr * growth rate * dt
-        #I would like this variable to be in KWNEuler, but this way is much easier
-        self._fv = np.zeros(self.bins + 1)
-
-        #Hidden variable for use in KWNEuler when adaptive time stepping is enabled
-        #This allows for PSD to revert to its previous value if a time constraint is not met
-        self._prevPSD = np.zeros(self.bins)
-        self._prevPSDbounds = np.zeros(self.bins)
-
         self._adaptiveBinSize = True
 
     def setAdaptiveBinSize(self, adaptive):
         '''
         For Euler implementation, sets whether to change the bin size when 
         the number of filled bins > maxBins or < minBins
 
@@ -145,14 +135,24 @@
             self.max = self.originalMax
             self.bins = self.originalBins
         self.PSDbounds = np.linspace(self.min, self.max, self.bins+1)
         self.PSDsize = 0.5 * (self.PSDbounds[:-1] + self.PSDbounds[1:])
             
         self.PSD = np.zeros(self.bins)
 
+        #Hidden variable for use in KWNEuler when determining composition assuming no diffusion in precipitate
+        #Represents d(PSD)/dr * growth rate * dt
+        #I would like this variable to be in KWNEuler, but this way is much easier
+        self._fv = np.zeros(self.bins + 1)
+
+        #Hidden variable for use in KWNEuler when adaptive time stepping is enabled
+        #This allows for PSD to revert to its previous value if a time constraint is not met
+        self._prevPSD = np.zeros(self.bins)
+        self._prevPSDbounds = np.zeros(self.bins+1)
+
     def changeSizeClasses(self, cMin, cMax, bins = None, resetPSD = False):
         '''
         Changes the size classes and resets the PSD
         
         Parameters
         ----------
         cMin : float
@@ -457,20 +457,22 @@
             Note: this is for grain boundary nucleation where the
                 reported precipitate radius differs from the radius
                 determined by precipitate curvature
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
+        else:
+            scale = scale * np.ones(self.PSDsize)
 
         if fill:
             axes.fill_between(self.PSDsize * scale, self.PSD, np.zeros(len(self.PSD)), *args, **kwargs)
         else:
             axes.plot(self.PSDsize * scale, self.PSD, *args, **kwargs)
-        self.setAxes(axes, logX, logY) 
+        self.setAxes(axes, scale, logX, logY) 
 
     def PlotDistributionDensity(self, axes, fill = False, logX = False, logY = False, scale = 1, *args, **kwargs):
         '''
         Plots the distribution density as a curve
         Defined as N_i / (R_i+1/2 - R_i-1/2)
         
         Parameters
@@ -488,29 +490,31 @@
             Note: this is for grain boundary nucleation where the
                 reported precipitate radius differs from the radius
                 determined by precipitate curvature
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
+        else:
+            scale = scale * np.ones(self.PSDsize)
 
         if fill:
             axes.fill_between(self.PSDsize * scale, self.PSD, np.zeros(len(self.PSD)), *args, **kwargs)
         else:
             axes.plot(self.PSDsize * scale, self.PSD / (self.PSDbounds[1:] - self.PSDbounds[:-1]), *args, **kwargs)
         
         #Set x-limits
         if logX:
             if self.min == 0:
-                axes.set_xlim([self.PSDbounds[1], self.max])
+                axes.set_xlim([self.PSDbounds[1]*scale[0], self.max*scale[-1]])
             else:
-                axes.set_xlim([self.min, self.max])
+                axes.set_xlim([self.min*scale[0], self.max*scale[-1]])
             axes.set_xscale('log')
         else:
-            axes.set_xlim([self.min, self.max]) 
+            axes.set_xlim([self.min*scale[0], self.max*scale[-1]]) 
 
         #Set y-limits
         if logY:
             axes.set_ylim([1e-1, np.amax([1.1 * np.amax(self.PSD / (self.PSDbounds[1:] - self.PSDbounds[:-1])), 1])])
             axes.set_yscale('log')
         else:
             axes.set_ylim([0, np.amax([1.1 * np.amax(self.PSD / (self.PSDbounds[1:] - self.PSDbounds[:-1])), 1])])
@@ -541,20 +545,22 @@
         '''
         kernel = sts.gaussian_kde(self.PSDsize, bw_method = bw_method, weights = self.PSD)
         x = np.linspace(self.min, self.max, 1000)   
         y = kernel(x) * self.ZeroMoment() * (self.PSDbounds[1] - self.PSDbounds[0])
 
         if hasattr(scale, '__len__'):
             scale = np.interp(x, self.PSDbounds, scale)
+        else:
+            scale = scale * np.ones(x)
         
         if fill:
             axes.fill_between(x * scale, y, np.zeros(len(y)), *args, **kwargs)
         else:
             axes.plot(x * scale, y, *args, **kwargs)
-        self.setAxes(axes, logX, logY) 
+        self.setAxes(axes, scale, logX, logY) 
             
     def PlotHistogram(self, axes, outline = 'outline bins', fill = True, logX = False, logY = False, scale = 1, *args, **kwargs):
         '''
         Plots the PSD as a histogram
         
         Parameters
         ----------
@@ -583,22 +589,24 @@
         else:
             xCoord, yCoord = np.zeros(1 + 2 * self.bins), np.zeros(1 + 2 * self.bins)
             xCoord[0], xCoord[1::2], xCoord[2::2] = self.PSDbounds[0], self.PSDbounds[:-1], self.PSDbounds[1:]
             yCoord[1::2], yCoord[2::2] = self.PSD, self.PSD
 
         if hasattr(scale, '__len__'):
             scale = np.interp(xCoord, self.PSDbounds, scale)
+        else:
+            scale = scale * np.ones(xCoord)
 
         if outline != 'no outline':
             axes.plot(xCoord * scale, yCoord, *args, **kwargs)
             if fill:
                 axes.fill_between(xCoord * scale, yCoord, np.zeros(len(yCoord)), alpha=0.3, *args, **kwargs)
         else:
             axes.fill_between(xCoord * scale, yCoord, np.zeros(len(yCoord)), *args, **kwargs)
-        self.setAxes(axes, logX, logY)
+        self.setAxes(axes, scale, logX, logY)
 
     def PlotCDF(self, axes, logX = False, scale = 1, order = 0, *args, **kwargs):
         '''
         Plots cumulative size distribution
         
         Parameters
         ----------
@@ -613,40 +621,42 @@
                 determined by precipitate curvature
         order : int (optional)
             Moment of specified order
         *args, **kwargs - extra arguments for plotting
         '''
         if hasattr(scale, '__len__'):
             scale = np.interp(self.PSDsize, self.PSDbounds, scale)
+        else:
+            scale = scale * np.ones(self.PSDsize)
 
         axes.plot(self.PSDsize * scale, self.CumulativeMoment(order) / self.Moment(order), *args, **kwargs)
-        self.setAxes(axes, logX, False) 
+        self.setAxes(axes, scale, logX, False) 
         axes.set_ylim([0, 1])
         
-    def setAxes(self, axes, logX = False, logY = False): 
+    def setAxes(self, axes, scale = 1, logX = False, logY = False): 
         '''
         Sets x- and y-axis to linear or log scale
         
         Parameters
         ----------
         axes : Axis
             Axis to plot on
         logX : bool (optional)
             Whether to set x-axis on log scale (defaults to False)
         logY : bool (optional)
             Whether to set y-axis on log scale (defaults to False)
         '''    
         if logX:
             if self.min == 0:
-                axes.set_xlim([self.PSDbounds[1], self.max])
+                axes.set_xlim([self.PSDbounds[1]*scale[0], self.max*scale[-1]])
             else:
-                axes.set_xlim([self.min, self.max])
+                axes.set_xlim([self.min*scale[0], self.max*scale[-1]])
             axes.set_xscale('log')
         else:
-            axes.set_xlim([self.min, self.max])
+            axes.set_xlim([self.min*scale[0], self.max*scale[-1]])
 
         #Don't set y limits if the PSD is empty
         if any(self.PSD > 0): 
             if logY:
                 axes.set_ylim([1e-1, np.amax([1.1 * np.amax(self.PSD), 1])])
                 axes.set_yscale('log')
             else:
```

### Comparing `kawin-0.1.2/kawin/ShapeFactors.py` & `kawin-0.2.0/kawin/ShapeFactors.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,18 +114,17 @@
         self.particleType = self.CUBIC
         self.setAspectRatio(ar)
         self._eqRadiusEquation = self._eqRadiusFactorCuboidal
         self._normalRadiiEquation = self._normalRadiiCuboidal
         self._kineticEquation = self._kineticFactorEquationCuboidal
         self._thermoEquation = self._thermoFactorEquationCuboidal
         
-        self.kineticFactorMin = 1
-        
-        #Thermodynamic factor for cuboidal precipitates is not 1 when aspect ratio is 1
+        #Thermodynamic and kinetic factor for cuboidal precipitates is not 1 when aspect ratio is 1
         self.thermoFactorMin = self._thermoFactorEquationCuboidal(1)
+        self.kineticFactorMin = self._kineticFactorEquationCuboidal(1.0001)
 
     def normalRadii(self, R):
         '''
         Radius along the 3 axis to give a spherical volume of 1
 
         Parameters
         ----------
```

### Comparing `kawin-0.1.2/kawin/Surrogate.py` & `kawin-0.2.0/kawin/Surrogate.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,15 +262,17 @@
         self.DGfunction = function
         self.DGepsilon = epsilon
         self.DGsmooth = np.amax([smooth, self.eps])
         
         self._createDGSurrogate()
 
     def _createDGSurrogate(self):
-        #Build surrogates
+        '''
+        Build surrogates for driving force
+        '''
         if self.linearDG:
             self.SurrogateDrivingForce = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
             self.SurrogatePrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
         else:
             self.linearDG = False
             self.LogSurrDG = Rbf(self.dGcoords[:,0], self.dGcoords[:,1], self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
             self.LogSurrPrecComp = Rbf(self.precCompCoords[:,0], self.precCompCoords[:,1], self.precComp, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
@@ -519,15 +521,17 @@
         self.ICfunction = function
         self.ICepsilon = epsilon
         self.ICsmooth = np.amax([smooth, self.eps])
 
         self._createICSurrogate()
 
     def _createICSurrogate(self):
-        #Build surrogates
+        '''
+        Build surrogates for interfacial composition
+        '''
         if self.linearIC:
             self.SurrogateParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xParent, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
             self.SurrogatePrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], self.xPrec, function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)  
         else:
             self.LogSurrParent = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xParent), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth)
             self.LogSurrPrec = Rbf(self.ICcoords[:,0], self.ICcoords[:,1], np.log10(self.xPrec), function = self.ICfunction, epsilon = self.ICepsilon, smooth=self.ICsmooth) 
             
@@ -688,14 +692,17 @@
         self.Difffunction = function
         self.Diffepsilon = epsilon
         self.Diffsmooth = np.amax([smooth, self.eps])
 
         self._createDiffSurrogate()
 
     def _createDiffSurrogate(self):
+        '''
+        Builds surrogate for diffusivity
+        '''
         #If only 1 data point, then create constant function
         if len(self.Diff) == 1:
             self.SurrogateDiff = lambda x, T: self.Diff[0]
             return
 
         #Build surrogates
         if self.linearDiff:
@@ -1093,15 +1100,17 @@
         self.DGfunction = function
         self.DGepsilon = epsilon
         self.DGsmooth = np.amax([smooth, self.eps])
 
         self._createDGSurrogate()
 
     def _createDGSurrogate(self):
-        #Build surrogates
+        '''
+        Builds surrogate for driving force
+        '''
         if self.linearDG:
             arguments = [self.dGcoords[:,i] for i in range(len(self.dGcoords[0]))]
             self.SurrogateDrivingForce = Rbf(*arguments, self.drivingForce, function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth)
             
             arguments = [self.precCompCoords[:,i] for i in range(len(self.dGcoords[0]))]
             self.SurrPrecComp = [Rbf(*arguments, self.precComp[:,i], function=self.DGfunction, epsilon=self.DGepsilon, smooth=self.DGsmooth) for i in range(len(self.elements))]
             self.SurrogatePrecComp = lambda x, T: np.array([self.SurrPrecComp[i](*x, T) for i in range(len(self.elements))])
@@ -1295,15 +1304,17 @@
         self.ICfunction = function
         self.ICepsilon = epsilon
         self.ICsmooth = np.amax([smooth, self.eps])
 
         self._createICSurrogate()
 
     def _createICSurrogate(self):
-        #Build surrogates
+        '''
+        Builds surrogate for interfacial composition and curvature
+        '''
         if self.linearIC:
             arguments = [self.ICcoords[:,i] for i in range(len(self.ICcoords[0]))]
             self.SurrogateMc = Rbf(*arguments, self.Mc, function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth)
             self.SurrogateBeta = Rbf(*arguments, self.beta, function=self.ICfunction, epislon=self.ICepsilon, smooth=self.ICsmooth)
 
             self.SurrDc = [Rbf(*arguments, self.Dc[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
             self.SurrCa = [Rbf(*arguments, self.Ca[:,i], function=self.ICfunction, epsilon=self.ICepsilon, smooth=self.ICsmooth) for i in range(len(self.elements))]
```

### Comparing `kawin-0.1.2/kawin/Thermodynamics.py` & `kawin-0.2.0/kawin/Thermodynamics.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,125 +26,133 @@
     orderingContribution = OCM = property(lambda self: self.models['ord'])
 
 class GeneralThermodynamics:
     '''
     Class for defining driving force and essential functions for
     binary and multicomponent systems using pycalphad for equilibrium
     calculations
-    
+
     Parameters
     ----------
-    database : str
-        File name for database
+    database : Database or str
+        pycalphad Database or file name for database
     elements : list
         Elements to consider
         Note: reference element must be the first index in the list
     phases : list
         Phases involved
         Note: matrix phase must be first index in the list
     drivingForceMethod : str (optional)
         Method used to calculate driving force
         Options are 'approximate' (default), 'sampling' and 'curvature' (not recommended)
     '''
 
     gOffset = 1      #Small value to add to precipitate phase for when order/disorder models are used
 
     def __init__(self, database, elements, phases, drivingForceMethod = 'approximate'):
-        self.db = Database(database)
-        self.elements = elements
+        if isinstance(database, str):
+            database = Database(database)
+        self.db = database
+        self.elements = copy.copy(elements)
 
         if 'VA' not in self.elements:
             self.elements.append('VA')
-            
+
+        if type(phases) == str:  # check if a single phase was passed as a string instead of a list of phases.
+            phases = [phases]
         self.phases = phases
         self.orderedPhase = {phases[i]: False for i in range(1, len(phases))}
         for i in range(1, len(phases)):
             if 'disordered_phase' in self.db.phases[phases[i]].model_hints:
                 if self.db.phases[phases[i]].model_hints['disordered_phase'] == self.phases[0]:
                     self.orderedPhase[phases[i]] = True
                     self._forceDisorder(self.phases[0])
-        
+
         #Build phase models assuming first phase is parent phase and rest of precipitate phases
         #If the same phase is used for matrix and precipitate phase, then force the matrix phase to remove the ordering contribution
         #This may be unnecessary as already disordered phase models will not be affected, but I guess just in case the matrix phase happens to be an ordered solution
         self.models = {self.phases[0]: Model(self.db, self.elements, self.phases[0])}
         self.models[self.phases[0]].state_variables = sorted([v.T, v.P, v.N, v.GE], key=str)
 
         for i in range(1, len(phases)):
             self.models[self.phases[i]] = ExtraGibbsModel(self.db, self.elements, self.phases[i])
             self.models[self.phases[i]].state_variables = sorted([v.T, v.P, v.N, v.GE], key=str)
 
         self.phase_records = build_phase_records(self.db, self.elements, self.phases,
                                                  self.models[self.phases[0]].state_variables,
                                                  self.models, build_gradients=True, build_hessians=True)
-        
+
         self.OCMphase_records = {}
         for i in range(1, len(self.phases)):
             if self.orderedPhase[self.phases[i]]:
-                self.OCMphase_records[self.phases[i]] = build_phase_records(self.db, self.elements, [self.phases[i]], 
+                self.OCMphase_records[self.phases[i]] = build_phase_records(self.db, self.elements, [self.phases[i]],
                                                                             self.models[self.phases[0]].state_variables,
-                                                                            {self.phases[i]: self.models[self.phases[i]]}, 
+                                                                            {self.phases[i]: self.models[self.phases[i]]},
                                                                             output='OCM', build_gradients=False, build_hessians=False)
 
 
         #Amount of points to sample per degree of freedom
         # sampling_pDens is for when using sampling method in driving force calculations
         # pDens is for equilibrium calculations
         self.sampling_pDens = 2000
         self.pDens = 500
-        
+
         #Stored variables of last time the class was used
         #This is so that these can be used again if the temperature has not changed since last usage
         self._prevTemperature = None
-        
+
         #Pertains to parent phase (composition, sampled points, equilibrium calculations)
         self._prevX = None
-        self._pointsParent = None
         self._parentEq = None
 
         #Pertains to precipitate phases (sampled points)
         self._pointsPrec = {self.phases[i]: None for i in range(1, len(self.phases))}
         self._orderingPoints = {self.phases[i]: None for i in range(1, len(self.phases))}
 
         self.setDrivingForceMethod(drivingForceMethod)
 
-        #Get mobility/diffusivity if exists
-        param_search = self.db.search
-        param_query_mob = (
-            (where('phase_name') == self.phases[0]) & \
-            (where('parameter_type') == 'MQ') | \
-            (where('parameter_type') == 'MF')
-        )
-
-        param_query_diff = (
-            (where('phase_name') == self.phases[0]) & \
-            (where('parameter_type') == 'DQ') | \
-            (where('parameter_type') == 'DF')
-        )
-
-        pMob = param_search(param_query_mob)
-        pDiff = param_search(param_query_diff)
-        self.mobModels = None
-        self.mobCallables = {} if len(pMob) > 0 else None
-        self.diffCallables = {} if len(pDiff) > 0 else None
-        if len(pMob) > 0 or len(pDiff) > 0:
-            self.mobModels = MobilityModel(self.db, self.elements, self.phases[0])
-            if len(pMob) > 0:
-                for c in self.phase_records[self.phases[0]].nonvacant_elements:
-                    bcp = build_callables(self.db, self.elements, [self.phases[0]], {self.phases[0]: self.mobModels},
-                                          parameter_symbols=None, output='mob_'+c, build_gradients=False, build_hessians=False,
-                                          additional_statevars=[v.T, v.P, v.N, v.GE])
-                    self.mobCallables[c] = bcp['mob_'+c]['callables'][self.phases[0]]
-            else:
-                for c in self.phase_records[self.phases[0]].nonvacant_elements:
-                    bcp = build_callables(self.db, self.elements, [self.phases[0]], {self.phases[0]: self.mobModels},
-                                          parameter_symbols=None, output='diff_'+c, build_gradients=False, build_hessians=False,
-                                          additional_statevars=[v.T, v.P, v.N, v.GE])
-                    self.diffCallables[c] = bcp['diff_'+c]['callables'][self.phases[0]]
+        self.mobModels = {p: None for p in self.phases}
+        self.mobCallables = {p: None for p in self.phases}
+        self.diffCallables = {p: None for p in self.phases}
+        for p in self.phases:
+            #Get mobility/diffusivity of phase p if exists
+            param_search = self.db.search
+            param_query_mob = (
+                (where('phase_name') == p) & \
+                (where('parameter_type') == 'MQ') | \
+                (where('parameter_type') == 'MF')
+            )
+
+            param_query_diff = (
+                (where('phase_name') == p) & \
+                (where('parameter_type') == 'DQ') | \
+                (where('parameter_type') == 'DF')
+            )
+
+            pMob = param_search(param_query_mob)
+            pDiff = param_search(param_query_diff)
+
+            if len(pMob) > 0 or len(pDiff) > 0:
+                self.mobModels[p] = MobilityModel(self.db, self.elements, p)
+                if len(pMob) > 0:
+                    self.mobCallables[p] = {}
+                    for c in self.phase_records[p].nonvacant_elements:
+                        bcp = build_callables(self.db, self.elements, [p], {p: self.mobModels[p]},
+                                            parameter_symbols=None, output='mob_'+c, build_gradients=False, build_hessians=False,
+                                            additional_statevars=[v.T, v.P, v.N, v.GE])
+                        self.mobCallables[p][c] = bcp['mob_'+c]['callables'][p]
+                else:
+                    self.diffCallables[p] = {}
+                    for c in self.phase_records[p].nonvacant_elements:
+                        bcp = build_callables(self.db, self.elements, [p], {p: self.mobModels[p]},
+                                            parameter_symbols=None, output='diff_'+c, build_gradients=False, build_hessians=False,
+                                            additional_statevars=[v.T, v.P, v.N, v.GE])
+                        self.diffCallables[p][c] = bcp['diff_'+c]['callables'][p]
 
+        #This applies to all phases since this is typically reflective of quenched-in vacancies
         self.mobility_correction = {A: 1 for A in self.elements}
 
         #Cached results
         self._compset_cache = {}
         self._compset_cache_df = {}
         self._matrix_cs = None
 
@@ -174,15 +182,15 @@
             newP['phase_name'] = newPhase
             self.db._parameters.insert(newP)
 
     def clearCache(self):
         '''
         Removes any cached data
         This is intended for surrogate training, where the cached data
-        will be removed incase 
+        will be removed incase
         '''
         self._compset_cache = {}
         self._compset_cache_df = {}
         self._matrix_cs = None
 
     def setDrivingForceMethod(self, drivingForceMethod):
         '''
@@ -197,15 +205,15 @@
             self._drivingForce = self._getDrivingForceApprox
         elif drivingForceMethod == 'sampling':
             self._drivingForce = self._getDrivingForceSampling
         elif drivingForceMethod == 'curvature':
             self._drivingForce = self._getDrivingForceCurvature
         else:
             raise Exception('Driving force method must be either \'approximate\', \'sampling\' or \'curvature\'')
-    
+
     def setDFSamplingDensity(self, density):
         '''
         Sets sampling density for sampling method in driving
         force calculations
 
         Default upon initialization is 2000
 
@@ -229,24 +237,24 @@
             Number of samples to take per degree of freedom in the phase
         '''
         self.pDens = density
 
     def setMobility(self, mobility):
         '''
         Allows user to define mobility functions
-    
+
         mobility : dict
             Dictionary of functions for each element (including reference)
             Each function takes in (v.T, v.P, v.N, v.GE, site fractions) and returns mobility
 
         Optional - only required for multicomponent systems where
             mobility terms are not defined in the TDB database
         '''
         self.mobCallables = mobility
-    
+
     def setDiffusivity(self, diffusivity):
         '''
         Allows user to define diffusivity functions
 
         diffusivity : dict
             Dictionary of functions for each element (including reference)
             Each function takes in (v.T, v.P, v.N, v.GE, site fractions) and returns diffusivity
@@ -271,14 +279,61 @@
         '''
         if element == 'all':
             for e in self.mobility_correction:
                 self.mobility_correction[e] = factor
         else:
             self.mobility_correction[element] = factor
 
+    def _getConditions(self, x, T, gExtra = 0):
+        '''
+        Creates dictionary of conditions from composition, temperature and gExtra
+
+        Parameters
+        ----------
+        x : list
+            Composition (excluding reference element)
+        T : float
+            Temperature
+        gExtra : float
+            Gibbs free energy to add to phase
+        '''
+        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
+        cond[v.P] = 101325
+        cond[v.T] = T
+        cond[v.GE] = gExtra
+        cond[v.N] = 1
+        return cond
+
+    def _createCompositionSet(self, eq, state_variables, phase, phase_amounts, idx):
+        '''
+        Creates a pycalphad CompositionSet from equilibrium results
+
+        Parameters
+        ----------
+        eq : pycalphad equilibrium result
+        state_variables : list
+            List of state variables
+        phase : str
+            Phase to create CompositionSet for
+        phase_amounts : list
+            Array of floats for phase fraction of each phase
+        idx : ndarray
+            Index array for the index of phase
+        '''
+        miscibility = False
+        cs = CompositionSet(self.phase_records[phase])
+        #If there's a miscibility gap in the matrix phase, then take the largest value
+        if len(idx) > 1:
+            idx = [idx[np.argmax(phase_amounts[idx])]]
+            miscibility = True
+        cs.update(eq.Y.isel(vertex=idx).values.ravel()[:cs.phase_record.phase_dof],
+                        phase_amounts[idx], state_variables)
+
+        return cs, miscibility
+
     def getEq(self, x, T, gExtra = 0, precPhase = None):
         '''
         Calculates equilibrium at specified x, T, gExtra
 
         This is separated from the interfacial composition function so that this can be used for getting curvature for interfacial composition from mobility
 
         Parameters
@@ -293,117 +348,235 @@
         precPhase : str
             Precipitate phase (default is first precipitate)
 
         Returns
         -------
         Dataset from pycalphad equilibrium results
         '''
-        if precPhase is None:
-            precPhase = self.phases[1]
+        phases = [self.phases[0]]
+        if precPhase != -1:
+            if precPhase is None:
+                precPhase = self.phases[1]
+            if isinstance(precPhase, str):
+                phases.append(precPhase)
+            else:
+                phases = [p for p in precPhase]
+        phaseRec = {p: self.phase_records[p] for p in phases}
+
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-        if hasattr(x, '__len__'):
-            #Remove first element if x lists composition of all elements
-            if len(x) == len(self.elements) - 1:
-                x = x[1:]
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
 
-            cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        else:
-            cond = {v.X(self.elements[1]): x}
-        cond[v.P] = 101325
-        cond[v.T] = T
-        cond[v.GE] = gExtra + self.gOffset
+        cond = self._getConditions(x, T, gExtra+self.gOffset)
 
-        eq = equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond, model=self.models, 
-                         phase_records={self.phases[0]: self.phase_records[self.phases[0]], precPhase: self.phase_records[precPhase]}, 
+        eq = equilibrium(self.db, self.elements, phases, cond, model=self.models, 
+                         phase_records=phaseRec, 
                          calc_opts={'pdens': self.pDens})
         return eq
 
-    def getInterdiffusivity(self, x, T):
+    def getLocalEq(self, x, T, gExtra = 0, precPhase = None, composition_sets = None):
+        phases = [self.phases[0]]
+        if precPhase != -1:
+            if precPhase is None:
+                precPhase = self.phases[1]
+            if isinstance(precPhase, str):
+                phases.append(precPhase)
+            else:
+                phases = [p for p in precPhase]
+
+        if not hasattr(x, '__len__'):
+            x = [x]
+
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+
+        cond = self._getConditions(x, T, gExtra)
+        result, composition_sets = local_equilibrium(self.db, self.elements, phases, cond,
+                                                         self.models, self.phase_records,
+                                                         composition_sets=composition_sets)
+        return result, composition_sets
+
+    def getInterdiffusivity(self, x, T, removeCache = True, phase = None):
         '''
         Gets interdiffusivity at specified x and T
         Requires TDB database to have mobility or diffusivity parameters
 
         Parameters
         ----------
         x : float, array or 2D array
             Composition
             Float or array for binary systems
             Array or 2D array for multicomponent systems
         T : float or array
             Temperature
             If array, must be same length as x
                 For multicomponent systems, must be same length as 0th axis
+        removeCache : boolean
+            If True, recalculates equilibrium to get interdiffusivity (default)
+            If False, will use calculation from driving force calcs (if available) to compute diffusivity
+        phase : str
+            Phase to compute diffusivity for (defaults to first or matrix phase)
+            This only needs to be used for multiphase diffusion simulations
 
         Returns
         -------
         interdiffusivity - will return array if T is an array
             For binary case - float or array of floats
             For multicomponent - matrix or array of matrices
         '''
         dnkj = []
 
         if hasattr(T, '__len__'):
             for i in range(len(T)):
-                dnkj.append(self._interdiffusivitySingle(x[i], T[i]))
+                dnkj.append(self._interdiffusivitySingle(x[i], T[i], removeCache, phase))
             return np.array(dnkj)
         else:
-            return self._interdiffusivitySingle(x, T)
+            return self._interdiffusivitySingle(x, T, removeCache, phase)
 
-    def _interdiffusivitySingle(self, x, T):
+    def _interdiffusivitySingle(self, x, T, removeCache = True, phase = None):
         '''
         Gets interdiffusivity at unique composition and temperature
 
         Parameters
         ----------
         x : float or array
             Composition
         T : float
             Temperature
-        
+        removeCache : boolean
+        phase : str
+
         Returns
         -------
         Interdiffusivity as a matrix (will return float in binary case)
         '''
+        if phase is None:
+            phase = self.phases[0]
+
         if not hasattr(x, '__len__'):
             x = [x]
-        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        cond[v.P] = 101325
-        cond[v.T] = T
-        cond[v.GE] = 0
-        cond['N'] = 1
-        eqPh = equilibrium(self.db, self.elements, self.phases[0], cond, model=self.models, phase_records={self.phases[0]: self.phase_records[self.phases[0]]}, calc_opts = {'pdens': self.pDens})
-
-        state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
-        stable_phases = eqPh.Phase.values.ravel()
-        phase_amounts = eqPh.NP.values.ravel()
-        matrix_idx = np.where(stable_phases == self.phases[0])[0]
-
-        cs_matrix = CompositionSet(self.phase_records[self.phases[0]])
-        cs_matrix.update(eqPh.Y.isel(vertex=matrix_idx).values.ravel()[:cs_matrix.phase_record.phase_dof],
-                            phase_amounts[matrix_idx], state_variables)
-        chemical_potentials = eqPh.MU.values.ravel()
 
-        if self.mobCallables is None:
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+
+        cond = self._getConditions(x, T, 0)
+
+        if removeCache:
+            self._matrix_cs = None
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [phase], cond,
+                                                        self.models, self.phase_records,
+                                                        composition_sets=self._matrix_cs)
+
+        cs_matrix = [cs for cs in self._matrix_cs if cs.phase_record.phase_name == phase][0]
+        chemical_potentials = self._parentEq.chemical_potentials
+
+        if self.mobCallables[phase] is None:
             Dnkj, _, _ = inverseMobility_from_diffusivity(chemical_potentials, cs_matrix,
-                                                                            self.elements[0], self.diffCallables,
+                                                                            self.elements[0], self.diffCallables[phase],
                                                                             diffusivity_correction=self.mobility_correction)
         else:
             Dnkj, _, _ = inverseMobility(chemical_potentials, cs_matrix, self.elements[0],
-                                                        self.mobCallables,
+                                                        self.mobCallables[phase],
                                                         mobility_correction=self.mobility_correction)
 
         if len(x) == 1:
             return Dnkj.ravel()[0]
         else:
             sortIndices = np.argsort(self.elements[1:-1])
             unsortIndices = np.argsort(sortIndices)
             Dnkj = Dnkj[unsortIndices,:]
             Dnkj = Dnkj[:,unsortIndices]
             return Dnkj
-            
+
+
+    def getTracerDiffusivity(self, x, T, removeCache = True, phase = None):
+        '''
+        Gets tracer diffusivity for element el at specified x and T
+        Requires TDB database to have mobility or diffusivity parameters
+
+        Parameters
+        ----------
+        x : float, array or 2D array
+            Composition
+            Float or array for binary systems
+            Array or 2D array for multicomponent systems
+        T : float or array
+            Temperature
+            If array, must be same length as x
+                For multicomponent systems, must be same length as 0th axis
+        removeCache : boolean
+        phase : str
+
+        Returns
+        -------
+        tracer diffusivity - will return array if T is an array
+        '''
+        td = []
+
+        if hasattr(T, '__len__'):
+            for i in range(len(T)):
+                td.append(self._tracerDiffusivitySingle(x[i], T[i], removeCache, phase))
+            return np.array(td)
+        else:
+            return self._tracerDiffusivitySingle(x, T, removeCache, phase)
+
+    def _tracerDiffusivitySingle(self, x, T, removeCache = True, phase = None):
+        '''
+        Gets tracer diffusivity at unique composition and temperature
+
+        Parameters
+        ----------
+        x : float or array
+            Composition
+        T : float
+            Temperature
+        el : str
+            Element to calculate diffusivity
+        
+        Returns
+        -------
+        Tracer diffusivity as a float
+        '''
+        if phase is None:
+            phase = self.phases[0]
+
+        if not hasattr(x, '__len__'):
+            x = [x]
+
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+
+        cond = self._getConditions(x, T, 0)
+
+        if removeCache:
+            self._matrix_cs = None
+            self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [phase], cond,
+                                                        self.models, self.phase_records,
+                                                        composition_sets=self._matrix_cs)
+
+        cs_matrix = [cs for cs in self._matrix_cs if cs.phase_record.phase_name == phase][0]
+
+        if self.mobCallables[phase] is None:
+            #NOTE: This is note tested yet
+            Dtrace = tracer_diffusivity_from_diff(cs_matrix, self.diffCallables[phase], diffusivity_correction=self.mobility_correction)
+        else:
+            Dtrace = tracer_diffusivity(cs_matrix, self.mobCallables[phase], mobility_correction=self.mobility_correction)
+
+        sortIndices = np.argsort(self.elements[:-1])
+        unsortIndices = np.argsort(sortIndices)
+
+        Dtrace = Dtrace[unsortIndices]
+
+        return Dtrace
 
     def getDrivingForce(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
         Gets driving force using method defined upon initialization
 
         Parameters
         ----------
@@ -438,15 +611,15 @@
             return dgArray, compArray
         else:
             return self._drivingForce(x, T, precPhase, returnComp, training)
 
     def _getDrivingForceSampling(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
         Gets driving force for nucleation by sampling
-        
+
         Parameters
         ----------
         x : float or array
             Composition of minor element in bulk matrix phase
             Use float for binary systems
             Use array for multicomponent systems
         T : float
@@ -463,49 +636,45 @@
         Precipitate composition will be None if driving force is negative or returnComp is False
         '''
         precPhase = self.phases[1] if precPhase is None else precPhase
 
         #Calculate equilibrium with only the parent phase -------------------------------------------------------------------------------------------
         if not hasattr(x, '__len__'):
             x = [x]
-        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        cond[v.P] = 101325
-        cond[v.T] = T
-        cond[v.GE] = 0
-        cond['N'] = 1
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
 
         #Equilibrium at matrix composition for only the parent phase
-        self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond, 
-                                                            self.models, self.phase_records, 
+        self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond,
+                                                            self.models, self.phase_records,
                                                             composition_sets = self._matrix_cs)
+
         #Remove cache when training
         if training:
             self._matrix_cs = None
 
-        self._prevX = x
-
         #Check if equilibrium has converged and chemical potential can be obtained
         #If not, then return None for driving force
         if any(np.isnan(self._parentEq.chemical_potentials)):
             return None, None
 
         #Sample precipitate phase and get driving force differences at all points -------------------------------------------------------------------
         #Sample points of precipitate phase
         if self._pointsPrec[precPhase] is None or self._prevTemperature != T:
             self._pointsPrec[precPhase] = calculate(self.db, self.elements, precPhase, P = 101325, T = T, GE=self.gOffset, pdens = self.sampling_pDens, model=self.models, output='GM', phase_records=self.phase_records)
             if self.orderedPhase[precPhase]:
                 self._orderingPoints[precPhase] = calculate(self.db, self.elements, precPhase, P = 101325, T = T, GE=self.gOffset, pdens = self.sampling_pDens, model=self.models, output='OCM', phase_records=self.OCMphase_records[precPhase])
             self._prevTemperature = T
-            
+
         #Get value of chemical potential hyperplane at composition of sampled points
         precComp = self._pointsPrec[precPhase].X.values.ravel()
         precComp = precComp.reshape((int(len(precComp) / (len(self.elements) - 1)), len(self.elements) - 1))
         mu = np.array([self._parentEq.chemical_potentials])
         mult = precComp * mu
-        
+
         #Difference between the chemical potential hyperplane and the samples points
         #The max driving force is the same as when the chemical potentials of the two phases are parallel
         diff = np.sum(mult, axis=1) - self._pointsPrec[precPhase].GM.values.ravel()
 
         #Find maximum driving force and corresponding composition -----------------------------------------------------------------------------------
         #For phases with order/disorder transition, a filter is applied such that it will only use points that are below the disordered energy surface
         if self.orderedPhase[precPhase]:
@@ -538,15 +707,15 @@
 
     def _getDrivingForceApprox(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
         Approximate method of driving force calculation
         Assumes equilibrium composition of precipitate phase
 
         Sampling method is used if driving force is negative
-        
+
         Parameters
         ----------
         x : float or array
             Composition of minor element in bulk matrix phase
             Use float for binary systems
             Use array for multicomponent systems
         T : float
@@ -563,56 +732,60 @@
         Precipitate composition will be None if driving force is negative or returnComp is False
         '''
         if precPhase is None:
             precPhase = self.phases[1]
 
         if not hasattr(x, '__len__'):
             x = [x]
-        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        cond[v.P] = 101325
-        cond[v.T] = T
-        cond[v.GE] = 0
-        cond[v.N] = 1
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
 
         #Create cache of composition set if not done so already or if training a surrogate
         #Training points for surrogates may be far apart, so starting from a previous
         #   composition set could give a bad starting position for the minimizer
         if self._compset_cache_df.get(precPhase, None) is None or training:
             #Calculate equilibrium ----------------------------------------------------------------------------------------------------------------------
             eq = self.getEq(x, T, 0, precPhase)
             #Cast values in state_variables to double for updating composition sets
             state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
             stable_phases = eq.Phase.values.ravel()
             phase_amounts = eq.NP.values.ravel()
             matrix_idx = np.where(stable_phases == self.phases[0])[0]
             precip_idx = np.where(stable_phases == precPhase)[0]
+            chemical_potentials = eq.MU.values.ravel()
+            x_precip = eq.isel(vertex=precip_idx).X.values.ravel()
 
             #If matrix phase is not stable, then use sampling method
             #   This may occur during surrogate training of interfacial composition,
             #   where we're trying to calculate the driving force at the precipitate composition
             #   In this case, the conditions will be at th precipitate composition which can result in
             #   only that phase being stable
             if len(matrix_idx) == 0:
                 return self._getDrivingForceSampling(x, T, precPhase, returnComp)
-            
+
             #Test that precipitate phase is stable and that we're not training a surrogate
             #If not, then there's no composition set to cache
             if len(precip_idx) > 0:
-                cs_matrix = CompositionSet(self.phase_records[self.phases[0]])
-                cs_matrix.update(eq.Y.isel(vertex=matrix_idx).values.ravel()[:cs_matrix.phase_record.phase_dof],
-                                phase_amounts[matrix_idx], state_variables)
-                cs_precip = CompositionSet(self.phase_records[precPhase])
-                cs_precip.update(eq.Y.isel(vertex=precip_idx).values.ravel()[:cs_precip.phase_record.phase_dof],
-                                phase_amounts[precip_idx], state_variables)
+                cs_matrix, miscMatrix = self._createCompositionSet(eq, state_variables, self.phases[0], phase_amounts, matrix_idx)
+                cs_precip, miscPrec = self._createCompositionSet(eq, state_variables, precPhase, phase_amounts, precip_idx)
+                x_precip = np.array(cs_precip.X)
+
                 composition_sets = [cs_matrix, cs_precip]
                 self._compset_cache_df[precPhase] = composition_sets
 
-            chemical_potentials = eq.MU.values.ravel()
-            ph = stable_phases[stable_phases != '']
-            x_precip = eq.isel(vertex=precip_idx).X.values.ravel()
+                if miscMatrix or miscPrec:
+                    result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
+                                                            self.models, self.phase_records,
+                                                            composition_sets=self._compset_cache_df[precPhase])
+                    self._compset_cache_df[precPhase] = composition_sets
+                    chemical_potentials = result.chemical_potentials
+                    cs_precip = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
+                    x_precip = np.array(cs_precip.X)
+
+            ph = np.unique(stable_phases[stable_phases != ''])
             ele = eq.component.values.ravel()
         else:
             result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
                                                          self.models, self.phase_records,
                                                          composition_sets=self._compset_cache_df[precPhase])
             self._compset_cache_df[precPhase] = composition_sets
             chemical_potentials = result.chemical_potentials
@@ -622,43 +795,42 @@
                 x_precip = np.array(cs_precip.X)
                 ele = list(cs_precip.phase_record.nonvacant_elements)
 
         #Check that equilibrium has converged
         #If not, then return None, None since driving force can't be obtained
         if any(np.isnan(chemical_potentials)):
             return None, None
-        
-        #If in two phase region, then calculate equilibrium using only parent phase and find free energy difference between chemical potential and free energy of preciptiate   
+
+        #If in two phase region, then calculate equilibrium using only parent phase and find free energy difference between chemical potential and free energy of preciptiate
         if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
             for i in range(len(ele)):
                 if ele[i] == self.elements[0]:
                     refIndex = i
                     break
 
             #Equilibrium at matrix composition for only the parent phase
             self._parentEq, self._matrix_cs = local_equilibrium(self.db, self.elements, [self.phases[0]], cond,
                                                                 self.models, self.phase_records,
                                                                 composition_sets=self._matrix_cs)
 
+
             #Remove caching if training surrogate in case training points are far apart
             if training:
                 self._matrix_cs = None
 
-            self._prevX = x
-
             #Check if equilibrium has converged and chemical potential can be obtained
             #If not, then return None for driving force
             if any(np.isnan(self._parentEq.chemical_potentials)):
                 return None, None
 
             sortIndices = np.argsort(self.elements[1:-1])
             unsortIndices = np.argsort(sortIndices)
 
             xP = x_precip
-            
+
             dg = np.sum(xP * self._parentEq.chemical_potentials) - np.sum(xP * chemical_potentials)
 
             #Remove reference element
             xP = np.delete(xP, refIndex)
 
             if returnComp:
                 if len(x) == 1:
@@ -673,15 +845,15 @@
 
     def _getDrivingForceCurvature(self, x, T, precPhase = None, returnComp = False, training = False):
         '''
         Gets driving force from curvature of free energy function
         Assumes small saturation
 
         Sampling method is used if driving force is negative
-        
+
         Parameters
         ----------
         x : float or array
             Composition of minor element in bulk matrix phase
             Use float for binary systems
             Use array for multicomponent systems
         T : float
@@ -698,69 +870,76 @@
         Precipitate composition will be None if driving force is negative or returnComp is False
         '''
         if precPhase is None:
             precPhase = self.phases[1]
 
         if not hasattr(x, '__len__'):
             x = [x]
-        cond = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        cond[v.P] = 101325
-        cond[v.T] = T
-        cond[v.GE] = 0
-        cond[v.N] = 1
+        cond = self._getConditions(x, T, 0)
+        self._prevX = x
 
         #Create cache of composition set if not done so already or if training a surrogate
         #Training points for surrogates may be far apart, so starting from a previous
         #   composition set could give a bad starting position for the minimizer
         if self._compset_cache_df.get(precPhase, None) is None or training:
             #Calculate equilibrium ----------------------------------------------------------------------------------------------------------------------
             eq = self.getEq(x, T, 0, precPhase)
             #Cast values in state_variables to double for updating composition sets
             state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
             stable_phases = eq.Phase.values.ravel()
             phase_amounts = eq.NP.values.ravel()
             matrix_idx = np.where(stable_phases == self.phases[0])[0]
             precip_idx = np.where(stable_phases == precPhase)[0]
+            chemical_potentials = eq.MU.values.ravel()
+            x_precip = eq.isel(vertex=precip_idx).X.values.ravel()
+            x_matrix = eq.isel(vertex=matrix_idx).X.values.ravel()
 
             #If matrix phase is not stable, then use sampling method
             #   This may occur during surrogate training of interfacial composition,
             #   where we're trying to calculate the driving force at the precipitate composition
             #   In this case, the conditions will be at th precipitate composition which can result in
             #   only that phase being stable
             if len(matrix_idx) == 0:
                 return self._getDrivingForceSampling(x, T, precPhase, returnComp)
-            
+
             #Test that precipitate phase is stable and that we're not training a surrogate
             #If not, then there's no composition set to cache
             if len(precip_idx) > 0:
-                cs_matrix = CompositionSet(self.phase_records[self.phases[0]])
-                cs_matrix.update(eq.Y.isel(vertex=matrix_idx).values.ravel()[:cs_matrix.phase_record.phase_dof],
-                                phase_amounts[matrix_idx], state_variables)
-                cs_precip = CompositionSet(self.phase_records[precPhase])
-                cs_precip.update(eq.Y.isel(vertex=precip_idx).values.ravel()[:cs_precip.phase_record.phase_dof],
-                                phase_amounts[precip_idx], state_variables)
+                cs_matrix, miscMatrix = self._createCompositionSet(eq, state_variables, self.phases[0], phase_amounts, matrix_idx)
+                cs_precip, miscPrec = self._createCompositionSet(eq, state_variables, precPhase, phase_amounts, precip_idx)
+                x_matrix = np.array(cs_matrix.X)
+                x_precip = np.array(cs_precip.X)
+                
                 composition_sets = [cs_matrix, cs_precip]
                 self._compset_cache_df[precPhase] = composition_sets
 
-            chemical_potentials = eq.MU.values.ravel()
-            ph = stable_phases[stable_phases != '']
-            x_precip = eq.isel(vertex=precip_idx).X.values.ravel()
-            x_matrix = eq.isel(vertex=matrix_idx).X.values.ravel()
+                if miscMatrix or miscPrec:
+                    result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
+                                                         self.models, self.phase_records,
+                                                         composition_sets=self._compset_cache_df[precPhase])
+                    self._compset_cache_df[precPhase] = composition_sets
+                    chemical_potentials = result.chemical_potentials
+                    cs_precip = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
+                    x_precip = np.array(cs_precip.X)
+
+                    cs_matrix = [cs for cs in composition_sets if cs.phase_record.phase_name == self.phases[0]][0]
+                    x_matrix = np.array(cs_matrix.X)
+
+            ph = np.unique(stable_phases[stable_phases != ''])
             ele = eq.component.values.ravel()
         else:
             result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
                                                          self.models, self.phase_records,
                                                          composition_sets=self._compset_cache_df[precPhase])
             self._compset_cache_df[precPhase] = composition_sets
             chemical_potentials = result.chemical_potentials
             ph = [cs.phase_record.phase_name for cs in composition_sets if cs.NP > 0]
             if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
                 cs_precip = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
                 x_precip = np.array(cs_precip.X)
-                ele = list(cs_precip.phase_record.nonvacant_elements)
 
                 cs_matrix = [cs for cs in composition_sets if cs.phase_record.phase_name == self.phases[0]][0]
                 x_matrix = np.array(cs_matrix.X)
 
                 ele = list(cs_precip.phase_record.nonvacant_elements)
 
         #Check that equilibrium has converged
@@ -776,21 +955,21 @@
                 if ele[i] == self.elements[0]:
                     refIndex = i
                     break
 
             #If in two phase region, then get curvature of parent phase and use it to calculate driving force ---------------------------------------
             sortIndices = np.argsort(self.elements[1:-1])
             unsortIndices = np.argsort(sortIndices)
- 
-            dMudxParent = dMudX(chemical_potentials, composition_sets[0], self.elements[0])       
+
+            dMudxParent = dMudX(chemical_potentials, composition_sets[0], self.elements[0])
             xM = np.delete(x_matrix, refIndex)
 
             xP = np.delete(x_precip, refIndex)
             xBar = np.array([xP - xM])
-            
+
             x = np.array(x)[sortIndices]
             xD = np.array([x - xM])
 
             dg = np.matmul(xD, np.matmul(dMudxParent, xBar.T))
 
             if returnComp:
                 if len(x) == 1:
@@ -803,15 +982,15 @@
             #If driving force is negative, then use sampling method ---------------------------------------------------------------------------------
             return self._getDrivingForceSampling(x, T, precPhase, returnComp)
 
 class BinaryThermodynamics (GeneralThermodynamics):
     '''
     Class for defining driving force and interfacial composition functions
     for a binary system using pyCalphad and thermodynamic databases
-    
+
     Parameters
     ----------
     database : str
         File name for database
     elements : list
         Elements to consider
         Note: reference element must be the first index in the list
@@ -828,15 +1007,15 @@
     def __init__(self, database, elements, phases, drivingForceMethod = 'approximate', interfacialCompMethod = 'equilibrium'):
         super().__init__(database, elements, phases, drivingForceMethod)
 
         if self.elements[1] < self.elements[0]:
             self.reverse = True
         else:
             self.reverse = False
-        
+
         #Guess composition for when finding tieline
         self._guessComposition = {self.phases[i]: (0, 1, 0.1) for i in range(1, len(self.phases))}
 
         self.setInterfacialMethod(interfacialCompMethod)
 
 
     def setInterfacialMethod(self, interfacialCompMethod):
@@ -850,19 +1029,19 @@
         '''
         if interfacialCompMethod == 'equilibrium':
             self._interfacialComposition = self._interfacialCompositionFromEq
         elif interfacialCompMethod == 'curvature':
             self._interfacialComposition = self._interfacialCompositionFromCurvature
         else:
             raise Exception('Interfacial composition method must be either \'equilibrium\' or \'curvature\'')
-        
+
     def setGuessComposition(self, conditions):
         '''
         Sets initial composition when calculating equilibrium for interfacial energy
-        
+
         Parameters
         ----------
         conditions : float, tuple or dict
             Guess composition(s) to solve equilibrium for
             This should encompass the region where a tieline can be found
             between the matrix and precipitate phases
             Options:    float - will set to all precipitate phases
@@ -877,15 +1056,15 @@
         else:
             for i in range(1, len(self.phases)):
                 self._guessComposition[self.phases[i]] = conditions
 
     def getInterfacialComposition(self, T, gExtra = 0, precPhase = None):
         '''
         Gets interfacial composition accounting for Gibbs-Thomson effect
-        
+
         Parameters
         ----------
         T : float or array
             Temperature in K
         gExtra : float or array (optional)
             Extra contributions to the precipitate Gibbs free energy
             Gibbs Thomson contribution defined as Vm * (2*gamma/R + g_Elastic)
@@ -894,15 +1073,15 @@
             Precipitate phase to consider (default is first precipitate in list)
 
         Note: for multiple conditions, only gExtra has to be an array
             This will calculate compositions for multiple gExtra at the input Temperature
 
             If T is also an array, then T and gExtra must be the same length
             where each index will pertain to a single condition
-        
+
         Returns
         -------
         (parent composition, precipitate composition)
         Both will be either float or array based off shape of gExtra
         Will return (None, None) if precipitate is unstable
         '''
         if hasattr(gExtra, '__len__'):
@@ -919,50 +1098,50 @@
                     cbArray.append(cb)
                 caArray = np.array(caArray)
                 cbArray = np.array(cbArray)
 
             return caArray, cbArray
         else:
             return self._interfacialComposition(T, gExtra, precPhase)
-        
+
 
     def _interfacialCompositionFromEq(self, T, gExtra = 0, precPhase = None):
         '''
         Gets interfacial composition by calculating equilibrum with Gibbs-Thomson effect
-        
+
         Parameters
         ----------
         T : float
             Temperature in K
         gExtra : float (optional)
             Extra contributions to the precipitate Gibbs free energy
             Gibbs Thomson contribution defined as Vm * (2*gamma/R + g_Elastic)
             Defaults to 0
         precPhase : str
             Precipitate phase to consider (default is first precipitate in list)
-        
+
         Returns
         -------
         (parent composition, precipitate composition)
         Both will be either float or array based off shape of gExtra
         Will return (None, None) if precipitate is unstable
         '''
         if precPhase is None:
             precPhase = self.phases[1]
 
         if hasattr(gExtra, '__len__'):
             gExtra = np.array(gExtra)
         else:
             gExtra = np.array([gExtra])
         gExtra += self.gOffset
-        
+
         #Compute equilibrium at guess composition
         cond = {v.X(self.elements[1]): self._guessComposition[precPhase], v.T: T, v.P: 101325, v.GE: gExtra}
-        eq = equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond, model=self.models, 
-                        phase_records={self.phases[0]: self.phase_records[self.phases[0]], precPhase: self.phase_records[precPhase]}, 
+        eq = equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond, model=self.models,
+                        phase_records={self.phases[0]: self.phase_records[self.phases[0]], precPhase: self.phase_records[precPhase]},
                         calc_opts = {'pdens': self.pDens})
 
         xParentArray = np.zeros(len(gExtra))
         xPrecArray = np.zeros(len(gExtra))
         for g in range(len(gExtra)):
             eqG = eq.where(eq.GE == gExtra[g], drop=True)
             gm = eqG.GM.values.ravel()
@@ -976,30 +1155,30 @@
                 if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
                     #Get indices for each phase
                     eqPa = eqSub.where(eqSub.Phase == self.phases[0], drop=True)
                     eqPr = eqSub.where(eqSub.Phase == precPhase, drop=True)
 
                     cParent = eqPa.X.values.ravel()
                     cPrec = eqPr.X.values.ravel()
-                    
+
                     #Get composition of element, use element index of 1 is the parent index is first alphabetically
                     if self.reverse:
                         xParent = cParent[0]
                         xPrec = cPrec[0]
                     else:
                         xParent = cParent[1]
                         xPrec = cPrec[1]
 
                     xParentArray[g] = xParent
                     xPrecArray[g] = xPrec
                     break
             if xParentArray[g] == 0:
                 xParentArray[g] = -1
                 xPrecArray[g] = -1
-                
+
         if len(gExtra) == 1:
             return xParentArray[0], xPrecArray[0]
         else:
             return xParentArray, xPrecArray
 
 
     def _interfacialCompositionFromCurvature(self, T, gExtra = 0, precPhase = None):
@@ -1013,33 +1192,33 @@
             Temperature in K
         gExtra : float (optional)
             Extra contributions to the precipitate Gibbs free energy
             Gibbs Thomson contribution defined as Vm * (2*gamma/R + g_Elastic)
             Defaults to 0
         precPhase : str
             Precipitate phase to consider (default is first precipitate in list)
-        
+
         Returns
         -------
         (parent composition, precipitate composition)
         Both will be either float or array based off shape of gExtra
         Will return (None, None) if precipitate is unstable
         '''
         if precPhase is None:
             precPhase = self.phases[1]
 
         if hasattr(gExtra, '__len__'):
             gExtra = np.array(gExtra)
         else:
             gExtra = np.array([gExtra])
-        
+
         #Compute equilibrium at guess composition
         cond = {v.X(self.elements[1]): self._guessComposition[precPhase], v.T: T, v.P: 101325, v.GE: self.gOffset}
-        eq = equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond, model=self.models, 
-                        phase_records={self.phases[0]: self.phase_records[self.phases[0]], precPhase: self.phase_records[precPhase]}, 
+        eq = equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond, model=self.models,
+                        phase_records={self.phases[0]: self.phase_records[self.phases[0]], precPhase: self.phase_records[precPhase]},
                         calc_opts = {'pdens': self.pDens})
 
         gm = eq.GM.values.ravel()
         for g in gm:
             eqSub = eq.where(eq.GM == g, drop=True)
 
             ph = eqSub.Phase.values.ravel()
@@ -1049,29 +1228,33 @@
             if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
                 #Cast values in state_variables to double for updating composition sets
                 state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
                 stable_phases = eqSub.Phase.values.ravel()
                 phase_amounts = eqSub.NP.values.ravel()
                 matrix_idx = np.where(stable_phases == self.phases[0])[0]
                 precip_idx = np.where(stable_phases == precPhase)[0]
-                
+
                 cs_matrix = CompositionSet(self.phase_records[self.phases[0]])
+                if len(matrix_idx) > 1:
+                    matrix_idx = [matrix_idx[np.argmax(phase_amounts[matrix_idx])]]
                 cs_matrix.update(eqSub.Y.isel(vertex=matrix_idx).values.ravel()[:cs_matrix.phase_record.phase_dof],
                                     phase_amounts[matrix_idx], state_variables)
                 cs_precip = CompositionSet(self.phase_records[precPhase])
+                if len(precip_idx) > 1:
+                    precip_idx = [precip_idx[np.argmax(phase_amounts[precip_idx])]]
                 cs_precip.update(eqSub.Y.isel(vertex=precip_idx).values.ravel()[:cs_precip.phase_record.phase_dof],
                                     phase_amounts[precip_idx], state_variables)
 
                 chemical_potentials = eqSub.MU.values.ravel()
                 cPrec = eqSub.isel(vertex=precip_idx).X.values.ravel()
                 cParent = eqSub.isel(vertex=matrix_idx).X.values.ravel()
 
                 dMudxParent = dMudX(chemical_potentials, cs_matrix, self.elements[0])
                 dMudxPrec = dMudX(chemical_potentials, cs_precip, self.elements[0])
-                
+
                 #Get composition of element, use element index of 1 is the parent index is first alphabetically
                 if self.reverse:
                     xParentEq = cParent[0]
                     xPrecEq = cPrec[0]
                 else:
                     xParentEq = cParent[1]
                     xPrecEq = cPrec[1]
@@ -1084,35 +1267,35 @@
                 else:
                     xParent = xParentEq
 
                 if dMudxPrec != 0:
                     xPrec = dMudxParent * (xParent - xParentEq) / dMudxPrec + xPrecEq
                 else:
                     xPrec = xPrecEq
-                
+
                 xParent[xParent < 0] = 0
                 xParent[xParent > 1] = 1
                 xPrec[xPrec < 0] = 0
                 xPrec[xPrec > 1] = 1
 
                 if len(gExtra) == 1:
                     return xParent[0], xPrec[0]
                 else:
                     return xParent, xPrec
 
         if len(gExtra) == 1:
             return -1, -1
         else:
             return -1*np.ones(len(gExtra)), -1*np.ones(len(gExtra))
-        
-        
+
+
     def plotPhases(self, ax, T, gExtra = 0, plotGibbsOffset = False, *args, **kwargs):
         '''
         Plots sampled points from the parent and precipitate phase
-        
+
         Parameters
         ----------
         ax : Axis
         T : float
             Temperature in K
         gExtra : float (optional)
             Extra contributions to the Gibbs free energy of precipitate
@@ -1121,35 +1304,35 @@
             If True and gExtra is not 0, the sampled points of the
                 precipitate phase will be plotted twice with gExtra and
                 with no extra Gibbs free energy contributions
             Defualts to False
         '''
         points = calculate(self.db, self.elements, self.phases[0], P=101325, T=T, GE=0, model=self.models, phase_records=self.phase_records, output='GM')
         ax.scatter(points.X.sel(component=self.elements[1]), points.GM / 1000, label=self.phases[0], *args, **kwargs)
-        
+
         #Add gExtra to precipitate phase
         for i in range(1, len(self.phases)):
             points = calculate(self.db, self.elements, self.phases[i], P=101325, T=T, GE=0, model=self.models, phase_records=self.phase_records, output='GM')
             ax.scatter(points.X.sel(component=self.elements[1]), (points.GM + gExtra) / 1000, label=self.phases[i], *args, **kwargs)
-            
+
             #Plot non-offset precipitate phase
             if plotGibbsOffset and gExtra != 0:
-                ax.scatter(points.X.sel(component=self.elements[1]), points.GM / 1000, color='silver', alpha=0.3, *args, **kwargs)                
-        
+                ax.scatter(points.X.sel(component=self.elements[1]), points.GM / 1000, color='silver', alpha=0.3, *args, **kwargs)
+
         ax.legend()
         ax.set_xlim([0, 1])
         ax.set_xlabel('Composition ' + self.elements[1])
         ax.set_ylabel('Gibbs Free Energy (kJ/mol)')
-        
-        
+
+
 class MulticomponentThermodynamics (GeneralThermodynamics):
     '''
     Class for defining driving force and (possibly) interfacial composition functions
     for a multicomponent system using pyCalphad and thermodynamic databases
-    
+
     Parameters
     ----------
     database : str
         File name for database
     elements : list
         Elements to consider
         Note: reference element must be the first index in the list
@@ -1158,30 +1341,30 @@
         Note: matrix phase must be first index in the list
     drivingForceMethod : str (optional)
         Method used to calculate driving force
         Options are 'approximate' (default), 'sampling' and 'curvature' (not recommended)
     '''
     def __init__(self, database, elements, phases, drivingForceMethod = 'approximate'):
         super().__init__(database, elements, phases, drivingForceMethod)
-        
+
         #Previous variables for curvature terms
         #Near saturation, pycalphad may detect only a single phase (if sampling density is too low)
-        #When this occurs, this will assume that the system is on the same tie-line and 
+        #When this occurs, this will assume that the system is on the same tie-line and
         #use the previously calculated values
-        self._prevDc = None
-        self._prevMc = None
-        self._prevGba = None
-        self._prevBeta = None
-        self._prevCa = None
-        self._prevCb = None
+        self._prevDc = {p: None for p in phases[1:]}
+        self._prevMc = {p: None for p in phases[1:]}
+        self._prevGba = {p: None for p in phases[1:]}
+        self._prevBeta = {p: None for p in phases[1:]}
+        self._prevCa = {p: None for p in phases[1:]}
+        self._prevCb = {p: None for p in phases[1:]}
 
     def getInterfacialComposition(self, x, T, gExtra = 0, precPhase = None):
         '''
         Gets interfacial composition by calculating equilibrum with Gibbs-Thomson effect
-        
+
         Parameters
         ----------
         T : float or array
             Temperature in K
         gExtra : float or array (optional)
             Extra contributions to the precipitate Gibbs free energy
             Gibbs Thomson contribution defined as Vm * (2*gamma/R + g_Elastic)
@@ -1190,15 +1373,15 @@
             Precipitate phase to consider (default is first precipitate in list)
 
         Note: for multiple conditions, only gExtra has to be an array
             This will calculate compositions for multiple gExtra at the input Temperature
 
             If T is also an array, then T and gExtra must be the same length
             where each index will pertain to a single condition
-        
+
         Returns
         -------
         (parent composition, precipitate composition)
         Both will be either float or array based off shape of gExtra
         Will return (None, None) if precipitate is unstable
         '''
         if hasattr(gExtra, '__len__'):
@@ -1212,15 +1395,15 @@
                 caArray.append(ca)
                 cbArray.append(cb)
             caArray = np.array(caArray)
             cbArray = np.array(cbArray)
             return caArray, cbArray
         else:
             return self._interfacialComposition(x, T, gExtra, precPhase)
-        
+
 
     def _interfacialComposition(self, x, T, gExtra = 0, precPhase = None):
         '''
         Gets interfacial composition, will return None, None if composition is in single phase region
 
         Parameters
         ----------
@@ -1228,15 +1411,15 @@
             Temperature in K
         gExtra : float (optional)
             Extra contributions to the precipitate Gibbs free energy
             Gibbs Thomson contribution defined as Vm * (2*gamma/R + g_Elastic)
             Defaults to 0
         precPhase : str
             Precipitate phase to consider (default is first precipitate in list)
-        
+
         Returns
         -------
         (parent composition, precipitate composition)
         Both will be either float or array based off shape of gExtra
         Will return (None, None) if precipitate is unstable
         '''
         if precPhase is None:
@@ -1262,15 +1445,15 @@
             eqPh = eq.where(eq.Phase == self.phases[0], drop=True)
             xM = eqPh.X.values.ravel()
             xM = xM[unsortIndices]
 
             eqPh = eq.where(eq.Phase == precPhase, drop=True)
             xP = eqPh.X.values.ravel()
             xP = xP[unsortIndices]
-            
+
             return xM, xP
 
         return None, None
 
     def _curvatureFactorFromEq(self, chemical_potentials, composition_sets, precPhase=None, training = False):
         '''
         Curvature factor (from Phillipes and Voorhees - 2013)
@@ -1292,48 +1475,48 @@
         {Gb^-1 Ga} - for calculating precipitate composition
         beta - Impingement rate
         Ca - interfacial composition of matrix phase
         Cb - interfacial composition of precipitate phase
 
         Will return (None, None, None, None, None, None) if single phase
         '''
+        if precPhase is None:
+            precPhase = self.phases[1]
+
         #Check if input equilibrium has converged
         if np.any(np.isnan(chemical_potentials)):
             if training:
                 return None, None, None, None, None, None
             else:
                 print('Warning: equilibrum was not able to be solved for, using results of previous calculation')
-                return self._prevDc, self._prevMc, self._prevGba, self._prevBeta, self._prevCa, self._prevCb
-
-        if precPhase is None:
-            precPhase = self.phases[1]
+                return self._prevDc[precPhase], self._prevMc[precPhase], self._prevGba[precPhase], self._prevBeta[precPhase], self._prevCa[precPhase], self._prevCb[precPhase]
 
         ele = list(composition_sets[0].phase_record.nonvacant_elements)
         refIndex = ele.index(self.elements[0])
 
         ph = [cs.phase_record.phase_name for cs in composition_sets]
 
         if len(ph) == 2 and self.phases[0] in ph and precPhase in ph:
             sortIndices = np.argsort(self.elements[1:-1])
             unsortIndices = np.argsort(sortIndices)
 
             matrix_cs = [cs for cs in composition_sets if cs.phase_record.phase_name == self.phases[0]][0]
 
-            if self.mobCallables is None:
+            if self.mobCallables[self.phases[0]] is None:
                 Dnkj, dMudxParent, invMob = inverseMobility_from_diffusivity(chemical_potentials, matrix_cs,
-                                                                             self.elements[0], self.diffCallables,
+                                                                             self.elements[0], self.diffCallables[self.phases[0]],
                                                                              diffusivity_correction=self.mobility_correction)
 
                 #NOTE: This is note tested yet
-                Dtrace = tracer_diffusivity_from_diff(matrix_cs, self.diffCallables, diffusivity_correction=self.mobility_correction)
+                Dtrace = tracer_diffusivity_from_diff(matrix_cs, self.diffCallables[self.phases[0]], diffusivity_correction=self.mobility_correction)
             else:
                 Dnkj, dMudxParent, invMob = inverseMobility(chemical_potentials, matrix_cs, self.elements[0],
-                                                            self.mobCallables,
+                                                            self.mobCallables[self.phases[0]],
                                                             mobility_correction=self.mobility_correction)
-                Dtrace = tracer_diffusivity(matrix_cs, self.mobCallables, mobility_correction=self.mobility_correction)
+                Dtrace = tracer_diffusivity(matrix_cs, self.mobCallables[self.phases[0]], mobility_correction=self.mobility_correction)
 
             xMFull = np.array(matrix_cs.X)
             xM = np.delete(xMFull, refIndex)
 
             precip_cs = [cs for cs in composition_sets if cs.phase_record.phase_name == precPhase][0]
             dMudxPrec = dMudX(chemical_potentials, precip_cs, self.elements[0])
             xPFull = np.array(precip_cs.X)
@@ -1351,34 +1534,38 @@
                 Gba = Gba[unsortIndices,:]
                 Gba = Gba[:,unsortIndices]
             else:
                 Gba = np.zeros(dMudxPrec.shape)
 
             betaNum = xBarFull**2
             betaDen = Dtrace * xMFull.flatten()
-            beta = 1 / np.sum(betaNum / betaDen)
+            bsum = np.sum(betaNum / betaDen)
+            if bsum == 0:
+                beta = self._prevBeta[precPhase]
+            else:
+                beta = 1 / bsum
 
-            self._prevDc = num[unsortIndices] / den
-            self._prevMc = 1 / den
-            self._prevGba = Gba
-            self._prevBeta = beta
-            self._prevCa = xM[unsortIndices]
-            self._prevCb = xP[unsortIndices]
+            self._prevDc[precPhase] = num[unsortIndices] / den
+            self._prevMc[precPhase] = 1 / den
+            self._prevGba[precPhase] = Gba
+            self._prevBeta[precPhase] = beta
+            self._prevCa[precPhase] = xM[unsortIndices]
+            self._prevCb[precPhase] = xP[unsortIndices]
 
-            return self._prevDc, self._prevMc, self._prevGba, self._prevBeta, self._prevCa, self._prevCb
+            return self._prevDc[precPhase], self._prevMc[precPhase], self._prevGba[precPhase], self._prevBeta[precPhase], self._prevCa[precPhase], self._prevCb[precPhase]
         else:
             if training:
                 return None, None, None, None, None, None
             else:
                 #print('Warning: only a single phase detected in equilibrium, using results of previous calculation')
-                #return self._prevDc, self._prevMc, self._prevGba, self._prevBeta, self._prevCa, self._prevCb
+                #return self._prevDc[precPhase], self._prevMc[precPhase], self._prevGba[precPhase], self._prevBeta[precPhase], self._prevCa[precPhase], self._prevCb[precPhase]
 
                 #If two-phase equilibrium is not found, then the temperature may have changed to where the precipitate is unstable
                 #Return None in this case
-                return None, None, None, self._prevBeta, None, None
+                return None, None, None, self._prevBeta[precPhase], None, None
 
 
     def curvatureFactor(self, x, T, precPhase = None, training = False):
         '''
         Curvature factor (from Phillipes and Voorhees - 2013) from composition and temperature
         This is the same as curvatureFactorEq, but will calculate equilibrium from x and T first
 
@@ -1400,64 +1587,68 @@
         Ca - interfacial composition of matrix phase
         Cb - interfacial composition of precipitate phase
 
         Will return (None, None, None, None, None, None) if single phase
         '''
         if precPhase is None:
             precPhase = self.phases[1]
-        if hasattr(x, '__len__'):
-            #Remove first element if x lists composition of all elements
-            if len(x) == len(self.elements) - 1:
-                x = x[1:]
+        if not hasattr(x, '__len__'):
+            x = [x]
 
-            conds = {v.X(self.elements[i+1]): x[i] for i in range(len(x))}
-        else:
-            conds = {v.X(self.elements[1]): x}
-        conds.update({v.N: 1, v.P: 1e5, v.GE: 0, v.T: T})
+        #Remove first element if x lists composition of all elements
+        if len(x) == len(self.elements) - 1:
+            x = x[1:]
+        cond = self._getConditions(x, T, 0)
 
         #Perform equilibrium from scratch if cache not set or when training surrogate
         if self._compset_cache.get(precPhase, None) is None or training:
             eq = self.getEq(x, T, 0, precPhase)
-            state_variables = np.array([conds[v.GE], conds[v.N], conds[v.P], conds[v.T]], dtype=np.float64)
+            state_variables = np.array([cond[v.GE], cond[v.N], cond[v.P], cond[v.T]], dtype=np.float64)
             stable_phases = eq.Phase.values.ravel()
             phase_amounts = eq.NP.values.ravel()
             matrix_idx = np.where(stable_phases == self.phases[0])[0]
             precip_idx = np.where(stable_phases == precPhase)[0]
 
             #If matrix phase is not stable (why?), then return previous values
             #Curvature can't be calculated if matrix phase isn't present
             if len(matrix_idx) == 0:
                 if training:
                     return None, None, None, None, None, None
                 else:
                     print('Warning: matrix phase not detected, using results of previous calculation')
                     return self._prevDc, self._prevMc, self._prevGba, self._prevBeta, self._prevCa, self._prevCb
 
-            cs_matrix = CompositionSet(self.phase_records[self.phases[0]])
-            cs_matrix.update(eq.Y.isel(vertex=matrix_idx).values.ravel()[:cs_matrix.phase_record.phase_dof],
-                             phase_amounts[matrix_idx], state_variables)
+            cs_matrix, miscMatrix = self._createCompositionSet(eq, state_variables, self.phases[0], phase_amounts, matrix_idx)
+
+            chemical_potentials = eq.MU.values.ravel()
 
             #If precipitate phase is not stable, then only store matrix phase in composition sets
             #Checks for single phase regions are done in _curvatureFactorFromEq,
             # so this will allow to fail there
             if len(precip_idx) == 0:
                 composition_sets = [cs_matrix]
                 self._compset_cache[precPhase] = None
             else:
-                cs_precip = CompositionSet(self.phase_records[precPhase])
-                cs_precip.update(eq.Y.isel(vertex=precip_idx).values.ravel()[:cs_precip.phase_record.phase_dof],
-                                phase_amounts[precip_idx], state_variables)
+                cs_precip, miscPrec = self._createCompositionSet(eq, state_variables, precPhase, phase_amounts, precip_idx)
+
                 composition_sets = [cs_matrix, cs_precip]
                 self._compset_cache[precPhase] = composition_sets
 
-            chemical_potentials = eq.MU.values.ravel()
+                if miscMatrix or miscPrec:
+                    result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
+                                                            self.models, self.phase_records,
+                                                            composition_sets=self._compset_cache[precPhase])
+                    self._compset_cache[precPhase] = composition_sets
+                    chemical_potentials = result.chemical_potentials
+
         else:
-            result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], conds,
+            result, composition_sets = local_equilibrium(self.db, self.elements, [self.phases[0], precPhase], cond,
                                                          self.models, self.phase_records,
                                                          composition_sets=self._compset_cache[precPhase])
+            self._compset_cache[precPhase] = composition_sets
             chemical_potentials = result.chemical_potentials
 
         result = self._curvatureFactorFromEq(chemical_potentials, composition_sets, precPhase, training)
         return result
 
     def getGrowthAndInterfacialComposition(self, x, T, dG, R, gExtra, precPhase = None, training = False):
         '''
@@ -1473,15 +1664,15 @@
             Driving force at given x and T
         R : float or array
             Precipitate radius
         gExtra : float or array
             Gibbs-Thomson contribution (must be same shape as R)
         precPhase : str (optional)
             Precipitate phase (defaults to first precipitate in list)
-        
+
         Returns
         -------
         (growth rate, matrix composition, precipitate composition, equilibrium matrix comp, equilibrium precipitate comp)
         growth rate will be float or array based off shape of R
         matrix and precipitate composition will be array or 2D array based
             off shape of R
         '''
```

### Comparing `kawin-0.1.2/kawin/tests/datasets.py` & `kawin-0.2.0/kawin/tests/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1200,8 +1200,482 @@
          CHROMIUM <GAS>'
    REF4591  'CR2<G> T.C.R.A.S. Class: 6'
    REF7504  'NI1<G> T.C.R.A.S Class: 1
          Data provided by T.C.R.A.S. October 1996'
    REF7553  'NI2<G> T.C.R.A.S Class: 5 
          Data provided by T.C.R.A.S. October 1996'
   ! 
+"""
+
+NICRAL_TDB_DIFF = """
+
+$ Same as NICRAL_TDB with the following changes
+$ Shortened to include just FCC_A1, FCC_L12, LIQUID
+$ Mobility parameters replaced with arbitrary diffusivity parameter to test diffusivity and tracer outputs
+$
+
+
+ ELEMENT /-   ELECTRON_GAS               .0000E+00   .0000E+00   .0000E+00!
+ ELEMENT VA   VACUUM                     .0000E+00   .0000E+00   .0000E+00!
+ ELEMENT AL   FCC_A1                    2.6982E+01  4.5773E+03  2.8322E+01!
+ ELEMENT CR   BCC_A2                    5.1996E+01  4.0500E+03  2.3560E+01!
+ ELEMENT NI   FCC_A1                    5.8690E+01  4.7870E+03  2.9796E+01!
+
+ SPECIES AL2                         AL2!
+ SPECIES CR2                         CR2!
+ SPECIES NI2                         NI2!
+
+ 
+ FUNCTION UNASS      298.15  0;,,N !
+
+
+ TYPE_DEFINITION % SEQ *!
+ DEFINE_SYSTEM_DEFAULT E 2 !
+ DEFAULT_COMMAND DEF_SYS_ELEMENT VA !
+ DEFAULT_COMMAND REJECT_PHASE NEWSIGMA !
+			  
+ TYPE_DEFINITION A GES A_P_D FCC_L12 MAGNETIC  -3.0 .28 !
+ TYPE_DEFINITION E GES A_P_D FCC_A1 MAGNETIC  -3.0 .28 !
+
+ TYPE_DEFINITION D GES A_P_D FCC_L12 DIS_PART FCC_A1 !
+
+ PHASE GAS:G %  1  1.0  !
+ CONST GAS:G :AL,AL2,CR,CR2,NI,NI2 :  !
+
+ PHASE LIQUID:L %  1  1.0  !
+ CONST LIQUID:L :AL,CR,NI :  !
+
+ PHASE FCC_A1  %E  2 1   1 !
+ CONST FCC_A1  :AL,CR,NI% : VA% :  !
+
+$ PHASE FCC_L12  %ADG  3 .75   .25   1 !
+ PHASE FCC_L12  %AD  3 .75   .25   1 !
+ CONST FCC_L12  :AL,CR,NI : AL,CR,NI : VA :  !
+
+ FUNCTION ZERO       298.15  0;,,N !
+ FUNCTION DP         298.15  +P-101325;,,N !
+ FUNCTION TROIS 298.15 3;,,N !
+ FUNCTION UNTIER 298.15 TROIS**(-1);,,N !
+
+$****************************************************************************
+$
+$                                                            UNARY PARAMETERS
+$
+$----------------------------------------------------------------------------
+$
+$                                                                          Al
+$
+$                                                                   FUNCTIONS
+$
+ FUNCTION F154T      298.15
+    +323947.58-25.1480943*T-20.859*T*LN(T)
+    +4.5665E-05*T**2-3.942E-09*T**3-24275.5*T**(-1);
+                    4300.0  Y
+    +342017.233-54.0526109*T-17.7891*T*LN(T)+6.822E-05*T**2
+    -1.91111667E-08*T**3-14782200*T**(-1);
+                    8200.0  Y
+    +542396.07-411.214335*T+22.2419*T*LN(T)-.00349619*T**2
+    +4.0491E-08*T**3-2.0366965E+08*T**(-1);  1.00000E+04  N !
+$
+ FUNCTION F625T      298.15
+    +496408.232+35.479739*T-41.6397*T*LN(T)
+    +.00249636*T**2-4.90507333E-07*T**3+85390.3*T**(-1);
+                     900.00  Y
+    +497613.221+17.368131*T-38.85476*T*LN(T)-2.249805E-04*T**2
+    -9.49003167E-09*T**3-5287.23*T**(-1);  2.80000E+03  N !
+$
+ FUNCTION GHSERAL    298.15
+    -7976.15+137.093038*T-24.3671976*T*LN(T)
+    -.001884662*T**2-8.77664E-07*T**3+74092*T**(-1);
+                     700.00  Y
+    -11276.24+223.048446*T-38.5844296*T*LN(T)
+    +.018531982*T**2-5.764227E-06*T**3+74092*T**(-1);
+                     933.60  Y
+    -11278.378+188.684153*T-31.748192*T*LN(T)
+    -1.231E+28*T**(-9);,,  N !
+$
+ FUNCTION GHCPAL     298.15  +5481-1.8*T+GHSERAL;,,N !
+$
+ FUNCTION GBCCAL     298.15  +10083-4.813*T+GHSERAL;,,N !
+$
+ FUNCTION GLIQAL     298.14
+    +11005.029-11.841867*T+7.934E-20*T**7+GHSERAL;
+                     933.59  Y
+    +10482.282-11.253974*T+1.231E+28*T**(-9)+GHSERAL;,,N !
+$
+$                                                                   GAS PHASE
+$
+ PARAMETER G(GAS,AL;0)  298.15  +F154T+R*T*LN(1E-05*P);,,N REF184 !
+ PARAMETER G(GAS,AL2;0)  298.15  +F625T+R*T*LN(1E-05*P);,,N REF448 !
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER   G(LIQUID,AL;0)   298.13
+      +11005.029-11.841867*T+7.934E-20*T**7+GHSERAL;
+                                933.60  Y
+      +10482.382-11.253974*T+1.231E+28*T**(-9)
+      +GHSERAL;,,N 91DIN !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER G(FCC_A1,AL:VA;0)  298.15  +GHSERAL;,,N 91DIN !
+$
+$
+$----------------------------------------------------------------------------
+$
+$                                                                          Cr
+$
+$                                                                   FUNCTIONS
+$
+ FUNCTION F7454T     298.15
+    +390765.331-31.5192154*T-21.36083*T*LN(T)
+    +7.253215E-04*T**2-1.588679E-07*T**3+10285.15*T**(-1);
+                     1100.0  Y
+    +393886.928-44.107465*T-19.96003*T*LN(T)+.001513089*T**2
+    -4.23648333E-07*T**3-722515*T**(-1);
+                     2000.0  Y
+    +421372.003-231.888524*T+5.362886*T*LN(T)-.00848877*T**2
+    +2.984635E-07*T**3-6015405*T**(-1);
+                     3300.0  Y
+    +305164.698+251.019831*T-55.20304*T*LN(T)+.005324585*T**2
+    -2.850405E-07*T**3+34951485*T**(-1);
+                     5100.0  Y
+    +1069921.1-1708.93262*T+175.0508*T*LN(T)-.025574185*T**2
+    +4.94447E-07*T**3-4.4276355E+08*T**(-1);
+                     7600.0  Y
+    -871952.838+1686.47356*T-204.5589*T*LN(T)+.007475225*T**2
+    -4.618745E-08*T**3+1.423504E+09*T**(-1);  1.00000E+04  N !
+$
+ FUNCTION F7735T     298.15  +598511.402+41.5353219*T-40.56798*T*LN(T)
+    +.004961847*T**2-1.61216717E-06*T**3+154422.85*T**(-1);
+                     800.00  Y
+    +613345.232-104.20799*T-19.7643*T*LN(T)-.007085085*T**2
+    -4.69883E-07*T**3-1738066.5*T**(-1);
+                     1400.0  Y
+    +642608.843-369.286259*T+17.64743*T*LN(T)-.02767321*T**2
+    +1.605906E-06*T**3-5831655*T**(-1);
+                     2300.0  Y
+    +553119.895+159.188556*T-52.07969*T*LN(T)-.004229401*T**2
+    +1.5939925E-07*T**3+14793625*T**(-1);
+                     3900.0  Y
+    +347492.339+623.137624*T-105.0428*T*LN(T)+3.9699545E-04*T**2
+    +1.51783483E-07*T**3+1.4843765E+08*T**(-1);
+                     5800.0  Y
+    -484185.055+2598.25559*T-334.7145*T*LN(T)+.028597625*T**2
+    -4.97520167E-07*T**3+7.135805E+08*T**(-1);  6.00000E+03  N !
+$
+ FUNCTION GHSERCR    298.14
+    -8856.94+157.48*T-26.908*T*LN(T)
+    +.00189435*T**2-1.47721E-06*T**3+139250*T**(-1);
+                     2180.0  Y
+    -34869.344+344.18*T-50*T*LN(T)-2.88526E+32*T**(-9);,,N !
+$
+ FUNCTION GCRLIQ     298.15
+    +24339.955-11.420225*T+2.37615E-21*T**7+GHSERCR;
+                     2180.0  Y
+    -16459.984+335.616316*T-50*T*LN(T);,,N !
+$
+ FUNCTION GFCCCR     298.15  +7284+.163*T+GHSERCR;,,N !
+$
+ FUNCTION GHCPCR     298.15  +4438+GHSERCR;,,N !
+$
+ FUNCTION ACRBCC     298.15  +1.7E-05*T+9.2E-09*T**2;,,N !
+ FUNCTION BCRBCC     298.15  +1+2.6E-11*P;,,N !
+ FUNCTION CCRBCC     298.15  2.08E-11;,,N !
+ FUNCTION DCRBCC     298.15  +1*LN(BCRBCC);,,N !
+ FUNCTION VCRBCC     298.15  +7.188E-06*EXP(ACRBCC);,,N !
+ FUNCTION ECRBCC     298.15  +1*LN(CCRBCC);,,N !
+ FUNCTION XCRBCC     298.15  +1*EXP(.8*DCRBCC)-1;,,N !
+ FUNCTION YCRBCC     298.15  +VCRBCC*EXP(-ECRBCC);,,N !
+ FUNCTION ZCRBCC     298.15  +1*LN(XCRBCC);,,N !
+ FUNCTION GPCRBCC    298.15  +YCRBCC*EXP(ZCRBCC);,,N !
+$
+ FUNCTION ACRLIQ     298.15  +1.7E-05*T+9.2E-09*T**2;,,N !
+ FUNCTION BCRLIQ     298.15  +1+4.65E-11*P;,,N !
+ FUNCTION CCRLIQ     298.15  3.72E-11;,,N !
+ FUNCTION DCRLIQ     298.15  +1*LN(BCRLIQ);,,N !
+ FUNCTION VCRLIQ     298.15  +7.653E-06*EXP(ACRLIQ);,,N !
+ FUNCTION ECRLIQ     298.15  +1*LN(CCRLIQ);,,N !
+ FUNCTION XCRLIQ     298.15  +1*EXP(.8*DCRLIQ)-1;,,N !
+ FUNCTION YCRLIQ     298.15  +VCRLIQ*EXP(-ECRLIQ);,,N !
+ FUNCTION ZCRLIQ     298.15  +1*LN(XCRLIQ);,,N !
+ FUNCTION GPCRLIQ    298.15  +YCRLIQ*EXP(ZCRLIQ);,,N !
+$
+$                                                                   GAS PHASE
+$
+ PARAMETER G(GAS,CR;0)  298.15  +F7454T+R*T*LN(1E-05*P);,,N REF4465 !
+ PARAMETER G(GAS,CR2;0)  298.15  +F7735T+R*T*LN(1E-05*P);,,  N REF4591 !
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER G(LIQUID,CR;0)  298.15  +GCRLIQ+GPCRLIQ;,,  N 91DIN !
+$
+$                                                                FCC_A1 PHASE
+$
+$
+$----------------------------------------------------------------------------
+$
+$                                                                          Ni
+$
+$                                                                   FUNCTIONS
+$
+ FUNCTION F13191T    298.15
+    +417658.868-44.7777921*T-20.056*T*LN(T)
+    -.0060415*T**2+1.24774E-06*T**3-16320*T**(-1);
+                     800.00  Y
+    +413885.448+9.41787679*T-28.332*T*LN(T)+.00173115*T**2
+    -8.399E-08*T**3+289050*T**(-1);
+                     3900.0  Y
+    +440866.732-62.5810038*T-19.819*T*LN(T)+5.067E-04*T**2
+    -4.93233333E-08*T**3-15879735*T**(-1);
+                     7600.0  Y
+    +848806.287-813.398164*T+64.69*T*LN(T)-.00731865*T**2
+    +8.71833333E-08*T**3-3.875846E+08*T**(-1);  10000.  N !
+$
+ FUNCTION F13265T    298.15
+    +638073.279-68.1901928*T-24.897*T*LN(T)
+    -.0313584*T**2+5.93355333E-06*T**3-14215*T**(-1);
+                     800.00  Y
+    +611401.772+268.084821*T-75.25401*T*LN(T)+.01088525*T**2
+    -7.08741667E-07*T**3+2633835*T**(-1);
+                     2100.0  Y
+    +637459.339+72.0712678*T-48.587*T*LN(T)-9.09E-05*T**2
+    +9.12933333E-08*T**3-1191755*T**(-1);
+                     4500.0 Y
+    +564540.781+329.599011*T-80.11301*T*LN(T)+.00578085*T**2
+    -1.08841667E-07*T**3+29137900*T**(-1);  6000.0  N !
+$
+ FUNCTION GHSERNI    298.14
+    -5179.159+117.854*T-22.096*T*LN(T)
+    -.0048407*T**2;
+                     1728.0  Y
+    -27840.655+279.135*T-43.1*T*LN(T)+1.12754E+31*T**(-9);,,  N   !
+$
+ FUNCTION GHCPNI     298.15  +1046+1.2552*T+GHSERNI;,,N !
+$
+ FUNCTION GBCCNI     298.15  +8715.084-3.556*T+GHSERNI;,,,   N !
+$
+$                                                                   GAS PHASE
+$
+ PARAMETER G(GAS,NI;0)  298.15  +F13191T+R*T*LN(1E-05*P);,,N REF7504 !
+ PARAMETER G(GAS,NI2;0)  298.15 +F13265T+R*T*LN(1E-05*P);,,N REF7553 !
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER G(LIQUID,NI;0) 298.13
+      +16414.686-9.397*T-3.82318E-21*T**7+GHSERNI;
+                            1728.0  Y
+      +18290.88-10.537*T-1.12754E+31*T**(-9)
+      +GHSERNI;,,N 91DIN !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER G(FCC_A1,NI:VA;0)  298.15  +GHSERNI;,,N 91DIN !
+ PARAMETER TC(FCC_A1,NI:VA;0)  298.15  633;,,N 89DIN !
+ PARAMETER BMAGN(FCC_A1,NI:VA;0)  298.15  .52;,,N 89DIN !
+$
+$
+$****************************************************************************
+$
+$                                                           BINARY PARAMETERS
+$
+$----------------------------------------------------------------------------
+$
+$                                                                       Al-Cr
+$                             Mainly from Saunders (COST507)
+$                             Metastable B2 and L12 from revision of Al-Cr-Ni
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER L(LIQUID,AL,CR;0)  298.15  -29000;,,N 91SAU1 !
+ PARAMETER L(LIQUID,AL,CR;1)  298.15  -11000;,,N 91SAU1 !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER G(FCC_A1,AL,CR:VA;0)  298.15  -45900+6*T;,,N 91SAU1 !
+$
+$
+$                                                               FCC_L12 PHASE
+$                                                                  metastable
+$ Present work: july 1999, study of Al-Cr-Ni, revision of NDTH.
+     FUN U1ALCR  298.15 -830;,,N  99DUP6 !
+     FUN U3ALCR  298.15 0.0; 6000.00   99DUP6 !
+     FUN U4ALCR  298.15 0.0; 6000.00 N  99DUP6 !
+   FUNCTION L04ALCR 298.15 U3ALCR;,,N !
+   FUNCTION L14ALCR 298.15 U4ALCR;,,N !
+   FUNCTION ALCR3 298.15 3*U1ALCR;,,N !
+   FUNCTION AL2CR2 298.15 4*U1ALCR;,,N !
+   FUNCTION AL3CR 298.15 3*U1ALCR;,,N !
+ PARAMETER G(FCC_L12,CR:AL:VA;0)  298.15  +ALCR3;,,  N  99DUP6 !
+ PARAMETER G(FCC_L12,AL:CR:VA;0)  298.15  +AL3CR;,,  N  99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:AL:VA;0) 298.15
+     -1.5*ALCR3+1.5*AL2CR2+1.5*AL3CR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:CR:VA;0) 298.15
+     +1.5*ALCR3+1.5*AL2CR2-1.5*AL3CR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:AL:VA;1) 298.15
+     +0.5*ALCR3-1.5*AL2CR2+1.5*AL3CR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:CR:VA;1) 298.15
+     -1.5*ALCR3+1.5*AL2CR2-0.5*AL3CR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,*:AL,CR:VA;0) 298.15 +L04ALCR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,*:AL,CR:VA;1) 298.15 +L14ALCR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:*:VA;0) 298.15 +3*L04ALCR;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,AL,CR:*:VA;1) 298.15 +3*L14ALCR;,,N 99DUP6 !
+$
+$
+$----------------------------------------------------------------------------
+$
+$                                                                       Al-Ni
+$                     Mainly from ND thesis,
+$                     slighly revised to get better solvus at low temperature
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER L(LIQUID,AL,NI;0)  298.15 -207109.28+41.31501*T;,,N 95DUP3 !
+ PARAMETER L(LIQUID,AL,NI;1)  298.15 -10185.79+5.8714*T;,,N 95DUP3 !
+ PARAMETER L(LIQUID,AL,NI;2)  298.15 +81204.81-31.95713*T;,,N 95DUP3 !
+ PARAMETER L(LIQUID,AL,NI;3)  298.15  +4365.35-2.51632*T;,,N 95DUP3 !
+ PARAMETER L(LIQUID,AL,NI;4)  298.15  -22101.64+13.16341*T;,,N 95DUP3 !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER TC(FCC_A1,AL,NI:VA;0)  298.15  -1112;,,N 95DUP3 !
+ PARAMETER TC(FCC_A1,AL,NI:VA;1)  298.15  1745;,,N 95DUP3 !
+ PARAMETER G(FCC_A1,AL,NI:VA;0)  298.15  -162407.75+16.212965*T;,,N 95DUP3 !
+ PARAMETER G(FCC_A1,AL,NI:VA;1)  298.15  +73417.798-34.914168*T;,,N 95DUP3 !   
+ PARAMETER G(FCC_A1,AL,NI:VA;2)  298.15  +33471.014-9.8373558*T;,,N 95DUP3 !   
+ PARAMETER G(FCC_A1,AL,NI:VA;3)  298.15  -30758.01+10.25267*T;,,N 95DUP3 !
+$
+$                                                               FCC_L12 PHASE
+$
+     FUN UALNI 298.15 -22212.8931+4.39570389*T;,,,N 99DUP3 !
+     FUN U1ALNI 298.15 2*UNTIER*UALNI;,,,N 99DUP3 !
+     FUN U3ALNI 298.15 0;,,,N 99DUP3 !
+     FUN U4ALNI 298.15 7203.60609-3.74273030*T;,,,N 99DUP3 !
+   FUNCTION L04ALNI 298.15 U3ALNI;,,N 99DUP3 !
+   FUNCTION L14ALNI 298.15 U4ALNI;,,N 99DUP3 !
+   FUNCTION ALNI3   298.15 +3*U1ALNI;,,,N 99DUP3 !
+   FUNCTION AL2NI2  298.15 +4*U1ALNI;,,,N 99DUP3 !
+   FUNCTION AL3NI   298.15 +3*U1ALNI;,,,N 99DUP3 !
+ PARAMETER G(FCC_L12,NI:AL:VA;0)  298.15  +ALNI3;,,N 99DUP3 !
+ PARAMETER G(FCC_L12,AL:NI:VA;0)  298.15  +AL3NI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:AL:VA;0) 298.15
+     -1.5*ALNI3+1.5*AL2NI2+1.5*AL3NI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:NI:VA;0) 298.15
+     +1.5*ALNI3+1.5*AL2NI2-1.5*AL3NI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:AL:VA;1) 298.15
+     +0.5*ALNI3-1.5*AL2NI2+1.5*AL3NI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:NI:VA;1) 298.15
+     -1.5*ALNI3+1.5*AL2NI2-0.5*AL3NI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,*:AL,NI:VA;0) 298.15 +L04ALNI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,*:AL,NI:VA;1) 298.15 +L14ALNI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:*:VA;0) 298.15 +3*L04ALNI;,,N 99DUP3 !
+ PARAMETER L(FCC_L12,AL,NI:*:VA;1) 298.15 +3*L14ALNI;,,N 99DUP3 !
+$
+$
+$----------------------------------------------------------------------------
+$
+$                                                                       Cr-Ni
+$                             Mainly from SSOL
+$                             Metastable B2 and L12 from revision of Al-Cr-Ni
+$ 
+$                                                                LIQUID PHASE
+$
+ PARAMETER L(LIQUID,CR,NI;0)  298.15  +318-7.3318*T;,,N 91LEE !
+ PARAMETER L(LIQUID,CR,NI;1)  298.15  +16941-6.3696*T;,,N 91LEE !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER G(FCC_A1,CR,NI:VA;0)  298.15  +8030-12.8801*T;,,N 91LEE !
+ PARAMETER G(FCC_A1,CR,NI:VA;1)  298.15  +33080-16.0362*T;,,N 91LEE !   
+ PARAMETER TC(FCC_A1,CR,NI:VA;0)  298.15  -3605;,,N 86DIN !
+ PARAMETER BMAGN(FCC_A1,CR,NI:VA;0)  298.15  -1.91;,,N 86DIN !
+$
+$
+$                                                               FCC_L12 PHASE
+$                                                                  metastable
+$ Present work: july 1999, study of Al-Cr-Ni, revision of NDTH.
+$ The L12 phase is metastable in the binary Cr-Ni while it was stable in NDTH.
+     FUN U1CRNI 298.15 -1980;,,,N 99DUP6 !
+$     FUN U1CRNI 298.15 -7060+3.63*T;,,,N 99DUP6 !
+     FUN U3CRNI 298.15 0;,,,N 99DUP6 !
+     FUN U4CRNI 298.15 0;,,,N 99DUP6 !
+   FUNCTION L04CRNI 298.15 U3CRNI;,,N 99DUP6 !
+   FUNCTION L14CRNI 298.15 U4CRNI;,,N 99DUP6 !
+   FUNCTION CRNI3   298.15 +3*U1CRNI;,,,N 99DUP6 !
+   FUNCTION CR2NI2  298.15 +4*U1CRNI;,,,N 99DUP6 !
+   FUNCTION CR3NI   298.15 +3*U1CRNI;,,,N 99DUP6 !
+ PARAMETER G(FCC_L12,NI:CR:VA;0)  298.15  +CRNI3;,,  N 99DUP6 !
+ PARAMETER G(FCC_L12,CR:NI:VA;0)  298.15  +CR3NI;,,  N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:CR:VA;0) 298.15
+     -1.5*CRNI3+1.5*CR2NI2+1.5*CR3NI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:NI:VA;0) 298.15
+     +1.5*CRNI3+1.5*CR2NI2-1.5*CR3NI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:CR:VA;1) 298.15
+     +0.5*CRNI3-1.5*CR2NI2+1.5*CR3NI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:NI:VA;1) 298.15
+     -1.5*CRNI3+1.5*CR2NI2-0.5*CR3NI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,*:CR,NI:VA;0) 298.15 +L04CRNI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,*:CR,NI:VA;1) 298.15 +L14CRNI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:*:VA;0) 298.15 +3*L04CRNI;,,N 99DUP6 !
+ PARAMETER L(FCC_L12,CR,NI:*:VA;1) 298.15 +3*L14CRNI;,,N 99DUP6 !
+$                                                        
+$
+$****************************************************************************
+$
+$                                                          TERNARY PARAMETERS
+$
+$----------------------------------------------------------------------------
+$
+$                                                                    Al-Cr-Ni
+$                                    July 1999, ND
+$                                    Revision. Main changes:
+$                                    - description of the A2/B2
+$                                    - new liquidus data taken into account
+$                                    - simpler ternary interaction parameters
+$
+$                                                                LIQUID PHASE
+$
+ PARAMETER L(LIQUID,AL,CR,NI;0)  298.15  16000;,,N 99DUP6 !
+$
+$                                                                FCC_A1 PHASE
+$
+ PARAMETER G(FCC_A1,AL,CR,NI:VA;0)  298.15  30300;,,N 99DUP6 !
+$
+$
+$                                                               FCC_L12 PHASE
+$
+   FUN U1ALCRNI 298.15 6650;,,N 99DUP6 !
+   FUN U2ALCRNI 298.15 0;,,N 99DUP6 !
+   FUN U3ALCRNI 298.15 0;,,N 99DUP6 !
+   FUN ALCRNI2 298.15 U1ALCR+2*U1ALNI+2*U1CRNI+U1ALCRNI;,,N 99DUP6 !
+   FUN ALCR2NI 298.15 2*U1ALCR+U1ALNI+2*U1CRNI+U2ALCRNI;,,N 99DUP6 !
+   FUN AL2CRNI 298.15 2*U1ALCR+2*U1ALNI+U1CRNI+U3ALCRNI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,CR,NI:AL:VA;0) 298.15
+     -1.5*ALCRNI2-1.5*ALCR2NI+ALCR3+ALNI3+6*AL2CRNI
+     -1.5*AL2CR2-1.5*AL2NI2-1.5*AL3CR-1.5*AL3NI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,CR,NI:CR:VA;0) 298.15
+     -1.5*ALCRNI2+6*ALCR2NI-1.5*ALCR3-1.5*AL2CRNI
+     -1.5*AL2CR2+AL3CR+CRNI3-1.5*CR2NI2-1.5*CR3NI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,CR,NI:NI:VA;0) 298.15
+     +6*ALCRNI2-1.5*ALCR2NI-1.5*ALNI3-1.5*AL2CRNI
+     -1.5*AL2NI2+AL3NI-1.5*CRNI3-1.5*CR2NI2+CR3NI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,CR:NI:VA;0) 298.15
+     +1.5*ALCR2NI+1.5*AL2CRNI-1.5*AL3NI-1.5*CR3NI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,NI:CR:VA;0) 298.15
+     +1.5*ALCRNI2+1.5*AL2CRNI-1.5*AL3CR-1.5*CRNI3;,,N 99DUP6 !
+ PARA L(FCC_L12,CR,NI:AL:VA;0) 298.15
+     +1.5*ALCRNI2+1.5*ALCR2NI-1.5*ALCR3-1.5*ALNI3;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,CR:NI:VA;1) 298.15
+     -1.5*ALCR2NI+1.5*AL2CRNI-0.5*AL3NI+0.5*CR3NI;,,N 99DUP6 !
+ PARA L(FCC_L12,AL,NI:CR:VA;1) 298.15
+     -1.5*ALCRNI2+1.5*AL2CRNI-0.5*AL3CR+0.5*CRNI3;,,N 99DUP6 !
+ PARA L(FCC_L12,CR,NI:AL:VA;1) 298.15
+     -1.5*ALCRNI2+1.5*ALCR2NI-0.5*ALCR3+0.5*ALNI3;,,N 99DUP6 !
+$
+$****************************************************************************
+$ Diffusion parameters
+$
+PARAMETER DQ(FCC_A1&AL,*;0) 298.15  -70000+R*T*LN(5E-5); 6000 N !
+PARAMETER DQ(FCC_A1&CR,*;0) 298.15  -40800+R*T*LN(3e-6); 6000 N !
+PARAMETER DQ(FCC_A1&NI,*;0) 298.15  -271960+R*T*LN(1.27E-4); 6000 N !
+$
 """
```

### Comparing `kawin-0.1.2/kawin/tests/test_PBM.py` & `kawin-0.2.0/kawin/tests/test_PBM.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     finalLength = pbm.PSDbounds[-1] + qBins * (pbm.PSDbounds[1] - pbm.PSDbounds[0])
     pbm.adjustSizeClassesEuler(False)
     assert(len(pbm.PSD) == bins+qBins and pbm.bins == len(pbm.PSD))
     assert_allclose(pbm.PSDbounds[-1], finalLength, rtol=1e-6)
     assert_allclose(pbm.max, finalLength, rtol=1e-6)
     assert(len(pbm.PSDbounds) == bins+qBins+1)
     assert(len(pbm.PSDsize) == bins+qBins)
-    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), rtol=1e-6)
+    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
     pbm.reset()
 
 def test_increaseBinSize():
     '''
     If number of bins > maxBins, then increase bin size to keep range with bins = minBins
     '''
     pbm.addSizeClasses(int(0.9*bins))
@@ -49,15 +49,15 @@
     finalLength = pbm.PSDbounds[-1] + qBins*(pbm.PSDbounds[1] - pbm.PSDbounds[0])
     pbm.adjustSizeClassesEuler(False)
     assert(len(pbm.PSD) == minBins and pbm.bins == len(pbm.PSD))
     assert_allclose(pbm.PSDbounds[-1], finalLength, rtol=1e-6)
     assert_allclose(pbm.max, finalLength, rtol=1e-6)
     assert(len(pbm.PSDbounds) == minBins+1)
     assert(len(pbm.PSDsize) == minBins)
-    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), rtol=1e-6)
+    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
     pbm.reset()
 
 def test_decreaseBinSize():
     '''
     If max filled bin < 1/2 minBins, then decrease bin size so the last filled bin is the max and bins = maxBins
     '''
     filledBin = int(1/4 * minBins)
@@ -65,15 +65,15 @@
     finalLength = pbm.PSDbounds[filledBin+1]
     pbm.adjustSizeClassesEuler(True)
     assert(len(pbm.PSD) == maxBins and pbm.bins == len(pbm.PSD))
     assert_allclose(pbm.PSDbounds[-1], finalLength, rtol=1e-6)
     assert_allclose(pbm.max, finalLength, rtol=1e-6)
     assert(len(pbm.PSDbounds) == maxBins+1)
     assert(len(pbm.PSDsize) == maxBins)
-    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), rtol=1e-6)
+    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
     pbm.reset()
 
 def test_nucleateSmall():
     '''
     If nucleate radius is smaller than PSD length, then no change
     '''
     pbm.Nucleate(10, 1e-9)
@@ -91,15 +91,15 @@
     r = 1e-7
     pbm.Nucleate(10, r)
     assert(len(pbm.PSD) == bins and pbm.bins == len(pbm.PSD))
     assert(len(pbm.PSDbounds) == bins+1)
     assert(len(pbm.PSDsize) == bins)
     assert(pbm.Moment(0) == 10)
     assert_allclose(pbm.PSDbounds[-1], 5*r, rtol=1e-6)
-    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), rtol=1e-6)
+    assert_allclose(pbm.PSDsize[0], 0.5*(pbm.PSDbounds[0] + pbm.PSDbounds[1]), atol=0, rtol=1e-6)
     pbm.reset()
 
 def test_DT():
     '''
     Calculated DT with constant growth rate
     DT = binSize / (2*max(growth rate))
     '''
```

### Comparing `kawin-0.1.2/kawin/tests/test_extraFactors.py` & `kawin-0.2.0/kawin/tests/test_extraFactors.py`

 * *Files identical despite different names*

### Comparing `kawin-0.1.2/kawin/tests/test_surrogate.py` & `kawin-0.2.0/kawin/tests/test_surrogate.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
     assert np.isscalar(xP) or (type(xP) == np.ndarray and xP.ndim == 0)
     assert hasattr(dgarray, '__len__') and len(dgarray) == 2
     assert hasattr(xParray, '__len__') and len(xParray) == 2
 
     #Compare to Thermodynamics, high tolerance since we're just checking that functions are interchangeable
-    assert_allclose(dg, dgT, rtol=1e-1)
-    assert_allclose(xP, xPT, rtol=1e-1)
+    assert_allclose(dg, dgT, atol=0, rtol=1e-1)
+    assert_allclose(xP, xPT, atol=0, rtol=1e-1)
 
 def test_Surr_binary_IC_output():
     '''
     Tests output of binary surrogate composition function
     This should give the same response as corresponding functions
     in Thermodynamics
 
@@ -70,16 +70,16 @@
     assert np.isscalar(xp) or (type(xp) == np.ndarray and xp.ndim == 0)
     assert hasattr(xmarray, '__len__') and len(xmarray) == 2
     assert hasattr(xparray, '__len__') and len(xparray) == 2
     assert hasattr(xmarray2, '__len__') and len(xmarray2) == 2
     assert hasattr(xparray2, '__len__') and len(xparray2) == 2
 
     #Compare to Thermodynamics, high tolerance since we're just checking that functions are interchangeable
-    assert_allclose(xm, xmT, rtol=1e-1)
-    assert_allclose(xp, xpT, rtol=1e-1)
+    assert_allclose(xm, xmT, atol=0, rtol=1e-1)
+    assert_allclose(xp, xpT, atol=0, rtol=1e-1)
 
 
 def test_Surr_binary_Diff_output():
     '''
     Tests output of binary surrogate diffusivity function
     This should give the same response as corresponding functions
     in Thermodynamics
@@ -98,15 +98,15 @@
     dnkj = surr.getInterdiffusivity(xtrain[3], 673.15)
     dnkjT = AlZrTherm.getInterdiffusivity(xtrain[3], 673.15)
     dnkjarray = surr.getInterdiffusivity([0.004, 0.005], [673.15, 683.15])
     assert np.isscalar(dnkj) or (type(dnkj) == np.ndarray and dnkj.ndim == 0)
     assert hasattr(dnkjarray, '__len__') and len(dnkjarray) == 2
 
     #Compare to Thermodynamics, high tolerance since we're just checking that functions are interchangeable
-    assert_allclose(dnkj, dnkjT, rtol=1e-1)
+    assert_allclose(dnkj, dnkjT, atol=0, rtol=1e-1)
 
 def test_Surr_binary_save():
     '''
     Checks that binary surrogate can be saved and loaded to get same values
     '''
     surr = BinarySurrogate(AlZrTherm)
     T = 673.15
@@ -147,15 +147,15 @@
     surr.save('kawin/tests/alzr')
 
     surr2 = BinarySurrogate.load('kawin/tests/alzr')
     a2, b2 = surr2.getDrivingForce(0.004, T)
 
     os.remove('kawin/tests/alzr')
 
-    assert_allclose(a, a2, rtol=1e-3)
+    assert_allclose(a, a2, atol=0, rtol=1e-3)
 
 def test_Surr_ternary_DG_output():
     '''
     Tests output of multicomponent surrogate driving force function
     This should give the same response as corresponding functions
     in Thermodynamics
 
@@ -174,16 +174,16 @@
 
     assert np.isscalar(dg) or (type(dg) == np.ndarray and dg.ndim == 0)
     assert xP.ndim == 1 and len(xP) == 2
     assert hasattr(dgarray, '__len__')
     assert xParray.shape == (3, 2)
 
     #Compare to Thermodynamics, high tolerance since we're just checking that functions are interchangeable
-    assert_allclose(dg, dgT, rtol=1e-1)
-    assert_allclose(xP, xPT, rtol=1e-1)
+    assert_allclose(dg, dgT, atol=0, rtol=1e-1)
+    assert_allclose(xP, xPT, atol=0, rtol=1e-1)
 
 def test_Surr_ternary_IC_output():
     '''
     Tests output of multicomponent surrogate interfacial composition function
     This should give the same response as corresponding functions
     in Thermodynamics
 
@@ -208,17 +208,17 @@
     assert hasattr(garray, '__len__') and len(garray) == 3
     assert caarray.shape == (3, 2)
     assert cbarray.shape == (3, 2)
     assert hasattr(caEQarray, '__len__') and len(caEQarray) == 2
     assert hasattr(caEQarray, '__len__') and len(caEQarray) == 2
 
     #Compare to Thermodynamics, high tolerance since we're just checking that functions are interchangeable
-    assert_allclose(g, gT, rtol=1e-1)
-    assert_allclose(ca, caT, rtol=1e-1)
-    assert_allclose(cb, cbT, rtol=1e-1)
+    assert_allclose(g, gT, atol=0, rtol=1e-1)
+    assert_allclose(ca, caT, atol=0, rtol=1e-1)
+    assert_allclose(cb, cbT, atol=0, rtol=1e-1)
 
 def test_Surr_ternary_save():
     '''
     Checks that multicomponent surrogate can be saved and loaded
     '''
     surr = MulticomponentSurrogate(NiCrAlTherm)
     T = [1073.15, 1123.15]
@@ -236,15 +236,15 @@
     surr2 = MulticomponentSurrogate.load('kawin/tests/nicral')
     a2, b2 = surr2.getDrivingForce([0.08, 0.1], T[0]+25, True)
     g2, ca2, cb2, _, _ = surr2.getGrowthAndInterfacialComposition([0.08, 0.1], T[0]+25, 900, 1e-9, 1000)
     beta2 = surr2.impingementFactor([0.08, 0.1], T[0]+25)
 
     os.remove('kawin/tests/nicral')
 
-    assert_allclose([a, b[0], b[1], g, ca[0], ca[1], cb[0], cb[1], beta], [a2, b2[0], b2[1], g2, ca2[0], ca2[1], cb2[0], cb2[1], beta2], rtol=1e-3)
+    assert_allclose([a, b[0], b[1], g, ca[0], ca[1], cb[0], cb[1], beta], [a2, b2[0], b2[1], g2, ca2[0], ca2[1], cb2[0], cb2[1], beta2], atol=0, rtol=1e-3)
 
 def test_Surr_ternary_save_missing():
     '''
     Checks that load function will not fail if one of the three surrogates are not trained yet
     '''
     surr = MulticomponentSurrogate(NiCrAlTherm)
     T = [1073.15, 1123.15]
@@ -254,8 +254,8 @@
     a, b = surr.getDrivingForce([0.08, 0.1], T[0]+25, True)
     surr.save('kawin/tests/nicral')
 
     surr2 = MulticomponentSurrogate.load('kawin/tests/nicral')
     a2, b2 = surr2.getDrivingForce([0.08, 0.1], T[0]+25, True)
     os.remove('kawin/tests/nicral')
 
-    assert_allclose([a, b[0], b[1]], [a2, b2[0], b2[1]], rtol=1e-3)
+    assert_allclose([a, b[0], b[1]], [a2, b2[0], b2[1]], atol=0, rtol=1e-3)
```

### Comparing `kawin-0.1.2/kawin/tests/test_thermodynamics.py` & `kawin-0.2.0/kawin/tests/test_thermodynamics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import numpy as np
 from numpy.testing import assert_allclose
-from kawin.Thermodynamics import BinaryThermodynamics, MulticomponentThermodynamics
+from kawin.Thermodynamics import BinaryThermodynamics, GeneralThermodynamics, MulticomponentThermodynamics
 from kawin.tests.datasets import *
+from pycalphad import Database
 
 AlZrTherm = BinaryThermodynamics(ALZR_TDB, ['AL', 'ZR'], ['FCC_A1', 'AL3ZR'], drivingForceMethod='approximate')
 NiCrAlTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
+NiCrAlThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'CR', 'AL'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
 NiAlCrTherm = MulticomponentThermodynamics(NICRAL_TDB, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
+NiAlCrThermDiff = MulticomponentThermodynamics(NICRAL_TDB_DIFF, ['NI', 'AL', 'CR'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
 AlCrNiTherm = MulticomponentThermodynamics(NICRAL_TDB, ['AL', 'CR', 'NI'], ['FCC_A1', 'FCC_L12'], drivingForceMethod='approximate')
 
 #Set constant sampling densities for each Thermodynamics object
 #pycalphad equilibrium results may change based off sampling density, so this is to make sure
 #tests won't failed unneccesarily because the default sampling densities are modified
 AlZrTherm.setDFSamplingDensity(2000)
 AlZrTherm.setEQSamplingDensity(500)
 NiCrAlTherm.setDFSamplingDensity(2000)
 NiCrAlTherm.setEQSamplingDensity(500)
+NiCrAlThermDiff.setDFSamplingDensity(2000)
+NiCrAlThermDiff.setEQSamplingDensity(500)
 NiAlCrTherm.setDFSamplingDensity(2000)
 NiAlCrTherm.setEQSamplingDensity(500)
+NiAlCrThermDiff.setDFSamplingDensity(2000)
+NiAlCrThermDiff.setEQSamplingDensity(500)
 AlCrNiTherm.setDFSamplingDensity(2000)
 AlCrNiTherm.setEQSamplingDensity(500)
 
 def test_DG_binary():
     '''
     Checks value of binary driving force calculation
     '''
     dg, _ = AlZrTherm.getDrivingForce(0.004, 673.15, training = True)
-    assert_allclose(dg, 6346.929428, rtol=1e-3)
+    assert_allclose(dg, 6346.929428, atol=0, rtol=1e-3)
 
 def test_DG_binary_output():
     '''
     Checks that output of binary driving force calculation follows input
     Ex. for f(x, T) -> (dg, xP)
         (scalar, scalar) input -> scalar
         (array, array) input -> array
@@ -43,15 +50,15 @@
     assert hasattr(xParray, '__len__') and len(xParray) == 2
 
 def test_DG_ternary():
     '''
     Checks value of ternary driving force calculation
     '''
     dg, _ = NiCrAlTherm.getDrivingForce([0.08, 0.1], 1073.15, training = True)
-    assert_allclose(dg, 244.012027, rtol=1e-3)
+    assert_allclose(dg, 244.012027, atol=0, rtol=1e-3)
 
 def test_DG_ternary_output():
     '''
     Checks that output of ternary driving force calculations follow input
     Ex. for f(x, T) -> (dg, xP)
         (array, scalar) -> scalar
         (2D array, array) -> array
@@ -69,23 +76,23 @@
     Ex. Input elements as [Ni, Cr, Al] should require composition to be [Cr, Al]
         Input elements as [Ni, Al, Cr] should require composition to be [Al, Cr]
         Input elements as [Al, Cr, Ni] should require composition to be [Cr, Ni]
     '''
     dg1, _ = NiCrAlTherm.getDrivingForce([0.08, 0.1], 1073.15, training = True)
     dg2, _ = NiAlCrTherm.getDrivingForce([0.1, 0.08], 1073.15, training = True)
     dg3, _ = AlCrNiTherm.getDrivingForce([0.08, 0.82], 1073.15, training = True)
-    assert_allclose(dg1, dg2, rtol=1e-3)
-    assert_allclose(dg2, dg3, rtol=1e-3)
+    assert_allclose(dg1, dg2, atol=0, rtol=1e-3)
+    assert_allclose(dg2, dg3, atol=0, rtol=1e-3)
 
 def test_IC_binary():
     '''
     Check value of interfacial composition for binary case
     '''
     xm, xp = AlZrTherm.getInterfacialComposition(673.15, 10000)
-    assert_allclose(xm, 0.0233507, rtol=1e-3)
+    assert_allclose(xm, 0.0233507, atol=0, rtol=1e-3)
 
 def test_IC_unstable():
     '''
     Checks that (-1, -1) is returned for unstable precipitate
     '''
     xm, xp = AlZrTherm.getInterfacialComposition(673.15, 50000)
     assert(xm == -1 and xp == -1)
@@ -110,15 +117,15 @@
     assert hasattr(xparray2, '__len__') and len(xparray2) == 2
 
 def test_Mob_binary():
     '''
     Checks value of binary interdiffusvity calculation
     '''
     dnkj = AlZrTherm.getInterdiffusivity(0.004, 673.15)
-    assert_allclose(dnkj, 1.280344e-20, rtol=1e-3)
+    assert_allclose(dnkj, 1.280344e-20, atol=0, rtol=1e-3)
 
 def test_Mob_binary_output():
     '''
     Checks output of binary mobility follows input
     Ex. f(x, T) = diff
         (scalar, scalar) -> scalar
         (array, array) -> array
@@ -129,15 +136,15 @@
     assert hasattr(dnkjarray, '__len__') and len(dnkjarray) == 2
 
 def test_Mob_ternary():
     '''
     Checks value of ternary interdiffusivity calculation
     '''
     dnkj = NiCrAlTherm.getInterdiffusivity([0.08, 0.1], 1073.15)
-    assert_allclose(dnkj, [[8.239509e-18, 4.433713e-18], [2.339385e-17, 5.049116e-17]], rtol=1e-3)
+    assert_allclose(dnkj, [[8.239509e-18, 4.433713e-18], [2.339385e-17, 5.049116e-17]], atol=0, rtol=1e-3)
 
 def test_Mob_ternary_output():
     '''
     Checks output of multicomponent mobility follows input
     Ex. f(x, T) = diff
         (array, scalar) -> 2D array
         (2D array, array) -> 3D array
@@ -154,15 +161,15 @@
     Ex. [Ni, Cr, Al] should give diffusivity matrix of [[D_CrCr, D_CrAl], [D_AlCr, D_AlAl]]
         and [Ni, Al, Cr] should give [[D_AlAl, D_AlCr], [D_CrAl, D_CrCr]]
     '''
     dnkj1 = NiCrAlTherm.getInterdiffusivity([0.08, 0.1], 1073.15)
     dnkj2 = NiAlCrTherm.getInterdiffusivity([0.1, 0.08], 1073.15)
     dnkj2[:,[0,1]] = dnkj2[:,[1,0]]
     dnkj2[[0,1],:] = dnkj2[[1,0],:]
-    assert_allclose(dnkj1, dnkj2, rtol=1e-3)
+    assert_allclose(dnkj1, dnkj2, atol=0, rtol=1e-3)
 
 def test_Curv_ternary():
     '''
     Checks that order of elements does not matter for curvature calculations
     '''
     n1, d1, g1, b1, ca1, cb1 = NiCrAlTherm.curvatureFactor([0.08, 0.1], 1073.15, training = True)
     n2, d2, g2, b2, ca2, cb2 = NiAlCrTherm.curvatureFactor([0.1, 0.08], 1073.15, training = True)
@@ -174,24 +181,24 @@
     ca2[[0,1]] = ca2[[1,0]]
     cb2[[0,1]] = cb2[[1,0]]
     ca3change = [ca3[0], 1-ca3[0]-ca3[1]]
     cb3change = [cb3[0], 1-cb3[0]-cb3[1]]
 
     #Will only test d3, b3 and ca3,cb3
     #n3 and g3 cannot be directly compared to n1 and g1
-    assert_allclose(n1, n2, rtol=1e-3)
-    assert_allclose(d1, d2, rtol=1e-3)
-    assert_allclose(d1, d3, rtol=1e-3)
-    assert_allclose(g1, g2, rtol=1e-3)
-    assert_allclose(b1, b2, rtol=1e-3)
-    assert_allclose(b1, b3, rtol=1e-3)
-    assert_allclose(ca1, ca2, rtol=1e-3)
-    assert_allclose(ca1, ca3change, rtol=1e-3)
-    assert_allclose(cb1, cb2, rtol=1e-3)
-    assert_allclose(cb1, cb3change, rtol=1e-3)
+    assert_allclose(n1, n2, atol=0, rtol=1e-3)
+    assert_allclose(d1, d2, atol=0, rtol=1e-3)
+    assert_allclose(d1, d3, atol=0, rtol=1e-3)
+    assert_allclose(g1, g2, atol=0, rtol=1e-3)
+    assert_allclose(b1, b2, atol=0, rtol=1e-3)
+    assert_allclose(b1, b3, atol=0, rtol=1e-3)
+    assert_allclose(ca1, ca2, atol=0, rtol=1e-3)
+    assert_allclose(ca1, ca3change, atol=0, rtol=1e-3)
+    assert_allclose(cb1, cb2, atol=0, rtol=1e-3)
+    assert_allclose(cb1, cb3change, atol=0, rtol=1e-3)
 
 def test_IC_ternary():
     '''
     Checks that order does not matter for growth and interfacial composition calculations
     Ignore equilibrium compositions since growth and interfacial compositions depend on them anyways
         If growth and interfacial compositions are correct, then equilibrium compositions are also correct
     '''
@@ -203,22 +210,22 @@
     ca2[[0,1]] = ca2[[1,0]]
     cb2[[0,1]] = cb2[[1,0]]
 
     #Change ca3,cb3 from [CR, NI] to [CR, AL]
     ca3change = [ca3[0], 1-ca3[0]-ca3[1]]
     cb3change = [cb3[0], 1-cb3[0]-cb3[1]]
 
-    assert_allclose(g1, -1.618827e-09, rtol=1e-3)
+    assert_allclose(g1, -1.618827e-09, atol=0, rtol=1e-3)
 
-    assert_allclose(g1, g2, rtol=1e-3)
-    assert_allclose(g1, g3, rtol=1e-3)
-    assert_allclose(ca1, ca2, rtol=1e-3)
-    assert_allclose(ca1, ca3change, rtol=1e-3)
-    assert_allclose(cb1, cb2, rtol=1e-3)
-    assert_allclose(cb1, cb3change, rtol=1e-3)
+    assert_allclose(g1, g2, atol=0, rtol=1e-3)
+    assert_allclose(g1, g3, atol=0, rtol=1e-3)
+    assert_allclose(ca1, ca2, atol=0, rtol=1e-3)
+    assert_allclose(ca1, ca3change, atol=0, rtol=1e-3)
+    assert_allclose(cb1, cb2, atol=0, rtol=1e-3)
+    assert_allclose(cb1, cb3change, atol=0, rtol=1e-3)
 
 def test_IC_ternary_output():
     '''
     Checks that output of IC follows input
     Ex. f(x, T, dG, R, gE) -> (gr, xM, xP)
         (array, scalar, scalar, scalar, scalar) -> (scalar, array, array)
         (array, scalar, scalar, array, array) -> (array, 2D array, 2D array)
@@ -227,8 +234,93 @@
     garray, caarray, cbarray, _, _ = NiCrAlTherm.getGrowthAndInterfacialComposition([0.08, 0.1], 1073.15, 900, [0.5e-9, 1e-9, 2e-9], [2000, 1000, 500], training = True)
 
     assert np.isscalar(g) or (type(g) == np.ndarray and g.ndim == 0)
     assert hasattr(ca, '__len__') and len(ca) == 2
     assert hasattr(cb, '__len__') and len(cb) == 2
     assert hasattr(garray, '__len__') and len(garray) == 3
     assert caarray.shape == (3, 2)
-    assert cbarray.shape == (3, 2)
+    assert cbarray.shape == (3, 2)
+
+
+def test_initialize_with_pycalphad_database():
+    """
+    Checks that a pycalphad Database object can be passed to the kawin.GeneralThermodynamics class.
+    """
+    GeneralThermodynamics(Database(ALZR_TDB), ['AL', 'ZR'], ['FCC_A1', 'AL3ZR'], drivingForceMethod='approximate')
+
+def test_initialize_with_single_phase():
+    """
+    Checks if a single phase was passed as a string instead of multiple phases passed as a list of strings.
+    """
+    GeneralThermodynamics(ALZR_TDB, ['AL', 'ZR'], 'FCC_A1')
+
+def test_Mob_tracer_ternary():
+    '''
+    Checks value of ternary tracer diffusivity calculation
+    '''
+    td = NiCrAlTherm.getTracerDiffusivity([0.08, 0.1], 1073.15)
+    assert_allclose(td, [8.039466e-18, 5.465542e-18, 1.520994e-17], rtol=1e-3)
+
+def test_Mob_tracer_ternary_output():
+    '''
+    Checks output of multicomponent mobility follows input
+    Ex. f(x, T) = diff
+        (array, scalar) -> 2D array
+        (2D array, array) -> 3D array
+    '''
+    td = NiCrAlTherm.getTracerDiffusivity([0.08, 0.1], 1073.15)
+    tdarray = NiCrAlTherm.getTracerDiffusivity([[0.08, 0.1], [0.085, 0.1]], [1073.15, 1078.15])
+
+    assert td.shape == (3,)
+    assert tdarray.shape == (2, 3)
+
+def test_Diff_ternary():
+    '''
+    Checks value of ternary interdiffusivity calculation
+    '''
+    dnkj = NiCrAlThermDiff.getInterdiffusivity([0.08, 0.1], 1073.15)
+    assert_allclose(dnkj, [[3.099307e-8, 0], [0, 1.958226e-8]], atol=0, rtol=1e-3)
+
+def test_Diff_ternary_output():
+    '''
+    Checks output of multicomponent mobility follows input
+    Ex. f(x, T) = diff
+        (array, scalar) -> 2D array
+        (2D array, array) -> 3D array
+    '''
+    dnkj = NiCrAlThermDiff.getInterdiffusivity([0.08, 0.1], 1073.15)
+    dnkjarray = NiCrAlThermDiff.getInterdiffusivity([[0.08, 0.1], [0.085, 0.1], [0.09, 0.1]], [1073.15, 1078.15, 1083.15])
+
+    assert dnkj.shape == (2, 2)
+    assert dnkjarray.shape == (3, 2, 2)
+
+def test_Diff_order():
+    '''
+    Test diffusivity matrix is given in correct order as input elements
+    Ex. [Ni, Cr, Al] should give diffusivity matrix of [[D_CrCr, D_CrAl], [D_AlCr, D_AlAl]]
+        and [Ni, Al, Cr] should give [[D_AlAl, D_AlCr], [D_CrAl, D_CrCr]]
+    '''
+    dnkj1 = NiCrAlThermDiff.getInterdiffusivity([0.08, 0.1], 1073.15)
+    dnkj2 = NiAlCrThermDiff.getInterdiffusivity([0.1, 0.08], 1073.15)
+    dnkj2[:,[0,1]] = dnkj2[:,[1,0]]
+    dnkj2[[0,1],:] = dnkj2[[1,0],:]
+    assert_allclose(dnkj1, dnkj2, atol=0, rtol=1e-3)
+
+def test_Diff_tracer_ternary():
+    '''
+    Checks value of ternary tracer diffusivity calculation
+    '''
+    td = NiCrAlThermDiff.getTracerDiffusivity([0.08, 0.1], 1073.15)
+    assert_allclose(td, [7.357088e-18, 3.099307e-8, 1.958226e-8], atol=0, rtol=1e-3)
+
+def test_Diff_tracer_ternary_output():
+    '''
+    Checks output of multicomponent mobility follows input
+    Ex. f(x, T) = diff
+        (array, scalar) -> 2D array
+        (2D array, array) -> 3D array
+    '''
+    td = NiCrAlTherm.getTracerDiffusivity([0.08, 0.1], 1073.15)
+    tdarray = NiCrAlTherm.getTracerDiffusivity([[0.08, 0.1], [0.085, 0.1]], [1073.15, 1078.15])
+
+    assert td.shape == (3,)
+    assert tdarray.shape == (2, 3)
```

### Comparing `kawin-0.1.2/kawin.egg-info/PKG-INFO` & `kawin-0.2.0/kawin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kawin
-Version: 0.1.2
+Version: 0.2.0
 Summary: Tool for simulating precipitation using the KWN model coupled with Calphad.
 Home-page: https://kawin.org/
 Author: Nicholas Ury
 Author-email: nury12n@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `kawin-0.1.2/kawin.egg-info/SOURCES.txt` & `kawin-0.2.0/kawin.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-.gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+kawin/Diffusion.py
 kawin/EffectiveDiffusion.py
 kawin/ElasticFactors.py
 kawin/FreeEnergyHessian.py
 kawin/GrainBoundaries.py
 kawin/KWNBase.py
 kawin/KWNEuler.py
 kawin/LebedevNodes.py
 kawin/LocalEquilibrium.py
 kawin/Mobility.py
 kawin/PopulationBalance.py
 kawin/ShapeFactors.py
+kawin/Strength.py
 kawin/Surrogate.py
 kawin/Thermodynamics.py
 kawin/__init__.py
 kawin.egg-info/PKG-INFO
 kawin.egg-info/SOURCES.txt
 kawin.egg-info/dependency_links.txt
 kawin.egg-info/requires.txt
 kawin.egg-info/top_level.txt
 kawin/tests/datasets.py
 kawin/tests/test_PBM.py
+kawin/tests/test_diffusion.py
 kawin/tests/test_extraFactors.py
+kawin/tests/test_strength.py
 kawin/tests/test_surrogate.py
 kawin/tests/test_thermodynamics.py
```

### Comparing `kawin-0.1.2/setup.py` & `kawin-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author_email='nury12n@gmail.com',
     description='Tool for simulating precipitation using the KWN model coupled with Calphad.',
     packages=['kawin', 'kawin.tests'],
     license='MIT',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     url='https://kawin.org/',
-    version='0.1.2',
+    version='0.2.0',
     install_requires=[
         'matplotlib>=3.3',
         'numpy>=1.13',
         'pycalphad>=0.10.1',
         'scipy',
         'setuptools_scm[toml]>=6.0',
     ],
```

