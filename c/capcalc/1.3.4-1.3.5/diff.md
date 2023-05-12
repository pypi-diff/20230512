# Comparing `tmp/capcalc-1.3.4.tar.gz` & `tmp/capcalc-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/capcalc-1.3.4.tar", last modified: Wed Jan 11 00:20:02 2023, max compression
+gzip compressed data, was "dist/capcalc-1.3.5.tar", last modified: Wed Jan 11 20:07:34 2023, max compression
```

## Comparing `capcalc-1.3.4.tar` & `capcalc-1.3.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:20:02.000000 capcalc-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-11 00:19:53.000000 capcalc-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-01-11 00:20:02.000000 capcalc-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-01-11 00:19:53.000000 capcalc-1.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    61945 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51125 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    62615 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/miscmath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22542 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/parser_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/behavioralprediction
--rwxr-xr-x   0 runner    (1001) docker     (123)     2414 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/capcalc_dispatcher
--rwxr-xr-x   0 runner    (1001) docker     (123)    44425 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/capfromtcs
--rwxr-xr-x   0 runner    (1001) docker     (123)     5113 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/clustercomp
--rwxr-xr-x   0 runner    (1001) docker     (123)    27685 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/clusternifti
--rwxr-xr-x   0 runner    (1001) docker     (123)    11941 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/clustersort
--rwxr-xr-x   0 runner    (1001) docker     (123)     4492 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/fitglm
--rwxr-xr-x   0 runner    (1001) docker     (123)     3974 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/kmeans
--rwxr-xr-x   0 runner    (1001) docker     (123)     2950 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/maptoroi
--rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/normtcs
--rwxr-xr-x   0 runner    (1001) docker     (123)     5771 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/roidecompose
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/statefiltertest
--rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/statematch
--rwxr-xr-x   0 runner    (1001) docker     (123)     7333 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/statlasgen
--rwxr-xr-x   0 runner    (1001) docker     (123)    22767 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/supercluster
--rwxr-xr-x   0 runner    (1001) docker     (123)     2774 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/tcfrom3col
--rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/scripts/updatemodel
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    27012 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-01-11 00:19:53.000000 capcalc-1.3.4/capcalc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-11 00:20:02.000000 capcalc-1.3.4/capcalc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-11 00:19:53.000000 capcalc-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-11 00:20:02.000000 capcalc-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-01-11 00:19:53.000000 capcalc-1.3.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-01-11 00:19:53.000000 capcalc-1.3.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:07:34.000000 capcalc-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-11 20:07:26.000000 capcalc-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-01-11 20:07:34.000000 capcalc-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-01-11 20:07:26.000000 capcalc-1.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61945 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51125 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62615 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/miscmath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22542 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/parser_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/behavioralprediction
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2414 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/capcalc_dispatcher
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42771 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/capfromtcs
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5113 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/clustercomp
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27685 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/clusternifti
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11941 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/clustersort
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4492 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/fitglm
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3974 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/kmeans
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2950 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/maptoroi
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2465 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/normtcs
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5771 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/roidecompose
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/statefiltertest
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/statematch
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7333 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/statlasgen
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22767 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/supercluster
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2774 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/tcfrom3col
+-rwxr-xr-x   0 runner    (1001) docker     (123)      799 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/scripts/updatemodel
+-rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27012 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-01-11 20:07:26.000000 capcalc-1.3.5/capcalc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-01-11 20:07:34.000000 capcalc-1.3.5/capcalc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-11 20:07:26.000000 capcalc-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-11 20:07:34.000000 capcalc-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-01-11 20:07:26.000000 capcalc-1.3.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-01-11 20:07:26.000000 capcalc-1.3.5/versioneer.py
```

### Comparing `capcalc-1.3.4/PKG-INFO` & `capcalc-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capcalc
-Version: 1.3.4
+Version: 1.3.5
 Summary: Tools for performing coactivation pattern analysis on fMRI data.
 Home-page: https://github.com/bbfrederick/capcalc
 Author: Blaise Frederick
 Author-email: bbfrederick@mclean.harvard.edu
 License: Apache Software License
 Description: Capcalc
         =======
```

### Comparing `capcalc-1.3.4/README.rst` & `capcalc-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/filter.py` & `capcalc-1.3.5/capcalc/filter.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/fit.py` & `capcalc-1.3.5/capcalc/fit.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/io.py` & `capcalc-1.3.5/capcalc/io.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/miscmath.py` & `capcalc-1.3.5/capcalc/miscmath.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/parser_funcs.py` & `capcalc-1.3.5/capcalc/parser_funcs.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/behavioralprediction` & `capcalc-1.3.5/capcalc/scripts/behavioralprediction`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/capcalc_dispatcher` & `capcalc-1.3.5/capcalc/scripts/capcalc_dispatcher`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/capfromtcs` & `capcalc-1.3.5/capcalc/scripts/capfromtcs`

 * *Files 5% similar despite different names*

```diff
@@ -349,15 +349,15 @@
     elif o == "--ppnorm":
         timenormmethod = "ppnorm"
         if verbose:
             print("will do p-p normalization")
     elif o == "--modelroot":
         trainedmodelroot = a
         if verbose:
-            print("will read trained models from", trainedmodelroot, "_*.joblib")
+            print("will read trained models from " + trainedmodelroot + "_*.joblib")
     elif o == "--initialcenters":
         initialcenters = a
         if verbose:
             print("will read in the initial cluster centers from", initialcenters)
     elif o == "--minhold":
         minholdlength = int(a)
         if verbose:
@@ -862,15 +862,15 @@
     for segment in range(numsegs):
         thesestatelabels = thestatelabels[segment * segsize : (segment + 1) * segsize]
 
         outputaffine = np.eye(4)
         rawtransmat, thestats, lenlist = capcalc_utils.statestats(
             thesestatelabels, n_clusters, 0, minout=minoutlength, minhold=minholdlength
         )
-        allrawtransmats.append(rawtransmat)
+        allrawtransmats.append(rawtransmat * 1.0)
         allstatestats.append(thestats)
         for i in range(n_clusters):
             alllenlists[i] += lenlist[i]
         normtransmat, offdiagtransmat = capcalc_utils.calcmats(rawtransmat, n_clusters)
         init_img = nib.Nifti1Image(normtransmat, outputaffine)
         init_hdr = init_img.header
         init_sizes = init_hdr["pixdim"]
@@ -978,84 +978,49 @@
             # ccalc_io.writenpvecs(thesilclusterstats[segment, :, :],
             #             outfilename + '_seg_' + str(segment).zfill(4) + '_silhouetteclusterstats.txt')
 
         for state in range(n_clusters):
             if thestats[state, 2] > 0:
                 silinfo[state].append(thesilclusterstats[segment, 0, state])
 
-    #
-    # There should be a parallel system here to construct subsegment specific statistics
-    #
-    """
-    for key in groups:
-        groups[key]["meaninstate"] = np.zeros(
-            (n_clusters, groups[key]["seglen"][0]), dtype="float"
-            allstatestats = []
-        groups[key]["alllenlists"] = []
-        for i in range(n_clusters):
-            groups[key]["alllenlists"].append([])
-        )
-        groups[key]["stdinstate"] = np.zeros((n_clusters, groups[key]["seglen"][0]), dtype="float")
-
-        for segment in range(numsegs):
-            thesestatelabels = thestatelabels[segment * segsize : (segment + 1) * segsize]
-    
-            outputaffine = np.eye(4)
-            rawtransmat, thestats, lenlist = capcalc_utils.statestats(
-                thesestatelabels, n_clusters, 0, minout=minoutlength, minhold=minholdlength
-            )
-            allstatestats.append(thestats)
-            for i in range(n_clusters):
-                alllenlists[i] += lenlist[i]
-            normtransmat = 1.0 * rawtransmat
-            for i in range(n_clusters):
-                if np.sum(rawtransmat[i, :]) > 0.0:
-                    normtransmat[i, :] /= np.sum(rawtransmat[i, :])
-            offdiagtransmat = 1.0 * rawtransmat
-            for i in range(n_clusters):
-                offdiagtransmat[i, i] = 0.0
-                if np.sum(offdiagtransmat[i, :]) > 0.0:
-                    offdiagtransmat[i, :] /= np.sum(offdiagtransmat[i, :])
-            init_img = nib.Nifti1Image(normtransmat, outputaffine)
-            init_hdr = init_img.header
-            init_sizes = init_hdr["pixdim"]
-            ccalc_io.savetonifti(
-                np.transpose(rawtransmat),
-                init_hdr,
-                outfilename + "_seg_" + str(segment).zfill(4) + "_rawtransmat",
-            )
-            ccalc_io.savetonifti(
-                np.transpose(normtransmat),
-                init_hdr,
-                outfilename + "_seg_" + str(segment).zfill(4) + "_normtransmat",
-            )
-            ccalc_io.savetonifti(
-                np.transpose(offdiagtransmat),
-                init_hdr,
-                outfilename + "_seg_" + str(segment).zfill(4) + "_offdiagtransmat",
-            )
-        """
-
     # now generate some summary information
     overallstatestats = []
