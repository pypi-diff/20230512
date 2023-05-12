# Comparing `tmp/katdal-0.9.tar.gz` & `tmp/katdal-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/katdal-0.9.tar", last modified: Tue Jan 16 12:48:16 2018, max compression
+gzip compressed data, was "dist/katdal-0.9.5.tar", last modified: Thu Feb 22 08:58:29 2018, max compression
```

## Comparing `katdal-0.9.tar` & `katdal-0.9.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-01-16 12:48:16.000000 katdal-0.9/
-drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-01-16 12:48:16.000000 katdal-0.9/katdal/
--rw-r--r--   0 schwardt   (501) staff       (20)    15245 2018-01-16 12:48:16.000000 katdal-0.9/katdal/__init__.py
--rw-r--r--   0 schwardt   (501) staff       (20)     6635 2018-01-10 12:06:16.000000 katdal-0.9/katdal/averager.py
--rw-r--r--   0 schwardt   (501) staff       (20)    34146 2018-01-10 12:06:16.000000 katdal-0.9/katdal/categorical.py
--rw-r--r--   0 schwardt   (501) staff       (20)     9643 2018-01-16 11:24:35.000000 katdal-0.9/katdal/chunkstore.py
--rw-r--r--   0 schwardt   (501) staff       (20)     2676 2018-01-16 11:24:35.000000 katdal-0.9/katdal/chunkstore_dict.py
--rw-r--r--   0 schwardt   (501) staff       (20)     3393 2018-01-16 11:24:35.000000 katdal-0.9/katdal/chunkstore_npy.py
--rw-r--r--   0 schwardt   (501) staff       (20)     5291 2018-01-16 11:24:35.000000 katdal-0.9/katdal/chunkstore_rados.py
--rw-r--r--   0 schwardt   (501) staff       (20)     6068 2018-01-16 11:24:35.000000 katdal-0.9/katdal/chunkstore_s3.py
--rw-r--r--   0 schwardt   (501) staff       (20)    34475 2018-01-12 11:47:15.000000 katdal-0.9/katdal/concatdata.py
--rw-r--r--   0 schwardt   (501) staff       (20)    59026 2018-01-10 12:06:16.000000 katdal-0.9/katdal/dataset.py
--rw-r--r--   0 schwardt   (501) staff       (20)     2709 2018-01-10 12:06:16.000000 katdal-0.9/katdal/datasources.py
--rw-r--r--   0 schwardt   (501) staff       (20)    22683 2018-01-10 12:06:16.000000 katdal-0.9/katdal/h5datav1.py
--rw-r--r--   0 schwardt   (501) staff       (20)    34741 2018-01-10 12:06:16.000000 katdal-0.9/katdal/h5datav2.py
--rw-r--r--   0 schwardt   (501) staff       (20)    55265 2018-01-12 08:40:29.000000 katdal-0.9/katdal/h5datav3.py
--rw-r--r--   0 schwardt   (501) staff       (20)    19372 2018-01-10 12:06:16.000000 katdal-0.9/katdal/lazy_indexer.py
--rw-r--r--   0 schwardt   (501) staff       (20)    46330 2018-01-10 12:06:16.000000 katdal-0.9/katdal/ms_extra.py
--rw-r--r--   0 schwardt   (501) staff       (20)    36708 2018-01-12 11:47:15.000000 katdal-0.9/katdal/sensordata.py
-drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-01-16 12:48:16.000000 katdal-0.9/katdal/test/
--rw-r--r--   0 schwardt   (501) staff       (20)        0 2017-07-14 15:34:02.000000 katdal-0.9/katdal/test/__init__.py
--rw-r--r--   0 schwardt   (501) staff       (20)     2322 2018-01-10 12:06:16.000000 katdal-0.9/katdal/test/test_categorical.py
--rw-r--r--   0 schwardt   (501) staff       (20)     4700 2018-01-16 11:24:35.000000 katdal-0.9/katdal/test/test_chunkstore.py
--rw-r--r--   0 schwardt   (501) staff       (20)     1062 2018-01-15 11:40:45.000000 katdal-0.9/katdal/test/test_chunkstore_dict.py
--rw-r--r--   0 schwardt   (501) staff       (20)     1589 2018-01-16 11:24:35.000000 katdal-0.9/katdal/test/test_chunkstore_npy.py
--rw-r--r--   0 schwardt   (501) staff       (20)     2655 2018-01-16 11:24:35.000000 katdal-0.9/katdal/test/test_chunkstore_rados.py
--rw-r--r--   0 schwardt   (501) staff       (20)     4028 2018-01-16 11:24:35.000000 katdal-0.9/katdal/test/test_chunkstore_s3.py
--rw-r--r--   0 schwardt   (501) staff       (20)    19054 2018-01-10 12:06:16.000000 katdal-0.9/katdal/visdatav4.py
-drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-01-16 12:48:16.000000 katdal-0.9/katdal.egg-info/
--rw-r--r--   0 schwardt   (501) staff       (20)        1 2018-01-16 12:48:15.000000 katdal-0.9/katdal.egg-info/dependency_links.txt
--rw-r--r--   0 schwardt   (501) staff       (20)        1 2016-12-14 20:22:05.000000 katdal-0.9/katdal.egg-info/not-zip-safe
--rw-r--r--   0 schwardt   (501) staff       (20)    14033 2018-01-16 12:48:15.000000 katdal-0.9/katdal.egg-info/PKG-INFO
--rw-r--r--   0 schwardt   (501) staff       (20)       79 2018-01-16 12:48:15.000000 katdal-0.9/katdal.egg-info/requires.txt
--rw-r--r--   0 schwardt   (501) staff       (20)      875 2018-01-16 12:48:15.000000 katdal-0.9/katdal.egg-info/SOURCES.txt
--rw-r--r--   0 schwardt   (501) staff       (20)        7 2018-01-16 12:48:15.000000 katdal-0.9/katdal.egg-info/top_level.txt
--rw-r--r--   0 schwardt   (501) staff       (20)    14033 2018-01-16 12:48:16.000000 katdal-0.9/PKG-INFO
--rw-r--r--   0 schwardt   (501) staff       (20)     9831 2017-07-14 15:34:02.000000 katdal-0.9/README.rst
-drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-01-16 12:48:16.000000 katdal-0.9/scripts/
--rwxr-xr-x   0 schwardt   (501) staff       (20)     2136 2018-01-10 12:06:16.000000 katdal-0.9/scripts/fix_ant_positions.py
--rwxr-xr-x   0 schwardt   (501) staff       (20)     2893 2018-01-10 12:06:16.000000 katdal-0.9/scripts/h5list.py
--rwxr-xr-x   0 schwardt   (501) staff       (20)    34422 2018-01-10 12:06:16.000000 katdal-0.9/scripts/h5toms.py
--rw-r--r--   0 schwardt   (501) staff       (20)       38 2018-01-16 12:48:16.000000 katdal-0.9/setup.cfg
--rwxr-xr-x   0 schwardt   (501) staff       (20)     2528 2018-01-10 12:06:16.000000 katdal-0.9/setup.py
+drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-02-22 08:58:29.000000 katdal-0.9.5/
+drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal/
+-rw-r--r--   0 schwardt   (501) staff       (20)    15632 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal/__init__.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     6635 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/averager.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    34146 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/categorical.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    18675 2018-02-01 21:00:43.000000 katdal-0.9.5/katdal/chunkstore.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     2688 2018-02-01 21:00:43.000000 katdal-0.9.5/katdal/chunkstore_dict.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     4416 2018-02-01 21:00:43.000000 katdal-0.9.5/katdal/chunkstore_npy.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     5846 2018-02-09 10:00:20.000000 katdal-0.9.5/katdal/chunkstore_rados.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     6868 2018-02-01 21:00:43.000000 katdal-0.9.5/katdal/chunkstore_s3.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    34475 2018-01-12 11:47:15.000000 katdal-0.9.5/katdal/concatdata.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    57388 2018-02-12 21:42:02.000000 katdal-0.9.5/katdal/dataset.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    11255 2018-02-19 10:00:36.000000 katdal-0.9.5/katdal/datasources.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    22683 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/h5datav1.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    34741 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/h5datav2.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    55776 2018-02-21 13:49:46.000000 katdal-0.9.5/katdal/h5datav3.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    20454 2018-02-09 10:00:20.000000 katdal-0.9.5/katdal/lazy_indexer.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    46330 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/ms_extra.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    36708 2018-01-12 11:47:15.000000 katdal-0.9.5/katdal/sensordata.py
+drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal/test/
+-rw-r--r--   0 schwardt   (501) staff       (20)        0 2017-07-14 15:34:02.000000 katdal-0.9.5/katdal/test/__init__.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     2322 2018-01-10 12:06:16.000000 katdal-0.9.5/katdal/test/test_categorical.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    10481 2018-02-01 21:00:43.000000 katdal-0.9.5/katdal/test/test_chunkstore.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     1062 2018-01-15 11:40:45.000000 katdal-0.9.5/katdal/test/test_chunkstore_dict.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     1589 2018-01-16 11:24:35.000000 katdal-0.9.5/katdal/test/test_chunkstore_npy.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     2655 2018-01-16 11:24:35.000000 katdal-0.9.5/katdal/test/test_chunkstore_rados.py
+-rw-r--r--   0 schwardt   (501) staff       (20)     4028 2018-01-16 11:24:35.000000 katdal-0.9.5/katdal/test/test_chunkstore_s3.py
+-rw-r--r--   0 schwardt   (501) staff       (20)    20048 2018-02-19 10:00:36.000000 katdal-0.9.5/katdal/visdatav4.py
+drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/
+-rw-r--r--   0 schwardt   (501) staff       (20)        1 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/dependency_links.txt
+-rw-r--r--   0 schwardt   (501) staff       (20)        1 2016-12-14 20:22:05.000000 katdal-0.9.5/katdal.egg-info/not-zip-safe
+-rw-r--r--   0 schwardt   (501) staff       (20)    14330 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/PKG-INFO
+-rw-r--r--   0 schwardt   (501) staff       (20)       79 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/requires.txt
+-rw-r--r--   0 schwardt   (501) staff       (20)      875 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/SOURCES.txt
+-rw-r--r--   0 schwardt   (501) staff       (20)        7 2018-02-22 08:58:29.000000 katdal-0.9.5/katdal.egg-info/top_level.txt
+-rw-r--r--   0 schwardt   (501) staff       (20)    14330 2018-02-22 08:58:29.000000 katdal-0.9.5/PKG-INFO
+-rw-r--r--   0 schwardt   (501) staff       (20)     9831 2017-07-14 15:34:02.000000 katdal-0.9.5/README.rst
+drwxr-xr-x   0 schwardt   (501) staff       (20)        0 2018-02-22 08:58:29.000000 katdal-0.9.5/scripts/
+-rwxr-xr-x   0 schwardt   (501) staff       (20)     2136 2018-01-10 12:06:16.000000 katdal-0.9.5/scripts/fix_ant_positions.py
+-rwxr-xr-x   0 schwardt   (501) staff       (20)     2893 2018-01-10 12:06:16.000000 katdal-0.9.5/scripts/h5list.py
+-rwxr-xr-x   0 schwardt   (501) staff       (20)    34422 2018-01-10 12:06:16.000000 katdal-0.9.5/scripts/h5toms.py
+-rw-r--r--   0 schwardt   (501) staff       (20)       38 2018-02-22 08:58:29.000000 katdal-0.9.5/setup.cfg
+-rwxr-xr-x   0 schwardt   (501) staff       (20)     2543 2018-01-31 13:22:49.000000 katdal-0.9.5/setup.py
```

### Comparing `katdal-0.9/katdal/__init__.py` & `katdal-0.9.5/katdal/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -208,14 +208,15 @@
 Finally, all the targets (or fields) in the data set are stored in a catalogue
 available at `d.catalogue`, and the original HDF5 file is still accessible via
 a back door installed at `d.file` in the case of a single-file data set.
 
 """
 
 import logging as _logging
+import urlparse
 
 from .dataset import DataSet, WrongVersion
 from .lazy_indexer import LazyTransform
 from .concatdata import ConcatenatedDataSet
 from .h5datav1 import H5DataV1
 from .h5datav2 import H5DataV2
 from .h5datav3 import H5DataV3
@@ -315,15 +316,22 @@
     data : :class:`DataSet` object
         Object providing :class:`DataSet` interface to file(s)
 
     """
     filenames = [filename] if isinstance(filename, basestring) else filename
     datasets = []
     for f in filenames:
