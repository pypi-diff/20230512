# Comparing `tmp/kerchunk-0.1.1.tar.gz` & `tmp/kerchunk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerchunk-0.1.1.tar", last modified: Mon Apr 17 13:29:33 2023, max compression
+gzip compressed data, was "kerchunk-0.1.2.tar", last modified: Fri May 12 19:38:58 2023, max compression
```

## Comparing `kerchunk-0.1.1.tar` & `kerchunk-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.971612 kerchunk-0.1.1/
--rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.1.1/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      155 2022-09-18 01:28:32.000000 kerchunk-0.1.1/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-04-17 13:29:33.971686 kerchunk-0.1.1/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.1.1/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.972353 kerchunk-0.1.1/kerchunk/
--rw-r--r--   0 mdurant    (502) staff       (20)      142 2022-09-18 01:28:32.000000 kerchunk-0.1.1/kerchunk/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-04-17 13:29:33.972405 kerchunk-0.1.1/kerchunk/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6203 2023-04-17 13:28:40.000000 kerchunk-0.1.1/kerchunk/codecs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    28247 2023-04-17 13:28:40.000000 kerchunk-0.1.1/kerchunk/combine.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8840 2023-03-13 19:21:13.000000 kerchunk-0.1.1/kerchunk/df.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8985 2022-10-31 16:19:59.000000 kerchunk-0.1.1/kerchunk/fits.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9429 2023-01-16 14:32:53.000000 kerchunk-0.1.1/kerchunk/grib2.py
--rw-r--r--   0 mdurant    (502) staff       (20)    22133 2023-04-12 17:06:54.000000 kerchunk-0.1.1/kerchunk/hdf.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9882 2022-12-09 18:27:45.000000 kerchunk-0.1.1/kerchunk/netCDF3.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3589 2023-03-13 14:06:07.000000 kerchunk-0.1.1/kerchunk/tiff.py
--rw-r--r--   0 mdurant    (502) staff       (20)    12231 2023-02-28 15:06:36.000000 kerchunk-0.1.1/kerchunk/utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)      963 2022-12-09 18:27:45.000000 kerchunk-0.1.1/kerchunk/zarr.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-17 13:29:33.971493 kerchunk-0.1.1/kerchunk.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      523 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      244 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/entry_points.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 14:47:57.000000 kerchunk-0.1.1/kerchunk.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        9 2023-04-17 13:29:33.000000 kerchunk-0.1.1/kerchunk.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.1.1/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      724 2023-04-17 13:29:33.972010 kerchunk-0.1.1/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     1247 2023-01-19 21:15:29.000000 kerchunk-0.1.1/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    70238 2022-09-18 01:28:32.000000 kerchunk-0.1.1/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-12 19:38:58.944133 kerchunk-0.1.2/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1063 2022-09-18 01:28:32.000000 kerchunk-0.1.2/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      155 2022-09-18 01:28:32.000000 kerchunk-0.1.2/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-05-12 19:38:58.944210 kerchunk-0.1.2/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     2433 2022-09-23 18:01:10.000000 kerchunk-0.1.2/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-12 19:38:58.944857 kerchunk-0.1.2/kerchunk/
+-rw-r--r--   0 mdurant    (502) staff       (20)      142 2022-09-18 01:28:32.000000 kerchunk-0.1.2/kerchunk/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-05-12 19:38:58.944947 kerchunk-0.1.2/kerchunk/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6203 2023-05-12 18:30:53.000000 kerchunk-0.1.2/kerchunk/codecs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    28916 2023-05-12 18:30:53.000000 kerchunk-0.1.2/kerchunk/combine.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9513 2023-05-12 19:34:47.000000 kerchunk-0.1.2/kerchunk/df.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8985 2022-10-31 16:19:59.000000 kerchunk-0.1.2/kerchunk/fits.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9429 2023-05-12 18:30:53.000000 kerchunk-0.1.2/kerchunk/grib2.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    22411 2023-05-12 19:38:16.000000 kerchunk-0.1.2/kerchunk/hdf.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9882 2022-12-09 18:27:45.000000 kerchunk-0.1.2/kerchunk/netCDF3.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3589 2023-03-13 14:06:07.000000 kerchunk-0.1.2/kerchunk/tiff.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    12231 2023-05-12 18:30:53.000000 kerchunk-0.1.2/kerchunk/utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      963 2022-12-09 18:27:45.000000 kerchunk-0.1.2/kerchunk/zarr.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-12 19:38:58.943975 kerchunk-0.1.2/kerchunk.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2883 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      523 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      244 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-21 14:47:57.000000 kerchunk-0.1.2/kerchunk.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      118 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        9 2023-05-12 19:38:58.000000 kerchunk-0.1.2/kerchunk.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       34 2022-09-18 01:28:32.000000 kerchunk-0.1.2/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      724 2023-05-12 19:38:58.944599 kerchunk-0.1.2/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     1247 2023-05-12 18:30:53.000000 kerchunk-0.1.2/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    70238 2022-09-18 01:28:32.000000 kerchunk-0.1.2/versioneer.py
```

### Comparing `kerchunk-0.1.1/LICENSE` & `kerchunk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/PKG-INFO` & `kerchunk-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Home-page: https://github.com/fsspec/kerchunk
 Author: Martin Durant
 Author-email: martin.durant@alumni.utoronto.ca
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kerchunk-0.1.1/README.md` & `kerchunk-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/codecs.py` & `kerchunk-0.1.2/kerchunk/codecs.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/combine.py` & `kerchunk-0.1.2/kerchunk/combine.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,18 @@
         Size below which binary blocks are included directly in the output
     :param preprocess: callable
         Acts on the references dict of all inputs before processing. See ``drop()``
         for an example.
     :param postprocess: callable
         Acts on the references dict before output.
         postprocess(dict)-> dict
