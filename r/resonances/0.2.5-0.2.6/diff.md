# Comparing `tmp/resonances-0.2.5.tar.gz` & `tmp/resonances-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resonances-0.2.5.tar", max compression
+gzip compressed data, was "resonances-0.2.6.tar", max compression
```

## Comparing `resonances-0.2.5.tar` & `resonances-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1071 2023-01-21 08:32:40.950152 resonances-0.2.5/LICENSE
--rw-r--r--   0        0        0     4670 2023-01-21 09:43:39.996420 resonances-0.2.5/README.md
--rw-r--r--   0        0        0     2059 2023-03-10 15:42:06.867347 resonances-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      417 2023-03-10 09:50:28.272800 resonances-0.2.5/resonances/__init__.py
--rw-r--r--   0        0        0      115 2023-01-21 08:32:40.952434 resonances-0.2.5/resonances/__main__.py
--rw-r--r--   0        0        0     1725 2023-01-21 08:32:40.952516 resonances-0.2.5/resonances/body.py
--rw-r--r--   0        0        0     1447 2023-01-21 08:32:40.952591 resonances-0.2.5/resonances/config.json
--rw-r--r--   0        0        0     1320 2023-02-18 10:50:00.878029 resonances-0.2.5/resonances/config.py
--rw-r--r--   0        0        0        0 2023-01-21 08:32:40.952748 resonances-0.2.5/resonances/data/__init__.py
--rw-r--r--   0        0        0     2805 2023-03-10 15:42:06.867683 resonances-0.2.5/resonances/data/astdys.py
--rw-r--r--   0        0        0     1120 2023-01-21 08:32:40.952931 resonances-0.2.5/resonances/data/const.py
--rw-r--r--   0        0        0      192 2023-01-21 08:32:40.953006 resonances-0.2.5/resonances/data/util.py
--rw-r--r--   0        0        0     4402 2023-01-21 08:32:40.953136 resonances-0.2.5/resonances/experiment/console.py
--rw-r--r--   0        0        0     1313 2023-03-10 15:42:06.867976 resonances-0.2.5/resonances/experiment/finder.py
--rw-r--r--   0        0        0     1209 2023-01-21 08:32:40.953297 resonances-0.2.5/resonances/experiment/loader.py
--rw-r--r--   0        0        0     1904 2023-01-21 08:32:40.953382 resonances-0.2.5/resonances/experiment/shape.py
--rw-r--r--   0        0        0     1377 2023-02-18 11:14:33.313263 resonances-0.2.5/resonances/logger.py
--rw-r--r--   0        0        0      616 2023-01-21 08:32:40.953582 resonances-0.2.5/resonances/matrix/matrix.py
--rw-r--r--   0        0        0     2350 2023-03-10 15:42:06.868386 resonances-0.2.5/resonances/matrix/three_body_matrix.py
--rw-r--r--   0        0        0     1912 2023-01-21 08:32:40.953752 resonances-0.2.5/resonances/matrix/two_body_matrix.py
--rw-r--r--   0        0        0        0 2023-01-21 08:32:40.953829 resonances-0.2.5/resonances/resonance/__init__.py
--rw-r--r--   0        0        0     1213 2023-01-21 08:32:40.953932 resonances-0.2.5/resonances/resonance/factory.py
--rw-r--r--   0        0        0    11846 2023-01-21 08:32:40.954070 resonances-0.2.5/resonances/resonance/libration.py
--rw-r--r--   0        0        0     1766 2023-01-21 08:32:40.954199 resonances-0.2.5/resonances/resonance/mmr.py
--rw-r--r--   0        0        0     3533 2023-03-10 15:42:06.868737 resonances-0.2.5/resonances/resonance/plot.py
--rw-r--r--   0        0        0     6164 2023-01-21 15:03:51.787348 resonances-0.2.5/resonances/resonance/three_body.py
--rw-r--r--   0        0        0     2236 2023-01-21 08:32:40.954444 resonances-0.2.5/resonances/resonance/two_body.py
--rw-r--r--   0        0        0    11110 2023-03-10 15:42:06.869044 resonances-0.2.5/resonances/simulation.py
--rw-r--r--   0        0        0     6644 1970-01-01 00:00:00.000000 resonances-0.2.5/setup.py
--rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 resonances-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-01-21 08:32:40.950152 resonances-0.2.6/LICENSE
+-rw-r--r--   0        0        0     6451 2023-05-12 15:05:24.085106 resonances-0.2.6/README.md
+-rw-r--r--   0        0        0     2059 2023-05-12 15:05:24.086018 resonances-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-03-10 09:50:28.272800 resonances-0.2.6/resonances/__init__.py
+-rw-r--r--   0        0        0      115 2023-01-21 08:32:40.952434 resonances-0.2.6/resonances/__main__.py
+-rw-r--r--   0        0        0     1725 2023-01-21 08:32:40.952516 resonances-0.2.6/resonances/body.py
+-rw-r--r--   0        0        0     1447 2023-01-21 08:32:40.952591 resonances-0.2.6/resonances/config.json
+-rw-r--r--   0        0        0     1320 2023-02-18 10:50:00.878029 resonances-0.2.6/resonances/config.py
+-rw-r--r--   0        0        0        0 2023-01-21 08:32:40.952748 resonances-0.2.6/resonances/data/__init__.py
+-rw-r--r--   0        0        0     3435 2023-05-12 15:05:24.086311 resonances-0.2.6/resonances/data/astdys.py
+-rw-r--r--   0        0        0     1120 2023-01-21 08:32:40.952931 resonances-0.2.6/resonances/data/const.py
+-rw-r--r--   0        0        0      192 2023-01-21 08:32:40.953006 resonances-0.2.6/resonances/data/util.py
+-rw-r--r--   0        0        0     4402 2023-01-21 08:32:40.953136 resonances-0.2.6/resonances/experiment/console.py
+-rw-r--r--   0        0        0     1313 2023-03-10 15:42:06.867976 resonances-0.2.6/resonances/experiment/finder.py
+-rw-r--r--   0        0        0     1209 2023-01-21 08:32:40.953297 resonances-0.2.6/resonances/experiment/loader.py
+-rw-r--r--   0        0        0     1904 2023-01-21 08:32:40.953382 resonances-0.2.6/resonances/experiment/shape.py
+-rw-r--r--   0        0        0     1377 2023-02-18 11:14:33.313263 resonances-0.2.6/resonances/logger.py
+-rw-r--r--   0        0        0      745 2023-05-12 15:05:24.086551 resonances-0.2.6/resonances/matrix/matrix.py
+-rw-r--r--   0        0        0     2350 2023-03-10 15:42:06.868386 resonances-0.2.6/resonances/matrix/three_body_matrix.py
+-rw-r--r--   0        0        0     1911 2023-05-12 15:05:24.086782 resonances-0.2.6/resonances/matrix/two_body_matrix.py
+-rw-r--r--   0        0        0        0 2023-01-21 08:32:40.953829 resonances-0.2.6/resonances/resonance/__init__.py
+-rw-r--r--   0        0        0     1213 2023-01-21 08:32:40.953932 resonances-0.2.6/resonances/resonance/factory.py
+-rw-r--r--   0        0        0    11846 2023-01-21 08:32:40.954070 resonances-0.2.6/resonances/resonance/libration.py
+-rw-r--r--   0        0        0     1925 2023-05-12 15:05:24.086983 resonances-0.2.6/resonances/resonance/mmr.py
+-rw-r--r--   0        0        0     3533 2023-03-10 15:42:06.868737 resonances-0.2.6/resonances/resonance/plot.py
+-rw-r--r--   0        0        0     6300 2023-05-12 15:05:24.087224 resonances-0.2.6/resonances/resonance/three_body.py
+-rw-r--r--   0        0        0     2303 2023-05-12 15:05:24.087456 resonances-0.2.6/resonances/resonance/two_body.py
+-rw-r--r--   0        0        0    11551 2023-05-12 15:05:24.087675 resonances-0.2.6/resonances/simulation.py
+-rw-r--r--   0        0        0      263 2023-05-12 15:05:24.087848 resonances-0.2.6/resonances/util.py
+-rw-r--r--   0        0        0     8449 1970-01-01 00:00:00.000000 resonances-0.2.6/setup.py
+-rw-r--r--   0        0        0     7731 1970-01-01 00:00:00.000000 resonances-0.2.6/PKG-INFO
```

### Comparing `resonances-0.2.5/LICENSE` & `resonances-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/README.md` & `resonances-0.2.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,18 +27,19 @@
 
 ## Mean-motion resonances
 
 For those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:
 
 ### Papers about the automatic identification of resonant asteroids
 