-        dataset = _file_action('__call__', f, ref_ant, time_offset, **kwargs)
+        # V4 RDB file with optional URL-style query string
+        if urlparse.urlsplit(f).path.endswith('.rdb'):
+            from .datasources import open_data_source
+            from .visdatav4 import VisibilityDataV4
+            dataset = VisibilityDataV4(open_data_source(f),
+                                       ref_ant, time_offset, **kwargs)
+        else:
+            dataset = _file_action('__call__', f, ref_ant, time_offset, **kwargs)
         datasets.append(dataset)
     return datasets[0] if isinstance(filename, basestring) else \
         ConcatenatedDataSet(datasets)
 
 
 def get_ants(filename):
     """Quick look function to get the list of antennas in a data file.
@@ -354,8 +362,8 @@
     targets : :class:'katpoint.Catalogue' object
         All targets in file
 
     """
     return _file_action('_get_targets', filename)
 
 # Automatically added by katversion
-__version__ = '0.9'
+__version__ = '0.9.5'
```

### Comparing `katdal-0.9/katdal/averager.py` & `katdal-0.9.5/katdal/averager.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/categorical.py` & `katdal-0.9.5/katdal/categorical.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/chunkstore_dict.py` & `katdal-0.9.5/katdal/chunkstore_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
     def __init__(self, **kwargs):
         error_map = {KeyError: ChunkNotFound, IndexError: ChunkNotFound}
         super(DictChunkStore, self).__init__(error_map)
         self.arrays = kwargs
 
     def get_chunk(self, array_name, slices, dtype):
-        """See the docstring of :meth:`ChunkStore.get`."""
+        """See the docstring of :meth:`ChunkStore.get_chunk`."""
         chunk_name, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
         with self._standard_errors(chunk_name):
             array = self.arrays[array_name]
             # Ensure that chunk is array (otherwise 0-dim array becomes number)
             chunk = array[slices] if slices != () else array
         if dtype != chunk.dtype:
             raise BadChunk('Chunk {!r}: requested dtype {} differs from '
                            'actual dtype {}'
                            .format(chunk_name, dtype, chunk.dtype))
         return chunk
 
     def put_chunk(self, array_name, slices, chunk):
-        """See the docstring of :meth:`ChunkStore.put`."""
+        """See the docstring of :meth:`ChunkStore.put_chunk`."""
         self.chunk_metadata(array_name, slices, chunk=chunk)
         self.get_chunk(array_name, slices, chunk.dtype)[()] = chunk
 
     get_chunk.__doc__ = ChunkStore.get_chunk.__doc__
     put_chunk.__doc__ = ChunkStore.put_chunk.__doc__
