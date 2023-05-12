# Comparing `tmp/pysfa-0.5.tar.gz` & `tmp/pysfa-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfa-0.5.tar", last modified: Wed May 10 18:20:17 2023, max compression
+gzip compressed data, was "pysfa-0.6.tar", last modified: Fri May 12 13:53:28 2023, max compression
```

## Comparing `pysfa-0.5.tar` & `pysfa-0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 18:20:06.000000 pysfa-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 18:20:17.631670 pysfa-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 18:20:06.000000 pysfa-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/SFA.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/data/41Firm.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/data/electricityFirms.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:20:17.631670 pysfa-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-10 18:20:06.000000 pysfa-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:53:28.430597 pysfa-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 13:53:17.000000 pysfa-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 13:53:28.430597 pysfa-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-12 13:53:17.000000 pysfa-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:53:28.430597 pysfa-0.6/pysfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/SFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:53:28.430597 pysfa-0.6/pysfa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:53:28.430597 pysfa-0.6/pysfa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-12 13:53:17.000000 pysfa-0.6/pysfa/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:53:28.430597 pysfa-0.6/pysfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 13:53:28.000000 pysfa-0.6/pysfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:53:28.430597 pysfa-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 13:53:17.000000 pysfa-0.6/setup.py
```

### Comparing `pysfa-0.5/LICENSE` & `pysfa-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/PKG-INFO` & `pysfa-0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.5
+Version: 0.6
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -59,10 +59,15 @@
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
+# print statistics
+print(res.get_pvalue())
+print(res.get_tvalue())
+print(res.get_std_err())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.5/README.md` & `pysfa-0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,15 @@
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
+# print statistics
+print(res.get_pvalue())
+print(res.get_tvalue())
+print(res.get_std_err())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.5/pysfa/SFA.py` & `pysfa-0.6/pysfa/SFA.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from sklearn.linear_model import LinearRegression
 from math import sqrt, pi, log
-from scipy.stats import norm
-import scipy.optimize as opt
+from scipy.stats import norm, t
+from scipy.optimize import minimize
 from .constant import FUN_PROD, FUN_COST, TE_teJ, TE_te, TE_teMod
 from .utils import tools
 
 
 class SFA:
     """Stochastic frontier analysis (SFA) 
     """
@@ -18,16 +18,16 @@
               y (float) : output variable. 
               x (float) : input variables.
               intercept (bool, optional): whether to include intercept. Defaults to True.
               lamda0 (float, optional): initial value of lambda. Defaults to 1.
               fun (String, optional): FUN_PROD (production function) or FUN_COST (cost function). Defaults to FUN_PROD.
               method (String, optional): TE_teJ, TE_te, or TE_teMod. Defaults to TE_teJ.
           """
-        self.y, self.x = tools.assert_valid_basic_data(y, x, fun)
         self.fun, self.intercept, self.lamda0, self.method = fun, intercept, lamda0, method
+        self.y, self.x = tools.assert_valid_basic_data(y, x, self.fun)
 
     def __mle(self):
 
         # initial OLS regression
         if self.intercept == False:
             reg = LinearRegression(fit_intercept=False).fit(X=self.x, y=self.y)
             parm = np.concatenate((reg.coef_, [self.lamda0]), axis=0)
@@ -41,37 +41,42 @@
             ''' Log-likelihood function'''
             N = len(self.x)
             if self.intercept == False:
                 K = len(self.x[0])
             elif self.intercept == True:
                 K = len(self.x[0]) + 1
             beta0, lamda0 = parm[0:K], parm[K]
-            e = self.__resfun(beta0)
-            s = np.sum(e**2)/N
-            z = -lamda0*e/sqrt(s)
+            res = self.__resfun(beta0)
+            sig2 = np.sum(res**2)/N
+            z = -lamda0*res/sqrt(sig2)
             pz = np.maximum(norm.cdf(z), 1e-323)
-            return N/2*log(pi/2) + N/2*log(s) - np.sum(np.log(pz)) + N/2.0
+            return N/2*log(pi/2) + N/2*log(sig2) - np.sum(np.log(pz)) + N/2.0
 
-        fit = opt.minimize(__loglik, parm, method='BFGS').x
+        fit = minimize(__loglik, parm, method='BFGS')
 
         # beta, residuals, lambda, sigma^2
         if self.intercept == False:
             K = len(self.x[0])
         elif self.intercept == True:
             K = len(self.x[0]) + 1
-        self.beta = fit[0:K]
+        self.beta = fit.x[0:K]
         self.residuals = self.__resfun(self.beta)
-        self.lamda = fit[K]
+        self.lamda = fit.x[K]
         self.sigma2 = np.sum(self.residuals ** 2)/self.residuals.shape[0]
 
         # sigma_u^2, sigma_v^2
         self.s2u = self.lamda**2 / (1+self.lamda**2) * self.sigma2
         self.s2v = self.sigma2 / (1+self.lamda**2)
 
-        return self.beta, self.residuals, self.lamda, self.sigma2, self.s2u, self.s2v
+        # calculate standard error, t-value, and p-value
+        self.vcov = fit.hess_inv
+        self.std_err = np.sqrt(np.diag(self.vcov))
+        self.tvalue = fit.x / self.std_err
+        self.pvalue = np.around(
+            2 * t.sf(abs(self.tvalue), len(self.x) - K), decimals=3)
 
     def __resfun(self, beta):
         if self.intercept == False:
             return self.y - np.dot(self.x, beta[0:])
         elif self.intercept == True:
             return self.y - beta[0] - np.dot(self.x, beta[1:])
 
@@ -112,47 +117,61 @@
             self.sign == -1
         else:
             self.sign = 1
         self.ustar = - self.sign * self.residuals * \
             self.lamda**2/(1+self.lamda**2)
         return np.exp(np.minimum(0, -self.ustar))
 
-    def get_technical_efficiency(self):
-        """
-        Args:
-              method (String, optional): TE_teJ, TE_te, or TE_teMod. Defaults to TE_teJ.
+    def __model_estimation(self):
+        '''Model estimation'''
 
