# Comparing `tmp/specex-0.6.1.tar.gz` & `tmp/specex-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specex-0.6.1.tar", last modified: Wed Apr 12 15:11:06 2023, max compression
+gzip compressed data, was "specex-0.6.3.tar", last modified: Fri May 12 08:36:58 2023, max compression
```

## Comparing `specex-0.6.1.tar` & `specex-0.6.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2022-04-01 11:26:21.000000 specex-0.6.1/LICENSE
--rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-04-12 15:11:06.738803 specex-0.6.1/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1513 2023-04-07 11:12:08.000000 specex-0.6.1/README.md
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1635 2023-04-12 13:06:36.000000 specex-0.6.1/pyproject.toml
--rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2023-04-12 15:11:06.738803 specex-0.6.1/setup.cfg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.735470 specex-0.6.1/src/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/src/specex/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1918 2023-03-06 07:50:03.000000 specex-0.6.1/src/specex/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    53746 2023-04-12 13:12:36.000000 specex-0.6.1/src/specex/cube.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     5175 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/lines.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    13737 2023-04-12 13:18:00.000000 specex-0.6.1/src/specex/plot.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    20267 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/rrspecex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    24593 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/sources.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    42648 2023-03-06 07:49:53.000000 specex-0.6.1/src/specex/specex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     8345 2023-02-14 07:35:23.000000 specex-0.6.1/src/specex/stack.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    38211 2023-04-12 15:03:32.000000 specex-0.6.1/src/specex/utils.py
--rwxr-xr-x   0 daddona   (1000) daddona   (1000)     4550 2022-12-15 19:17:38.000000 specex-0.6.1/src/specex/zeropoints.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/src/specex.egg-info/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)      607 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/SOURCES.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/dependency_links.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)      287 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/entry_points.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)       46 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/requires.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        7 2023-04-12 15:11:06.000000 specex-0.6.1/src/specex.egg-info/top_level.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-04-12 15:11:06.738803 specex-0.6.1/test/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_cubestack.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1970 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_cutout.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1524 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_rrspecex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      583 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_sources.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1133 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_specex.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      706 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_specexplot.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      756 2022-12-15 19:17:38.000000 specex-0.6.1/test/test_zeropointinfo.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-05-12 08:36:58.822550 specex-0.6.3/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2022-04-01 11:26:21.000000 specex-0.6.3/LICENSE
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-05-12 08:36:58.822550 specex-0.6.3/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1513 2023-04-14 08:15:29.000000 specex-0.6.3/README.md
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1635 2023-05-12 08:34:50.000000 specex-0.6.3/pyproject.toml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2023-05-12 08:36:58.822550 specex-0.6.3/setup.cfg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-05-12 08:36:58.822550 specex-0.6.3/src/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-05-12 08:36:58.822550 specex-0.6.3/src/specex/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1918 2023-03-06 07:50:03.000000 specex-0.6.3/src/specex/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    53746 2023-04-14 08:15:29.000000 specex-0.6.3/src/specex/cube.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    13039 2023-05-11 09:18:42.000000 specex-0.6.3/src/specex/lines.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    14057 2023-04-14 08:15:29.000000 specex-0.6.3/src/specex/plot.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    20267 2023-05-11 11:31:28.000000 specex-0.6.3/src/specex/rrspecex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    24593 2022-12-15 19:17:38.000000 specex-0.6.3/src/specex/sources.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    42767 2023-04-14 08:15:29.000000 specex-0.6.3/src/specex/specex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8345 2023-02-14 07:35:23.000000 specex-0.6.3/src/specex/stack.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    42121 2023-04-14 08:16:31.000000 specex-0.6.3/src/specex/utils.py
+-rwxr-xr-x   0 daddona   (1000) daddona   (1000)     4550 2022-12-15 19:17:38.000000 specex-0.6.3/src/specex/zeropoints.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-05-12 08:36:58.822550 specex-0.6.3/src/specex.egg-info/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4025 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      607 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/SOURCES.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/dependency_links.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      287 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/entry_points.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       46 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/requires.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        7 2023-05-12 08:36:58.000000 specex-0.6.3/src/specex.egg-info/top_level.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2023-05-12 08:36:58.822550 specex-0.6.3/test/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_cubestack.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1970 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_cutout.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1524 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_rrspecex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      583 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_sources.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1133 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_specex.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      706 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_specexplot.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      756 2022-12-15 19:17:38.000000 specex-0.6.3/test/test_zeropointinfo.py
```

### Comparing `specex-0.6.1/LICENSE` & `specex-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/PKG-INFO` & `specex-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specex
-Version: 0.6.1
+Version: 0.6.3
 Summary: Extract spectra from fits cubes
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
```

### Comparing `specex-0.6.1/README.md` & `specex-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/pyproject.toml` & `specex-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "specex"
-version = "0.6.1"
+version = "0.6.3"
 description = "Extract spectra from fits cubes"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["spectroscopy", "spectra", "spectrum", "spectral cubes"]
 authors = [
  {name = "Maurizio D'Addona"},
```

### Comparing `specex-0.6.1/src/specex/__init__.py` & `specex-0.6.3/src/specex/__init__.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex/cube.py` & `specex-0.6.3/src/specex/cube.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex/plot.py` & `specex-0.6.3/src/specex/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,16 @@
 
     if args.cutout is not None:
         try:
             big_image = load_rgb_fits(args.cutout)
         except FileNotFoundError:
             print(f"ERROR: file not found '{args.cutout}'")
             sys.exit(1)
-        except IndexError:
+
+        if big_image is None:
             big_image = {
                 'data': fits.getdata(args.cutout),
                 'wcs': wcs.WCS(fits.getheader(args.cutout)),
                 'type': 'gray'
             }
 
         cutout_size = apu.Quantity(args.cutout_size)
@@ -238,23 +239,31 @@
                 ]
             except KeyError:
                 print(
                     f"Skipping file with invalid header: {spectrum_fits_file}"
                 )
                 continue
             else:
+
+                try:
+                    object_coord_frame = main_header['FRAME']
+                except KeyError:
+                    object_coord_frame = 'fk5'
+
                 obj_center = SkyCoord(
                     object_ra, object_dec,
-                    unit='deg'
+                    unit='deg',
+                    frame=object_coord_frame
                 )
 
             info_dict = {
                 'ID': f"{object_id}",
                 'RA': obj_center.ra.to_string(precision=2),
                 'DEC': obj_center.dec.to_string(precision=2),
+                'FRAME': str(object_coord_frame).upper()
             }
             for key in ['Z', 'SN', 'SN_EMISS']:
                 try:
                     info_dict[key] = f"{main_header[key]:.4f}"
                 except KeyError:
                     continue
 
@@ -363,14 +372,15 @@
                 smoothing=args.smoothing,
                 extra_info=info_dict,
                 extraction_info={
                     'mode': extraction_mode,
                     'apertures': specex_apertures,
                     'aperture_ra': object_ra,
                     'aperture_dec': object_dec,
+                    'frame': object_coord_frame
                 },
                 wave_range=wave_range
             )
 
             if args.outdir is None:
                 outdir = os.path.dirname(spectrum_fits_file)
             else:
```

### Comparing `specex-0.6.1/src/specex/rrspecex.py` & `specex-0.6.3/src/specex/rrspecex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex/sources.py` & `specex-0.6.3/src/specex/sources.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex/specex.py` & `specex-0.6.3/src/specex/specex.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,16 @@
         exit_on_errors=False
     )
 
     # Get spectral and celstial WCS from the cube
     cube_wcs = wcs.WCS(spec_hdu.header)
     celestial_wcs = cube_wcs.celestial
     spectral_wcs = cube_wcs.spectral