```

### Comparing `katdal-0.9/katdal/chunkstore_npy.py` & `katdal-0.9.5/katdal/chunkstore_npy.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 import os
 
 import numpy as np
 
 from .chunkstore import ChunkStore, StoreUnavailable, ChunkNotFound, BadChunk
 
 
+def load_npy_header(filename):
+    """Load NPY file header only to obtain shape and dtype information."""
+    with open(filename, 'r') as fp:
+        # Header version: either (1, 0) or (2, 0)
+        ver = np.lib.format.read_magic(fp)
+        shape, fortran_order, dtype = np.lib.format._read_array_header(fp, ver)
+    return shape, fortran_order, dtype
+
+
 class NpyFileChunkStore(ChunkStore):
     """A store of chunks (i.e. N-dimensional arrays) based on NPY files.
 
     Each chunk is stored in a separate binary file in NumPy ``.npy`` format.
     The filename is constructed as
 
       "<path>/<array>/<idx>.npy"
@@ -47,39 +56,53 @@
     Raises
     ------
     :exc:`chunkstore.StoreUnavailable`
         If path does not exist / is not readable
     """
 
     def __init__(self, path):
-        super(NpyFileChunkStore, self).__init__({IOError: ChunkNotFound})
+        super(NpyFileChunkStore, self).__init__({IOError: ChunkNotFound,
+                                                 ValueError: ChunkNotFound})
         if not os.path.isdir(path):
             raise StoreUnavailable('Directory {!r} does not exist'.format(path))
         self.path = path
 
     def get_chunk(self, array_name, slices, dtype):
-        """See the docstring of :meth:`ChunkStore.get`."""
+        """See the docstring of :meth:`ChunkStore.get_chunk`."""
         chunk_name, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
         filename = os.path.join(self.path, chunk_name) + '.npy'
         with self._standard_errors(chunk_name):
             chunk = np.load(filename, allow_pickle=False)
         if dtype != chunk.dtype:
             raise BadChunk('Requested dtype {} differs from NPY file dtype {}'
                            .format(dtype, chunk.dtype))
         return chunk
 
     def put_chunk(self, array_name, slices, chunk):
-        """See the docstring of :meth:`ChunkStore.put`."""
+        """See the docstring of :meth:`ChunkStore.put_chunk`."""
         chunk_name, shape = self.chunk_metadata(array_name, slices, chunk=chunk)
         filename = os.path.join(self.path, chunk_name) + '.npy'
         # Ensure any subdirectories are in place
         try:
             os.makedirs(os.path.dirname(filename))
         except OSError as e:
             # Be happy if someone already created the path
             if e.errno != os.errno.EEXIST:
                 raise
         with self._standard_errors(chunk_name):
             np.save(filename, chunk, allow_pickle=False)
 
+    def has_chunk(self, array_name, slices, dtype):
+        """See the docstring of :meth:`ChunkStore.has_chunk`."""
+        chunk_name, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
+        filename = os.path.join(self.path, chunk_name) + '.npy'
+        try:
+            with self._standard_errors(chunk_name):
+                npy_shape, _, npy_dtype = load_npy_header(filename)
+        except ChunkNotFound:
+            return False
+        else:
+            return npy_dtype == dtype and npy_shape == shape
+
     get_chunk.__doc__ = ChunkStore.get_chunk.__doc__
     put_chunk.__doc__ = ChunkStore.put_chunk.__doc__
+    has_chunk.__doc__ = ChunkStore.has_chunk.__doc__
```

### Comparing `katdal-0.9/katdal/chunkstore_rados.py` & `katdal-0.9.5/katdal/chunkstore_rados.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @classmethod
     def from_config(cls, config, pool, keyring=None, timeout=5.):
         """Construct RADOS chunk store from config and specified pool.
 
         Parameters
         ----------
         config : string or dict
-            Path to Ceph configuration file or config dict version of that file
+            Path to Ceph config file or config dict
         pool : string
             Name of the Ceph pool
         keyring : string, optional
             Path to client keyring file (if not provided by `conf` or override)
         timeout : float, optional
             RADOS client timeout, in seconds (set to None to leave unchanged)
 
@@ -96,15 +96,15 @@
             ioctx = cluster.open_ioctx(pool)
         # A missing config file or pool also triggers ObjectNotFound
         except (rados.TimedOut, rados.ObjectNotFound) as e:
             raise StoreUnavailable(str(e))
         return cls(ioctx)
 
     def get_chunk(self, array_name, slices, dtype):
-        """See the docstring of :meth:`ChunkStore.get`."""
+        """See the docstring of :meth:`ChunkStore.get_chunk`."""
         dtype = np.dtype(dtype)
         key, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
         expected_bytes = int(np.prod(shape)) * dtype.itemsize
         with self._standard_errors(key):
             # Try to read an extra byte to see if data is more than expected
             data_str = self.ioctx.read(key, expected_bytes + 1)
         actual_bytes = len(data_str)
@@ -116,15 +116,29 @@
             raise BadChunk('Chunk {!r}: dtype {} and shape {} implies an '
                            'object size of {} bytes, got {} bytes instead'
                            .format(key, dtype, shape, expected_bytes,
                                    actual_bytes))
         return np.ndarray(shape, dtype, data_str)
 
     def put_chunk(self, array_name, slices, chunk):
-        """See the docstring of :meth:`ChunkStore.put`."""
+        """See the docstring of :meth:`ChunkStore.put_chunk`."""
         key, shape = self.chunk_metadata(array_name, slices, chunk=chunk)
         data_str = chunk.tobytes()
         with self._standard_errors(key):
             self.ioctx.write_full(key, data_str)
 
+    def has_chunk(self, array_name, slices, dtype):
+        """See the docstring of :meth:`ChunkStore.has_chunk`."""
+        dtype = np.dtype(dtype)
+        key, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
+        expected_bytes = int(np.prod(shape)) * dtype.itemsize
+        try:
+            with self._standard_errors(key):
+                actual_bytes, _ = self.ioctx.stat(key)
+        except ChunkNotFound:
+            return False
+        else:
+            return actual_bytes == expected_bytes
+
     get_chunk.__doc__ = ChunkStore.get_chunk.__doc__
     put_chunk.__doc__ = ChunkStore.put_chunk.__doc__
+    has_chunk.__doc__ = ChunkStore.has_chunk.__doc__
```

### Comparing `katdal-0.9/katdal/chunkstore_s3.py` & `katdal-0.9.5/katdal/chunkstore_s3.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     _botocore_import_error = None
 except ImportError as e:
     botocore = None
     _botocore_import_error = e
 else:
     import botocore.config
     import botocore.session
-    from botocore.exceptions import EndpointConnectionError, NoCredentialsError
+    from botocore.exceptions import (EndpointConnectionError,
+                                     NoCredentialsError, ClientError)
 
 from .chunkstore import ChunkStore, StoreUnavailable, ChunkNotFound, BadChunk
 
 
 class S3ChunkStore(ChunkStore):
     """A store of chunks (i.e. N-dimensional arrays) based on the Amazon S3 API.
 
@@ -114,15 +115,15 @@
             # Quick smoke test to see if the S3 server is available
             client.list_buckets()
         except (EndpointConnectionError, NoCredentialsError, ValueError) as e:
             raise StoreUnavailable(str(e))
         return cls(client)
 
     def get_chunk(self, array_name, slices, dtype):