-1. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).
-1. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
 1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).
-1. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).
+2. Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+3. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).
+4. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+5. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).
 
 ### Papers about mean-motion resonances
 
 1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).
 1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).
 1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).
 1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).
@@ -52,27 +53,50 @@
 1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).
 1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).
 
 ## References
 
 Whenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):
 
-1. **The package itself**: to be published
-1. **The Libration module and automatic identification of librations**: to be published
-1. **Mass identification of mean-motion resonances:** Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+1. **The package itself**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing. https://doi.org/10.1016/j.ascom.2023.100707
+
+```tex
+@article{Smirnov2023,
+  title    = {A new python package for identifying celestial bodies trapped in mean-motion resonances},
+  journal  = {Astronomy and Computing},
+  year     = {2023},
+  issn     = {2213-1337},
+  doi      = {https://doi.org/10.1016/j.ascom.2023.100707},
+  url      = {https://www.sciencedirect.com/science/article/pii/S2213133723000227},
+  author   = {E.A. Smirnov},
+  keywords = {Mean-motion resonances, Python, Identification, Asteroids},
+  abstract = {In this paper, a new open-source package ‘resonances’ written in python is introduced. It allows to find, analyse, and plot two-body and three-body mean-motion eccentricity-type resonances in the Solar and other planetary systems. The package has a better accuracy of the automatic identification procedure for resonant objects compared to previous studies. Furthermore, it has built-in integrations with AstDyS and NASA JPL catalogues. The code is extensively documented and tested with automatic tests. The package is available on GitHub under MIT Licence.}
+}
+```
+
+2. **The Libration module and automatic identification of librations**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+
+3. **Mass identification of mean-motion resonances:** 
+
+* Smirnov, E. A., & Dovgalev, I. S. (2018). Identification of Asteroids in Two-Body Resonances. Solar System Research, 52(4), 347–354. https://doi.org/10.1134/S0038094618040056 
+* Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
 
 ## Authors
 
 The authors of the package:
 
 - [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))
 
 ## Acknowledgement
 
