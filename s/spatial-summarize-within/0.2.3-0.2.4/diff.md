# Comparing `tmp/spatial_summarize_within-0.2.3.tar.gz` & `tmp/spatial_summarize_within-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.2.3.tar", last modified: Fri May 12 05:31:49 2023, max compression
+gzip compressed data, was "spatial_summarize_within-0.2.4.tar", last modified: Fri May 12 18:09:51 2023, max compression
```

## Comparing `spatial_summarize_within-0.2.3.tar` & `spatial_summarize_within-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 05:31:49.747791 spatial_summarize_within-0.2.3/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.3/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 05:31:49.747675 spatial_summarize_within-0.2.3/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.3/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-12 05:31:49.747825 spatial_summarize_within-0.2.3/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-12 05:31:38.000000 spatial_summarize_within-0.2.3/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 05:31:49.746883 spatial_summarize_within-0.2.3/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.3/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.3/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2446 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.3/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.3/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.3/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 05:31:49.747508 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 05:31:49.000000 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-12 05:31:49.000000 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-12 05:31:49.000000 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-12 05:31:49.000000 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-12 05:31:49.000000 spatial_summarize_within-0.2.3/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.457204 spatial_summarize_within-0.2.4/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.2.4/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 18:09:51.457085 spatial_summarize_within-0.2.4/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2170 2023-05-08 23:11:41.000000 spatial_summarize_within-0.2.4/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-12 18:09:51.457240 spatial_summarize_within-0.2.4/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-12 18:09:42.000000 spatial_summarize_within-0.2.4/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.456228 spatial_summarize_within-0.2.4/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2447 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2455 2023-05-12 06:16:37.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2448 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2429 2023-05-12 05:30:36.000000 spatial_summarize_within-0.2.4/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-12 18:09:51.456930 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-12 18:09:51.000000 spatial_summarize_within-0.2.4/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.2.3/LICENSE` & `spatial_summarize_within-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.3/README.md` & `spatial_summarize_within-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.3/spatial_summarize_within/max_within.py` & `spatial_summarize_within-0.2.4/spatial_summarize_within/max_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.3/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-0.2.4/spatial_summarize_within/mean_within.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         # Calculate the area of each polygon in intersect dataframe
         temp_intersect["intersect_area"] = temp_intersect.area
         # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
         temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
         # Calculate the weighted mean
         columns = columns
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"])
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results and calculate the mean
         temp_result = temp_intersect.groupby(key).mean(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
```

### Comparing `spatial_summarize_within-0.2.3/spatial_summarize_within/min_within.py` & `spatial_summarize_within-0.2.4/spatial_summarize_within/min_within.py`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-0.2.3/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-0.2.4/spatial_summarize_within/sum_within.py`

 * *Files identical despite different names*

