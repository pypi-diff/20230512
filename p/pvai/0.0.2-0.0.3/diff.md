# Comparing `tmp/pvai-0.0.2.tar.gz` & `tmp/pvai-0.0.3.tar.gz`

## Comparing `pvai-0.0.2.tar` & `pvai-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/__init__.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/analysis.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/categorical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/.ipynb_checkpoints/analysis-checkpoint.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 pvai-0.0.2/src/pvai/.ipynb_checkpoints/categorical-checkpoint.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pvai-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pvai-0.0.2/README.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pvai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 pvai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/__init__.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/analysis.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/cleaning.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/.ipynb_checkpoints/analysis-checkpoint.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 pvai-0.0.3/src/pvai/.ipynb_checkpoints/cleaning-checkpoint.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pvai-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pvai-0.0.3/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pvai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 pvai-0.0.3/PKG-INFO
```

### Comparing `pvai-0.0.2/src/pvai/analysis.py` & `pvai-0.0.3/src/pvai/analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import numpy as np
 
 class POD():
     '''
     obj_pod = POD() : creates object
     
+    ---variables---
+    obj_pod.mean_variables: the mean per variable of the original training data
+    obj_pod.input_matrix: the centered training data ( original training data = centered + mean )
+    obj_pod.temp_modes, obj_pod.sing_values, obj_pod.spatial_modes: original values corresponding to training data
+    obj_pot.xxx_tr: the truncated version, allows to retain the original (tm_tr,sv_tr,sm_tr)
+    obj_pot.explained_var_ratio: explained variance ratio based on cumsum(SV**2)/sum(SV**2)
+    
     ---methods---
     obj_pod.fit(): gives temp_modes, sing_values, spatial_modes as attributes to obj_pod
     obj_pod.truncate(n): truncate the global library of modes and singular values (orginal library is retained)
     obj_pod.get_temp_modes(): outputs temporal modes for new samples, based on library of modes and singular values from fit
                               when using truncated = True, the truncated library is used
     obj_pod.reconstruct(): outputs reconstruction from temporal modes, based on library of modes and singular values from fit
                            when using truncated = True, the truncated library is used
-    ---variables---
-    obj_pod.mean_variables: the mean per variable of the original training data
-    obj_pod.input_matrix: the centered training data ( original training data = centered + mean )
-    obj_pod.temp_modes, obj_pod.sing_values, obj_pod.spatial_modes: original values corresponding to training data
-    obj_pot.xxx_tr: the truncated version, allows to retain the original (tm_tr,sv_tr,sm_tr)
-    obj_pot.explained_var_ratio: explained variance ratio based on cumsum(SV**2)/sum(SV**2)
     '''
     
     def __init__(self):
         self.mean_variables = None
         self.input_matrix = None
         self.temp_modes = None
         self.sing_values = None
@@ -28,33 +29,39 @@
         self.tm_tr = None
         self.sv_tr = None
         self.sm_tr = None
         self.explained_var_ratio = None
         print('new POD object')
         
     def fit(self,input_matrix):
+        '''obj_pod.fit(): gives temp_modes, sing_values, spatial_modes as attributes to obj_pod'''
         self.mean_variables = np.mean(input_matrix,axis=0)
         self.input_matrix = input_matrix - self.mean_variables
         self.temp_modes, self.sing_values, self.spatial_modes = np.linalg.svd(self.input_matrix, full_matrices=False)
         self.explained_var_ratio = np.cumsum(self.sing_values ** 2) / np.sum(self.sing_values ** 2)
         print('fitted %i samples, for %i modes and %i variables'%(input_matrix.shape[0],len(self.sing_values),input_matrix.shape[1]))
         print(f'first mode where exp var ratio is larger than 99% is {np.where(self.explained_var_ratio>0.99)[0][0]}')
         
     def truncate(self,n):
+        '''obj_pod.truncate(n): truncate the global library of modes and singular values (orginal library is retained)'''
         self.tm_tr = self.temp_modes[:,:n]
         self.sv_tr = self.sing_values[:n]
         self.sm_tr = self.spatial_modes[:n,:]
         print('truncated from %s to %s modes'%(str(self.spatial_modes.shape[0]),str(self.sm_tr.shape[0])))
 
     def get_temp_modes(self,input_samples,truncated=False):
+        '''obj_pod.get_temp_modes(input_samples,truncated=False): outputs temporal modes for new samples,
+        based on library of modes and singular values from fit when using truncated = True, the truncated library is used'''
         if truncated:
             temp_modes = (input_samples - self.mean_variables).dot(self.sm_tr.T).dot(np.linalg.inv(np.diag(self.sv_tr)))
         else:
             temp_modes = (input_samples - self.mean_variables).dot(self.spatial_modes.T).dot(np.linalg.inv(np.diag(self.sing_values)))     
         return(temp_modes)
     
     def reconstruct(self,temp_modes,truncated=False):
+        '''obj_pod.reconstruct(): outputs reconstruction from temporal modes, based on library of modes and singular values
+        from fit when using truncated = True, the truncated library is used'''
         if truncated:
             reconstruction = temp_modes.dot(np.diag(self.sv_tr)).dot(self.sm_tr)+self.mean_variables     
         else:
             reconstruction = temp_modes.dot(np.diag(self.sing_values)).dot(self.spatial_modes)+self.mean_variables
         return(reconstruction)
