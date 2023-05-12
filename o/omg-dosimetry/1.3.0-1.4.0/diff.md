# Comparing `tmp/omg_dosimetry-1.3.0.tar.gz` & `tmp/omg_dosimetry-1.4.0.tar.gz`

## Comparing `omg_dosimetry-1.3.0.tar` & `omg_dosimetry-1.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/requirements.txt
--rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/OMG_Logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/__init__.py
--rw-r--r--   0        0        0    42147 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/analysis.py
--rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/calibration.py
--rw-r--r--   0        0        0    41899 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/imageRGB.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/src/omg_dosimetry/tiff2dose.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/LICENSE
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/requirements.txt
+-rw-r--r--   0        0        0    27306 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/OMG_Logo.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/__init__.py
+-rw-r--r--   0        0        0    44160 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/analysis.py
+-rw-r--r--   0        0        0    37873 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/calibration.py
+-rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/imageRGB.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/src/omg_dosimetry/tiff2dose.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 omg_dosimetry-1.4.0/PKG-INFO
```

### Comparing `omg_dosimetry-1.3.0/requirements.txt` & `omg_dosimetry-1.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/src/omg_dosimetry/OMG_Logo.png` & `omg_dosimetry-1.4.0/src/omg_dosimetry/OMG_Logo.png`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/src/omg_dosimetry/analysis.py` & `omg_dosimetry-1.4.0/src/omg_dosimetry/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 Written by Jean-Francois Cabana
 Version 2023-03-08
 """
 
 import numpy as np
 import scipy.ndimage.filters as spf
 import copy
+import matplotlib
 import matplotlib.pyplot as plt
 import os
 from pylinac.core.utilities import is_close
 import math
 from scipy.signal import medfilt
 import pickle
 from pylinac.core import pdf
 import io
 from pathlib import Path
 import pymedphys
 from matplotlib.widgets  import RectangleSelector, MultiCursor, Cursor
 import webbrowser
 from .imageRGB import load, ArrayImage, equate_images
 import bz2
+import time
 
 class DoseAnalysis(): 
     
     def __init__(self, film_dose=None, ref_dose=None, film_dose_factor=1, ref_dose_factor=1, flipLR=False, flipUD=False, rot90=0, ref_dose_sum=False): 
         if film_dose is not None: self.film_dose = load(film_dose)
         if rot90: self.film_dose.array = np.rot90(self.film_dose.array, k=rot90)
         if flipLR: self.film_dose.array = np.fliplr(self.film_dose.array)
@@ -212,19 +214,21 @@
             self.film_dose.crop(bottom,'bottom')  
             
             self.fig.canvas.mpl_disconnect(self.cid)
             plt.close(self.fig)   
             self.wait = False
             return
         
-    def gamma_analysis(self, film_filt=0, doseTA=3.0, distTA=3.0, threshold=0.1, norm_val='max', local_gamma=False):
+    def gamma_analysis(self, film_filt=0, doseTA=3.0, distTA=3.0, threshold=0.1, norm_val='max', local_gamma=False, max_gamma=None, random_subset=None):
         """ Perform Gamma analysis """
         self.doseTA, self.distTA = doseTA, distTA
         self.film_filt, self.threshold, self.norm_val = film_filt, threshold, norm_val        
-        self.GammaMap = self.computeGamma(doseTA=doseTA, distTA=distTA, threshold=threshold, norm_val=norm_val, local_gamma=local_gamma)       
+        start_time = time.time()
+        self.GammaMap = self.computeGamma(doseTA=doseTA, distTA=distTA, threshold=threshold, norm_val=norm_val, local_gamma=local_gamma, max_gamma=max_gamma, random_subset=random_subset)       
+        print("--- Calcul Gamma fait en %s seconds ---" % (time.time() - start_time))
         self.computeDiff()
     
     def computeHDmedianDiff(self, threshold=0.8, ref = 'max'):
         """ Compute median difference between film and reference doses in high dose region. """
         if ref == 'max': HDthreshold = threshold * self.ref_dose.array.max()
         else:  HDthreshold = threshold * ref
         film_HD = self.film_dose.array[self.ref_dose.array > HDthreshold]
@@ -236,15 +240,15 @@
         """ Compute the difference map with the reference image.
             Returns self.DiffMap = film_dose - ref_dose """
         self.DiffMap = ArrayImage(self.film_dose.array - self.ref_dose.array, dpi=self.film_dose.dpi)
         self.RelError = ArrayImage(100*(self.film_dose.array - self.ref_dose.array)/self.ref_dose.array, dpi=self.film_dose.dpi)
         self.DiffMap.MSE =  sum(sum(self.DiffMap.array**2)) / len(self.film_dose.array[(self.film_dose.array > 0)]) 
         self.DiffMap.RMSE = self.DiffMap.MSE**0.5    
     
-    def computeGamma(self, doseTA=2, distTA=2, threshold=0.1, norm_val=None, local_gamma=False):
+    def computeGamma(self, doseTA=2, distTA=2, threshold=0.1, norm_val=None, local_gamma=False, max_gamma=None, random_subset=None):
         """Comput Gamma (using pymedphys.gamma) """
         print("Computing {}% {} mm Gamma...".format(doseTA, distTA))
 #       # error checking
         if not is_close(self.film_dose.dpi, self.ref_dose.dpi, delta=3):
             raise AttributeError("The image DPIs to not match: {:.2f} vs. {:.2f}".format(self.film_dose.dpi, self.ref_dose.dpi))
         same_x = is_close(self.film_dose.shape[1], self.ref_dose.shape[1], delta=1.1)
         same_y = is_close(self.film_dose.shape[0], self.ref_dose.shape[0], delta=1.1)
@@ -264,16 +268,24 @@
 
         # set coordinates [mm]
         x_coord = (np.array(range(0, self.ref_dose.shape[0])) / self.ref_dose.dpmm - self.ref_dose.physical_shape[0]/2).tolist()
         y_coord = (np.array(range(0, self.ref_dose.shape[1])) / self.ref_dose.dpmm - self.ref_dose.physical_shape[1]/2).tolist()
         axes_reference, axes_evaluation = (x_coord, y_coord), (x_coord, y_coord)
         dose_reference, dose_evaluation = ref_dose.array, film_dose.array
 
+        # set film_dose = 0 to Nan to avoid computing on padded pixels
+        dose_evaluation[dose_evaluation == 0] = 'nan'
+        
+        # Compute the number of pixels to analyze
+        if random_subset:
+            random_subset = int(len(dose_reference[dose_reference >= threshold].flat) * random_subset)
+        
         # Gamma computation and set maps
-        gamma = pymedphys.gamma(axes_reference, dose_reference, axes_evaluation, dose_evaluation, doseTA, distTA, threshold*100, local_gamma=local_gamma)
+        gamma = pymedphys.gamma(axes_reference, dose_reference, axes_evaluation, dose_evaluation, doseTA, distTA, threshold*100,
+                                local_gamma=local_gamma, interp_fraction=10, max_gamma=max_gamma, random_subset=random_subset)
         GammaMap = ArrayImage(gamma, dpi=film_dose.dpi)
               
         fail = np.zeros(GammaMap.shape)
         fail[(GammaMap.array > 1.0)] = 1
         GammaMap.fail = ArrayImage(fail, dpi=film_dose.dpi)
         
         passed = np.zeros(GammaMap.shape)
@@ -413,35 +425,53 @@
         
         if diff:
             diff_prof = film_prof - ref_prof
             ax.plot(x_axis, diff_prof,'g-', linewidth=2)
             
     
     def show_results(self, fig=None, x=None, y=None):       
-        if x is None: x = np.floor(self.ref_dose.shape[1] / 2).astype(int)
-        if y is None: y = np.floor(self.ref_dose.shape[0] / 2).astype(int)
+        a = None
+        if x is None:
+            x = np.floor(self.ref_dose.shape[1] / 2).astype(int)
+        elif x == 'max':
+            a = np.unravel_index(self.ref_dose.array.argmax(), self.ref_dose.array.shape)
+            x = a[1]
+        if y is None:
+            y = np.floor(self.ref_dose.shape[0] / 2).astype(int)
+        elif y == 'max':
+            if a is None:
+                a = np.unravel_index(self.ref_dose.array.argmax(), self.ref_dose.array.shape)
+            y = a[0]
          
         fig, ((ax1,ax2),(ax3,ax4),(ax5,ax6)) = plt.subplots(3,2, figsize=(10, 8))
         fig.tight_layout()
         axes = [ax1,ax2,ax3,ax4,ax5,ax6]
         max_dose_comp = np.percentile(self.ref_dose.array,[98])[0].round(decimals=-1)
         clim = [0, max_dose_comp]  
 
         self.film_dose.plotCB(ax1, clim=clim, title='Film dose')
         self.ref_dose.plotCB(ax2, clim=clim, title='Reference dose')
-        self.GammaMap.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
+        # gamma_map = ArrayImage(copy.copy(self.GammaMap.array))
+        # np.nan_to_num(gamma_map.array, copy=False, nan=1.0)
+        masked_array = np.ma.array(self.GammaMap.array, mask=np.isnan(self.GammaMap.array))
+        gamma_map = ArrayImage(masked_array)
+        cmap = matplotlib.cm.bwr
+        cmap.set_bad('k',1.)
+        gamma_map.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
+
+        # self.GammaMap.plotCB(ax3, clim=[0,2], cmap='bwr', title='Gamma map ({:.2f}% pass; {:.2f} mean)'.format(self.GammaMap.passRate, self.GammaMap.mean))
         
         min_value = max(-20, np.percentile(self.DiffMap.array,[1])[0].round(decimals=0))
         max_value = min(20, np.percentile(self.DiffMap.array,[99])[0].round(decimals=0))
         clim = [min_value, max_value]    
         self.RelError.plotCB(ax4, cmap='jet', clim=clim, title='Relative Error (%) (RMSE={:.2f})'.format(self.DiffMap.RMSE))
         self.show_profiles(axes, x=x, y=y)
         
         fig.canvas.mpl_connect('button_press_event', lambda event: self.set_profile(event, axes))
-        fig.canvas.mpl_connect('motion_notify_event', lambda event: self.moved_and_pressed(event, axes))
+        #fig.canvas.mpl_connect('motion_notify_event', lambda event: self.moved_and_pressed(event, axes))
         
     def show_profiles(self, axes, x, y):
         self.plot_profile(ax=axes[-2], profile='x', title='Horizontal profile (y={})'.format(y), position=y)
         self.plot_profile(ax=axes[-1], profile='y', title='Vertical profile (x={})'.format(x), position=x)
         
         for i in range(0,4):
             ax = axes[i]
@@ -449,18 +479,27 @@
                 ax.lines[-1].remove()
             ax.plot((x,x),(0,self.ref_dose.shape[0]),'w--', linewidth=1)
             ax.plot((0,self.ref_dose.shape[1]),(y,y),'w--', linewidth=1) 
         plt.multi = MultiCursor(None, (axes[0],axes[1],axes[2],axes[3]), color='r', lw=1, horizOn=True)
         plt.show()
         
     def set_profile(self, event, axes):
-        x = int(event.xdata)
-        y = int(event.ydata)
-        self.show_profiles(axes,x=x, y=y)
-        plt.gcf().canvas.draw_idle()
+        # Only clicks inside this axis are valid.
+        try: # use try/except in case we are not using Qt backend
+            zooming_panning = ( plt.gcf().canvas.cursor().shape() != 0 ) # 0 is the arrow, which means we are not zooming or panning.
+        except:
+            zooming_panning = False
+        if zooming_panning: 
+            return
+        if event.inaxes in axes[0:4]:
+            if event.button == 1:
+                x = int(event.xdata)
+                y = int(event.ydata)
+                self.show_profiles(axes,x=x, y=y)
+                plt.gcf().canvas.draw_idle()
         
     def moved_and_pressed(self, event, axes):
         if event.button==1:
             self.set_profile(event, axes)  
         
     def register(self, shift_x=0, shift_y=0, threshold=10, register_using_gradient=False, markers_center=None, rot=0):
         self.register_using_gradient = register_using_gradient
```

