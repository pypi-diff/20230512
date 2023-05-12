# Comparing `tmp/starextractor-0.1.2-py3-none-any.whl.zip` & `tmp/starextractor-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 8711 bytes, number of entries: 9
--rw-r--r--  2.0 unx      564 b- defN 23-Apr-05 03:18 starextractor/__init__.py
--rw-r--r--  2.0 unx     5068 b- defN 23-May-11 09:19 starextractor/classes.py
+Zip file size: 10151 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       31 b- defN 23-May-12 07:36 starextractor/__init__.py
+-rw-r--r--  2.0 unx     5713 b- defN 23-May-12 07:03 starextractor/classes.py
 -rw-r--r--  2.0 unx     3814 b- defN 23-May-11 09:11 starextractor/image.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-May-12 07:26 starextractor/invariantfeatures.py
 -rw-r--r--  2.0 unx     2937 b- defN 23-Apr-05 07:44 starextractor/plot.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4278 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      735 b- defN 23-May-11 15:07 starextractor-0.1.2.dist-info/RECORD
-9 files, 18570 bytes uncompressed, 7443 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4740 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      825 b- defN 23-May-12 07:36 starextractor-0.1.3.dist-info/RECORD
+10 files, 22311 bytes uncompressed, 8739 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: starextractor/classes.py
 Comment: 
 
 Filename: starextractor/image.py
 Comment: 
 
+Filename: starextractor/invariantfeatures.py
+Comment: 
+
 Filename: starextractor/plot.py
 Comment: 
 
-Filename: starextractor-0.1.2.dist-info/LICENSE
+Filename: starextractor-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: starextractor-0.1.2.dist-info/METADATA
+Filename: starextractor-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: starextractor-0.1.2.dist-info/WHEEL
+Filename: starextractor-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: starextractor-0.1.2.dist-info/top_level.txt
+Filename: starextractor-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: starextractor-0.1.2.dist-info/RECORD
+Filename: starextractor-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starextractor/__init__.py

```diff
@@ -1,13 +1 @@
-"""
-slrfield package
-
-This package is an archive of scientific routines for data processing related to SLR(Satellite Laser Ranging).   
-Currently, operations on SLR data include:
-
-1. Download CPF(Consolidated Prediction Format) ephemeris files automatically from **CDDIS**(Crustal Dynamics Data Information System) or **EDC**(EUROLAS Data Center);
-2. Parse the CPF ephemeris files;
-3. Calculate the position of targets in GCRF;
-4. Predict the azimuth, altitude, distance of targets, and the time of flight for laser pulse etc.;
-"""
-
 from .classes import AstroImage
```

## starextractor/classes.py

```diff
@@ -1,11 +1,12 @@
 from photutils.aperture import CircularAperture,aperture_photometry
 
 from .image import read_image,source_extract
 from .plot import show_image
+from .invariantfeatures import _generate_invariants
 
 class AstroImage(object):
     """
     Class AstroImage
     """    
 
     def __init__(self,info):  
@@ -55,42 +56,43 @@
         Parameters:    
         max_control_points -> [int,optional,default=50] Maximum number of sources to extract
         fwhm -> [float,optional,default=15] Priori Full-width half-maximum (FWHM) of the Gaussian kernel in units of pixels used in DAOStarFinder
         mask -> [bool,optional,default=False] A True value indicates the edge area of an image is masked. Masked pixels are ignored when searching for stars.
         Outputs:
         sources -> Instance of class Source with its attributes as follows:
             xy_centroids -> [2d array of float] Pixel coordinates of the star centroids
-            _offset -> [array of float] Pixel coordinates of the center of the image
+            offset -> [array of float] Pixel coordinates of the center of the image
             _image_raw -> [2d array of float] raw grayscale image
             _image -> [2d array of float] signal, i.e. subtracting the background gray value from the raw grayscale image
             _apertures -> A circular aperture defined in pixel coordinates.
             brightness -> [array of float]  Brightness(Grayvalues) of star spots
             snr -> [array of float] Signal Noise Ratio(SNR) of star spots
             mask_rectangle -> [None or tuple] If None, then no mask rectangle is generated; Else, a rectangle defined by the bottom left corner point, width and height is generated
         """
         image_raw = self.image_raw
         # Search for star spots in an image and extract them
-        xy_centroids,_offset,_image,_bkg_rms,_mask_rectangle = source_extract(image_raw,max_control_points,fwhm,mask)
+        xy_centroids,offset,_image,_bkg_rms,_mask_rectangle = source_extract(image_raw,max_control_points,fwhm,mask)
+        xy = xy_centroids - offset # move the origin to the center of image from the center of the bottom left pixel.
 
         # Do photometry
         _apertures = CircularAperture(xy_centroids, r=fwhm)
         phot_table = aperture_photometry(_image, _apertures) 
         noise_table = aperture_photometry(_bkg_rms, _apertures)
 
         brightness = phot_table['aperture_sum'].value
         noise = noise_table['aperture_sum'].value
         snr = brightness/noise # Signal Noise Ratio
 
-        dict_values = xy_centroids,_offset,image_raw,_image,_apertures,brightness,snr,_mask_rectangle
-        dict_keys = 'xy','_offset','image_raw','_image','_apertures','brightness','snr','_mask_rectangle'
+        dict_values = xy,offset,image_raw,_image,_apertures,brightness,snr,_mask_rectangle
+        dict_keys = 'xy','offset','image_raw','_image','_apertures','brightness','snr','_mask_rectangle'
         info = dict(zip(dict_keys, dict_values))
 
         return Source(info)      
 
-    def show_image(self,fig_out=None):
+    def show(self,fig_out=None):
         """
         Show raw image
 
         Parameters:
         fig_out -> [str,optional,default=None] In not None, save the output image to a file defined by fig_out
 
         """
@@ -112,21 +114,34 @@
         for key in info.keys():
             setattr(self, key, info[key])
 
     def __repr__(self):
     
         return 'Instance of class Source'
 
-    def show_image(self,fig_out=None):
+    def show(self,fig_out=None):
         """
         Show raw image with stars marked
 
         Inputs:
             fig_out -> [str,optional,default=None] In not None, save the image to a file defined by fig_out
         """
         if fig_out is None:
             plot_kwargs = {'mark':(self._apertures,'blue')}
         else:
             plot_kwargs = {'mark':(self._apertures,'blue'),'figname':fig_out}
-        show_image(self.image_raw,origin='lower',mask_rectangle=self._mask_rectangle,**plot_kwargs)      
+        show_image(self.image_raw,origin='lower',mask_rectangle=self._mask_rectangle,**plot_kwargs)     
+
+    def invariantfeatures(self):
+        """
+        Calculate the unique invariants (L2/L1,L1/L0), where L2 >= L1 >= L0 are the three sides of the triangle composed of centroids.
+        At the same time, record an array of the indices of centroids that correspond to each invariant.
+        """
+        inv_uniq, triang_vrtx_uniq = _generate_invariants(self.xy)
+
+        info = self.info.copy()
+        info.update({'invariants':inv_uniq,'asterisms':triang_vrtx_uniq})
+
+        return Source(info)
+
```

