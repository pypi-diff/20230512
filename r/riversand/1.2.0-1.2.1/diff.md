# Comparing `tmp/riversand-1.2.0.tar.gz` & `tmp/riversand-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riversand-1.2.0.tar", last modified: Thu Mar 30 14:17:57 2023, max compression
+gzip compressed data, was "riversand-1.2.1.tar", last modified: Fri May 12 10:33:28 2023, max compression
```

## Comparing `riversand-1.2.0.tar` & `riversand-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-30 14:17:57.694241 riversand-1.2.0/
--rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.0/LICENSE
--rw-rw-r--   0 user      (1001) user      (1001)     3519 2023-03-30 14:17:57.694241 riversand-1.2.0/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)     2774 2023-03-13 11:37:26.000000 riversand-1.2.0/README.md
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-30 14:17:57.694241 riversand-1.2.0/riversand/
--rw-rw-r--   0 user      (1001) user      (1001)      496 2023-02-23 15:28:06.000000 riversand-1.2.0/riversand/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)       23 2023-03-30 14:12:06.000000 riversand-1.2.0/riversand/_version_.py
--rw-rw-r--   0 user      (1001) user      (1001)    27596 2023-03-20 14:53:36.000000 riversand-1.2.0/riversand/calc.py
--rw-rw-r--   0 user      (1001) user      (1001)    55106 2023-03-30 08:26:19.000000 riversand-1.2.0/riversand/geospatial.py
--rw-rw-r--   0 user      (1001) user      (1001)     2855 2023-02-25 19:58:58.000000 riversand-1.2.0/riversand/params.py
--rw-rw-r--   0 user      (1001) user      (1001)    10857 2023-03-30 14:04:11.000000 riversand-1.2.0/riversand/plot.py
--rw-rw-r--   0 user      (1001) user      (1001)    20640 2023-03-21 07:26:49.000000 riversand-1.2.0/riversand/utils.py
--rw-rw-r--   0 user      (1001) user      (1001)     9269 2023-02-25 20:02:22.000000 riversand-1.2.0/riversand/xml.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-03-30 14:17:57.694241 riversand-1.2.0/riversand.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)     3519 2023-03-30 14:17:57.000000 riversand-1.2.0/riversand.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      351 2023-03-30 14:17:57.000000 riversand-1.2.0/riversand.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-03-30 14:17:57.000000 riversand-1.2.0/riversand.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       59 2023-03-30 14:17:57.000000 riversand-1.2.0/riversand.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       10 2023-03-30 14:17:57.000000 riversand-1.2.0/riversand.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-03-30 14:17:57.694241 riversand-1.2.0/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     1269 2023-03-30 14:17:20.000000 riversand-1.2.0/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-12 10:33:28.309025 riversand-1.2.1/
+-rw-rw-r--   0 user      (1001) user      (1001)    35150 2023-02-25 18:17:07.000000 riversand-1.2.1/LICENSE
+-rw-rw-r--   0 user      (1001) user      (1001)     3519 2023-05-12 10:33:28.309025 riversand-1.2.1/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)     2774 2023-03-13 11:37:26.000000 riversand-1.2.1/README.md
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-12 10:33:28.309025 riversand-1.2.1/riversand/
+-rw-rw-r--   0 user      (1001) user      (1001)      537 2023-05-05 13:22:06.000000 riversand-1.2.1/riversand/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)       23 2023-05-05 13:21:40.000000 riversand-1.2.1/riversand/_version.py
+-rw-rw-r--   0 user      (1001) user      (1001)    27596 2023-03-20 14:53:36.000000 riversand-1.2.1/riversand/calc.py
+-rw-rw-r--   0 user      (1001) user      (1001)    59009 2023-05-12 09:12:03.000000 riversand-1.2.1/riversand/geospatial.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2853 2023-05-11 16:34:05.000000 riversand-1.2.1/riversand/params.py
+-rw-rw-r--   0 user      (1001) user      (1001)    10857 2023-03-30 14:04:11.000000 riversand-1.2.1/riversand/plot.py
+-rw-rw-r--   0 user      (1001) user      (1001)    20640 2023-03-21 07:26:49.000000 riversand-1.2.1/riversand/utils.py
+-rw-rw-r--   0 user      (1001) user      (1001)     9269 2023-02-25 20:02:22.000000 riversand-1.2.1/riversand/xml.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-12 10:33:28.309025 riversand-1.2.1/riversand.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)     3519 2023-05-12 10:33:28.000000 riversand-1.2.1/riversand.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      350 2023-05-12 10:33:28.000000 riversand-1.2.1/riversand.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-12 10:33:28.000000 riversand-1.2.1/riversand.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       59 2023-05-12 10:33:28.000000 riversand-1.2.1/riversand.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       10 2023-05-12 10:33:28.000000 riversand-1.2.1/riversand.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-12 10:33:28.309025 riversand-1.2.1/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     1269 2023-05-12 09:24:36.000000 riversand-1.2.1/setup.py
```

### Comparing `riversand-1.2.0/LICENSE` & `riversand-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/PKG-INFO` & `riversand-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.0
+Version: 1.2.1
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `riversand-1.2.0/README.md` & `riversand-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/riversand/calc.py` & `riversand-1.2.1/riversand/calc.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/riversand/geospatial.py` & `riversand-1.2.1/riversand/geospatial.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 For multi-catchment datasets, the catchment identifier is set with .set_cid()
 A list of catchment names is obtained with .catchments.get_name()
 The project is validated with .validate()
 
 Calculations are performed with:
 results = rv.process_single_catchment()
 results = rv.process_multi_catchment()
+results = rv.catchment_stats()
     
 The current version of the online calculator is obtained from calc.py
 version = calc.get_version()
 
 """
 
 import os, sys
@@ -844,14 +845,17 @@
         if self.elevation is None:
             raise ValueError("Missing elevation raster")
         if self.samples is None:
             raise ValueError("Missing sample data")           
         if self.catchments is None:
             raise ValueError("Missing catchment polygons") 
             
+        if len(self.catchments.catchments)>1:
+            raise ValueError("Use .process_multi_catchment() if shapefile has more than one polygon")
+            
         if isinstance(shielding, str):
             if shielding not in {'topo', 'sample'}:
                 raise ValueError("Invalid shielding: must be 'topo', 'sample' or numeric")
         if isinstance(shielding, Number):
             if not (0<=shielding<=1):
                 raise ValueError("Invalid shielding: must be 0..1")
         if (shielding=='topo') and (self.shielding is None):
@@ -859,16 +863,17 @@
         if (shielding=='sample') and ('shielding' not in self.samples.keys()):
             raise ValueError("Invalid shielding='sample' but no shielding in sample data")
             
         if unit not in params.units.keys():
             raise ValueError("Invalid unit='{}': see params.units for valid options"
                              .format(unit))
             
+            
         result_cols = ['name', 'scaling', 'nuclide',
-                       'E', 'delE-', 'delE+', 'NRMSE', 'error']
+                       'E', 'delE-', 'delE+', 'NRMSE', 'Tavg', 'error']
         results = pd.DataFrame(columns=result_cols)
         
         errR, errS, errC = self.validate(verbose=False, multi=False)
         if len(errR+errS+errC)>0:
             print("Cannot validate dataset for single-catchment processing; "+
                              "use '.validate()' for details")
             return results
@@ -990,31 +995,34 @@
                                                     unit=unit, fname=plot,
                                                     fullname=fullname)
                     
                 finally:
                     results.loc[idx, 'name'] = name    
                     results.loc[idx, 'scaling'] = scaling
                     results.loc[idx, 'nuclide'] = nuclide
+                    
                     results.loc[idx, 'E'] = E
                     results.loc[idx, 'delE-'] = delE[0]
                     results.loc[idx, 'delE+'] = delE[1]
                     results.loc[idx, 'NRMSE'] = NRMSE
+                    results.loc[idx, 'Tavg'] = np.round(160/sample_data['density']/E,)
             
                     if err==[]:
                         results.loc[idx, 'error'] = ''
                     else:
                         results.loc[idx, 'error'] = "; ".join(err)
                     ## possible error messages:
                     # 'NRMSE = ...'
                     # 'Root finding did not converge'
                     # 'Cannot compute uncertainty'
                     # 'Server cannot resolve erosion rates, dropping duplicates'
         
         return results
     
+        
     def process_multi_catchment(self,
             bins=500, scaling='LSDn', shielding=1, unit='mm/yr',
             plot=None,
             url=None, verbose=True) -> pd.DataFrame:
         """
         Calculate catchmentwide erosion rates for a multi-catchment shapefile.
         
@@ -1069,16 +1077,17 @@
         if (shielding=='sample') and ('shielding' not in self.samples.keys()):
             raise ValueError("Invalid shielding='sample' but no shielding in sample data")
             
         if unit not in params.units.keys():
             raise ValueError("Invalid unit='{}': see params.units for valid options"
                              .format(unit))
             
+            
         result_cols = ['name', 'scaling', 'nuclide', 'qtz',
-                       'E', 'delE-', 'delE+', 'NRMSE', 'error']
+                       'E', 'delE-', 'delE+', 'NRMSE', 'Tavg', 'error']
         results = pd.DataFrame(columns=result_cols)
         results['name'] = self.samples['name']
 
         errR, errS, errC = self.validate(verbose=False, multi=True)
         if len(errR+errS+errC)>0:
             print("Cannot validate dataset for multi-catchment processing; "+
                   "use '.validate()' for details")
@@ -1217,20 +1226,21 @@
                             print(Estr)
                             
                        
                         
             results.loc[idx, 'name'] = sample_data['name']   
             results.loc[idx, 'scaling'] = scaling
             results.loc[idx, 'nuclide'] = nuclide
-            results.loc[idx, 'qtz'] = 100-Qpc
+            results.loc[idx, 'qtz'] = np.round(100-Qpc,1)
                         
             results.loc[idx, 'E'] = E
             results.loc[idx, 'delE-'] = delE[0]
             results.loc[idx, 'delE+'] = delE[1]
             results.loc[idx, 'NRMSE'] = NRMSE
+            results.loc[idx, 'Tavg'] = np.round(160/sample_data['density']/E,)
                 
             if error_code:
                 if verbose:
                     print(error_code)
                     
                 results.loc[idx, 'error'] = error_code
                 # 'catchment out of bounds'
@@ -1252,15 +1262,97 @@
             if 'quartz' not in clips.keys():
                 results.drop(columns=['qtz'], inplace=True)
         except:
             pass
         
         return results
     
+    
+    def catchment_stats(self,
+            bins=100, verbose=True) -> pd.DataFrame:
+        """
+        Calculate topo statistics for a multi-catchment shapefile.
+        
+        Parameters
+        ----------
+        bins : numeric, optional
+            bin size in meters for elevation binning. The default is 500.
+    
+        Returns
+        -------
+        results : pd.DataFrame
+            Table of results for each sample.
+            
+        """
+        
+        from riversand.utils import eliminate_quartzfree, get_topostats
+        
+        if self.elevation is None:
+            raise ValueError("Missing elevation raster")
+        if self.samples is None:
+            raise ValueError("Missing sample data")           
+        if self.catchments is None:
+            raise ValueError("Missing catchment polygons")
+            
+        # # multi / single is determined by the number of polygons but cid must be set to identify the polygons
+        # if self.cid is None:
+        #     raise ValueError("No catchment identifier defined; use .set_cid()")
+        # if self.cid not in self.catchments.attrs: # self.set_cid() does not allow to set an invalid cid
+        #     raise ValueError("Invalid catchment identifier cid='{}'; use .set_cid()"
+        #                                   .format(self.cid))
+            
+        topo_cols = ['name', 'centr_lat', 'centr_long', 'mean_elev',
+                     'relief', 'area', 'mean_sf', 'qtz_pc']
+        results = pd.DataFrame(columns=topo_cols)
+            
+        errR, errS, errC = self.validate(verbose=False) # 'multi' determined from number of catchments
+        if len(errR+errS+errC)>0:
+            print("Cannot validate dataset; "+
+                  "use '.validate()' for details")
+            return results
 
+        if verbose:
+            print("Processing ", end="")
+            end = ""
+            
+        for idx, c in enumerate(self.catchments.catchments):
+            if self.cid:
+                name = c['properties'][self.cid]
+            else:
+                name = ""
+            results.loc[idx, 'name'] = name
+            if verbose:
+                print(end+name, end="")
+                end = ", "
+                
+            try:
+                clips = self.clip_all_rasters(idx) # function calls rv.validate()
+            except ValueError as e:
+                results.loc[idx, 'error'] = 'catchment out of bounds'
+            else:
+                if 'quartz' in clips.keys():
+                    clips, Qpc = eliminate_quartzfree(clips, verbose=False, Qpc=True)
+                    results.loc[idx, 'qtz_pc'] = np.round(100-Qpc,1)
+                topostats, summary = get_topostats(clips, bins=bins, centroid='from_clipped') # accepts iterable as bins
+                
+                results.loc[idx, 'area'] = summary['areakm2']
+                results.loc[idx, 'relief'] = np.nanmax(clips['elevation'])-np.nanmin(clips['elevation'])
+                if 'shielding' in clips.keys():
+                    results.loc[idx, 'mean_sf'] = np.nanmean(clips['shielding'])
+                results.loc[idx, 'centr_lat'] = summary['lat']
+                results.loc[idx, 'centr_long'] = summary['long']
+                results.loc[idx, 'mean_elev'] = np.nanmean(clips['elevation'])
+        
+        if verbose:
+            print(" finished.")
+        
+        results = results.sort_values(by=['name'], ignore_index=True)
+        
+        return results
+    
     
     def __repr__(self):
         s = []
         if self.elevation or self.shielding or self.quartz:
             s += ["---------------"]
             s += ["Raster data:\n"]
         if self.elevation:
```