-        calculate technical efficiency
-        """
         self.__mle()
         if self.method == TE_teJ:
-            return self.__teJ()
+            self.te = self.__teJ()
         elif self.method == TE_te:
-            return self.__te()
+            self.te = self.__te()
         elif self.method == TE_teMod:
-            return self.__teMod()
+            self.te = self.__teMod()
         else:
             raise ValueError("Undefined decomposition technique.")
 
+        return self.beta, self.residuals, self.lamda, self.sigma2, self.s2u, self.s2v, self.std_err, self.tvalue, self.pvalue, self.te
+
     def get_beta(self):
         '''Return the estimated coefficients'''
-        return self.__mle()[0]
+        return self.__model_estimation()[0]
 
     def get_residuals(self):
         '''Return the residuals'''
-        return self.__mle()[1]
+        return self.__model_estimation()[1]
 
     def get_lambda(self):
         '''Return the lambda'''
-        return self.__mle()[2]
+        return self.__model_estimation()[2]
 
     def get_sigma2(self):
         '''Return the sigma2'''
-        return self.__mle()[3]
+        return self.__model_estimation()[3]
 
     def get_sigmau2(self):
         '''Return the sigma_u**2'''
-        return self.__mle()[4]
+        return self.__model_estimation()[4]
 
     def get_sigmav2(self):
         '''Return the sigma_v**2'''
-        return self.__mle()[5]
+        return self.__model_estimation()[5]
+
+    def get_std_err(self):
+        '''Return the standard errors'''
+        return self.__model_estimation()[6]
+
+    def get_tvalue(self):
+        '''Return the standard errors'''
+        return self.__model_estimation()[7]
+
+    def get_pvalue(self):
+        '''Return the standard errors'''
+        return self.__model_estimation()[8]
+
+    def get_technical_efficiency(self):
+        '''Return the technical efficiency'''
+        return self.__model_estimation()[9]
```

### Comparing `pysfa-0.5/pysfa/constant.py` & `pysfa-0.6/pysfa/constant.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/pysfa/data/41Firm.csv` & `pysfa-0.6/pysfa/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/pysfa/data/electricityFirms.csv` & `pysfa-0.6/pysfa/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/pysfa/dataset.py` & `pysfa-0.6/pysfa/dataset.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/pysfa/utils/tools.py` & `pysfa-0.6/pysfa/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.5/pysfa.egg-info/PKG-INFO` & `pysfa-0.6/pysfa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.5
+Version: 0.6
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -59,10 +59,15 @@
 
 # print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
+# print statistics
+print(res.get_pvalue())
+print(res.get_tvalue())
+print(res.get_std_err())
+
 # print TE
 print(res.get_technical_efficiency())
 ```
```

### Comparing `pysfa-0.5/setup.py` & `pysfa-0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pysfa',
-    version='0.5',
+    version='0.6',
     description='A Python Package for Stochastic Frontier Analysis',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Sheng Dai, Zhiqiang Liao',
     author_email='sheng.dai@utu.fi',
```

