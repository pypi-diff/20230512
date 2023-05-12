# Comparing `tmp/tpfi-1.0.5.tar.gz` & `tmp/tpfi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpfi-1.0.5.tar", max compression
+gzip compressed data, was "tpfi-1.0.6.tar", max compression
```

## Comparing `tpfi-1.0.5.tar` & `tpfi-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-05-11 02:14:49.669951 tpfi-1.0.5/LICENSE
--rw-r--r--   0        0        0     2271 2023-05-11 02:14:49.925952 tpfi-1.0.5/README.md
--rw-r--r--   0        0        0      563 2023-05-11 02:14:49.677951 tpfi-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      154 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/__init__.py
--rw-r--r--   0        0        0    15258 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/tpfi.py
--rw-r--r--   0        0        0     5333 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/utils.py
--rw-r--r--   0        0        0       22 2023-05-11 02:14:49.677951 tpfi-1.0.5/src/tpfi/version.py
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 tpfi-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-12 04:17:51.238296 tpfi-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2271 2023-05-12 04:17:51.594298 tpfi-1.0.6/README.md
+-rw-r--r--   0        0        0      563 2023-05-12 04:17:51.246296 tpfi-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/__init__.py
+-rw-r--r--   0        0        0    15241 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/tpfi.py
+-rw-r--r--   0        0        0     5333 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/utils.py
+-rw-r--r--   0        0        0       22 2023-05-12 04:17:51.246296 tpfi-1.0.6/src/tpfi/version.py
+-rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 tpfi-1.0.6/PKG-INFO
```

### Comparing `tpfi-1.0.5/LICENSE` & `tpfi-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.5/README.md` & `tpfi-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.5/pyproject.toml` & `tpfi-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpfi"
-version = "1.0.5"
+version = "1.0.6"
 description = "Plot identification charts for Kepler, K2 and TESS."
 authors = ["Keyu Xing <kyxing@mail.bnu.edu.cn>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/keyuxing/tpfi"
 repository = "https://github.com/keyuxing/tpfi"
```

### Comparing `tpfi-1.0.5/src/tpfi/tpfi.py` & `tpfi-1.0.6/src/tpfi/tpfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,14 @@
     ax_tpf.invert_xaxis()
 
     if r is None:
         at = AnchoredText("No Gaia DR3 Data", frameon=False, loc="upper left", prop=dict(size=13))
         ax_tpf.add_artist(at)
     else:
         target_gaia_id = r[0]["source_id"]
-        print(r)
         r.sort("phot_g_mean_mag")
         this = np.nonzero(r["source_id"] == target_gaia_id)[0][0]
         magnitude_limit = max(r["phot_g_mean_mag"][0] + 3, mag_limit)
         r = r[r["phot_g_mean_mag"] < magnitude_limit][: max(this + 50, 300)]
 
         qr = QTable([r["ra"].filled(), r["dec"].filled(), r["pmra"].filled(0), r["pmdec"].filled(0)])
         coords_gaia = SkyCoord(
```

### Comparing `tpfi-1.0.5/src/tpfi/utils.py` & `tpfi-1.0.6/src/tpfi/utils.py`

 * *Files identical despite different names*

### Comparing `tpfi-1.0.5/PKG-INFO` & `tpfi-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpfi
-Version: 1.0.5
+Version: 1.0.6
 Summary: Plot identification charts for Kepler, K2 and TESS.
 Home-page: https://github.com/keyuxing/tpfi
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