-        """See the docstring of :meth:`ChunkStore.get`."""
+        """See the docstring of :meth:`ChunkStore.get_chunk`."""
         dtype = np.dtype(dtype)
         chunk_name, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
         bucket, key = self.split(chunk_name, 1)
         with self._standard_errors(chunk_name):
             response = self.client.get_object(Bucket=bucket, Key=key)
         with contextlib.closing(response['Body']) as stream:
             data_str = stream.read()
@@ -131,16 +132,33 @@
             raise BadChunk('Chunk {!r}: dtype {} and shape {} implies an '
                            'object size of {} bytes, got {} bytes instead'
                            .format(chunk_name, dtype, shape, expected_bytes,
                                    len(data_str)))
         return np.ndarray(shape, dtype, data_str)
 
     def put_chunk(self, array_name, slices, chunk):
-        """See the docstring of :meth:`ChunkStore.put`."""
+        """See the docstring of :meth:`ChunkStore.put_chunk`."""
         chunk_name, shape = self.chunk_metadata(array_name, slices, chunk=chunk)
         bucket, key = self.split(chunk_name, 1)
         data_str = chunk.tobytes()
         with self._standard_errors(chunk_name):
             self.client.put_object(Bucket=bucket, Key=key, Body=data_str)
 
+    def has_chunk(self, array_name, slices, dtype):
+        """See the docstring of :meth:`ChunkStore.has_chunk`."""
+        dtype = np.dtype(dtype)
+        chunk_name, shape = self.chunk_metadata(array_name, slices, dtype=dtype)
+        bucket, key = self.split(chunk_name, 1)
+        try:
+            response = self.client.head_object(Bucket=bucket, Key=key)
+        except ClientError as err:
+            if err.response['Error']['Code'] != '404':
+                raise
+            return False
+        else:
+            actual_bytes = response['ContentLength']
+            expected_bytes = int(np.prod(shape)) * dtype.itemsize
+            return actual_bytes == expected_bytes
+
     get_chunk.__doc__ = ChunkStore.get_chunk.__doc__
     put_chunk.__doc__ = ChunkStore.put_chunk.__doc__
+    has_chunk.__doc__ = ChunkStore.has_chunk.__doc__
```

### Comparing `katdal-0.9/katdal/concatdata.py` & `katdal-0.9.5/katdal/concatdata.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/dataset.py` & `katdal-0.9.5/katdal/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,62 +50,14 @@
     try:
         return np.array_equal(a1, a2)
     except AttributeError:
         a1, a2 = np.asarray(a1), np.asarray(a2)
         return (a1.shape == a2.shape) and np.all(a1 == a2)
 
 
-class AttrsSensors(object):
-    """Metadata in the form of attributes and sensors.
-
-    Parameters
-    ----------
-    attrs : mapping from string to object
-        Metadata attributes
-    sensors : mapping from string to :class:`SensorData` objects
-        Metadata sensor cache mapping sensor names to raw sensor data
-    name : string, optional
-        Identifier that describes the origin of the metadata (backend-specific)
-
-    """
-    def __init__(self, attrs, sensors, name='custom'):
-        self.attrs = attrs
-        self.sensors = sensors
-        self.name = name
-
-
-class VisFlagsWeights(object):
-    """Correlator data in the form of visibilities, flags and weights.
-
-    Parameters
-    ----------
-    vis : array-like of complex64, shape (*T*, *F*, *B*)
-        Complex visibility data as a function of time, frequency and baseline
-    flags : array-like of uint8, shape (*T*, *F*, *B*)
-        Flags as a function of time, frequency and baseline
-    weights : array-like of float32, shape (*T*, *F*, *B*)
-        Visibility weights as a function of time, frequency and baseline
-    name : string, optional
-        Identifier that describes the origin of the data (backend-specific)
-
-    """
-    def __init__(self, vis, flags, weights, name='custom'):
-        if not (vis.shape == flags.shape == weights.shape):
-            raise ValueError("Shapes of vis %s, flags %s and weights %s differ"
-                             % (vis.shape, flags.shape, weights.shape))
-        self.vis = vis
-        self.flags = flags
-        self.weights = weights
-        self.name = name
-
-    @property
-    def shape(self):
-        return self.vis.shape
-
-
 class Subarray(object):
     """Subarray specification.
 
     A subarray is determined by the specific correlation products produced by the
     correlator and the antenna objects associated with the inputs found in the
     correlation products.
 
@@ -568,18 +520,18 @@
                 continue
             if min_freq < model.min_freq_MHz and \
                min_freq > 0.6 * model.min_freq_MHz or \
                max_freq > model.max_freq_MHz and \
                max_freq < 1.6 * model.max_freq_MHz:
                 new_min_freq = min(min_freq, model.min_freq_MHz)
                 new_max_freq = max(max_freq, model.max_freq_MHz)
-                logger.warn('Extending flux density model frequency range of '
-                            '%r from %d-%d MHz to %d-%d MHz', target.name,
-                            model.min_freq_MHz, model.max_freq_MHz,
-                            new_min_freq, new_max_freq)
+                logger.warning('Extending flux density model frequency range '
+                               'of %r from %d-%d MHz to %d-%d MHz', target.name,
+                               model.min_freq_MHz, model.max_freq_MHz,
+                               new_min_freq, new_max_freq)
                 model.min_freq_MHz = new_min_freq
                 model.max_freq_MHz = new_max_freq
 
     def _set_keep(self, time_keep=None, freq_keep=None, corrprod_keep=None,
                   weights_keep=None, flags_keep=None):
         """Set time, frequency and/or correlation product selection masks.
```

### Comparing `katdal-0.9/katdal/h5datav1.py` & `katdal-0.9.5/katdal/h5datav1.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/h5datav2.py` & `katdal-0.9.5/katdal/h5datav2.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/h5datav3.py` & `katdal-0.9.5/katdal/h5datav3.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,23 +349,29 @@
             np.array(zip(WEIGHT_NAMES, WEIGHT_DESCRIPTIONS))
         self._weights_select = []
         self._weights_keep = 'all'
 
         # ------ Extract observation parameters and script log ------
 
         self.obs_params = {}
-        # Replay obs_params sensor if available and update obs_params dict accordingly
-        try:
-            obs_params = self.sensor.get('Observation/params', extract=False)['value']
-        except KeyError:
-            obs_params = []
-        for obs_param in obs_params:
-            if obs_param:
-                key, val = obs_param.split(' ', 1)
-                self.obs_params[key] = np.lib.utils.safe_eval(val)
+        # obs_params is a telstate attribute in v3.9 so try that first
+        if 'capture_block_id' in f.attrs:
+            attr_name = f.attrs['capture_block_id'] + '_obs_params'
+            self.obs_params = self._get_telstate_attr(attr_name, {})
+        if not self.obs_params:
+            try:
+                # Replay obs_params sensor if available
+                obs_params = self.sensor.get('Observation/params',
+                                             extract=False)['value']
+            except KeyError:
+                obs_params = []
+            for obs_param in obs_params:
+                if obs_param:
+                    key, val = obs_param.split(' ', 1)
+                    self.obs_params[key] = np.lib.utils.safe_eval(val)
         # Get observation script parameters, with defaults
         self.observer = self.obs_params.get('observer', '')
         self.description = self.obs_params.get('description', '')
         self.experiment_id = self.obs_params.get('experiment_id', '')
         # Extract script log data verbatim (it is not a standard sensor anyway)
         try:
             self.obs_script_log = self.sensor.get('Observation/script_log', extract=False)['value'].tolist()