+    thetimestats = []
+    alllens = 0
+    for i in range(n_clusters):
+        alllens += np.sum(np.asarray(alllenlists[i], dtype="float"))
+
     for i in range(n_clusters):
         lenarray = np.asarray(alllenlists[i], dtype="float")
         if len(lenarray) > 2:
             overallstatestats.append(
                 [
-                    100.0 * np.sum(lenarray) / len(thestates),
+                    100.0 * np.sum(lenarray) / alllens,
                     len(lenarray),
                     np.sum(lenarray),
                     np.min(lenarray),
                     np.max(lenarray),
                     np.mean(lenarray),
                     np.median(lenarray),
                     np.std(lenarray),
                 ]
             )
+            thetimestats.append(
+                [
+                    100.0 * np.sum(lenarray) / alllens,
+                    sampletime * len(lenarray),
+                    sampletime * np.sum(lenarray),
+                    sampletime * np.min(lenarray),
+                    sampletime * np.max(lenarray),
+                    sampletime * np.mean(lenarray),
+                    sampletime * np.median(lenarray),
+                    sampletime * np.std(lenarray),
+                ]
+            )
+
     cols = [
         "% TRs in state",
         "Number of runs in state",
         "Total TRs in state",
         "Min run (TRs)",
         "Max run (TRs)",
         "Mean run (TRs)",
@@ -1063,16 +1028,15 @@
         "StdDev run (TRs)",
     ]
     df = pd.DataFrame(data=overallstatestats, columns=cols)
     df.to_csv(
         outfilename + "_overall_statestats.csv",
         index=False,
     )
-    thetimestats = 1.0 * overallstatestats
-    thetimestats[:, 2:] *= sampletime
+
     cols = [
         "% Seconds in state",
         "Number of runs in state",
         "Total seconds in state",
         "Min run (sec)",
         "Max run (sec)",
         "Mean run (sec)",
@@ -1080,17 +1044,17 @@
         "StdDev run (sec)",
     ]
     df = pd.DataFrame(data=thetimestats, columns=cols)
     df.to_csv(
         outfilename + "_overall_statetimestats.csv",
         index=False,
     )
-    overallrawtransmat = rawtransmat[0] * 0.0
+    overallrawtransmat = allrawtransmats[0] * 0.0
     for segment in range(numsegs):
-        overallrawtransmat += rawtransmat[segment]
+        overallrawtransmat += allrawtransmats[segment]
     overallnormtransmat, overalloffdiagtransmat = capcalc_utils.calcmats(
         overallrawtransmat, n_clusters
     )
     init_img = nib.Nifti1Image(overallnormtransmat, outputaffine)
     init_hdr = init_img.header
     init_sizes = init_hdr["pixdim"]
     ccalc_io.savetonifti(
```

### Comparing `capcalc-1.3.4/capcalc/scripts/clustercomp` & `capcalc-1.3.5/capcalc/scripts/clustercomp`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/clusternifti` & `capcalc-1.3.5/capcalc/scripts/clusternifti`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/clustersort` & `capcalc-1.3.5/capcalc/scripts/clustersort`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/fitglm` & `capcalc-1.3.5/capcalc/scripts/fitglm`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/kmeans` & `capcalc-1.3.5/capcalc/scripts/kmeans`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/maptoroi` & `capcalc-1.3.5/capcalc/scripts/maptoroi`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/normtcs` & `capcalc-1.3.5/capcalc/scripts/normtcs`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/roidecompose` & `capcalc-1.3.5/capcalc/scripts/roidecompose`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/statefiltertest` & `capcalc-1.3.5/capcalc/scripts/statefiltertest`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/statematch` & `capcalc-1.3.5/capcalc/scripts/statematch`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/statlasgen` & `capcalc-1.3.5/capcalc/scripts/statlasgen`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/supercluster` & `capcalc-1.3.5/capcalc/scripts/supercluster`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/tcfrom3col` & `capcalc-1.3.5/capcalc/scripts/tcfrom3col`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/scripts/updatemodel` & `capcalc-1.3.5/capcalc/scripts/updatemodel`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/stats.py` & `capcalc-1.3.5/capcalc/stats.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/util.py` & `capcalc-1.3.5/capcalc/util.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc/utils.py` & `capcalc-1.3.5/capcalc/utils.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/capcalc.egg-info/PKG-INFO` & `capcalc-1.3.5/capcalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capcalc
-Version: 1.3.4
+Version: 1.3.5
 Summary: Tools for performing coactivation pattern analysis on fMRI data.
 Home-page: https://github.com/bbfrederick/capcalc
 Author: Blaise Frederick
 Author-email: bbfrederick@mclean.harvard.edu
 License: Apache Software License
 Description: Capcalc
         =======
```

### Comparing `capcalc-1.3.4/capcalc.egg-info/SOURCES.txt` & `capcalc-1.3.5/capcalc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/setup.py` & `capcalc-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `capcalc-1.3.4/versioneer.py` & `capcalc-1.3.5/versioneer.py`

 * *Files identical despite different names*

