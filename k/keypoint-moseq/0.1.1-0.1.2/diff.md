# Comparing `tmp/keypoint-moseq-0.1.1.tar.gz` & `tmp/keypoint-moseq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keypoint-moseq-0.1.1.tar", last modified: Thu May 11 22:14:11 2023, max compression
+gzip compressed data, was "keypoint-moseq-0.1.2.tar", last modified: Fri May 12 21:11:44 2023, max compression
```

## Comparing `keypoint-moseq-0.1.1.tar` & `keypoint-moseq-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.779245 keypoint-moseq-0.1.1/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.1/LICENSE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.1/NOTICE.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-11 22:14:11.779396 keypoint-moseq-0.1.1/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-11 19:57:02.000000 keypoint-moseq-0.1.1/README.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.780825 keypoint-moseq-0.1.1/keypoint_moseq/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-11 22:14:11.780952 keypoint-moseq-0.1.1/keypoint_moseq/_version.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.1/keypoint_moseq/analysis.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.1/keypoint_moseq/calibration.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/fitting.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-11 21:25:41.000000 keypoint-moseq-0.1.1/keypoint_moseq/io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.1/keypoint_moseq/util.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    68316 2023-05-11 21:54:06.000000 keypoint-moseq-0.1.1/keypoint_moseq/viz.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-11 22:14:11.778779 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      152 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-11 22:14:11.000000 keypoint-moseq-0.1.1/keypoint_moseq.egg-info/top_level.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      733 2023-05-11 22:14:11.780345 keypoint-moseq-0.1.1/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.1/setup.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.1/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.508317 keypoint-moseq-0.1.2/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     8355 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.2/LICENSE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      725 2023-04-19 14:03:24.000000 keypoint-moseq-0.1.2/NOTICE.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-12 21:11:44.508450 keypoint-moseq-0.1.2/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1426 2023-05-11 19:57:02.000000 keypoint-moseq-0.1.2/README.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.509549 keypoint-moseq-0.1.2/keypoint_moseq/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1007 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2023-05-12 21:11:44.509630 keypoint-moseq-0.1.2/keypoint_moseq/_version.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    28353 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.2/keypoint_moseq/analysis.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17681 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.2/keypoint_moseq/calibration.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17318 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/fitting.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    41843 2023-05-11 21:25:41.000000 keypoint-moseq-0.1.2/keypoint_moseq/io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    27401 2023-05-11 19:55:30.000000 keypoint-moseq-0.1.2/keypoint_moseq/util.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    68259 2023-05-12 18:45:18.000000 keypoint-moseq-0.1.2/keypoint_moseq/viz.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2023-05-12 21:11:44.507974 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      333 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      455 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      170 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       15 2023-05-12 21:11:44.000000 keypoint-moseq-0.1.2/keypoint_moseq.egg-info/top_level.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      752 2023-05-12 21:11:44.509184 keypoint-moseq-0.1.2/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      246 2023-05-04 21:42:40.000000 keypoint-moseq-0.1.2/setup.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83607 2023-05-04 15:16:47.000000 keypoint-moseq-0.1.2/versioneer.py
```

### Comparing `keypoint-moseq-0.1.1/LICENSE.md` & `keypoint-moseq-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/NOTICE.md` & `keypoint-moseq-0.1.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/README.md` & `keypoint-moseq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/__init__.py` & `keypoint-moseq-0.1.2/keypoint_moseq/__init__.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/analysis.py` & `keypoint-moseq-0.1.2/keypoint_moseq/analysis.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/calibration.py` & `keypoint-moseq-0.1.2/keypoint_moseq/calibration.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/fitting.py` & `keypoint-moseq-0.1.2/keypoint_moseq/fitting.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/io.py` & `keypoint-moseq-0.1.2/keypoint_moseq/io.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/util.py` & `keypoint-moseq-0.1.2/keypoint_moseq/util.py`

 * *Files identical despite different names*

### Comparing `keypoint-moseq-0.1.1/keypoint_moseq/viz.py` & `keypoint-moseq-0.1.2/keypoint_moseq/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,29 +255,29 @@
     if results is None:
         results = load_results(path=path, name=name, project_dir=project_dir)
 
     syllable_key = 'syllables' if not use_reindexed else 'syllables_reindexed'
     syllables = {k:res[syllable_key] for k,res in results.items()}
     frequencies = get_frequencies(syllables)
     frequencies = frequencies[frequencies>min_frequency]
-    xmax = max(minlength, len(frequencies))
+    xmax = max(minlength, np.max(np.nonzero(frequencies>min_frequency)[0])+1)
 
     fig, ax = plt.subplots()
     ax.bar(range(len(frequencies)),frequencies,width=1)
     ax.set_ylabel('probability')
     ax.set_xlabel('syllable rank')
     ax.set_xlim(-1,xmax+1)
     ax.set_title('Frequency distribution')
     ax.set_yticks([])
     return fig, ax
 
 
 def plot_duration_distribution(results=None, path=None, project_dir=None, 
-                               name=None, use_reindexed=True, lim=None,
-                               num_bins=30, fps=None, show_median=True):
+                               name=None, lim=None, num_bins=30, fps=None, 
+                               show_median=True):
     """
     Plot a histogram showing the frequency of each syllable.
     
     Caller must provide a results dictionary, a path to a results .h5,
     or a project directory and model name, in which case the results are
     loaded from `{project_dir}/{name}/results.h5`.
 
@@ -318,17 +318,16 @@
         Figure containing the histogram.
     
     ax : matplotlib.axes.Axes
         Axes containing the histogram.
     """
     if results is None:
         results = load_results(path=path, name=name, project_dir=project_dir)
-
-    syllable_key = 'syllables' if not use_reindexed else 'syllables_reindexed'
-    syllables = {k:res[syllable_key] for k,res in results.items()}
+        
+    syllables = {k:res['syllables'] for k,res in results.items()}
     durations = get_durations(syllables)
     
     if lim is None:
         lim = int(np.percentile(durations, 95))
     binsize = max(int(np.floor(lim/num_bins)),1)
 
     if fps is not None:
```

### Comparing `keypoint-moseq-0.1.1/setup.cfg` & `keypoint-moseq-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 	pyyaml
 	vidio
 	holoviews[recommended]
 	bokeh
 	pandas
 	tables
 	tabulate
+	jaxtyping==0.2.14
 	jax-moseq==0.0.3
 
 [options.package_data]
 * = *.md
 
 [versioneer]
 VCS = git
```

### Comparing `keypoint-moseq-0.1.1/versioneer.py` & `keypoint-moseq-0.1.2/versioneer.py`

 * *Files identical despite different names*

