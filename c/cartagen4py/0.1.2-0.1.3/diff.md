# Comparing `tmp/cartagen4py-0.1.2.tar.gz` & `tmp/cartagen4py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartagen4py-0.1.2.tar", last modified: Mon Feb 27 10:15:01 2023, max compression
+gzip compressed data, was "cartagen4py-0.1.3.tar", last modified: Fri May 12 08:29:32 2023, max compression
```

## Comparing `cartagen4py-0.1.2.tar` & `cartagen4py-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)    26526 2023-02-21 11:16:18.000000 cartagen4py-0.1.2/LICENSE
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)      809 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/PKG-INFO
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)      229 2023-02-24 11:02:28.000000 cartagen4py-0.1.2/README.md
-drwxrwxr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/cartagen4py/
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       36 2023-02-27 09:51:31.000000 cartagen4py-0.1.2/cartagen4py/__init__.py
-drwxrwxr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/cartagen4py/algorithms/
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       46 2023-02-24 11:36:50.000000 cartagen4py-0.1.2/cartagen4py/algorithms/__init__.py
-drwxrwxr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/cartagen4py/algorithms/buildings/
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       29 2023-02-24 11:34:26.000000 cartagen4py-0.1.2/cartagen4py/algorithms/buildings/__init__.py
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)    15181 2023-02-27 10:13:34.000000 cartagen4py-0.1.2/cartagen4py/algorithms/buildings/squaring.py
-drwxrwxr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/cartagen4py.egg-info/
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)      809 2023-02-27 10:15:01.000000 cartagen4py-0.1.2/cartagen4py.egg-info/PKG-INFO
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)      349 2023-02-27 10:15:01.000000 cartagen4py-0.1.2/cartagen4py.egg-info/SOURCES.txt
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)        1 2023-02-27 10:15:01.000000 cartagen4py-0.1.2/cartagen4py.egg-info/dependency_links.txt
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       24 2023-02-27 10:15:01.000000 cartagen4py-0.1.2/cartagen4py.egg-info/requires.txt
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       12 2023-02-27 10:15:01.000000 cartagen4py-0.1.2/cartagen4py.egg-info/top_level.txt
--rw-rw-r--   0 justinberli  (1000) justinberli  (1000)       38 2023-02-27 10:15:01.596484 cartagen4py-0.1.2/setup.cfg
--rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     1666 2023-02-27 10:14:53.000000 cartagen4py-0.1.2/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.3/README.md
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:29:32.092576 cartagen4py-0.1.3/cartagen4py/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-04-21 09:00:14.000000 cartagen4py-0.1.3/cartagen4py/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/cartagen4py/algorithms/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       68 2023-04-21 08:51:33.000000 cartagen4py-0.1.3/cartagen4py/algorithms/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      118 2023-03-30 13:41:05.000000 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4454 2023-03-30 13:45:12.000000 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/amalgamation.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7432 2023-03-30 13:44:15.000000 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/random_displacement.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7988 2023-04-21 08:51:00.000000 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14749 2023-05-10 10:01:58.000000 cartagen4py-0.1.3/cartagen4py/algorithms/buildings/squaring.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/cartagen4py.egg-info/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-12 08:29:32.000000 cartagen4py-0.1.3/cartagen4py.egg-info/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      497 2023-05-12 08:29:32.000000 cartagen4py-0.1.3/cartagen4py.egg-info/SOURCES.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-12 08:29:32.000000 cartagen4py-0.1.3/cartagen4py.egg-info/dependency_links.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-12 08:29:32.000000 cartagen4py-0.1.3/cartagen4py.egg-info/requires.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-12 08:29:32.000000 cartagen4py-0.1.3/cartagen4py.egg-info/top_level.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-12 08:29:32.096577 cartagen4py-0.1.3/setup.cfg
+-rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     1683 2023-05-12 08:28:23.000000 cartagen4py-0.1.3/setup.py
```

### Comparing `cartagen4py-0.1.2/PKG-INFO` & `cartagen4py-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
-Author: Guillaume Touya
+Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
-License: GPLv3
+License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
 Platform: Mac OSX
 Platform: Windows
 Platform: Unix
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cartagen4py-0.1.2/cartagen4py/algorithms/buildings/squaring.py` & `cartagen4py-0.1.3/cartagen4py/algorithms/buildings/squaring.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,20 +163,26 @@
         #S = np.zeros(2 * nb_points + len(self.indicesRight) + len(self.indicesFlat) + len(self.indicesHrObt) + len(self.indicesHrAig))
         for i, p in enumerate(points):
             S[2*i] = p[0]
             S[2*i+1] = p[1]
         offset = 2 * nb_points
         for i, t in enumerate(self.indicesRight):
             v1, v2 = self.__get_vecs_around(t, points)
