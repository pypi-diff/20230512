# Comparing `tmp/imgio-0.9.2.tar.gz` & `tmp/imgio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgio-0.9.2.tar", last modified: Tue Mar 14 15:39:23 2023, max compression
+gzip compressed data, was "imgio-0.9.3.tar", last modified: Fri May 12 13:31:44 2023, max compression
```

## Comparing `imgio-0.9.2.tar` & `imgio-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-14 15:39:23.932439 imgio-0.9.2/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-0.9.2/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-0.9.2/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-03-14 15:39:23.932439 imgio-0.9.2/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-0.9.2/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-14 15:39:23.928439 imgio-0.9.2/imgio/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-03-14 15:16:30.000000 imgio-0.9.2/imgio/__init__.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    29914 2023-03-14 15:22:53.000000 imgio-0.9.2/imgio/imgio.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4168 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/pfm.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4580 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/pnm.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-14 15:39:23.932439 imgio-0.9.2/imgio/test-images/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/GrayRampsDiagonal.exr
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/landscape_8.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_1.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_2.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_3.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_4.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_5.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_6.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_7.jpg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-0.9.2/imgio/test-images/portrait_8.jpg
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-14 15:39:23.928439 imgio-0.9.2/imgio.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/not-zip-safe
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-03-14 15:39:23.000000 imgio-0.9.2/imgio.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       46 2023-03-14 15:16:06.000000 imgio-0.9.2/requirements.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-03-14 15:39:23.932439 imgio-0.9.2/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-0.9.2/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 13:31:44.625995 imgio-0.9.3/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imgio-0.9.3/LICENSE
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       87 2023-03-13 15:45:56.000000 imgio-0.9.3/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-12 13:31:44.625995 imgio-0.9.3/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      661 2023-03-14 15:37:15.000000 imgio-0.9.3/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 13:31:44.621995 imgio-0.9.3/imgio/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      312 2023-05-12 13:30:33.000000 imgio-0.9.3/imgio/__init__.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    29811 2023-05-12 13:11:45.000000 imgio-0.9.3/imgio/imgio.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4168 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/pfm.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4580 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/pnm.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 13:31:44.625995 imgio-0.9.3/imgio/test-images/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    62336 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/GrayRampsDiagonal.exr
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   139435 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137359 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140965 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140588 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137611 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   137628 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   140645 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   141286 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/landscape_8.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   129059 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_1.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136072 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_2.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135813 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_3.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   131520 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_4.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   133715 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_5.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   136257 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_6.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   135366 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_7.jpg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)   132543 2023-03-13 15:45:56.000000 imgio-0.9.3/imgio/test-images/portrait_8.jpg
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-12 13:31:44.621995 imgio-0.9.3/imgio.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      253 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      872 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/not-zip-safe
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       40 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        6 2023-05-12 13:31:44.000000 imgio-0.9.3/imgio.egg-info/top_level.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       46 2023-03-14 15:16:06.000000 imgio-0.9.3/requirements.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      128 2023-05-12 13:31:44.625995 imgio-0.9.3/setup.cfg
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      605 2023-03-13 15:45:56.000000 imgio-0.9.3/setup.py
```

### Comparing `imgio-0.9.2/LICENSE` & `imgio-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/README.md` & `imgio-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/imgio.py` & `imgio-0.9.3/imgio/imgio.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,23 @@
         _enforce(pyexr is not None, "OpenEXR support not installed")
         frame, maxval = _reraise(lambda: _read_exr(filespec, verbose))
         return frame, maxval
     if filetype in [".pnm", ".pgm", ".ppm"]:
         frame, maxval = _reraise(lambda: pnm.read(filespec, verbose))
         return frame, maxval
     if filetype in [".png", ".bmp", ".tif", ".tiff", ".jpg", ".jpeg", ".insp"]:
-        _print(verbose, "Reading file %s "%(filespec), end='')
         formatstr = "jpg" if filetype == ".insp" else filetype[1:]
         frame = _reraise(lambda: _imread.imread(filespec, formatstr=formatstr))
         maxval = 255 if frame.dtype == np.uint8 else 65535
         must_squeeze = (frame.ndim > 2 and frame.shape[2] == 1)
         frame = frame.squeeze(axis=2) if must_squeeze else frame
         frame = _reraise(lambda: _exif_rotate(frame, filespec))
         h, w = frame.shape[:2]
         c = frame.shape[2] if frame.ndim > 2 else 1