@@ -446,20 +452,26 @@
                     logger.warning('Guessed receiver band from most common '
                                    'indexer position - this is not reliable!')
         if not band:
             logger.warning('Could not figure out receiver band - '
                            'please provide it via band parameter')
         # Populate antenna -> receiver mapping and figure out noise diode
         for ant in cam_ants:
-            # Try sanitised version of RX serial number first
-            rx_sensor = 'TelescopeState/%s_rx_serial_number' % (ant,)
-            rx_serial = self.sensor[rx_sensor][0] if rx_sensor in self.sensor else 0
-            if rx_serial == 0:
-                rx_sensor = 'Antennas/%s/rsc_rx%s_serial_number' % (ant, band)
-                rx_serial = self.sensor[rx_sensor][0] if rx_sensor in self.sensor else 0
+            rx_sensor_options = (
+                # Since 2018-01-16 MKAT / ARx only has this version
+                'TelescopeState/%s_rsc_rx%s_serial_number' % (ant, band),
+                # RTS since 2017-11-15
+                'TelescopeState/%s_rx_serial_number' % (ant,),
+                # Original TelescopeModel version
+                'Antennas/%s/rsc_rx%s_serial_number' % (ant, band))
+            rx_serial = 0
+            for rx_sensor in rx_sensor_options:
+                if rx_sensor in self.sensor:
+                    rx_serial = self.sensor[rx_sensor][0]
+                    break
             if band:
                 self.receivers[ant] = '%s.%d' % (band, rx_serial)
             nd_sensor = 'TelescopeState/%s_dig_%s_band_noise_diode' % (ant, band)
             if nd_sensor in self.sensor:
                 # A sensor alias would be ideal for this but it only deals with suffixes ATM
                 new_nd_sensor = 'Antennas/%s/nd_coupler' % (ant,)
                 self.sensor[new_nd_sensor] = self.sensor.get(nd_sensor, extract=False)
```

### Comparing `katdal-0.9/katdal/lazy_indexer.py` & `katdal-0.9.5/katdal/lazy_indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,7 +326,43 @@
         return new_shape
 
     @property
     def dtype(self):
         """Type of data array after transformation, i.e. `self[:].dtype`."""
         return reduce(lambda dtype, transform: transform.dtype if transform.dtype is not None else dtype,
                       self.transforms, self._initial_dtype)
+
+
+class DaskLazyIndexer(object):
+    """Turn a dask Array into a LazyIndexer by computing it upon indexing."""
+    def __init__(self, dataset, keep=()):
+        self.name = getattr(dataset, 'name', '')
+        try:
+            dataset = dataset[keep]
+        except NotImplementedError:
+            # XXX Once dask is a katdal install requirement this can move out
+            import dask.array as da
+            # Dask does not like multiple boolean indices: go one dim at a time
+            for dim, keep_per_dim in enumerate(keep):
+                dataset = da.take(dataset, keep_per_dim, axis=dim)
+        self.dataset = dataset
+        self.transforms = []
+
+    def __getitem__(self, keep):
+        return self.dataset[keep].compute()
+
+    def __len__(self):
+        """Length operator."""
+        return self.shape[0]
+
+    def __iter__(self):
+        """Iterator."""
+        for index in range(len(self)):
+            yield self[index]
+
+    @property
+    def shape(self):
+        return self.dataset.shape
+
+    @property
+    def dtype(self):
+        return self.dataset.dtype
```

### Comparing `katdal-0.9/katdal/ms_extra.py` & `katdal-0.9.5/katdal/ms_extra.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/sensordata.py` & `katdal-0.9.5/katdal/sensordata.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/test/test_categorical.py` & `katdal-0.9.5/katdal/test/test_categorical.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/test/test_chunkstore_dict.py` & `katdal-0.9.5/katdal/test/test_chunkstore_dict.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/test/test_chunkstore_npy.py` & `katdal-0.9.5/katdal/test/test_chunkstore_npy.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/test/test_chunkstore_rados.py` & `katdal-0.9.5/katdal/test/test_chunkstore_rados.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/test/test_chunkstore_s3.py` & `katdal-0.9.5/katdal/test/test_chunkstore_s3.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/katdal/visdatav4.py` & `katdal-0.9.5/katdal/visdatav4.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,52 +22,63 @@
 import katpoint
 
 from .dataset import (DataSet, BrokenFile, Subarray, SpectralWindow,
                       DEFAULT_SENSOR_PROPS, DEFAULT_VIRTUAL_SENSORS,
                       _robust_target)
 from .sensordata import SensorCache
 from .categorical import CategoricalData
+from .lazy_indexer import DaskLazyIndexer
 
 
 logger = logging.getLogger(__name__)
 
 # Simplify the scan activities to derive the basic state of the antenna
 # (slewing, scanning, tracking, stopped)
 SIMPLIFY_STATE = {'scan_ready': 'slew', 'scan': 'scan', 'scan_complete': 'scan',
                   'load_scan': 'scan', 'track': 'track', 'slew': 'slew'}
 
 SENSOR_PROPS = dict(DEFAULT_SENSOR_PROPS)
 SENSOR_PROPS.update({
     '*activity': {'greedy_values': ('slew', 'stop'), 'initial_value': 'slew',
                   'transform': lambda act: SIMPLIFY_STATE.get(act, 'stop')},
     '*ap_indexer_position': {'initial_value': ''},
-    '*ku_frequency': {'categorical': True},
     '*noise_diode': {'categorical': True, 'greedy_values': (True,),
                      'initial_value': 0.0, 'transform': lambda x: x > 0.0},
     '*serial_number': {'initial_value': 0},
     '*target': {'initial_value': '', 'transform': _robust_target},
 })
 
 SENSOR_ALIASES = {
     'nd_coupler': 'dig_noise_diode',
 }
 
 
 def _calc_azel(cache, name, ant):
     """Calculate virtual (az, el) sensors from actual ones in sensor cache."""
-    real_sensor = 'Antennas/%s/pos_actual_scan_%s' % \
+    real_sensor = '%s_pos_actual_scan_%s' % \
                   (ant, 'azim' if name.endswith('az') else 'elev')
     cache[name] = sensor_data = katpoint.deg2rad(cache.get(real_sensor))
     return sensor_data
 
 
 VIRTUAL_SENSORS = dict(DEFAULT_VIRTUAL_SENSORS)
 VIRTUAL_SENSORS.update({'Antennas/{ant}/az': _calc_azel,
                         'Antennas/{ant}/el': _calc_azel})
 
+FLAG_NAMES = ('reserved0', 'static', 'cam', 'data_lost',
+              'ingest_rfi', 'predicted_rfi', 'cal_rfi', 'reserved7')
+FLAG_DESCRIPTIONS = ('reserved - bit 0',
+                     'predefined static flag list',
+                     'flag based on live CAM information',
+                     'no data was received',
+                     'RFI detected in ingest',
+                     'RFI predicted from space based pollutants',
+                     'RFI detected in calibration',
+                     'reserved - bit 7')
+
 # -----------------------------------------------------------------------------
 # -- CLASS :  VisibilityDataV4
 # -----------------------------------------------------------------------------
 
 
 class VisibilityDataV4(DataSet):
     """Access format version 4 visibility data and metadata.
@@ -79,98 +90,68 @@
     source : :class:`DataSource` object
         Correlator data (visibilities, flags and weights) and metadata
     ref_ant : string, optional
         Name of reference antenna, used to partition data set into scans
         (default is first antenna in use)
     time_offset : float, optional
         Offset to add to all correlator timestamps, in seconds
-    centre_freq : float, optional
-        Override centre frequency if provided, in Hz
-    band : string, optional
-        Override receiver band if provided (e.g. 'l') - used to find ND models
-    keepdims : {False, True}, optional
-        Force vis / weights / flags to be 3-dimensional, regardless of selection
     kwargs : dict, optional
         Extra keyword arguments, typically meant for other formats and ignored
 
     """