-- Many thanks to the co-authors of the papers (prof. I. I. Shevchenko, I. Dovgalev Dr. E. Popova).
+- Many thanks to the co-authors of the papers (prof. I. I. Shevchenko, I. Dovgalev, and Dr. E. Popova).
 - The creators of [REBOUND integrator](https://rebound.readthedocs.io).
 - The creators of [Astropy](http://astropy.org).
 - The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.
 
 ## Contributing
 
 Feel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).
```

### Comparing `resonances-0.2.5/pyproject.toml` & `resonances-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resonances"
-version = "0.2.5"
+version = "0.2.6"
 description = "Identification of mean-motion resonances"
 authors = ["Evgeny Smirnov <smirik@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://smirik.github.io/resonances/"
 repository = "https://github.com/smirik/resonances"
 documentation = "http://smirik.github.io/resonances/"
```

### Comparing `resonances-0.2.5/resonances/body.py` & `resonances-0.2.6/resonances/body.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/config.json` & `resonances-0.2.6/resonances/config.json`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/config.py` & `resonances-0.2.6/resonances/config.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/data/astdys.py` & `resonances-0.2.6/resonances/data/astdys.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,95 @@
 import pandas as pd
 import numpy as np
 from pathlib import Path
+import os
 import urllib.request
 
 import resonances.config
 import resonances.logger
+from resonances.util import convert_mjd_to_date
 
 
 class astdys:
-
     catalog = None
 
     @classmethod
     def search(cls, num):
         num = str(num)
         if cls.catalog is None:
             cls.load()
 
         if num in cls.catalog['num'].values:
             return cls.catalog.loc[cls.catalog['num'] == num].to_dict('records')[0]
 
         return None
 
     @classmethod
+    def catalog_time(cls):
+        if cls.catalog is None:
+            cls.load()
+
+        elems = cls.search(1)
+        return convert_mjd_to_date(elems['epoch'])
+
+    @classmethod
     def search_possible_resonant_asteroids(cls, mmr, sigma=0.02):
         if cls.catalog is None:
             cls.load()
         axis = mmr.resonant_axis
         df = cls.catalog[(cls.catalog['a'] >= axis - sigma) & (cls.catalog['a'] <= axis + sigma)]
         return df
 
     @classmethod
+    def astdys_full_filename(cls) -> str:
+        filename = f"{os.getcwd()}/{resonances.config.get('astdys.catalog')}"
+        return filename
+
+    @classmethod
+    def catalog_full_filename(cls) -> str:
+        filename = f"{os.getcwd()}/{resonances.config.get('catalog')}"
+        return filename
+
+    @classmethod
     def load(cls):
+        filename = cls.catalog_full_filename()
         if cls.catalog is None:
-            output_file = Path(resonances.config.get('catalog'))
+            output_file = Path(filename)
             if not output_file.exists():
                 cls.build()
 
-        cls.catalog = pd.read_csv(resonances.config.get('catalog'))
+        cls.catalog = pd.read_csv(filename)
         cls.catalog['num'] = cls.catalog['num'].astype(str)
 
     @classmethod
     def rebuild(cls):
-        input_file = Path(resonances.config.get('astdys.catalog'))
+        input_file = Path(cls.astdys_full_filename())
         if input_file.exists():
             input_file.unlink()
         cls.build()
 
     @classmethod
     def build(cls):
-        input_file = Path(resonances.config.get('astdys.catalog'))
+        input_file = Path(cls.astdys_full_filename())
         if not input_file.exists():
             resonances.logger.info('Cannot find AstDyS catalog. Trying to download it...')
             try:
                 urllib.request.urlretrieve(resonances.config.get('astdys.catalog.url'), 'cache/allnum.cat')
             except Exception:
                 raise Exception(
                     "No input catalog available. Cannot download it too. Put AstDys allnum.cat or allnum.csv in the cache directory!"
                 )
             resonances.logger.info('Successfully downloaded. Continue working...')
 
         cat = cls.transform_astdys_catalog()
-        cat.to_csv(resonances.config.get('catalog'), index=False)
+        cat.to_csv(cls.catalog_full_filename(), index=False)
 
     @classmethod
     def transform_astdys_catalog(cls):
-        catalog = pd.read_csv(resonances.config.get('astdys.catalog'), delim_whitespace=True, skiprows=5)
+        catalog = pd.read_csv(cls.astdys_full_filename(), delim_whitespace=True, skiprows=5)
         cat = catalog.rename(
             columns={
                 '!': 'num',
                 'Name,': 'epoch',
                 'Epoch(MJD),': 'a',
                 'a,': 'e',
                 'e,': 'inc',
@@ -79,9 +99,11 @@
             }
         )
         cat['num'] = cat['num'].str.replace("'", "")
         deg_cols = ['inc', 'Omega', 'omega', 'M']
         for col in deg_cols:
             cat[col] = cat[col].map(lambda x: float(x) * np.pi / 180)
 
-        cat.drop(cat.columns[[1, 8, 9, 10, 11]], axis=1, inplace=True)
+        column_to_move = 'epoch'
+        cat = cat[[col for col in cat.columns if col != column_to_move] + [column_to_move]]
+        cat.drop(cat.columns[[8, 9, 10]], axis=1, inplace=True)
         return cat
```

### Comparing `resonances-0.2.5/resonances/data/const.py` & `resonances-0.2.6/resonances/data/const.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/experiment/console.py` & `resonances-0.2.6/resonances/experiment/console.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/experiment/finder.py` & `resonances-0.2.6/resonances/experiment/finder.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/experiment/loader.py` & `resonances-0.2.6/resonances/experiment/loader.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/experiment/shape.py` & `resonances-0.2.6/resonances/experiment/shape.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/logger.py` & `resonances-0.2.6/resonances/logger.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/matrix/three_body_matrix.py` & `resonances-0.2.6/resonances/matrix/three_body_matrix.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/matrix/two_body_matrix.py` & `resonances-0.2.6/resonances/matrix/two_body_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pandas as pd
 
 import resonances
 from resonances.matrix.matrix import Matrix
 
 
 class TwoBodyMatrix(Matrix):
-
     catalog_file = 'matrix.2body.file'
 
     @classmethod
     def build(cls):
         primary_max = resonances.config.get('matrix.2body.primary_max')
         m_max = resonances.config.get('matrix.2body.coefficients_max')
         q_max = resonances.config.get('matrix.2body.max_order')
```

### Comparing `resonances-0.2.5/resonances/resonance/factory.py` & `resonances-0.2.6/resonances/resonance/factory.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/resonance/libration.py` & `resonances-0.2.6/resonances/resonance/libration.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/resonance/mmr.py` & `resonances-0.2.6/resonances/resonance/mmr.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,19 @@
             return 'Saturn'
         elif letter == 'U':
             return 'Uranus'
         elif letter == 'N':
             return 'Neptune'
         raise Exception('Bad notation used. Only the following letter are available: R (for Mercury), V, E, M, J, S, U, N ')
 
+    def get_letter_from_planet_name(self, planet_name: str) -> str:
+        if 'Mercury' == planet_name:
+            return 'R'
+        return planet_name[0]
+
     @property
     def resonant_axis(self):
         if self._resonant_axis is None:
             self._resonant_axis = self.calculate_resonant_axis()
         return self._resonant_axis
 
     @resonant_axis.setter
```

### Comparing `resonances-0.2.5/resonances/resonance/plot.py` & `resonances-0.2.6/resonances/resonance/plot.py`

 * *Files identical despite different names*

### Comparing `resonances-0.2.5/resonances/resonance/three_body.py` & `resonances-0.2.6/resonances/resonance/three_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,30 +49,30 @@
             coeff3 = -coeff3
         coeff = [coeff1, coeff2, coeff3, 0, 0, (0 - coeff1 - coeff2 - coeff3)]
         return coeff, planets_names
 
     def to_s(self):
         s = '{:d}{:.1}{:+d}{:.1}{:+d}{:+d}{:+d}{:+d}'.format(
             int(self.coeff[0]),
-            self.planets_names[0],
+            self.get_letter_from_planet_name(self.planets_names[0]),
             int(self.coeff[1]),
-            self.planets_names[1],
+            self.get_letter_from_planet_name(self.planets_names[1]),
             int(self.coeff[2]),
             int(self.coeff[3]),
             int(self.coeff[4]),
             int(self.coeff[5]),
         )
         return s
 
     def to_short(self):
         s = '{:d}{:.1}{:+d}{:.1}{:+d}'.format(
             int(self.coeff[0]),
-            self.planets_names[0],
+            self.get_letter_from_planet_name(self.planets_names[0]),
             int(self.coeff[1]),
-            self.planets_names[1],
+            self.get_letter_from_planet_name(self.planets_names[1]),
             int(self.coeff[2]),
         )
         return s
 
     @property
     def resonant_axis(self):
         if self._resonant_axis is None:
```

### Comparing `resonances-0.2.5/resonances/resonance/two_body.py` & `resonances-0.2.6/resonances/resonance/two_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from resonances.resonance.mmr import MMR
 from resonances.data import const
 import rebound
 
 
 class TwoBody(MMR):
     def __init__(self, coeff, planets_names=None):
-
         if isinstance(coeff, str):
             coeff, planets_names = self.init_from_short_notation(coeff)
 
         super().__init__(coeff, planets_names)
 
         if np.gcd(self.coeff[0], self.coeff[1]) > 1:
             raise Exception('The integers should have gcd equals 1. Given {}.'.format(', '.join(str(e) for e in coeff)))
@@ -41,25 +40,25 @@
             coeff2 = -coeff2
         coeff = [coeff1, coeff2, 0, (0 - coeff1 - coeff2)]
         return coeff, planets_names
 
     def to_s(self):
         s = '{:d}{:.1}{:+d}{:+d}{:+d}'.format(
             int(self.coeff[0]),
-            self.planets_names[0],
+            self.get_letter_from_planet_name(self.planets_names[0]),
             int(self.coeff[1]),
             int(self.coeff[2]),
             int(self.coeff[3]),
         )
         return s
 
     def to_short(self):
         s = '{:d}{:.1}{:+d}'.format(
             int(self.coeff[0]),
-            self.planets_names[0],
+            self.get_letter_from_planet_name(self.planets_names[0]),
             int(self.coeff[1]),
         )
         return s
 
     def calculate_resonant_axis(self):
         if len(self.planets_names) != 1:
             raise Exception('Cannot calculate resonant axis if the planet is not specified!')
```

### Comparing `resonances-0.2.5/resonances/simulation.py` & `resonances-0.2.6/resonances/simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import rebound
 from pathlib import Path
 from typing import List
+import os
 
 import resonances
 from resonances.data.astdys import astdys
 from resonances.resonance import plot
 
 
 class Simulation:
@@ -56,23 +57,33 @@
             self.save_only_undetermined = resonances.config.get('save.only.undetermined')
         else:
             self.save_only_undetermined = False
 
         self.save_additional_data = resonances.config.get('save.additional.data')
         self.plot = resonances.config.get('plot')
 
-    def create_solar_system(self):
-        solar_file = Path(resonances.config.get('solar_system_file'))
+        self.initial_data_source = 'astdys'
 
+    def solar_system_full_filename(self) -> str:
+        catalog_file = f"{os.getcwd()}/{resonances.config.get('solar_system_file')}"
+        return catalog_file
+
+    def create_solar_system(self, date: str = ''):
+        solar_file = Path(self.solar_system_full_filename())
         if solar_file.exists():
-            self.sim = rebound.Simulation(resonances.config.get('solar_system_file'))
+            self.sim = rebound.Simulation(self.solar_system_full_filename())
         else:
             self.sim = rebound.Simulation()
-            self.sim.add(self.list_of_planets(), date='2020-12-17 00:00')  # date of AstDyS current catalogue
-            self.sim.save(resonances.config.get('solar_system_file'))
+            if date != '':
+                self.sim.add(self.list_of_planets(), date=date)
+            elif self.initial_data_source == 'astdys':
+                self.sim.add(self.list_of_planets(), date=f"{astdys.catalog_time()} 00:00")  # date of AstDyS current catalogue
+            else:
+                self.sim.add(self.list_of_planets())
+            self.sim.save(self.solar_system_full_filename())
 
     def add_body(self, elem_or_num, mmr: resonances.MMR, name='asteroid'):
         body = resonances.Body()
 
         if isinstance(elem_or_num, int) or (isinstance(elem_or_num, str)):
             elem = astdys.search(elem_or_num)
         elif isinstance(elem_or_num, dict):
```

### Comparing `resonances-0.2.5/setup.py` & `resonances-0.2.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                      'ir = resonances.experiment.console:identifier',
                      'simulation-shape = '
                      'resonances.experiment.console:calc_shape',
                      'ss = resonances.experiment.console:calc_shape']}
 
 setup_kwargs = {
     'name': 'resonances',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'Identification of mean-motion resonances',
-    'long_description': '# Mean-Motion Resonances\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Resonances](https://github.com/smirik/resonances/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/smirik/resonances/actions/workflows/ci.yml)\n\n`resonances` is an open-source package dedicated to the identification of mean-motion resonances of small bodies. Many examples are for the Solar system; however, you might use the package for any possible planetary system, including exoplanets.\n\nFor more information, [read the documentation](https://smirik.github.io/resonances/).\n\n**Note:** while this app has many functional and integration tests built in, it is still in the dev stage. Hence, it might include some inconsistencies. So, any community help is appreciated!\n\n## Features\n\nThe package:\n\n- can automatically identify two-body and three-body mean-motion resonance in the Solar system,\n- accurately differentiates different types of resonances (pure, transient, uncertain),\n- provides an interface for mass tasks (i.e. find resonant areas in a planetary system),\n- can plot time series and periodograms,\n- and, yeah, it is well tested ;)\n\nIt actively uses [REBOUND integrator](https://rebound.readthedocs.io) maintained by Hanno Rein and others.\n\n## Installation\n\nTo install resonances on your system, follow the instructions on the appropriate [installation guide](https://smirik.github.io/resonances/install/)\n\n## Mean-motion resonances\n\nFor those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:\n\n### Papers about the automatic identification of resonant asteroids\n\n1. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).\n1. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).\n1. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).\n\n### Papers about mean-motion resonances\n\n1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).\n1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).\n1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).\n1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).\n1. Milani, A., Cellino, A., Knezevic, Z., Novaković, B. & Spoto, F. Asteroid families classification: Exploiting very large datasets. Icarus 239, 46–73 (2014).\n1. Murray, N. & Holman, M. Diffusive chaos in the outer asteroid belt. The Astronomical Journal 114, 1246 (1997).\n1. Murray, N., Holman, M. & Potter, M. On the Origin of Chaos in the Asteroid Belt. The Astronomical Journal 116, 2583–2589 (1998).\n1. Shevchenko, I. I. On the Lyapunov exponents of the asteroidal motion subject to resonances and encounters. Proc. IAU 2, 15–30 (2006).\n\n### Books\n\n1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).\n1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).\n\n## References\n\nWhenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):\n\n1. **The package itself**: to be published\n1. **The Libration module and automatic identification of librations**: to be published\n1. **Mass identification of mean-motion resonances:** Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n\n## Authors\n\nThe authors of the package:\n\n- [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))\n\n## Acknowledgement\n\n- Many thanks to the co-authors of the papers (prof. I.\xa0I. Shevchenko, I.\xa0Dovgalev Dr.\xa0E.\xa0Popova).\n- The creators of [REBOUND integrator](https://rebound.readthedocs.io).\n- The creators of [Astropy](http://astropy.org).\n- The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.\n\n## Contributing\n\nFeel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).\n\n## License\n\nMIT\n',
+    'long_description': '# Mean-Motion Resonances\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Resonances](https://github.com/smirik/resonances/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/smirik/resonances/actions/workflows/ci.yml)\n\n`resonances` is an open-source package dedicated to the identification of mean-motion resonances of small bodies. Many examples are for the Solar system; however, you might use the package for any possible planetary system, including exoplanets.\n\nFor more information, [read the documentation](https://smirik.github.io/resonances/).\n\n**Note:** while this app has many functional and integration tests built in, it is still in the dev stage. Hence, it might include some inconsistencies. So, any community help is appreciated!\n\n## Features\n\nThe package:\n\n- can automatically identify two-body and three-body mean-motion resonance in the Solar system,\n- accurately differentiates different types of resonances (pure, transient, uncertain),\n- provides an interface for mass tasks (i.e. find resonant areas in a planetary system),\n- can plot time series and periodograms,\n- and, yeah, it is well tested ;)\n\nIt actively uses [REBOUND integrator](https://rebound.readthedocs.io) maintained by Hanno Rein and others.\n\n## Installation\n\nTo install resonances on your system, follow the instructions on the appropriate [installation guide](https://smirik.github.io/resonances/install/)\n\n## Mean-motion resonances\n\nFor those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:\n\n### Papers about the automatic identification of resonant asteroids\n\n1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).\n2. Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707\n3. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).\n4. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n5. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).\n\n### Papers about mean-motion resonances\n\n1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).\n1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).\n1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).\n1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).\n1. Milani, A., Cellino, A., Knezevic, Z., Novaković, B. & Spoto, F. Asteroid families classification: Exploiting very large datasets. Icarus 239, 46–73 (2014).\n1. Murray, N. & Holman, M. Diffusive chaos in the outer asteroid belt. The Astronomical Journal 114, 1246 (1997).\n1. Murray, N., Holman, M. & Potter, M. On the Origin of Chaos in the Asteroid Belt. The Astronomical Journal 116, 2583–2589 (1998).\n1. Shevchenko, I. I. On the Lyapunov exponents of the asteroidal motion subject to resonances and encounters. Proc. IAU 2, 15–30 (2006).\n\n### Books\n\n1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).\n1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).\n\n## References\n\nWhenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):\n\n1. **The package itself**: \n\n* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing. https://doi.org/10.1016/j.ascom.2023.100707\n\n```tex\n@article{Smirnov2023,\n  title    = {A new python package for identifying celestial bodies trapped in mean-motion resonances},\n  journal  = {Astronomy and Computing},\n  year     = {2023},\n  issn     = {2213-1337},\n  doi      = {https://doi.org/10.1016/j.ascom.2023.100707},\n  url      = {https://www.sciencedirect.com/science/article/pii/S2213133723000227},\n  author   = {E.A. Smirnov},\n  keywords = {Mean-motion resonances, Python, Identification, Asteroids},\n  abstract = {In this paper, a new open-source package ‘resonances’ written in python is introduced. It allows to find, analyse, and plot two-body and three-body mean-motion eccentricity-type resonances in the Solar and other planetary systems. The package has a better accuracy of the automatic identification procedure for resonant objects compared to previous studies. Furthermore, it has built-in integrations with AstDyS and NASA JPL catalogues. The code is extensively documented and tested with automatic tests. The package is available on GitHub under MIT Licence.}\n}\n```\n\n2. **The Libration module and automatic identification of librations**: \n\n* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707\n\n3. **Mass identification of mean-motion resonances:** \n\n* Smirnov, E. A., & Dovgalev, I. S. (2018). Identification of Asteroids in Two-Body Resonances. Solar System Research, 52(4), 347–354. https://doi.org/10.1134/S0038094618040056 \n* Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.\n\n## Authors\n\nThe authors of the package:\n\n- [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))\n\n## Acknowledgement\n\n- Many thanks to the co-authors of the papers (prof. I.\xa0I. Shevchenko, I.\xa0Dovgalev, and Dr.\xa0E.\xa0Popova).\n- The creators of [REBOUND integrator](https://rebound.readthedocs.io).\n- The creators of [Astropy](http://astropy.org).\n- The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.\n\n## Contributing\n\nFeel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).\n\n## License\n\nMIT\n',
     'author': 'Evgeny Smirnov',
     'author_email': 'smirik@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://smirik.github.io/resonances/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `resonances-0.2.5/PKG-INFO` & `resonances-0.2.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resonances
-Version: 0.2.5
+Version: 0.2.6
 Summary: Identification of mean-motion resonances
 Home-page: http://smirik.github.io/resonances/
 License: MIT
 Keywords: astronomy,nbody,resonance,mmr
 Author: Evgeny Smirnov
 Author-email: smirik@gmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -59,18 +59,19 @@
 
 ## Mean-motion resonances
 
 For those who are not familiar with the mean-motion resonances, here is the list of papers used to develop this package:
 
 ### Papers about the automatic identification of resonant asteroids
 
-1. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).
-1. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
 1. Smirnov, E. A. & Dovgalev, I. S. Identification of Asteroids in Two-Body Resonances. Solar System Research 52, 347–354 (2018).