### Comparing `riversand-1.2.0/riversand/params.py` & `riversand-1.2.1/riversand/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 *******************************************************************************
 
 """
 
 import os
-out_path = './plots'
+out_path = 'plots'
 if not os.path.exists(out_path):
     os.makedirs(out_path)
 
 
 #url = "https://hess.ess.washington.edu/cgi-bin/matweb"
 url = "http://stoneage.hzdr.de/cgi/matweb"
```

### Comparing `riversand-1.2.0/riversand/plot.py` & `riversand-1.2.1/riversand/plot.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/riversand/utils.py` & `riversand-1.2.1/riversand/utils.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/riversand/xml.py` & `riversand-1.2.1/riversand/xml.py`

 * *Files identical despite different names*

### Comparing `riversand-1.2.0/riversand.egg-info/PKG-INFO` & `riversand-1.2.1/riversand.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riversand
-Version: 1.2.0
+Version: 1.2.1
 Summary: Catchmentwide erosion rate calculator
 Home-page: https://github.com/kstueb/riversand
 Author: Konstanze Stuebner
 Author-email: kstueb@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `riversand-1.2.0/setup.py` & `riversand-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from distutils.core import setup   
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()   
 setup(                                
    name = 'riversand',
-   version = '1.2.0',
+   version = '1.2.1',
    packages = ['riversand'],
    author = 'Konstanze Stuebner',
    author_email = 'kstueb@gmail.com',
    url = 'https://github.com/kstueb/riversand',
    description = 'Catchmentwide erosion rate calculator',
    classifiers = ["Programming Language :: Python",
                   "Programming Language :: Python :: 3",
```