-    def __init__(self, source, ref_ant='', time_offset=0.0, centre_freq=None,
-                 band=None, keepdims=False, **kwargs):
+    def __init__(self, source, ref_ant='', time_offset=0.0, **kwargs):
         DataSet.__init__(self, source.name, ref_ant, time_offset)
         attrs = source.metadata.attrs
 
         # ------ Extract timestamps ------
 
         self.source = source
         self.file = {}
         self.version = '4.0'
-        stream_name = 'sdp_l0'
-        self.dump_period = attrs[stream_name + '_int_time']
-        self._timestamps = source.timestamps[:]
-        self._keepdims = keepdims
-
-        # Check dimensions of timestamps vs those of visibility data
-        num_dumps = len(self._timestamps)
-        if source.data and (num_dumps != source.data.shape[0]):
-            raise BrokenFile('Number of timestamps received from ingest '
-                             '(%d) differs from number of dumps in data (%d)' %
-                             (num_dumps, source.data.shape[0]))
-        # The expected_dumps should always be an integer (like num_dumps),
-        # unless the timestamps and/or dump period are messed up in the file,
-        # so threshold of this test is a bit arbitrary (e.g. could use > 0.5).
-        # The last dump might only be partially filled by ingest, so ignore it.
-        if num_dumps > 1:
-            expected_dumps = 2 + (self._timestamps[-2] -
-                                  self._timestamps[0]) / self.dump_period
-            if abs(expected_dumps - num_dumps) >= 0.01:
-                # Warn the user, as this is anomalous
-                logger.warning("Irregular timestamps detected: expected %.3f "
-                               "dumps based on dump period and start/end times, "
-                               "got %d instead", expected_dumps, num_dumps)
-        self._timestamps += self.time_offset
-        if self._timestamps[0] < 1e9:
+        self.dump_period = attrs['int_time']
+        num_dumps = len(source.timestamps)
+        source.timestamps += self.time_offset
+        if source.timestamps[0] < 1e9:
             logger.warning("Data set has invalid first correlator timestamp "
-                           "(%f)", self._timestamps[0])
+                           "(%f)", source.timestamps[0])
         half_dump = 0.5 * self.dump_period
-        self.start_time = katpoint.Timestamp(self._timestamps[0] - half_dump)
-        self.end_time = katpoint.Timestamp(self._timestamps[-1] + half_dump)
-        self._time_keep = np.ones(num_dumps, dtype=np.bool)
+        self.start_time = katpoint.Timestamp(source.timestamps[0] - half_dump)
+        self.end_time = katpoint.Timestamp(source.timestamps[-1] + half_dump)
+        self._time_keep = np.full(num_dumps, True)
+        all_dumps = [0, num_dumps]
 
         # Assemble sensor cache