-1. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).
+2. Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+3. Smirnov, E. A. & Shevchenko, I. I. Massive identification of asteroids in three-body resonances. Icarus 222, 220–228 (2013).
+4. Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+5. Nesvorný, D. & Morbidelli, A. Three-Body Mean Motion Resonances and the Chaotic Structure of the Asteroid Belt. The Astronomical Journal 116, 3029–3037 (1998).
 
 ### Papers about mean-motion resonances
 
 1. Chirikov, B. V. A universal instability of many-dimensional oscillator systems. Physics reports 52, 263–379 (1979).
 1. Gallardo, T. Strength, stability and three dimensional structure of mean motion resonances in the solar system. Icarus 317, 121–134 (2019).
 1. Gallardo, T. Atlas of the mean motion resonances in the Solar System. Icarus 184, 29–38 (2006).
 1. Gallardo, T., Coito, L. & Badano, L. Planetary and satellite three body mean motion resonances. Icarus 274, 83–98 (2016).
@@ -84,27 +85,50 @@
 1. Murray, C. D. & Dermott, S. F. Solar system dynamics. (Cambridge Univ. Press, 2012).
 1. Morbidelli, A. Modern celestial mechanics: aspects of solar system dynamics. (2002).
 
 ## References
 
 Whenever you use this package, we are kindly asking you to refer to one of the following papers (please choose the appropriate):
 