-    wcs_frame = wcs.utils.wcs_to_celestial_frame(cube_wcs)
+    # wcs_frame = wcs.utils.wcs_to_celestial_frame(cube_wcs)
+    coord_frame = 'fk5'  # frame of source coordinates
 
     # TODO: we assume here that the distorsion across the sky plane is
     #       negligible, but it is very bold to assume this is always the case.
     #       A more general approach that takes into account also distortion
     #       in function of the position on the sky is needed.
     # Get the pixelscales in arcsec/pixel.
     cube_pixelscale_x, cube_pixelscale_y = [
@@ -785,15 +786,15 @@
             )
         dec_unit = 'deg'
 
     # Get the objects positions in the cube (in pixels)
     obj_sky_coords = SkyCoord(
         sources[args.key_ra], sources[args.key_dec],
         unit=(ra_unit, dec_unit),
-        frame=wcs_frame
+        frame=coord_frame
     )
 
     obj_x, obj_y = wcs.utils.skycoord_to_pixel(
         coords=obj_sky_coords,
         wcs=celestial_wcs
     )
 
@@ -1054,14 +1055,15 @@
             x.to_string() for x in specex_apertures[obj_id]
         ]
 
         main_header = {
             'CUBE': (basename_with_ext, "Spectral cube used for extraction"),
             'RA': (obj_ra, "Ra of the center of the object"),
             'DEC': (obj_dec, "Dec of the center of the object"),
+            'FRAME': (coord_frame, "Ra and Dec sky frame"),
             'NPIX': (np.sum(mask), 'Number of pixels used for this spectra'),
             'HISTORY': f'Extracted on {str(my_time)}',
             'ID': obj_id,
             'SN': (sn_spec, "SNR of the total spectrum"),
             'SN_EMISS': (sn_em, "SNR due to emission lines only"),
             'EXT_MODE': (mode, "Spex extraction mode"),
             'EXT_APER': (
```

### Comparing `specex-0.6.1/src/specex/stack.py` & `specex-0.6.3/src/specex/stack.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex/utils.py` & `specex-0.6.3/src/specex/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,177 @@
 from urllib import request
 
 import numpy as np
 
 import matplotlib.pyplot as plt
 from matplotlib.gridspec import GridSpec
 from matplotlib import patches
+import matplotlib.patheffects as PathEffects
 
 from scipy.signal import savgol_filter
 from scipy.ndimage import rotate
-
 from astropy.io import fits
 from astropy.visualization import ZScaleInterval
 from astropy import wcs as apwcs
 from astropy import units as apu
 from astropy import coordinates
 
 from .lines import get_lines
 
 
 _SDSS_SPECTRAL_TEMPLATES_PACKAGE = "http://classic.sdss.org/dr5/algorithms/spectemplates/spectemplatesDR2.tar.gz"
 
 
+class ScaleBar:
+    """A simple scalebar."""
+
+    def __init__(self, ax, x0=0.025, y0=0.025, length=1, size=0.025,
+                 orientation='hor', n_subunits=2, text=None, fontsize=8,
+                 units='arcsec', scale_factor=1):
+
+        self.ax = ax
+        self.units = units
+        self.start_pos = (x0, y0)
+        self.scale_factor = scale_factor
+        self.size = size
+
+        if orientation.lower().startswith('h'):
+            self.end_pos = (x0 + length, y0)
+        else:
+            self.end_pos = (x0, y0 + length)
+
+        self.orientation = orientation
+        self.n_subunits = n_subunits
+        self.length = length
+        self.scale_bar_elements = []
+
+        if text is None:
+            text = f"{length:.1f}"
+
+        length, _ = (
+            ax.transData + ax.transAxes.inverted()
+        ).transform([length, 0])
+
+        self.text_handler = ax.text(
+            x0 + length / 2,
+            y0 + 2 * size,
+            text,
+            horizontalalignment='center',
+            verticalalignment='bottom',
+            transform=ax.transAxes,
+            fontsize=fontsize
+        )
+
+        self.text_handler.set_path_effects(
+            (
+                PathEffects.withStroke(
+                    linewidth=3, foreground='white'
+                ),
+            )
+        )
+
+        delta = length / n_subunits
+
+        for i in range(n_subunits):
+            if orientation.lower().startswith('h'):
+                x = x0 + i*delta
+                y = y0
+                wid = delta
+                hei = size
+            else:
+                x = x0
+                y = y0 + i*delta
+                wid = size
+                hei = delta
+
+            if i % 2:
+                facecolor = 'white'
+                edgecolor = 'black'
+            else:
+                facecolor = 'black'
+                edgecolor = 'white'
+
+            scale_bar_element = patches.Rectangle(
+                (x, y),
+                wid,
+                hei,
+                transform=ax.transAxes,
+                facecolor=facecolor,
+                edgecolor=edgecolor,
+                lw=1,
+                ls='-',
+            )
+
+            ax.add_artist(scale_bar_element)
+            self.scale_bar_elements.append(scale_bar_element)
+
+    def update(self):
+        """
+        Update the ScaleBar.
+
+        Returns
+        -------
+        None.
+
+        """
+        length, _ = (
+            self.ax.transData + self.ax.transAxes.inverted()
+        ).transform([self.length, 0])
+
+        delta = length / self.n_subunits
+
+        self.text_handler.set_x(self.start_pos[0] + length / 2)
+        self.text_handler.set_y(self.start_pos[1] + 2 * self.size)
+
+        for i, rect in enumerate(self.scale_bar_elements):
+            if self.orientation.lower().startswith('h'):
+                x = self.start_pos[0] + i*delta
+                y = self.start_pos[1]
+                wid = delta
+                hei = self.size
+            else:
+                x = self.start_pos[0]
+                y = self.start_pos[1] + i*delta
+                wid = self.size
+                hei = delta
+
+            rect.set_x(x)
+            rect.set_y(y)
+            rect.set_width(wid)
+            rect.set_height(hei)
+
+    def set_wcs(self, wcs):
+        """
+        Set the WCS.
+
+        Parameters
+        ----------
+        wcs : astropy.wcs.WCS
+            The WCS to use.
+
+        Returns
+        -------
+        None.
+
+        """
+        star_coords = wcs.pixel_to_world(
+            *self.start_pos
+        )
+
+        end_coords = wcs.pixel_to_world(
+            *self.end_pos
+        )
+
+        sep = star_coords.separation(end_coords).to(self.units)
+        sep /= self.scale_factor
+
+        self.text_handler.set_text(f"{sep:.2f}")
+        self.update()
+
+
 def get_pbar(partial, total=None, wid=32, common_char='\u2588',
              upper_char='\u2584', lower_char='\u2580'):
     """
     Return a nice text/unicode progress bar showing partial and total progress.
 
     Parameters
     ----------
@@ -377,15 +524,15 @@
     return fig, ax
 
 
 def get_ellipse_skypoints(center: coordinates.SkyCoord,
                           a: apu.quantity.Quantity,
                           b: apu.quantity.Quantity,
                           angle: apu.quantity.Quantity = 0*apu.deg,
-                          n_points: int = 25) -> list:
+                          n_points: int = 20) -> list:
     """
     Get points of an ellips on the skyplane.
 
     Parameters
     ----------
     center : astropy.coordinates.SkyCoord
         DESCRIPTION.
@@ -626,20 +773,14 @@
     ax0.set_xlim(w_min, w_max)
 
     # Plot a cutout
     if cutout is not None:
         ax1 = fig.add_subplot(gs[:3, -1], projection=cutout_wcs)
         ax2 = fig.add_subplot(gs[3:, -1])
 
-        if cutout_wcs is not None:
-            ra_cunit, dec_cunit = cutout_wcs.celestial.wcs.cunit
-        else:
-            ra_cunit = apu.deg
-            dec_cunit = apu.deg
-
         ax1.axis('off')
         ax1.imshow(
             cutout,
             origin='lower',
             aspect='equal',
             vmin=cutout_vmin,
             vmax=cutout_vmax,
@@ -649,25 +790,26 @@
 
         # Check if there are info about the specex extraction
         try:
             ext_mode = extraction_info['mode']
             ext_apertures = extraction_info['apertures']
             e_ra = extraction_info['aperture_ra']
             e_dec = extraction_info['aperture_dec']
+            e_frame = extraction_info['frame']
         except (TypeError, KeyError):
             # No extraction info present, just ignore
             pass
         else:
             # If there are extraction info, read the information
             e_wid, e_hei, e_ang = ext_apertures
 
             e_cc = coordinates.SkyCoord(
                 e_ra, e_dec,
-                unit=(ra_cunit, dec_cunit),
-                frame=apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
+                unit=('deg', 'deg'),
+                frame=e_frame
             )
 
             # and then draw extraction apertures
             if ext_mode.lower() in [
                     'kron_ellipse', 'kron_circular', 'circular_aperture'
             ]:
                 e_world_points = get_ellipse_skypoints(
@@ -681,35 +823,38 @@
                     [x.ra.value, x.dec.value]
                     for x in e_world_points
                 ])
 
                 ax1.plot(
                     e_world_points_values[..., 0],
                     e_world_points_values[..., 1],
-                    color='#0000ff',
+                    color='black',
                     ls='-',
-                    lw=0.8,
+                    lw=1,
                     alpha=0.7,
                     zorder=1,
-                    transform=ax1.get_transform(
-                        apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
-                    )
+                    transform=ax1.get_transform(e_frame)
                 )
                 ax1.plot(
                     e_world_points_values[..., 0],
                     e_world_points_values[..., 1],
-                    color='#00ff00',
+                    color='cyan',
                     ls='--',
-                    lw=0.8,
+                    lw=1,
                     alpha=0.7,
                     zorder=2,
-                    transform=ax1.get_transform(
-                        apwcs.utils.wcs_to_celestial_frame(cutout_wcs)
-                    )
+                    transform=ax1.get_transform(e_frame)
+                )
+
+                scbar = ScaleBar(
+                    ax1,
+                    length=cutout.shape[1]/2
                 )
+                scbar.set_wcs(cutout_wcs)
+                scbar.update()
     else:
         ax1 = None
         ax2 = fig.add_subplot(gs[:, -1])
 
     ax0.set_aspect('auto')
 
     # Plot only original spectrum or also a smoothed version
@@ -1057,22 +1202,28 @@
     """
     x = np.ma.array(x, mask=np.isnan(x))
     x_bar = np.ma.median(x, axis=axis)
     mad = np.ma.median(np.ma.abs(x - x_bar), axis=axis)
     return scale*mad
 
 
-def get_spectrum_snr(flux, var=None, smoothing_window=51, smoothing_order=11):
+def get_spectrum_snr(flux: np.ndarray,
+                     var: Optional[np.ndarray] = None,
+                     smoothing_window: Optional[int] = 51,
+                     smoothing_order: Optional[int] = 11):
     """
     Compute the SRN of a spectrum.
 
     Parameters
     ----------
     flux : numpy.ndarray
         The spectrum itself.
+    var : numpy.ndarray, optional
+        The variance of the spectrum itself.
+        The default value is None.
     smoothing_window : int, optional
         Parameter to be passed to the smoothing function.
         The default is 51.
     smoothing_order : int, optional
         Parameter to be passed to the smoothing function.
         The default is 11.
```

### Comparing `specex-0.6.1/src/specex/zeropoints.py` & `specex-0.6.3/src/specex/zeropoints.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/src/specex.egg-info/PKG-INFO` & `specex-0.6.3/src/specex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specex
-Version: 0.6.1
+Version: 0.6.3
 Summary: Extract spectra from fits cubes
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
```

### Comparing `specex-0.6.1/src/specex.egg-info/SOURCES.txt` & `specex-0.6.3/src/specex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_cubestack.py` & `specex-0.6.3/test/test_cubestack.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_cutout.py` & `specex-0.6.3/test/test_cutout.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_rrspecex.py` & `specex-0.6.3/test/test_rrspecex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_sources.py` & `specex-0.6.3/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_specex.py` & `specex-0.6.3/test/test_specex.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_specexplot.py` & `specex-0.6.3/test/test_specexplot.py`

 * *Files identical despite different names*

### Comparing `specex-0.6.1/test/test_zeropointinfo.py` & `specex-0.6.3/test/test_zeropointinfo.py`

 * *Files identical despite different names*