## Comparing `starextractor-0.1.2.dist-info/LICENSE` & `starextractor-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starextractor-0.1.2.dist-info/METADATA` & `starextractor-0.1.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starextractor
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to extract stars from an astronomical image
 Home-page: https://github.com/lcx366/STAREXTRACTOR
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: source extract,stars
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: photutils
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: pillow
+Requires-Dist: scipy
 
 # Welcome to the STAREXTRACTOR package
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![PyPI status](https://img.shields.io/pypi/status/starextractor.svg)](https://pypi.python.org/pypi/starextractor/) [![GitHub contributors](https://img.shields.io/github/contributors/lcx366/STAREXTRACTOR.svg)](https://GitHub.com/lcx366/STAREXTRACTOR/graphs/contributors/) [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/lcx366/STAREXTRACTOR/graphs/commit-activity) [![GitHub license](https://img.shields.io/github/license/lcx366/STAREXTRACTOR.svg)](https://github.com/lcx366/STAREXTRACTOR/blob/master/LICENSE) [![Documentation Status](https://readthedocs.org/projects/starextractor/badge/?version=latest)](http://starextractor.readthedocs.io/?badge=latest) [![Build Status](https://travis-ci.org/lcx366/starextractor.svg?branch=master)](https://travis-ci.org/lcx366/starextractor)
 
 This package is an archive of scientific routines for data processing related to the source extraction from an astronomical image.
 Currently, operations on source extraction include:
@@ -59,49 +60,58 @@
 ```python
 >>> print(image.image_raw,image.res) # original grayscale image and its resolution
 ```
 
 ### Show the raw image
 
 ```python
->>> image.show_image()
->>> #image.show_image('figs/raw_image.png') # save image to a file
+>>> image.show()
+>>> #image.show('figs/raw_image.png') # save image to a file
 ```
 
 <p align="middle">
   <img src="readme_figs/image_raw.png" width="500" />
 </p>
 
 ### Extract the centroid coordinates of the star spots and do photometry
 
 Estimate the centroids coordinates, brightness(sum of gray value within an aperture),  and SNR of star spots.
 
 ```python
->>> sources = image.find_source(fwhm=12,max_control_points=50,mask=True)
->>> print(sources.xy,sources.brightness,sources.snr)
+>>> sources = image.find_source(fwhm=12,mask=True)
+>>> print(sources.xy,sources.brightness,sources.snr,sources.offset)
 ```
 
-### Show the raw image
+### Calculate the triangle invariants and the asterism indices of the star spots.
+
+```python
+>>> sources = sources.invariantfeatures()
+>>> print(sources.invariants,sources.asterisms)
+```
+
+### Show the extracted sources in image
 
 ```python
->>> sources.show_image()
->>> #sources.show_image('figs/sources.png') # save image to a file
+>>> sources.show()
+>>> #sources.show('figs/sources.png') # save image to a file
 ```
 
 <p align="middle">
   <img src="readme_figs/centroids.png" width="500" />
 </p>
 
 ## Change log
 
-- **0.1.2 — May 11,  2023**
+- **0.1.3 — May 12,  2023**
   
   - The class `Centriod` is *deprecated*, and the class `Source` is used instead
+  - Add method `.invariantfeatures()` to class `Source`, which calculates the triangle invariants and the asterism indices of the star spots
 
 - **0.1.0 — Apr 5,  2023**
   
   - The ***starextractor*** package was released.
 
 ## Reference
 
 - [photutils](https://photutils.readthedocs.io/en/stable/index.html)
 - [Photometry Methods](http://srmastro.uvacreate.virginia.edu/astr313/lectures/photometry/photometry_methods.html)
+- [Astroalign]([Astroalign documentation &mdash; astroalign 2.4.2 documentation](https://astroalign.quatrope.org/en/latest/))
```