-    :param validate_dataet: callable
-    :param validate_variable: callable
-    :param validate_chunk: callable
+    :param out: dict-like or None
+        This allows you to supply an fsspec.implementations.reference.LazyReferenceMapper
+        to write out parquet as the references get filled, or some other dictionary-like class
+        to customise how references get stored
     """
 
     def __init__(
         self,
         path,
         indicts=None,
         coo_map=None,
@@ -101,14 +102,15 @@
         identical_dims=None,
         target_options=None,
         remote_protocol=None,
         remote_options=None,
         inline_threshold=500,
         preprocess=None,
         postprocess=None,
+        out=None,
     ):
         self._fss = None
         self._paths = None
         self._indicts = indicts
         self.ds = None
         self.path = path
         if concat_dims is None:
@@ -134,15 +136,15 @@
         self.inline = inline_threshold
         self.cf_units = None
         self.identical_dims = identical_dims or []
         if set(self.coo_map).intersection(set(self.identical_dims)):
             raise ValueError("Values being mapped cannot also be identical")
         self.preprocess = preprocess
         self.postprocess = postprocess
-        self.out = {}
+        self.out = out or {}
         self.done = set()
 
     @property
     def fss(self):
         """filesystem instances being analysed, one per input dataset"""
         import collections.abc
 
@@ -157,16 +159,21 @@
                 for path in self.path:
                     self._paths.append(path.get("templates", {}).get("u", None))
             else:
                 self._paths = []
                 for of in fsspec.open_files(self.path, **self.target_options):
                     self._paths.append(of.full_name)
                 fs = fsspec.core.url_to_fs(self.path[0], **self.target_options)[0]
-                fo_list = fs.cat(self.path)
-                fo_list = [ujson.loads(v) for v in fo_list.values()]
+                try:
+                    # JSON path
+                    fo_list = fs.cat(self.path)
+                    fo_list = [ujson.loads(v) for v in fo_list.values()]
+                except (IOError, TypeError, ValueError):
+                    # tries again sequentially in comprehension below
+                    fo_list = self.path
 
             self._fss = [
                 fsspec.filesystem(
                     "reference",
                     fo=fo,
                     remote_protocol=self.remote_protocol,
                     remote_options=self.remote_options,
@@ -361,30 +368,35 @@
             for c, cv in cvalues.copy().items():
                 if isinstance(cv, np.ndarray):
                     cv = cv.ravel()
                 if isinstance(cv, (np.ndarray, list, tuple)):
                     cv = tuple(sorted(set(cv)))[0]
                     cvalues[c] = cv
 
-            for v, _, attrs in fs.walk("", detail=False):
+            dirs = fs.ls("", detail=False)
+            while dirs:
+                v = dirs.pop(0)
                 if v in self.coo_map or v in skip or v.startswith(".z"):
                     # already made coordinate variables and metadata
                     continue
-                if ".zgroup" in attrs:
-                    if v:
-                        # non-base groups need group metadata copied
-                        for fn in [".zgroup", ".zattrs"]:
-                            self.out[f"{v}/{fn}"] = m[f"{v}/{fn}"]
+                fns = fs.ls(v, detail=False)
+                if f"{v}/.zgroup" in fns:
+                    # recurse into groups - copy meta, add to dirs to process and don't look
+                    # for references in this dir
+                    self.out[f"{v}/.zgroup"] = m[f"{v}/.zgroup"]
+                    if f"{v}/.zattrs" in fns:
+                        self.out[f"{v}/.zattrs"] = m[f"{v}/.zattrs"]
+                    dirs.extend([f for f in fns if not f.startswith(f"{v}/.z")])
                     continue
                 if v in self.identical_dims:
                     if f"{v}/.zarray" in self.out:
                         continue
-                    for k, val in fs.references.items():
+                    for k in fs.ls(v, detail=False):
                         if k.startswith(f"{v}/"):
-                            self.out[k] = val
+                            self.out[k] = fs.references[k]
                     continue
                 logger.debug("Second pass: %s, %s", i, v)
 
                 zarray = ujson.loads(m[f"{v}/.zarray"])
                 if v not in chunk_sizes:
                     chunk_sizes[v] = zarray["chunks"]
                 elif chunk_sizes[v] != zarray["chunks"]:
@@ -435,15 +447,15 @@
                     self.out[f"{var or v}/.zarray"] = ujson.dumps(zarray)
                     # other attributes copied as-is from first occurrence of this array
                     self.out[f"{var or v}/.zattrs"] = ujson.dumps(zattrs)
                 else:
                     k = self.out[f"{var or v}/.zarray"]
                     ch = ujson.loads(k)["chunks"]
 
-                for fn in fs.ls(v, detail=False):
+                for fn in fns:
                     # loop over the chunks and copy the references
                     if ".z" in fn:
                         continue
                     key_parts = fn.split("/")[-1].split(".")
                     key = f"{var or v}/"
                     for loc, c in enumerate(coord_order):
                         if c in self.coos:
```

### Comparing `kerchunk-0.1.1/kerchunk/df.py` & `kerchunk-0.1.2/kerchunk/df.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,46 +96,64 @@
     storage_options = {} if storage_options is None else storage_options
     json_obj = _normalize_json(json_obj)
     with fsspec.open(fname, "wb", **storage_options) as f:
         f.write(json_obj)
 
 
 def refs_to_dataframe(
-    refs,
+    fo,
     url,
+    target_protocol=None,
+    target_options=None,
     storage_options=None,
     record_size=10_000,
     categorical_threshold=10,
     **kwargs,
 ):
     """Write references as a parquet files store.
 
     The directory structure should mimic a normal zarr store but instead of standard chunk
     keys, references are saved as parquet dataframes.
 
     Parameters
     ----------