-        _print(verbose, "(w=%d, h=%d, c=%d, maxval=%d)"%(w, h, c, maxval))
+        _print(verbose, "Reading file %s (w=%d, h=%d, c=%d, maxval=%d)"%(filespec, w, h, c, maxval))
         return frame, maxval
     raise ImageIOError("unrecognized file type `%s`."%(filetype))
 
 def imwrite(filespec, image, maxval=255, packed=False, verbose=False):
     """
     Writes the given image to the given file, returns nothing. Grayscale images
     are expected to be provided as NumPy arrays with shape H x W, color images
@@ -127,20 +126,19 @@
         _reraise(lambda: _write_npy(filespec, image, verbose))
     elif filetype in [".pnm", ".pgm", ".ppm"]:
         _reraise(lambda: pnm.write(filespec, image, maxval, verbose))
     elif filetype in [".png", ".tif", ".tiff", ".jpg", ".jpeg", ".insp"]:
         _disallow(image.ndim == 3 and image.shape[2] != 3, "image.shape must be (m, n) or (m, n, 3); was %s."%(str(image.shape)))
         _disallow(filetype in [".jpg", ".jpeg"] and maxval != 255, "maxval must be 255 for a JPEG; was %d."%(maxval))
         _disallow(filetype == ".png" and maxval not in [255, 65535], "maxval must be 255 or 65535 for a PNG; was %d."%(maxval))
-        _print(verbose, "Writing file %s "%(filespec), end='')
         formatstr = "jpg" if filetype == ".insp" else filetype[1:]
         _reraise(lambda: _imread.imsave(filespec, image, formatstr=formatstr, opts={'jpeg:quality': 95}))
         h, w = image.shape[:2]
         c = image.shape[2] if image.ndim > 2 else 1
-        _print(verbose, "(w=%d, h=%d, c=%d, maxval=%d)"%(w, h, c, maxval))
+        _print(verbose, "Writing file %s (w=%d, h=%d, c=%d, maxval=%d)"%(filespec, w, h, c, maxval))
     else:
         raise ImageIOError("unrecognized file type `%s`."%(filetype))
 
 def selftest():
     """
     Runs the full suite of unit tests that comes bundled with the package.
     """
@@ -198,25 +196,24 @@
         img = np.rot90(img, rot90_ccw_steps)  # 0/90/180/270 CCW
     return img
 
 def _read_exr(filespec, verbose=False):
     exr = pyexr.open(filespec)
     data = exr.get()
     maxval = np.max(data)
-    _print(verbose, "Reading OpenEXR file %s "%(filespec), end='')
-    _print(verbose, "(w=%d, h=%d, c=%d, %s)"%(exr.width, exr.height, len(exr.channels), data.dtype))
+    w, h, ch, dt = exr.width, exr.height, len(exr.channels), data.dtype
+    _print(verbose, "Reading OpenEXR file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, dt))
     return data, maxval
 
 def _read_npy(filespec, verbose=False):
     data = np.load(filespec)
     _enforce(data.ndim == 3, "NumPy file %s image has unsupported shape %s"%(filespec, str(data.shape)))
     maxval = np.max(data)
     h, w, ch = data.shape
-    _print(verbose, "Reading NumPy file %s "%(filespec), end='')
-    _print(verbose, "(w=%d, h=%d, c=%d, %s)"%(w, h, ch, data.dtype))
+    _print(verbose, "Reading NumPy file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, data.dtype))
     return data, maxval
 
 def _write_npy(filespec, image, verbose=False):
     _enforce(image.ndim == 3, "image.shape must be (m, n, c) for .npy; was %s."%(str(image.shape)))
     h, w, ch = image.shape
     if verbose:
         print("Writing file %s (w=%d, h=%d, c=%d, %s)"%(filespec, w, h, ch, image.dtype))
@@ -228,16 +225,16 @@
         buf = infile.read()
         shape = (height, width)
         maxval = 2 ** bpp - 1
         wordsize = 2 if bpp > 8 else 1
         packed = len(buf) < (width * height * wordsize)
         if header_size is None:
             header_size = len(buf) - (width * height * wordsize)
-        _print(verbose, "Reading raw Bayer file %s "%(filespec), end='')
-        _print(verbose, "(w=%d, h=%d, maxval=%d, header=%d, packed=%r)"%(width, height, maxval, header_size, packed))
+        fs, w, h, hdrsz = filespec, width, height, header_size
+        _print(verbose, "Reading raw Bayer file %s (w=%d, h=%d, maxval=%d, header=%d, packed=%r)"%(fs, w, h, maxval, hdrsz, packed))
         if not packed:
             dtype = "<u2" if bpp > 8 else np.uint8
             pixels = np.frombuffer(buf, dtype, count=width * height, offset=header_size)
             pixels = pixels.reshape(shape).astype(np.uint8 if bpp <= 8 else np.uint16)
         else:
             # TODO: packed raw support
             raise ImageIOError("Packed RAW reading not implemented yet!")
```

### Comparing `imgio-0.9.2/imgio/pfm.py` & `imgio-0.9.3/imgio/pfm.py`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/pnm.py` & `imgio-0.9.3/imgio/pnm.py`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/GrayRampsDiagonal.exr` & `imgio-0.9.3/imgio/test-images/GrayRampsDiagonal.exr`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_1.jpg` & `imgio-0.9.3/imgio/test-images/landscape_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_2.jpg` & `imgio-0.9.3/imgio/test-images/landscape_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_3.jpg` & `imgio-0.9.3/imgio/test-images/landscape_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_4.jpg` & `imgio-0.9.3/imgio/test-images/landscape_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_5.jpg` & `imgio-0.9.3/imgio/test-images/landscape_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_6.jpg` & `imgio-0.9.3/imgio/test-images/landscape_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_7.jpg` & `imgio-0.9.3/imgio/test-images/landscape_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/landscape_8.jpg` & `imgio-0.9.3/imgio/test-images/landscape_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_1.jpg` & `imgio-0.9.3/imgio/test-images/portrait_1.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_2.jpg` & `imgio-0.9.3/imgio/test-images/portrait_2.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_3.jpg` & `imgio-0.9.3/imgio/test-images/portrait_3.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_4.jpg` & `imgio-0.9.3/imgio/test-images/portrait_4.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_5.jpg` & `imgio-0.9.3/imgio/test-images/portrait_5.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_6.jpg` & `imgio-0.9.3/imgio/test-images/portrait_6.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_7.jpg` & `imgio-0.9.3/imgio/test-images/portrait_7.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio/test-images/portrait_8.jpg` & `imgio-0.9.3/imgio/test-images/portrait_8.jpg`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/imgio.egg-info/SOURCES.txt` & `imgio-0.9.3/imgio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgio-0.9.2/setup.py` & `imgio-0.9.3/setup.py`

 * *Files identical despite different names*

