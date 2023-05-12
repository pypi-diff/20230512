# Comparing `tmp/geomulticorr-0.1.3.tar.gz` & `tmp/geomulticorr-0.1.4.tar.gz`

## Comparing `geomulticorr-0.1.3.tar` & `geomulticorr-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/__init__.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/geomorph.py
--rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/pair.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/pzone.py
--rw-r--r--   0        0        0    20444 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/session.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/spine.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/thumb.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/xzone.py
--rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
--rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/src/geomulticorr/resources/project_template/map_template-project.qgz
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_geomorph.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_pair.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_pzone.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_session.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_thumb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/tests/test_xzone.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/LICENSE.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/geomorph.py
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/pair.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/pzone.py
+-rw-r--r--   0        0        0    20383 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/session.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/spine.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/thumb.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/xzone.py
+-rwxr-xr-x   0        0        0    12941 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/map_styles/vector-field_style_1.qml
+-rw-r--r--   0        0        0 19431424 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/src/geomulticorr/resources/project_template/map_template-project.qgz
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_geomorph.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_pair.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_pzone.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_session.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_thumb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/tests/test_xzone.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 geomulticorr-0.1.4/PKG-INFO
```

### Comparing `geomulticorr-0.1.3/src/geomulticorr/geomorph.py` & `geomulticorr-0.1.4/src/geomulticorr/geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/pair.py` & `geomulticorr-0.1.4/src/geomulticorr/pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/pzone.py` & `geomulticorr-0.1.4/src/geomulticorr/pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/session.py` & `geomulticorr-0.1.4/src/geomulticorr/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,25 +101,24 @@
             project_name = Path(target_root_path).name
 
             # Here we copy the template
             os.system(f"cp -r {project_template_location} {target_root_path}")
 
             # Here we change the name of the initial data
             os.rename(
-                src = f"{os.path.join(target_root_path, 'raster-data_template-project')}",
-                dst = f"{os.path.join(target_root_path, 'raster-data_' + project_name)}")
-
-            os.rename(
                 src = f"{os.path.join(target_root_path, 'geodatabase_template-project.gpkg')}",
                 dst = f"{os.path.join(target_root_path, 'geodatabase_' + project_name + '.gpkg')}")
 
             os.rename(
                 src = f"{os.path.join(target_root_path, 'map_template-project.qgz')}",
                 dst = f"{os.path.join(target_root_path, 'map_' + project_name + '.qgz')}")
 
+            # And we create en empty folder raster-data_project-name
+            Path(target_root_path, 'raster-data_' + project_name).mkdir()
+
         # Load project data into the current session
         self.p_root = str(target_root_path)
         self.project_name = Path(self.p_root).name
         self.p_raster_data = str(Path(self.p_root, f'raster-data_{self.project_name}'))
         self.p_geodb = os.path.join(target_root_path, f'geodatabase_{self.project_name}.gpkg')
 
         # There is underscore before the attribute name because
```

### Comparing `geomulticorr-0.1.3/src/geomulticorr/spine.py` & `geomulticorr-0.1.4/src/geomulticorr/spine.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/thumb.py` & `geomulticorr-0.1.4/src/geomulticorr/thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/xzone.py` & `geomulticorr-0.1.4/src/geomulticorr/xzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/resources/map_styles/vector-field_style_1.qml` & `geomulticorr-0.1.4/src/geomulticorr/resources/map_styles/vector-field_style_1.qml`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg` & `geomulticorr-0.1.4/src/geomulticorr/resources/project_template/geodatabase_template-project.gpkg`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/src/geomulticorr/resources/project_template/map_template-project.qgz` & `geomulticorr-0.1.4/src/geomulticorr/resources/project_template/map_template-project.qgz`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/tests/test_geomorph.py` & `geomulticorr-0.1.4/tests/test_geomorph.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/tests/test_pair.py` & `geomulticorr-0.1.4/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/tests/test_pzone.py` & `geomulticorr-0.1.4/tests/test_pzone.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/tests/test_session.py` & `geomulticorr-0.1.4/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/tests/test_thumb.py` & `geomulticorr-0.1.4/tests/test_thumb.py`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/LICENSE.md` & `geomulticorr-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomulticorr-0.1.3/pyproject.toml` & `geomulticorr-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geomulticorr"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Thibaut Duvanel", email="thibaut.duvanel@univ-smb.fr" },
 ]
 description = "A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `geomulticorr-0.1.3/PKG-INFO` & `geomulticorr-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomulticorr
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python lib to study earth-surface displacements from optical images with Ames Stereo Pipeline
 Author-email: Thibaut Duvanel <thibaut.duvanel@univ-smb.fr>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