### Comparing `omg_dosimetry-1.3.0/src/omg_dosimetry/calibration.py` & `omg_dosimetry-1.4.0/src/omg_dosimetry/calibration.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/src/omg_dosimetry/imageRGB.py` & `omg_dosimetry-1.4.0/src/omg_dosimetry/imageRGB.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,17 +357,17 @@
         if clim is None:
             min_value = np.percentile(self.array,[0.1])[0].round(decimals=-0)
             max_value = np.percentile(self.array,[99.9])[0].round(decimals=-0)
             clim = [min_value, max_value]    
         fig = plt.gcf()
             
         if self.array.ndim > 2 and self.array.max() > 255:
-            cax = ax.imshow(self.array / 65535., cmap=cmap, **kwargs) 
+            cax = ax.imshow(self.array / 65535., cmap=cmap, interpolation='nearest', **kwargs) 
         else:
-            cax = ax.imshow(self.array, cmap=cmap, **kwargs)
+            cax = ax.imshow(self.array, cmap=cmap, interpolation='nearest', **kwargs)
         cax.set_clim(clim)
         fig.colorbar(cax, ax=ax)   
         ax.set_title(title)
         ax.axis('image')      
         if show:
             plt.show()
         return cax
```

### Comparing `omg_dosimetry-1.3.0/src/omg_dosimetry/tiff2dose.py` & `omg_dosimetry-1.4.0/src/omg_dosimetry/tiff2dose.py`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/.gitignore` & `omg_dosimetry-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/LICENSE` & `omg_dosimetry-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/README.md` & `omg_dosimetry-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `omg_dosimetry-1.3.0/pyproject.toml` & `omg_dosimetry-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "omg_dosimetry"
-version = "1.3.0"
+version = "1.4.0"
 authors = [
   { name="JF Cabana", email="jean-francois.cabana.cisssca@ssss.gouv.qc.ca" },
 ]
 description = "Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `omg_dosimetry-1.3.0/PKG-INFO` & `omg_dosimetry-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omg_dosimetry
-Version: 1.3.0
+Version: 1.4.0
 Summary: Optimized Multichannel Gafchromic Dosimetry (OMG Dosimetry)
 Project-URL: Homepage, https://bitbucket.org/cric_levis/omg-film-dosimetry
 Author-email: JF Cabana <jean-francois.cabana.cisssca@ssss.gouv.qc.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