```

### Comparing `pvai-0.0.2/src/pvai/.ipynb_checkpoints/analysis-checkpoint.py` & `pvai-0.0.3/src/pvai/.ipynb_checkpoints/analysis-checkpoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import numpy as np
 
 class POD():
     '''
     obj_pod = POD() : creates object
     
+    ---variables---
+    obj_pod.mean_variables: the mean per variable of the original training data
+    obj_pod.input_matrix: the centered training data ( original training data = centered + mean )
+    obj_pod.temp_modes, obj_pod.sing_values, obj_pod.spatial_modes: original values corresponding to training data
+    obj_pot.xxx_tr: the truncated version, allows to retain the original (tm_tr,sv_tr,sm_tr)
+    obj_pot.explained_var_ratio: explained variance ratio based on cumsum(SV**2)/sum(SV**2)
+    
     ---methods---
     obj_pod.fit(): gives temp_modes, sing_values, spatial_modes as attributes to obj_pod
     obj_pod.truncate(n): truncate the global library of modes and singular values (orginal library is retained)
     obj_pod.get_temp_modes(): outputs temporal modes for new samples, based on library of modes and singular values from fit
                               when using truncated = True, the truncated library is used
     obj_pod.reconstruct(): outputs reconstruction from temporal modes, based on library of modes and singular values from fit
                            when using truncated = True, the truncated library is used
-    ---variables---
-    obj_pod.mean_variables: the mean per variable of the original training data
-    obj_pod.input_matrix: the centered training data ( original training data = centered + mean )
-    obj_pod.temp_modes, obj_pod.sing_values, obj_pod.spatial_modes: original values corresponding to training data
-    obj_pot.xxx_tr: the truncated version, allows to retain the original (tm_tr,sv_tr,sm_tr)
-    obj_pot.explained_var_ratio: explained variance ratio based on cumsum(SV**2)/sum(SV**2)
     '''
     
     def __init__(self):
         self.mean_variables = None
         self.input_matrix = None
         self.temp_modes = None
         self.sing_values = None
@@ -28,33 +29,39 @@
         self.tm_tr = None
         self.sv_tr = None
         self.sm_tr = None
         self.explained_var_ratio = None
         print('new POD object')
         
     def fit(self,input_matrix):
+        '''obj_pod.fit(): gives temp_modes, sing_values, spatial_modes as attributes to obj_pod'''
         self.mean_variables = np.mean(input_matrix,axis=0)
         self.input_matrix = input_matrix - self.mean_variables
         self.temp_modes, self.sing_values, self.spatial_modes = np.linalg.svd(self.input_matrix, full_matrices=False)
         self.explained_var_ratio = np.cumsum(self.sing_values ** 2) / np.sum(self.sing_values ** 2)
         print('fitted %i samples, for %i modes and %i variables'%(input_matrix.shape[0],len(self.sing_values),input_matrix.shape[1]))
         print(f'first mode where exp var ratio is larger than 99% is {np.where(self.explained_var_ratio>0.99)[0][0]}')
         
     def truncate(self,n):
+        '''obj_pod.truncate(n): truncate the global library of modes and singular values (orginal library is retained)'''
         self.tm_tr = self.temp_modes[:,:n]
         self.sv_tr = self.sing_values[:n]
         self.sm_tr = self.spatial_modes[:n,:]
         print('truncated from %s to %s modes'%(str(self.spatial_modes.shape[0]),str(self.sm_tr.shape[0])))
 
     def get_temp_modes(self,input_samples,truncated=False):
+        '''obj_pod.get_temp_modes(input_samples,truncated=False): outputs temporal modes for new samples,
+        based on library of modes and singular values from fit when using truncated = True, the truncated library is used'''
         if truncated:
             temp_modes = (input_samples - self.mean_variables).dot(self.sm_tr.T).dot(np.linalg.inv(np.diag(self.sv_tr)))
         else:
             temp_modes = (input_samples - self.mean_variables).dot(self.spatial_modes.T).dot(np.linalg.inv(np.diag(self.sing_values)))     
         return(temp_modes)
     
     def reconstruct(self,temp_modes,truncated=False):
+        '''obj_pod.reconstruct(): outputs reconstruction from temporal modes, based on library of modes and singular values
+        from fit when using truncated = True, the truncated library is used'''
         if truncated:
             reconstruction = temp_modes.dot(np.diag(self.sv_tr)).dot(self.sm_tr)+self.mean_variables     
         else:
             reconstruction = temp_modes.dot(np.diag(self.sing_values)).dot(self.spatial_modes)+self.mean_variables
         return(reconstruction)
```

### Comparing `pvai-0.0.2/LICENSE.txt` & `pvai-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pvai-0.0.2/pyproject.toml` & `pvai-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling","numpy==1.21.5","pandas==1.3.5"]
+requires = ["hatchling","numpy==1.21.5","pandas==1.3.5","matplotlib"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pvai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Francis De Voogt", email="francisdevoogt@hotmail.com" },
 ]
 description = "Data processing package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