-        self.sensor = SensorCache(source.metadata.sensors, self._timestamps,
+        self.sensor = SensorCache(source.metadata.sensors, source.timestamps,
                                   self.dump_period, self._time_keep,
                                   SENSOR_PROPS, VIRTUAL_SENSORS, SENSOR_ALIASES)
 
+        # ------ Extract flags ------
+
+        # Internal flag mask overridden whenever _flags_keep is set via select()
+        self._flags_select = np.array([255], dtype=np.uint8)
+        self._flags_keep = 'all'
+
         # ------ Extract observation parameters and script log ------
 
-        self.obs_params = {}
-        # Replay obs_params sensor if available and update obs_params dict accordingly
-        try:
-            obs_params = self.sensor.get('obs_params', extract=False)['value']
-        except KeyError:
-            obs_params = []
-        for obs_param in obs_params:
-            if obs_param:
-                key, val = obs_param.split(' ', 1)
-                self.obs_params[key] = np.lib.utils.safe_eval(val)
+        self.obs_params = attrs['obs_params']
         # Get observation script parameters, with defaults
         self.observer = self.obs_params.get('observer', '')
         self.description = self.obs_params.get('description', '')
         self.experiment_id = self.obs_params.get('experiment_id', '')
         # Extract script log data verbatim (it is not a standard sensor anyway)
         try:
             self.obs_script_log = self.sensor.get('obs_script_log',
                                                   extract=False)['value'].tolist()
         except KeyError:
             self.obs_script_log = []
 
         # ------ Extract subarrays ------
 
         # List of correlation products as pairs of input labels
-        corrprods = attrs[stream_name + '_bls_ordering']
+        corrprods = attrs['bls_ordering']
         # Crash if there is mismatch between labels and data shape (bad labels?)
         if source.data and (len(corrprods) != source.data.shape[2]):
             raise BrokenFile('Number of baseline labels (containing expected '
                              'antenna names) received from correlator (%d) '
                              'differs from number of baselines in data (%d)' %
                              (len(corrprods), source.data.shape[2]))
         # Find all antennas in subarray with valid katpoint Antenna objects
@@ -190,96 +171,56 @@
         # By default, only pick antennas that were in use by the script
         obs_ants = self.obs_params.get('ants')
         # Otherwise fall back to the list of antennas common to CAM and SDP / CBF
         obs_ants = obs_ants.split(',') if obs_ants else list(cam_ants & sdp_ants)
         self.ref_ant = obs_ants[0] if not ref_ant else ref_ant
 
         self.subarrays = subs = [Subarray(ants, corrprods)]
-        self.sensor['Observation/subarray'] = CategoricalData(subs, [0, num_dumps])
-        self.sensor['Observation/subarray_index'] = CategoricalData([0], [0, num_dumps])
+        self.sensor['Observation/subarray'] = CategoricalData(subs, all_dumps)
+        self.sensor['Observation/subarray_index'] = CategoricalData([0], all_dumps)
         # Store antenna objects in sensor cache too, for use in virtual sensors
         for ant in ants:
             sensor_name = 'Antennas/%s/antenna' % (ant.name,)
-            self.sensor[sensor_name] = CategoricalData([ant], [0, num_dumps])
+            self.sensor[sensor_name] = CategoricalData([ant], all_dumps)
 
         # ------ Extract spectral windows / frequencies ------
 
-        # Get the receiver band identity ('l', 's', 'u', 'x') if not overridden
-        band = attrs.get('sub_band', '') if not band else band
-        if not band:
-            logger.warning('Could not figure out receiver band - '
-                           'please provide it via band parameter')
+        # Get the receiver band identity ('l', 's', 'u', 'x')
+        band = attrs['sub_band']
         # Populate antenna -> receiver mapping and figure out noise diode
         for ant in cam_ants:
             # Try sanitised version of RX serial number first
-            rx_sensor = 'TelescopeState/%s_rx_serial_number' % (ant,)
-            rx_serial = self.sensor[rx_sensor][0] if rx_sensor in self.sensor else 0
-            if rx_serial == 0:
-                rx_sensor = 'Antennas/%s/rsc_rx%s_serial_number' % (ant, band)
-                rx_serial = self.sensor[rx_sensor][0] if rx_sensor in self.sensor else 0
-            if band:
-                self.receivers[ant] = '%s.%d' % (band, rx_serial)
-            nd_sensor = 'TelescopeState/%s_dig_%s_band_noise_diode' % (ant, band)
+            rx_serial = attrs.get('%s_rsc_rx%s_serial_number' % (ant, band), 0)
+            self.receivers[ant] = '%s.%d' % (band, rx_serial)
+            nd_sensor = '%s_dig_%s_band_noise_diode' % (ant, band)
             if nd_sensor in self.sensor:
                 # A sensor alias would be ideal for this but it only deals with suffixes ATM
                 new_nd_sensor = 'Antennas/%s/nd_coupler' % (ant,)
                 self.sensor[new_nd_sensor] = self.sensor.get(nd_sensor, extract=False)
-        # Mapping describing current receiver information on MeerKAT
-        # XXX Update this as new receivers come online
-        rx_table = {
-            # Standard L-band receiver
-            'l': dict(band='L', centre_freq=1284e6, sideband=1),
-            # Standard UHF receiver
-            'u': dict(band='UHF', centre_freq=816e6, sideband=1),
-            # Custom Ku receiver for RTS
-            'x': dict(band='Ku', sideband=1),
-        }
-        spw_params = rx_table.get(band, dict(band='', sideband=1))
-        # Use CBF spectral parameters by default
-        num_chans = attrs['cbf_n_chans']
-        bandwidth = attrs['cbf_bandwidth']
-        # Cater for non-standard receivers, starting with Ku-band
-        if spw_params['band'] == 'Ku':
-            if 'anc_siggen_ku_frequency' in self.sensor:
-                siggen_freq = self.sensor.get('anc_siggen_ku_frequency')[0]
-                spw_params['centre_freq'] = 100. * siggen_freq + 1284e6
-        # "Fake UHF": a real receiver + L-band digitiser and flipped spectrum
-        elif spw_params['band'] == 'UHF' and bandwidth == 856e6:
-            spw_params['centre_freq'] = 428e6
-            spw_params['sideband'] = -1
-        # If the file has SDP output stream parameters, use those instead
-        num_chans = attrs.get(stream_name + '_n_chans', num_chans)
-        bandwidth = attrs.get(stream_name + '_bandwidth', bandwidth)
-        stream_centre_freq = attrs.get(stream_name + '_center_freq')
-        if stream_centre_freq is not None:
-            spw_params['centre_freq'] = stream_centre_freq
-        # Get channel width from original CBF / SDP parameters
-        spw_params['channel_width'] = bandwidth / num_chans
+        num_chans = attrs['n_chans']
+        bandwidth = attrs['bandwidth']
+        centre_freq = attrs['center_freq']
+        channel_width = bandwidth / num_chans
         # Continue with different channel count, but invalidate centre freq
         # (keep channel width though)
         if source.data and (num_chans != source.data.shape[1]):
             logger.warning('Number of channels reported in metadata (%d) differs'
                            ' from actual number of channels in data (%d) - '
                            'trusting the latter', num_chans, source.data.shape[1])
             num_chans = source.data.shape[1]
-            spw_params.pop('centre_freq', None)
-        # Override centre frequency if provided
-        if centre_freq:
-            spw_params['centre_freq'] = centre_freq
-        if 'centre_freq' not in spw_params:
-            # Choose something really obviously wrong but continue otherwise
-            spw_params['centre_freq'] = 0.0
-            logger.warning('Could not figure out centre frequency, setting it to '
-                           '0 Hz - please provide it via centre_freq parameter')
-        spw_params['num_chans'] = num_chans
-        spw_params['product'] = attrs.get('sub_product', '')
+            centre_freq = 0.0
+        product = attrs.get('sub_product', '')
+        sideband = 1
+        band_map = dict(l='L', s='S', u='UHF', x='X')
+        spw_params = (centre_freq, channel_width, num_chans, product, sideband,
+                      band_map[band])
         # We only expect a single spectral window within a single v4 data set
-        self.spectral_windows = spws = [SpectralWindow(**spw_params)]
-        self.sensor['Observation/spw'] = CategoricalData(spws, [0, num_dumps])
-        self.sensor['Observation/spw_index'] = CategoricalData([0], [0, num_dumps])
+        self.spectral_windows = spws = [SpectralWindow(*spw_params)]
+        self.sensor['Observation/spw'] = CategoricalData(spws, all_dumps)
+        self.sensor['Observation/spw_index'] = CategoricalData([0], all_dumps)
 
         # ------ Extract scans / compound scans / targets ------
 
         # Use the activity sensor of reference antenna to partition the data
         # set into scans (and to set their states)
         scan = self.sensor.get(self.ref_ant + '_activity')
         # If the antenna starts slewing on the second dump, incorporate the
@@ -290,15 +231,15 @@
         if len(scan) > 1 and scan.events[1] == 1 and scan[1] == 'slew':
             scan.events, scan.indices = scan.events[1:], scan.indices[1:]
             scan.events[0] = 0
         # Use labels to partition the data set into compound scans
         try:
             label = self.sensor.get('obs_label')
         except KeyError:
-            label = CategoricalData([''], [0, num_dumps])
+            label = CategoricalData([''], all_dumps)
         # Discard empty labels (typically found in raster scans, where first
         # scan has proper label and rest are empty) However, if all labels are
         # empty, keep them, otherwise whole data set will be one pathological
         # compscan...
         if len(label.unique_values) > 1:
             label.remove('')
         # Create duplicate scan events where labels are set during a scan
@@ -343,46 +284,138 @@
         self._fix_flux_freq_range()
 
         # Apply default selection and initialise all members that depend
         # on selection in the process
         self.select(spw=0, subarray=0, ants=obs_ants)
 
     @property
+    def _flags_keep(self):
+        # Reverse flag indices as np.packbits has bit 0 as the MSB (we want LSB)
+        selection = np.flipud(np.unpackbits(self._flags_select))
+        assert len(FLAG_NAMES) == len(selection), \
+            'Expected %d flag types, got %s' % (len(selection), FLAG_NAMES)
+        return [name for name, bit in zip(FLAG_NAMES, selection) if bit]
+
+    @_flags_keep.setter
+    def _flags_keep(self, names):
+        # Ensure a sequence of flag names
+        names = FLAG_NAMES if names == 'all' else \
+            names.split(',') if isinstance(names, basestring) else names
+        # Create boolean list for desired flags
+        selection = np.zeros(8, dtype=np.uint8)
+        assert len(FLAG_NAMES) == len(selection), \
+            'Expected %d flag types, got %d' % (len(selection), FLAG_NAMES)
+        for name in names:
+            try:
+                selection[FLAG_NAMES.index(name)] = 1
+            except ValueError:
+                logger.warning("%r is not a legitimate flag type, "
+                               "supported ones are %s", name, FLAG_NAMES)
+        # Pack index list into bit mask
+        # Reverse flag indices as np.packbits has bit 0 as the MSB (we want LSB)
+        flagmask = np.packbits(np.flipud(selection))
+        if not flagmask:
+            logger.warning('No valid flags were selected - setting all flags '
+                           'to False by default')
+        self._flags_select = flagmask
+
+    @property
     def timestamps(self):
         """Visibility timestamps in UTC seconds since Unix epoch.
 
         The timestamps are returned as an array of float64, shape (*T*,),
         with one timestamp per integration aligned with the integration
         *midpoint*.
 
         """
-        return self._timestamps[self._time_keep]
+        return self.source.timestamps[self._time_keep]
+
+    @property
+    def vis(self):
+        r"""Complex visibility data as a function of time, frequency and baseline.
+
+        The visibility data are returned as an array indexer of complex64, shape
+        (*T*, *F*, *B*), with time along the first dimension, frequency along the
+        second dimension and correlation product ("baseline") index along the
+        third dimension. The returned array always has all three dimensions,
+        even for scalar (single) values. The number of integrations *T* matches
+        the length of :meth:`timestamps`, the number of frequency channels *F*
+        matches the length of :meth:`freqs` and the number of correlation
+        products *B* matches the length of :meth:`corr_products`. To get the
+        data array itself from the indexer `x`, do `x[:]` or perform any other
+        form of indexing on it. Only then will data be loaded into memory.
+
+        The sign convention of the imaginary part is consistent with an
+        electric field of :math:`e^{i(\omega t - jz)}` i.e. phase that
+        increases with time.
+        """
+        # Create first-stage index from dataset selectors
+        stage1 = (self._time_keep, self._freq_keep, self._corrprod_keep)
+        return DaskLazyIndexer(self.source.data.vis, stage1)
+
+    @property
+    def weights(self):
+        """Visibility weights as a function of time, frequency and baseline.
+
+        The weights data are returned as an array indexer of float32, shape
+        (*T*, *F*, *B*), with time along the first dimension, frequency along the
+        second dimension and correlation product ("baseline") index along the
+        third dimension. The number of integrations *T* matches the length of
+        :meth:`timestamps`, the number of frequency channels *F* matches the
+        length of :meth:`freqs` and the number of correlation products *B*
+        matches the length of :meth:`corr_products`. To get the data array
+        itself from the indexer `x`, do `x[:]` or perform any other form of
+        indexing on it. Only then will data be loaded into memory.
+
+        """
+        stage1 = (self._time_keep, self._freq_keep, self._corrprod_keep)
+        return DaskLazyIndexer(self.source.data.weights, stage1)
+
+    @property
+    def flags(self):
+        """Flags as a function of time, frequency and baseline.
+
+        The flags data are returned as an array indexer of bool, shape
+        (*T*, *F*, *B*), with time along the first dimension, frequency along the
+        second dimension and correlation product ("baseline") index along the
+        third dimension. The number of integrations *T* matches the length of
+        :meth:`timestamps`, the number of frequency channels *F* matches the
+        length of :meth:`freqs` and the number of correlation products *B*
+        matches the length of :meth:`corr_products`. To get the data array
+        itself from the indexer `x`, do `x[:]` or perform any other form of
+        indexing on it. Only then will data be loaded into memory.
+
+        """
+        stage1 = (self._time_keep, self._freq_keep, self._corrprod_keep)
+        flags = self.source.data.flags
+        flags = np.bitwise_and(self._flags_select, flags).view(np.bool_)
+        return DaskLazyIndexer(flags, stage1)
 
     @property
     def temperature(self):
         """Air temperature in degrees Celsius."""
-        names = ['anc_weather_temperature']
+        names = ['anc_air_temperature']
         return self.sensor.get_with_fallback('temperature', names)
 
     @property
     def pressure(self):
         """Barometric pressure in millibars."""
-        names = ['anc_weather_pressure']
+        names = ['anc_air_pressure']
         return self.sensor.get_with_fallback('pressure', names)
 
     @property
     def humidity(self):
         """Relative humidity as a percentage."""
-        names = ['anc_weather_humidity']
+        names = ['anc_air_relative_humidity']
         return self.sensor.get_with_fallback('humidity', names)
 
     @property
     def wind_speed(self):
         """Wind speed in metres per second."""
-        names = ['anc_weather_wind_speed']
+        names = ['anc_mean_wind_speed']
         return self.sensor.get_with_fallback('wind_speed', names)
 
     @property
     def wind_direction(self):
         """Wind direction as an azimuth angle in degrees."""
-        names = ['anc_weather_wind_direction']
+        names = ['anc_wind_direction']
         return self.sensor.get_with_fallback('wind_direction', names)
```

### Comparing `katdal-0.9/katdal.egg-info/PKG-INFO` & `katdal-0.9.5/katdal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: katdal
-Version: 0.9
+Version: 0.9.5
 Summary: Karoo Array Telescope data access library to interact with HDF5 and MS files
 Home-page: https://github.com/ska-sa/katdal
 Author: Ludwig Schwardt
 Author-email: ludwig@ska.ac.za
 License: Modified BSD
 Description-Content-Type: UNKNOWN
 Description: katdal
@@ -220,14 +220,21 @@
         available at ``d.catalogue``, and the original HDF5 file is still accessible via
         a back door installed at ``d.file`` in the case of a single-file data set.
         
         
         History
         =======
         
+        0.9.5 (2018-02-22)
+        ------------------
+        * New HDF5 v3.9 file format in anticipation of v4 (affects obs_params)
+        * Fix receiver serial numbers in recent MeerKAT data sets
+        * Add dask support to ChunkStore
+        * katdal.open() works on v4 RDB files
+        
         0.9 (2018-01-16)
         ----------------
         * New ChunkStore and telstate-based parser for future v4 format
         * Use python-casacore (>=2.2.1) to create Measurement Sets instead of blank.ms
         * Read new-style noise diode sensor names, serial numbers and L0 stream metadata
         * Select multiple polarisations (useful for cross-pol)
         * Relax the "expected number of dumps" check to avoid spurious warnings
```

### Comparing `katdal-0.9/katdal.egg-info/SOURCES.txt` & `katdal-0.9.5/katdal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `katdal-0.9/PKG-INFO` & `katdal-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: katdal
-Version: 0.9
+Version: 0.9.5
 Summary: Karoo Array Telescope data access library to interact with HDF5 and MS files
 Home-page: https://github.com/ska-sa/katdal
 Author: Ludwig Schwardt
 Author-email: ludwig@ska.ac.za
 License: Modified BSD
 Description-Content-Type: UNKNOWN
 Description: katdal
@@ -220,14 +220,21 @@
         available at ``d.catalogue``, and the original HDF5 file is still accessible via
         a back door installed at ``d.file`` in the case of a single-file data set.
         
         
         History
         =======
         
+        0.9.5 (2018-02-22)
+        ------------------
+        * New HDF5 v3.9 file format in anticipation of v4 (affects obs_params)
+        * Fix receiver serial numbers in recent MeerKAT data sets
+        * Add dask support to ChunkStore
+        * katdal.open() works on v4 RDB files
+        
         0.9 (2018-01-16)
         ----------------
         * New ChunkStore and telstate-based parser for future v4 format
         * Use python-casacore (>=2.2.1) to create Measurement Sets instead of blank.ms
         * Read new-style noise diode sensor names, serial numbers and L0 stream metadata
         * Select multiple polarisations (useful for cross-pol)
         * Relax the "expected number of dumps" check to avoid spurious warnings
```

### Comparing `katdal-0.9/README.rst` & `katdal-0.9.5/README.rst`

 * *Files identical despite different names*

### Comparing `katdal-0.9/scripts/fix_ant_positions.py` & `katdal-0.9.5/scripts/fix_ant_positions.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/scripts/h5list.py` & `katdal-0.9.5/scripts/h5list.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/scripts/h5toms.py` & `katdal-0.9.5/scripts/h5toms.py`

 * *Files identical despite different names*

### Comparing `katdal-0.9/setup.py` & `katdal-0.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,8 +58,8 @@
       install_requires=['numpy', 'katpoint', 'h5py'],
       extras_require={
         'ms': ['python-casacore >= 2.2.1'],
         's3': ['botocore'],
         # rados is not in PyPI but available as Debian package python-rados
         'rados': ['rados']
       },
-      tests_require=['nose'])
+      tests_require=['nose', 'dask[array]'])
```