-            d = v1.dot(v2) 
+            d = v1.dot(v2)
+            # print(v1)
+            # print(v2)
+            # print(d)
             S[offset + i] = d
         offset = 2 * nb_points + len(self.indicesRight)
         for i, t in enumerate(self.indicesFlat):
             v1, v2 = self.__get_vecs_around(t, points)
-            d = np.cross(v1, v2).item(0) 
+            d = np.cross(v1, v2).item(0)
+            print(v1)
+            print(v2)
+            print(d)
             S[offset + i] = d
         offset = 2 * nb_points + len(self.indicesRight) + len(self.indicesFlat)
         #for i, t in enumerate(self.indicesHrAig):
         #    v1, v2 = self.__get_vecs_around(t, points)
         #    d = v1.dot(v2) 
         #    S[offset + i] = d
         #offset = 2 * nb_points + len(self.indicesRight) + len(self.indicesFlat) + len(self.indicesHrAig)
@@ -194,15 +200,14 @@
         #nb_half_rights = len(self.indicesHrAig) + len(self.indicesHrObt)
         wfix = np.full(2*nb_points, self.poidsPtfFixe)
         wRight = np.full(nb_rights, self.poids90)
         wFlat = np.full(nb_flats, self.poids0)
         #wHr = np.full(nb_half_rights, self.poids45)
         self.P = np.diag(np.concatenate((wfix, wRight, wFlat)))
 
-
     ## new vectors
     def __partial_derivatives_dotp(self, points, indices):
         nb_points = len(points)
         nb_indices = len(indices)
         m = np.zeros((nb_indices, 2*nb_points))
         for i, t in enumerate(indices):
             idx_prec, idx, idx_suiv = t[0], t[1], t[2]
@@ -242,15 +247,15 @@
             m[i][2*idx] = dfx
             m[i][2*idx + 1] = dfy
             # df en Xi+1, Yi+1
             dfx = -p[1] + pr[1]
             dfy = p[0] - pr[0]
             m[i][2*idx_suiv] = dfx
             m[i][2*idx_suiv + 1] = dfy
-        return 
+        return m
 
 
     def __get_A(self, points):
         nb_points = len(points) #- 1
         id = np.identity(2 * nb_points)
         partialR = self.__partial_derivatives_dotp(points, self.indicesRight)
         partialCross = self.__partial_derivatives_cross(points, self.indicesFlat)
@@ -322,28 +327,8 @@
             #print(index_of_lines)
             for idx_l in index_of_lines:
                 r = self.__get_rank_point_in_shape(idx_p, idx_l)
                 #print(idx_l, r, new_points[idx_p])
                 new_s[idx_l][r] = np.array(new_points[idx_p])
                 if r == 0 and is_poly:
                     new_s[idx_l][-1] = np.array(new_points[idx_p])
-        return new_s
-
-
-
-# if __name__ == '__main__':
-#     from shapely.wkt import loads
-#     from shapely.geometry import Polygon, LineString
-#     import geopandas
-
-
-#     zipfile = "zip:///home/justinberli/Documents/Python Packages/CartAGen4Py/CartAGen4Py/data/test_squaring.zip"
-#     df = geopandas.read_file(zipfile)
-#     polygons = df.geometry
-
-#     #lines = [loads(wkt)]
-#     sq = Squarer(pfixe=5)
-#     with np.printoptions(precision=3, suppress=True):
-#         points = sq.square(polygons)
-
-#     new_s = sq.get_shapes_from_new_points(polygons, points)
-#     print(new_s)
+        return new_s
```

### Comparing `cartagen4py-0.1.2/cartagen4py.egg-info/PKG-INFO` & `cartagen4py-0.1.3/cartagen4py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
-Author: Guillaume Touya
+Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
-License: GPLv3
+License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
 Platform: Mac OSX
 Platform: Windows
 Platform: Unix
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cartagen4py-0.1.2/setup.py` & `cartagen4py-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 if sys.version_info[:2] < (3, 8):
     error = ('cartagen4py requires Python 3.8 or later (%d.%d detected).' % sys.version_info[:2])
     sys.stderr.write(error + "\n")
     sys.exit(1)
 
 # General informations
 name = 'cartagen4py'
-version = '0.1.2'
+version = '0.1.3'
 description = 'Python package to generalise geographic objects for cartographic purposes'
 url = 'https://github.com/LostInZoom/cartagen4py'
-author = 'Guillaume Touya'
+author = 'Guillaume Touya, Justin Berli'
 author_email = 'guillaume.touya@ign.fr'
-lic = 'GPLv3'
+lic = 'CeCILL-C'
 packages = [
     'cartagen4py',
     'cartagen4py.algorithms',
     'cartagen4py.algorithms.buildings'
 ]
 
 # Requirements and dependencies
```

