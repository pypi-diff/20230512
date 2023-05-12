# Comparing `tmp/napari-stpt-0.1.0.1.tar.gz` & `tmp/napari-stpt-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-stpt-0.1.0.1.tar", last modified: Wed May 10 17:06:56 2023, max compression
+gzip compressed data, was "napari-stpt-0.1.0.2.tar", last modified: Fri May 12 15:41:10 2023, max compression
```

## Comparing `napari-stpt-0.1.0.1.tar` & `napari-stpt-0.1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 17:06:56.601086 napari-stpt-0.1.0.1/
--rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.1/LICENSE
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-10 17:06:56.596086 napari-stpt-0.1.0.1/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.1/README.md
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 17:06:56.435084 napari-stpt-0.1.0.1/napari_stpt/
--rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.1/napari_stpt/__init__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.1/napari_stpt/__main__.py
--rw-r--r--   0 tristan   (1000) tristan   (1000)   138851 2023-05-10 17:05:58.000000 napari-stpt-0.1.0.1/napari_stpt/napari_stpt.py
-drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-10 17:06:56.570086 napari-stpt-0.1.0.1/napari_stpt.egg-info/
--rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/PKG-INFO
--rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/SOURCES.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/dependency_links.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/entry_points.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       78 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/requires.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-05-10 17:06:56.000000 napari-stpt-0.1.0.1/napari_stpt.egg-info/top_level.txt
--rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-05-10 17:06:56.602086 napari-stpt-0.1.0.1/setup.cfg
--rw-r--r--   0 tristan   (1000) tristan   (1000)     1283 2023-05-10 17:06:35.000000 napari-stpt-0.1.0.1/setup.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.124565 napari-stpt-0.1.0.2/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)    35149 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.2/LICENSE
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-12 15:41:10.123565 napari-stpt-0.1.0.2/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3170 2021-07-01 22:42:19.000000 napari-stpt-0.1.0.2/README.md
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.051564 napari-stpt-0.1.0.2/napari_stpt/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       46 2021-10-27 12:13:32.000000 napari-stpt-0.1.0.2/napari_stpt/__init__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      267 2022-01-28 14:11:11.000000 napari-stpt-0.1.0.2/napari_stpt/__main__.py
+-rw-r--r--   0 tristan   (1000) tristan   (1000)   139569 2023-05-12 14:48:30.000000 napari-stpt-0.1.0.2/napari_stpt/napari_stpt.py
+drwxr-xr-x   0 tristan   (1000) tristan   (1000)        0 2023-05-12 15:41:10.121565 napari-stpt-0.1.0.2/napari_stpt.egg-info/
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     3607 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/PKG-INFO
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      313 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/SOURCES.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)        1 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/dependency_links.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       58 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/entry_points.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)      108 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/requires.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       12 2023-05-12 15:41:09.000000 napari-stpt-0.1.0.2/napari_stpt.egg-info/top_level.txt
+-rw-r--r--   0 tristan   (1000) tristan   (1000)       38 2023-05-12 15:41:10.124565 napari-stpt-0.1.0.2/setup.cfg
+-rw-r--r--   0 tristan   (1000) tristan   (1000)     1335 2023-05-12 15:40:33.000000 napari-stpt-0.1.0.2/setup.py
```

### Comparing `napari-stpt-0.1.0.1/LICENSE` & `napari-stpt-0.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.1/PKG-INFO` & `napari-stpt-0.1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.1/README.md` & `napari-stpt-0.1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `napari-stpt-0.1.0.1/napari_stpt/napari_stpt.py` & `napari-stpt-0.1.0.2/napari_stpt/napari_stpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,21 +423,25 @@
             self.ds1 = xr.open_zarr(file_name)
 
         
         # Read the image spacing
         if self.old_method:
             self.spacing = (self.ds1['S001'].attrs['scale'])
         else:
-            self.spacing = [0,0]
+            self.spacing = [1,1]
             try:
-                self.spacing[0] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["x"])
-                self.spacing[1] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["y"])
-                # self.spacing[2] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["z"])
+                self.spacing[0] = float(json.loads(self.ds1.attrs['multiscale'])['metadata']['scale'][0])
+                self.spacing[1] = float(json.loads(self.ds1.attrs['multiscale'])['metadata']['scale'][1])
             except:
-                print("spacing not defined")
+                try:
+                    self.spacing[0] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["x"])
+                    self.spacing[1] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["y"])
+                    # self.spacing[2] = 10 * float(json.loads(self.ds1['S001'].attrs['scale'])["z"])
+                except:
+                    print("spacing not defined")
                 
                 
         if load_in_reference:
             self.spacing = reference_spacing
             
             
                 
@@ -465,16 +469,19 @@
         # Get number of sections
         if self.axio:
             self.number_of_sections = len(list(self.ds1))
             self.optical_slices_available = 1
         else:
             if self.old_method:
                 self.number_of_sections = len(set(self.ds1.attrs['cube_reg']['slice']))
-            else:    
-                self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
+            else:
+                try:
+                    self.number_of_sections = int(json.loads(self.ds1['S001'].attrs['raw_meta'])['sections'])
+                except:
+                    self.number_of_sections = int(json.loads(self.ds1.attrs['multiscale'])['metadata']['number_of_sections'])
         
         if verbose:
             print(f"Number of sections: {self.number_of_sections}")
             
             
         #print("")
         #print(self.ds1.attrs)
@@ -554,15 +561,18 @@
         self.slice_spacing = float(self.m_slice_spacing.text())
 
         # Get the optical slice spacing
         if self.old_method or self.axio:
             # assume that the optical slices do not overlap
             optical_section_spacing = self.slice_spacing / self.optical_slices_available
         else:
-            optical_section_spacing = float(json.loads(self.ds1['S001'].attrs['raw_meta'])['zres'])
+            try:
+                optical_section_spacing = float(json.loads(self.ds1['S001'].attrs['raw_meta'])['zres'])
+            except:
+                optical_section_spacing = float(json.loads(self.ds1.attrs['multiscale'])['metadata']['optical_section_spacing'])
 
         if verbose:
             print(f"optical_slices zres: {optical_section_spacing}")
 
 
         # Calculate how many optical slices to use
         if self.optical_slices_available > 1:
@@ -2552,15 +2562,16 @@
         else:
             self.old_method = False
             self.axio = False
             self.image_folders = {
                 '/storage/processed.2022/stpt/',
                 '/storage/processed/stpt/',
                 '/storage/imaxt.processed.2022/stpt/',
-                '/data/meds1_c/storage/processed0/stpt/'
+                '/data/meds1_c/storage/processed0/stpt/',
+                '/storage/tristan/imaxt_zarr/'
             }
             print("setting STPT method")
 
         file_list = []
         for folder in self.image_folders:
             print(sys.platform)
             if sys.platform == 'linux':
@@ -2679,15 +2690,16 @@
         hbox = QtWidgets.QHBoxLayout()
         self.comboBoxPath = ExtendedComboBox()
 
         self.image_folders = {
             '/storage/processed.2022/stpt/',
             '/storage/processed/stpt/',
             '/storage/imaxt.processed.2022/stpt/',
-            '/data/meds1_c/storage/processed0/stpt/'
+            '/data/meds1_c/storage/processed0/stpt/',
+            '/storage/tristan/imaxt_zarr/'
         }
         file_list = []
         for folder in self.image_folders:
             self.search_folder = QtWidgets.QLineEdit(folder)
             if os.path.exists(self.search_folder.text()):
                 for f in os.scandir(self.search_folder.text()):
                     if f.is_dir():
```