-1. **The package itself**: to be published
-1. **The Libration module and automatic identification of librations**: to be published
-1. **Mass identification of mean-motion resonances:** Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
+1. **The package itself**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing. https://doi.org/10.1016/j.ascom.2023.100707
+
+```tex
+@article{Smirnov2023,
+  title    = {A new python package for identifying celestial bodies trapped in mean-motion resonances},
+  journal  = {Astronomy and Computing},
+  year     = {2023},
+  issn     = {2213-1337},
+  doi      = {https://doi.org/10.1016/j.ascom.2023.100707},
+  url      = {https://www.sciencedirect.com/science/article/pii/S2213133723000227},
+  author   = {E.A. Smirnov},
+  keywords = {Mean-motion resonances, Python, Identification, Asteroids},
+  abstract = {In this paper, a new open-source package ‘resonances’ written in python is introduced. It allows to find, analyse, and plot two-body and three-body mean-motion eccentricity-type resonances in the Solar and other planetary systems. The package has a better accuracy of the automatic identification procedure for resonant objects compared to previous studies. Furthermore, it has built-in integrations with AstDyS and NASA JPL catalogues. The code is extensively documented and tested with automatic tests. The package is available on GitHub under MIT Licence.}
+}
+```
+
+2. **The Libration module and automatic identification of librations**: 
+
+* Smirnov, E. A. (2023). A new python package for identifying celestial bodies trapped in mean-motion resonances. Astronomy and Computing, 100707. https://doi.org/10.1016/j.ascom.2023.100707
+
+3. **Mass identification of mean-motion resonances:** 
+
+* Smirnov, E. A., & Dovgalev, I. S. (2018). Identification of Asteroids in Two-Body Resonances. Solar System Research, 52(4), 347–354. https://doi.org/10.1134/S0038094618040056 
+* Smirnov, E. A., Dovgalev, I. S. & Popova, E. A. Asteroids in three-body mean motion resonances with planets. Icarus (2017) doi:10.1016/j.icarus.2017.09.032.
 
 ## Authors
 
 The authors of the package:
 
 - [Evgeny Smirnov](https://github.com/smirik) ([FB](https://facebook.com/smirik), [Telegram](https://t.me/smirik))
 
 ## Acknowledgement
 
-- Many thanks to the co-authors of the papers (prof. I. I. Shevchenko, I. Dovgalev Dr. E. Popova).
+- Many thanks to the co-authors of the papers (prof. I. I. Shevchenko, I. Dovgalev, and Dr. E. Popova).
 - The creators of [REBOUND integrator](https://rebound.readthedocs.io).
 - The creators of [Astropy](http://astropy.org).
 - The creators of `numpy`, `scipy`, `pandas`, and `matplotlib`.
 
 ## Contributing
 
 Feel free to contribute to the code by sending pull requests [to the repository](https://github.com/smirik/resonances).
```