-    refs: str | dict
+    fo : str | dict
         Location of a JSON file containing references or a reference set already loaded
         into memory.
-    url: str
+    url : str
         Location for the output, together with protocol. This must be a writable
         directory.
+    target_protocol : str
+        Used for loading the reference file, if it is a path. If None, protocol
+        will be derived from the given path
+    target_options : dict
+        Extra FS options for loading the reference file ``fo``, if given as a path
     storage_options: dict | None
         Passed to fsspec when for writing the parquet.
     record_size : int
         Number of references to store in each reference file (default 10000). Bigger values
         mean fewer read requests but larger memory footprint.
     categorical_threshold : int
         Encode urls as pandas.Categorical to reduce memory footprint if the ratio
         of the number of unique urls to total number of refs for each variable
         is greater than or equal to this number. (default 10)
     **kwargs : dict
         Additional keyword arguments passed to fastparquet.
     """
+    # Taken from fsspec/implementations/reference.py
+    if isinstance(fo, str):
+        # JSON file
+        dic = dict(**(target_options or {}), protocol=target_protocol)
+        with fsspec.open(fo, "rb", **dic) as f:
+            logger.info("Read reference from URL %s", fo)
+            refs = ujson.load(f)
+    else:
+        # Mapping object
+        refs = fo
+
     if "refs" in refs:
         refs = refs["refs"]
 
     fs, _ = fsspec.core.url_to_fs(url)
     fs.makedirs(url, exist_ok=True)
     fields = get_variables(refs, consolidated=True)
     # write into .zmetadata at top level, one fewer read on access
```

### Comparing `kerchunk-0.1.1/kerchunk/fits.py` & `kerchunk-0.1.2/kerchunk/fits.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/grib2.py` & `kerchunk-0.1.2/kerchunk/grib2.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/hdf.py` & `kerchunk-0.1.2/kerchunk/hdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -516,18 +516,29 @@
             if num_chunks == 0:
                 # No data ever written...
                 return dict()
 
             # Go over all the dataset chunks...
             stinfo = dict()
             chunk_size = dset.chunks
-            for index in range(num_chunks):
-                blob = dsid.get_chunk_info(index)
-                key = tuple([a // b for a, b in zip(blob.chunk_offset, chunk_size)])
-                stinfo[key] = {"offset": blob.byte_offset, "size": blob.size}
+
+            def get_key(blob):
+                return tuple([a // b for a, b in zip(blob.chunk_offset, chunk_size)])
+
+            def store_chunk_info(blob):
+                stinfo[get_key(blob)] = {"offset": blob.byte_offset, "size": blob.size}
+
+            has_chunk_iter = callable(getattr(dsid, "chunk_iter", None))
+
+            if has_chunk_iter:
+                dsid.chunk_iter(store_chunk_info)
+            else:
+                for index in range(num_chunks):
+                    store_chunk_info(dsid.get_chunk_info(index))
+
             return stinfo
 
 
 def _simple_type(x):
     if isinstance(x, bytes):
         return x.decode()
     if isinstance(x, np.number):
```

### Comparing `kerchunk-0.1.1/kerchunk/netCDF3.py` & `kerchunk-0.1.2/kerchunk/netCDF3.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/tiff.py` & `kerchunk-0.1.2/kerchunk/tiff.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/utils.py` & `kerchunk-0.1.2/kerchunk/utils.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk/zarr.py` & `kerchunk-0.1.2/kerchunk/zarr.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/kerchunk.egg-info/PKG-INFO` & `kerchunk-0.1.2/kerchunk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerchunk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Functions to make reference descriptions for ReferenceFileSystem
 Home-page: https://github.com/fsspec/kerchunk
 Author: Martin Durant
 Author-email: martin.durant@alumni.utoronto.ca
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kerchunk-0.1.1/kerchunk.egg-info/SOURCES.txt` & `kerchunk-0.1.2/kerchunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/setup.cfg` & `kerchunk-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/setup.py` & `kerchunk-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `kerchunk-0.1.1/versioneer.py` & `kerchunk-0.1.2/versioneer.py`

 * *Files identical despite different names*