### Comparing `napari-stpt-0.1.0.1/napari_stpt.egg-info/PKG-INFO` & `napari-stpt-0.1.0.2/napari_stpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-stpt
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: napari viewer which can read stpt images as zarr files
 Home-page: https://github.com/TristanWhitmarsh/napari-stpt
 Author: Tristan Whitmarsh
 Author-email: tw401@cam.ac.uk
 License: GNU
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `napari-stpt-0.1.0.1/setup.py` & `napari-stpt-0.1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # this grabs the requirements from requirements.txt
 #REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # This call to setup() does all the work
 setup(
     name="napari-stpt",
-    version="0.1.0.1",
+    version="0.1.0.2",
     description="napari viewer which can read stpt images as zarr files",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/TristanWhitmarsh/napari-stpt",
     author="Tristan Whitmarsh",
     author_email="tw401@cam.ac.uk",
     license="GNU",
@@ -30,14 +30,16 @@
     ],
     packages=["napari_stpt"],
     include_package_data=True,
     install_requires=[
         'opencv-python==4.5.1.48',
         'napari',
         'numpy',
+        'xarray==0.20.1',
         'zarr',
+        'PySide2',
         'SimpleITK',
-        'napari-animation',
+        'napari-animation==0.0.5',
         'tifffile'
     ],
     entry_points={"console_scripts": ["napari-stpt=napari_stpt.__main__:main"]},
 )
```

