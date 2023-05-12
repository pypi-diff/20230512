# Comparing `tmp/scubas-0.1.2.tar.gz` & `tmp/scubas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scubas-0.1.2.tar", last modified: Thu Mar  2 23:22:58 2023, max compression
+gzip compressed data, was "scubas-0.1.3.tar", last modified: Fri May 12 02:31:57 2023, max compression
```

## Comparing `scubas-0.1.2.tar` & `scubas-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-03-02 23:22:58.000000 scubas-0.1.2/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1076 2023-02-09 21:26:26.000000 scubas-0.1.2/LICENSE
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      958 2023-03-02 23:22:58.000000 scubas-0.1.2/PKG-INFO
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      182 2023-02-15 17:45:10.000000 scubas-0.1.2/README.md
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       22 2023-02-15 16:56:39.000000 scubas-0.1.2/scubas/__init__.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        0 2023-02-09 21:36:12.000000 scubas-0.1.2/scubas/analysis.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    19448 2023-03-02 23:22:57.000000 scubas-0.1.2/scubas/cables.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    21360 2023-02-18 02:47:03.000000 scubas-0.1.2/scubas/conductivity.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    12799 2023-03-02 22:44:14.000000 scubas-0.1.2/scubas/datasets.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     8607 2023-03-02 23:22:57.000000 scubas-0.1.2/scubas/models.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     3784 2023-02-25 03:24:06.000000 scubas-0.1.2/scubas/plotlib.py
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2006 2023-02-20 16:30:25.000000 scubas-0.1.2/scubas/utils.py
-drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      958 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/PKG-INFO
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      323 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/SOURCES.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        1 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/dependency_links.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       56 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/requires.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        7 2023-03-02 23:22:58.000000 scubas-0.1.2/scubas.egg-info/top_level.txt
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       38 2023-03-02 23:22:58.000000 scubas-0.1.2/setup.cfg
--rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1340 2023-03-02 23:22:54.000000 scubas-0.1.2/setup.py
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1076 2023-02-09 21:26:26.000000 scubas-0.1.3/LICENSE
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2693 2023-05-12 02:31:57.836293 scubas-0.1.3/PKG-INFO
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1671 2023-05-12 00:59:59.000000 scubas-0.1.3/README.md
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/scubas/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       22 2023-02-15 16:56:39.000000 scubas-0.1.3/scubas/__init__.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    19544 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas/cables.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    21360 2023-02-18 02:47:03.000000 scubas-0.1.3/scubas/conductivity.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)    12799 2023-03-02 22:44:14.000000 scubas-0.1.3/scubas/datasets.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     8959 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas/models.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     3784 2023-02-25 03:24:06.000000 scubas-0.1.3/scubas/plotlib.py
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2008 2023-05-12 01:48:19.000000 scubas-0.1.3/scubas/utils.py
+drwxrwxr-x   0 shibaji   (1000) shibaji   (1000)        0 2023-05-12 02:31:57.836293 scubas-0.1.3/scubas.egg-info/
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     2693 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/PKG-INFO
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)      304 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/SOURCES.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        1 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/dependency_links.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       56 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/requires.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)        7 2023-05-12 02:31:57.000000 scubas-0.1.3/scubas.egg-info/top_level.txt
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)       38 2023-05-12 02:31:57.836293 scubas-0.1.3/setup.cfg
+-rw-rw-r--   0 shibaji   (1000) shibaji   (1000)     1755 2023-05-12 01:29:56.000000 scubas-0.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scubas-0.1.2/LICENSE` & `scubas-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scubas-0.1.2/scubas/cables.py` & `scubas-0.1.3/scubas/cables.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,24 +160,26 @@
         o = "Z: %s (Ohm/km)\n" % (frexp102str(self.Z * 1e3))
         o += "Y: %s (S/km)\n" % (frexp102str(self.Y * 1e3))
         o += "Z0: %s (Ohm)\n" % (frexp102str(self.Z0))
         o += "gma: %s (/km)\n" % (frexp102str(self.gma * 1e3))
         o += "Ad: %s (km)" % (frexp102str(1e-3 / self.gma))
         return o
 
-    def compile_oml(self, bfield_data_files=[], p=None):
+    def compile_oml(self, bfield_data_files=[], p=None, csv_file_date_name="Date"):
         """
         Create ocean model
         """
         self.model = OceanModel(
             self.elec_params.site,
             flim=self.elec_params.flim,
         )
         if bfield_data_files and len(bfield_data_files) > 0:
-            self.model.read_Bfield_data(bfield_data_files)
+            self.model.read_Bfield_data(
+                bfield_data_files, csv_file_date_name=csv_file_date_name
+            )
             self.model.to_Efields(p=p)
             self.compute_eqv_pi_circuit()
         return self
 
     def add_active_termination(self):
         """
         Adding active terminations
```

### Comparing `scubas-0.1.2/scubas/conductivity.py` & `scubas-0.1.3/scubas/conductivity.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.2/scubas/datasets.py` & `scubas-0.1.3/scubas/datasets.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.2/scubas/models.py` & `scubas-0.1.3/scubas/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,23 +156,29 @@
             df["Y"] = df["H"] * np.sin(np.deg2rad(df["D"] / 60.0))
             del df["H"], df["D"]
         if return_header:
             return df, header_records
         else:
             return df
 
-    def read_Bfield_data(self, files, return_xyzf=True):
+    def read_Bfield_data(self, files, return_xyzf=True, csv_file_date_name="Date"):
         """
         Read B-Files
         """
         self.Bfield = pd.DataFrame()
         for file in files:
-            self.Bfield = pd.concat(
-                [self.Bfield, self.read_iaga(file, return_xyzf, return_header=False)]
-            )
+            file_type = file.split(".")[-1]
+            if file_type == "txt":
+                o = self.read_iaga(file, return_xyzf, return_header=False)
+            elif file_type == "csv":
+                o = pd.read_csv(file, parse_dates=[csv_file_date_name])
+                o = o.rename(columns={csv_file_date_name: "Time"})
+                o = o.set_index("Time")
+                o.index.name = "Time"
+            self.Bfield = pd.concat([self.Bfield, o])
         return self.Bfield
 
     def to_Efields(self, Bfield=None, components=["X", "Y"], p=None):
         """
         Compute Et using numerical FFT and IFFT block
         Bfield: Dataframe containing B-field
         components: [X and Y] for B-fields
```

### Comparing `scubas-0.1.2/scubas/plotlib.py` & `scubas-0.1.3/scubas/plotlib.py`

 * *Files identical despite different names*

### Comparing `scubas-0.1.2/scubas/utils.py` & `scubas-0.1.3/scubas/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""utility.py: Module is used to implement utility methods"""
+"""utility.py: Module is used to implement utility methods.
+"""
 
 __author__ = "Chakraborty, S."
 __copyright__ = ""
 __credits__ = []
 __license__ = "MIT"
 __version__ = "1.0."
 __maintainer__ = "Chakraborty, S."
```

