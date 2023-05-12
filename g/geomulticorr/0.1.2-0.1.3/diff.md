# Comparing `tmp/geomulticorr-0.1.2.tar.gz` & `tmp/geomulticorr-0.1.3.tar.gz`

## Comparing `geomulticorr-0.1.2.tar` & `geomulticorr-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20444 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_pair.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20444 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_pair.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/PKG-INFO
```

### Comparing `geomulticorr-0.1.2/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.3/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/pair.py` & `geomulticorr-0.1.3/src/geomulticorr/pair.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,17 @@
         try:
             return self.pa_dispY_geoim
         except AttributeError:
             self.pa_dispY_geoim = rt.pre_process(str(self.pa_dispf_path), geoim=True, nBands=2)
             return self.pa_dispY_geoim
     
     def get_vx_geoim(self):
+        """
+        Ajouter les années en décimal pour convertir les vitesses, plus précis qu'en base 365 jours par 365 jours
+        """
         return self.get_dispX_geoim() / abs(self.pa_left.th_year - self.pa_right.th_year)
 
     def get_vy_geoim(self):
         return self.get_dispY_geoim() / abs(self.pa_left.th_year - self.pa_right.th_year)
 
     def get_vmagn_geoim(self):
         return self.get_magn_geoim() / abs(self.pa_left.th_year - self.pa_right.th_year)
@@ -208,16 +211,23 @@
             --corr-memory-limit-mb 8000 \
             --save-left-right-disparity-difference\
             --ip-per-tile 200 \
             --min-num-ip 5"
 
         # Launch
         os.system(corr_command)
+        self.pa_status='complete'
         return True
 
+    def corr_eval(self):
+        """
+        Appel de la fonction d'ASP pour générer un raster SNR
+        """
+        pass
+
     def save_corrdata(self, verbose=False):
         """
         Move the ASP outputs from GeoMultiCorr temporal storage location
         """
 
         # Hide ugly warnings about symlinks
         verbose_mode = {False:' > /dev/null 2>&1', True:''}
@@ -232,14 +242,20 @@
         os.system(f"mv {departure} {destination} {verbose_mode[verbose]}")
         if self.pa_asp_path.exists():
             os.system(f"rm -rf {departure}")
             return True
 
         return False
 
+    def del_useless_data(self):
+        """
+        Suppression des données inutiles
+        """
+        pass
+
     def compute_magnitude(self):
 
         assert self.pa_dispf_path.exists(), 'this pair is not yet correlate'
 
         # Check if the file is ever existing
         if self.pa_magn_path.exists():
             return self.get_magn_geoim()
@@ -297,14 +313,17 @@
         # Switch from matrixian to geographic spatial referential
         dy_in_meters_switched = dy_in_meters * -1
 
         # Compute vector norm (magnitude) in meters
         d_in_meters = (dx_in_meters ** 2 + dy_in_meters_switched ** 2) **0.5
 
         # Convert into annual velocity
+        """
+        Ajouter les années en décimal pour convertir les vitesses, plus précis qu'en base 365 jours par 365 jours
+        """
         time_gap = abs(self.pa_left.th_year - self.pa_right.th_year)
         dx_in_meters_per_year = dx_in_meters / time_gap
         dy_in_meters_per_year = dy_in_meters / time_gap
         d_in_meters_per_year  = d_in_meters  / time_gap
 
         # Compute displacement geographic direction (vector orientation)
         array_complex_dx_dy = np.apply_along_axis(lambda args: [complex(*args)], 0, [dx_in_meters.array,dy_in_meters_switched.array]).reshape(nCols, nRows)
@@ -322,15 +341,19 @@
             dx_in_meters_per_year,
             dy_in_meters_per_year,
             d_in_meters_per_year,
             direction
         ])
         
         vectors = rt.vectorize(to_vectorize).set_crs(epsg=2154)
-    
+
+        """
+        changer le nom des colonnes attributaires
+        """
+
         # Write vector layer in geopackage
         if write == True:
             current_vector_layer_name = f"{output_pixel_size}_{self.pa_key}"
             vectors.to_file(self.pa_vect_path, layer=current_vector_layer_name)
 
             # Copy .qml file
             template_style = 'styles/vector-field_style_1.qml'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geomulticorr-0.1.2/src/geomulticorr/pzone.py` & `geomulticorr-0.1.3/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/session.py` & `geomulticorr-0.1.3/src/geomulticorr/session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/spine.py` & `geomulticorr-0.1.3/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/thumb.py` & `geomulticorr-0.1.3/src/geomulticorr/thumb.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def __init__(self, target_path):
         target_path = Path(target_path)
 
         # Vérification de l'existence du fichier pointé par l'adresse 
         # et de la validité du nom au regard du pattern défini
         assert target_path.exists(), 'fichier inexistant'
-        assert THUMBNAME_PATTERN.match(target_path.name), 'filename don\'t match with gmc_thumbname pattern'
+        assert THUMBNAME_PATTERN.match(target_path.name), 'filename don\'t match with thumbname pattern'
 
         self.th_path = str(target_path)
         self.th_key = target_path.name.split('.')[0]
         self.th_pz_name, self.th_date, self.th_sensor = self.th_key.split('_')
         self.th_year = int(self.th_date.split('-')[0])
         self.geometry = rt.drawGeomExtent(self.th_path, geomType='shly')
         self.th_valid=0
```

### Comparing `geomulticorr-0.1.2/src/geomulticorr/xzone.py` & `geomulticorr-0.1.3/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.3/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.3/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.3/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/tests/test_geomorph.py` & `geomulticorr-0.1.3/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/tests/test_pair.py` & `geomulticorr-0.1.3/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/tests/test_pzone.py` & `geomulticorr-0.1.3/tests/test_pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/tests/test_session.py` & `geomulticorr-0.1.3/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/tests/test_thumb.py` & `geomulticorr-0.1.3/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/LICENSE.md` & `geomulticorr-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.2/pyproject.toml` & `geomulticorr-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.2/PKG-INFO` & `geomulticorr-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

