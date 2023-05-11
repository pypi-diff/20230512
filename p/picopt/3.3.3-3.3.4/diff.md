# Comparing `tmp/picopt-3.3.3.tar.gz` & `tmp/picopt-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopt-3.3.3.tar", max compression
+gzip compressed data, was "picopt-3.3.4.tar", max compression
```

## Comparing `picopt-3.3.3.tar` & `picopt-3.3.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     7482 2023-05-10 21:32:11.250373 picopt-3.3.3/README.md
--rw-r--r--   0        0        0       64 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/__init__.py
--rw-r--r--   0        0        0     7124 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/cli.py
--rw-r--r--   0        0        0    14506 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/config.py
--rw-r--r--   0        0        0      286 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/config_default.yaml
--rw-r--r--   0        0        0      457 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/configurable.py
--rw-r--r--   0        0        0      501 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/data.py
--rw-r--r--   0        0        0       25 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/container.py
--rw-r--r--   0        0        0     5508 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/factory.py
--rw-r--r--   0        0        0     1360 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/gif.py
--rw-r--r--   0        0        0     5667 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/handler.py
--rw-r--r--   0        0        0     2988 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/image.py
--rw-r--r--   0        0        0     1660 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/jpeg.py
--rw-r--r--   0        0        0     1902 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/png.py
--rw-r--r--   0        0        0     4294 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/webp.py
--rw-r--r--   0        0        0     4468 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/webp_animated.py
--rw-r--r--   0        0        0     4042 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/handlers/zip.py
--rw-r--r--   0        0        0     2276 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/old_timestamps.py
--rw-r--r--   0        0        0       22 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/pillow/__init__.py
--rw-r--r--   0        0        0      777 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/pillow/header.py
--rwxr-xr-x   0        0        0     1052 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/pillow/png_bit_depth.py
--rwxr-xr-x   0        0        0      996 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/pillow/webp_lossless.py
--rw-r--r--   0        0        0     2599 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/stats.py
--rw-r--r--   0        0        0    15806 2023-05-10 21:32:11.258373 picopt-3.3.3/picopt/walk.py
--rw-r--r--   0        0        0     4173 2023-05-10 21:32:11.258373 picopt-3.3.3/pyproject.toml
--rw-r--r--   0        0        0      560 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/__init__.py
--rw-r--r--   0        0        0       22 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/__init__.py
--rw-r--r--   0        0        0     2813 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/test_containers.py
--rw-r--r--   0        0        0     4447 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/test_images_dir.py
--rw-r--r--   0        0        0     2454 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/test_old_timestamps.py
--rw-r--r--   0        0        0     1140 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/test_one_container.py
--rw-r--r--   0        0        0     5084 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/integration/test_timestamps.py
--rw-r--r--   0        0        0   292448 2023-05-10 21:32:11.258373 picopt-3.3.3/tests/test_files/containers/igp-twss.epub
--rw-r--r--   0        0        0    93725 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/containers/test_cbr.cbr
--rw-r--r--   0        0        0    93408 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/containers/test_cbz.cbz
--rw-r--r--   0        0        0    93675 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/containers/test_rar.rar
--rw-r--r--   0        0        0     2974 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/containers/test_zip.zip
--rw-r--r--   0        0        0    93676 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/07themecamplist.pdf
--rw-r--r--   0        0        0    59640 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/eight.tif
--rw-r--r--   0        0        0   230578 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/mri.tif
--rw-r--r--   0        0        0    16383 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/test_animated_gif.gif
--rw-r--r--   0        0        0    63435 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/test_animated_png.png
--rw-r--r--   0        0        0    13610 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/test_animated_webp.webp
--rw-r--r--   0        0        0   141430 2023-05-10 21:32:11.262373 picopt-3.3.3/tests/test_files/images/test_bmp.bmp
--rw-r--r--   0        0        0   138952 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_gif.gif
--rw-r--r--   0        0        0    97373 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_jpg.jpg
--rw-r--r--   0        0        0     7967 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_png.png
--rw-r--r--   0        0        0     3435 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_png_16rgba.png
--rw-r--r--   0        0        0    27661 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_pnm.pnm
--rw-r--r--   0        0        0    22664 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_pre-optimized_jpg.jpg
--rw-r--r--   0        0        0   256572 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_pre-optimized_png.png
--rw-r--r--   0        0        0        6 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_txt.txt
--rw-r--r--   0        0        0     5334 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_webp_lossless.webp
--rw-r--r--   0        0        0     8914 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_webp_lossless_pre-optimized.webp
--rw-r--r--   0        0        0     2764 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_webp_lossy.webp
--rw-r--r--   0        0        0     1508 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/images/test_webp_lossy_pre-optimized.webp
--rw-r--r--   0        0        0        3 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/invalid/test_invalid_cbr.cbr
--rw-r--r--   0        0        0        3 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/invalid/test_invalid_cbz.cbz
--rw-r--r--   0        0        0        0 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/invalid/test_invalid_gif.gif
--rw-r--r--   0        0        0        0 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/invalid/test_invalid_jpg.jpg
--rw-r--r--   0        0        0        0 2023-05-10 21:32:11.266373 picopt-3.3.3/tests/test_files/invalid/test_invalid_png.png
--rw-r--r--   0        0        0   879952 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/test_files/invalid/test_mpeg.mpeg
--rw-r--r--   0        0        0       80 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/test_files/invalid/test_rar.rar
--rw-r--r--   0        0        0      167 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/test_files/invalid/test_zip.zip
--rw-r--r--   0        0        0       18 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/unit/__init__.py
--rw-r--r--   0        0        0     1923 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/unit/test_cli.py
--rw-r--r--   0        0        0      871 2023-05-10 21:32:11.270374 picopt-3.3.3/tests/unit/test_png_bit_depth.py
--rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.3/PKG-INFO
+-rw-r--r--   0        0        0     7482 2023-05-11 23:08:13.212386 picopt-3.3.4/README.md
+-rw-r--r--   0        0        0       64 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/__init__.py
+-rw-r--r--   0        0        0     7124 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/cli.py
+-rw-r--r--   0        0        0    14506 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/config.py
+-rw-r--r--   0        0        0      286 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/config_default.yaml
+-rw-r--r--   0        0        0      457 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/configurable.py
+-rw-r--r--   0        0        0      501 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/data.py
+-rw-r--r--   0        0        0       25 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/container.py
+-rw-r--r--   0        0        0     5508 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/factory.py
+-rw-r--r--   0        0        0     1360 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/gif.py
+-rw-r--r--   0        0        0     6071 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/handler.py
+-rw-r--r--   0        0        0     2988 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/image.py
+-rw-r--r--   0        0        0     1875 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/jpeg.py
+-rw-r--r--   0        0        0     1902 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/png.py
+-rw-r--r--   0        0        0     4299 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/webp.py
+-rw-r--r--   0        0        0     4468 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/webp_animated.py
+-rw-r--r--   0        0        0     4047 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/handlers/zip.py
+-rw-r--r--   0        0        0     2276 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/old_timestamps.py
+-rw-r--r--   0        0        0       22 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/pillow/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/pillow/header.py
+-rwxr-xr-x   0        0        0     1052 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/pillow/png_bit_depth.py
+-rwxr-xr-x   0        0        0      996 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/pillow/webp_lossless.py
+-rw-r--r--   0        0        0     2599 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/stats.py
+-rw-r--r--   0        0        0    15806 2023-05-11 23:08:13.220394 picopt-3.3.4/picopt/walk.py
+-rw-r--r--   0        0        0     4173 2023-05-11 23:08:13.220394 picopt-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/test_containers.py
+-rw-r--r--   0        0        0     4447 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/test_images_dir.py
+-rw-r--r--   0        0        0     2454 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/test_old_timestamps.py
+-rw-r--r--   0        0        0     1140 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/test_one_container.py
+-rw-r--r--   0        0        0     5084 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/integration/test_timestamps.py
+-rw-r--r--   0        0        0   292448 2023-05-11 23:08:13.220394 picopt-3.3.4/tests/test_files/containers/igp-twss.epub
+-rw-r--r--   0        0        0    93725 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/containers/test_cbr.cbr
+-rw-r--r--   0        0        0    93408 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/containers/test_cbz.cbz
+-rw-r--r--   0        0        0    93675 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/containers/test_rar.rar
+-rw-r--r--   0        0        0     2974 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/containers/test_zip.zip
+-rw-r--r--   0        0        0    93676 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/07themecamplist.pdf
+-rw-r--r--   0        0        0    59640 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/eight.tif
+-rw-r--r--   0        0        0   230578 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/mri.tif
+-rw-r--r--   0        0        0    16383 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/test_animated_gif.gif
+-rw-r--r--   0        0        0    63435 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/test_animated_png.png
+-rw-r--r--   0        0        0    13610 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/test_animated_webp.webp
+-rw-r--r--   0        0        0   141430 2023-05-11 23:08:13.224398 picopt-3.3.4/tests/test_files/images/test_bmp.bmp
+-rw-r--r--   0        0        0   138952 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_gif.gif
+-rw-r--r--   0        0        0    97373 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_jpg.jpg
+-rw-r--r--   0        0        0     7967 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_png.png
+-rw-r--r--   0        0        0     3435 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_png_16rgba.png
+-rw-r--r--   0        0        0    27661 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_pnm.pnm
+-rw-r--r--   0        0        0    22664 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_pre-optimized_jpg.jpg
+-rw-r--r--   0        0        0   256572 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_pre-optimized_png.png
+-rw-r--r--   0        0        0        6 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_txt.txt
+-rw-r--r--   0        0        0     5334 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_webp_lossless.webp
+-rw-r--r--   0        0        0     8914 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_webp_lossless_pre-optimized.webp
+-rw-r--r--   0        0        0     2764 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_webp_lossy.webp
+-rw-r--r--   0        0        0     1508 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/images/test_webp_lossy_pre-optimized.webp
+-rw-r--r--   0        0        0        3 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/invalid/test_invalid_cbr.cbr
+-rw-r--r--   0        0        0        3 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/invalid/test_invalid_cbz.cbz
+-rw-r--r--   0        0        0        0 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/invalid/test_invalid_gif.gif
+-rw-r--r--   0        0        0        0 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/invalid/test_invalid_jpg.jpg
+-rw-r--r--   0        0        0        0 2023-05-11 23:08:13.228402 picopt-3.3.4/tests/test_files/invalid/test_invalid_png.png
+-rw-r--r--   0        0        0   879952 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/test_files/invalid/test_mpeg.mpeg
+-rw-r--r--   0        0        0       80 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/test_files/invalid/test_rar.rar
+-rw-r--r--   0        0        0      167 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/test_files/invalid/test_zip.zip
+-rw-r--r--   0        0        0       18 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1923 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      871 2023-05-11 23:08:13.232406 picopt-3.3.4/tests/unit/test_png_bit_depth.py
+-rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.4/PKG-INFO
```

### Comparing `picopt-3.3.3/README.md` & `picopt-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/cli.py` & `picopt-3.3.4/picopt/cli.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/config.py` & `picopt-3.3.4/picopt/config.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/container.py` & `picopt-3.3.4/picopt/handlers/container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/factory.py` & `picopt-3.3.4/picopt/handlers/factory.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/gif.py` & `picopt-3.3.4/picopt/handlers/gif.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/handler.py` & `picopt-3.3.4/picopt/handlers/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,63 +69,72 @@
 
     @classmethod
     def native_input_file_formats(cls) -> set[FileFormat]:
         """Return input formats handled without conversion."""
         return {cls.OUTPUT_FILE_FORMAT}
 
     @classmethod
-    def _output_suffix(cls) -> str:
-        """Return the suffix without a leading dot."""
-        return cls.OUTPUT_FORMAT_STR.lower()
-
-    @classmethod
-    def output_suffix(cls) -> str:
-        """Generate the output suffix for the handler."""
-        return "." + cls._output_suffix()
-
-    @classmethod
     def is_handler_available(
         cls,
         convert_handlers: dict,
         available_programs: set,
         file_format: FileFormat,
     ):
         """Can this handler run with available programs."""
         handled_file_formats = cls.native_input_file_formats() | convert_handlers.get(
             cls, set()
         )
         return file_format in handled_file_formats and bool(
             available_programs & set(cls.PROGRAMS.keys())
         )
 
+    @classmethod
+    def get_default_suffix(cls):
+        """Get the default suffix based on the format."""
+        # overridden in jpeg
+        return "." + cls.OUTPUT_FORMAT_STR.lower()
+
+    @classmethod
+    def get_suffixes(cls, default_suffix: str) -> frozenset:
+        """Initialize suffix instance variables."""
+        # overridden in jpeg
+        return frozenset((default_suffix,))
+
     def __init__(
         self,
         config: AttrDict,
         path_info: PathInfo,
         input_file_format: FileFormat,
         metadata: Metadata,
     ):
         """Initialize handler."""
         self.config: AttrDict = config
         self.original_path: Path = path_info.path
         self.working_paths: set[Path] = set()
-        self.final_path: Path = self.original_path.with_suffix(self.output_suffix())
+        default_suffix = self.get_default_suffix()
+        self._suffixes = self.get_suffixes(default_suffix)
+        self.output_suffix: str = (
+            self.original_path.suffix
+            if self.original_path
+            and self.original_path.suffix.lower() in self._suffixes
+            else default_suffix
+        )
+        self.final_path: Path = self.original_path.with_suffix(self.output_suffix)
         self.input_file_format: FileFormat = input_file_format
         self.metadata = metadata
         self.convert = input_file_format != self.OUTPUT_FILE_FORMAT
         self.is_case_sensitive = path_info.is_case_sensitive
 
     def get_working_path(self, identifier: str = "") -> Path:
         """Return a working path with a custom suffix."""
         suffixes = [self.original_path.suffix, self.WORKING_SUFFIX]
         if identifier:
             suffixes += [identifier]
-        suffixes += [self._output_suffix()]
         suffix = ".".join(suffixes)
-
+        suffix += self.output_suffix
         return self.original_path.with_suffix(suffix)
 
     def cleanup_after_optimize(self, last_working_path: Path) -> tuple[int, int]:
         """Replace old file with better one or discard new wasteful file."""
         bytes_in = 0
         bytes_out = 0
         try:
```

### Comparing `picopt-3.3.3/picopt/handlers/image.py` & `picopt-3.3.4/picopt/handlers/image.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/jpeg.py` & `picopt-3.3.4/picopt/handlers/jpeg.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,22 @@
         ("mozjpeg", "jpegtran")
     )
     _ARGS_PREFIX = ["-optimize", "-progressive", "-copy"]
     _MOZJPEG_ARGS_PREFIX = [PROGRAMS["mozjpeg"], *_ARGS_PREFIX]
     _JPEGTRAN_ARGS_PREFIX = [PROGRAMS["jpegtran"], *_ARGS_PREFIX]
 
     @classmethod
-    def _output_suffix(cls) -> str:
-        """JPEG suffix does not match format."""
-        return "jpg"
+    def get_default_suffix(cls) -> str:
+        """Override default suffix for jpeg."""
+        return ".jpg"
+
+    @classmethod
+    def get_suffixes(cls, default_suffix: str) -> frozenset:
+        """Initialize suffix instance variables."""
+        return frozenset((default_suffix, "." + cls.OUTPUT_FORMAT_STR.lower()))
 
     def _jpegtran(self, args: list[str], old_path: Path, new_path: Path) -> Path:
         """Run the jpegtran type program."""
         args = copy(args)
         if not bin:
             return old_path
         if self.config.keep_metadata:
```

### Comparing `picopt-3.3.3/picopt/handlers/png.py` & `picopt-3.3.4/picopt/handlers/png.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/webp.py` & `picopt-3.3.4/picopt/handlers/webp.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def pil2png(self, old_path: Path, new_path: Path) -> Path:
         """Internally convert unhandled formats to uncompressed png for cwebp."""
         if (
             self.input_file_format in self._PIL2PNG_FILE_FORMATS
             and self.PREFERRED_PROGRAM in self.config.computed.available_programs
         ):
-            new_path = new_path.with_suffix(Png.output_suffix())
+            new_path = new_path.with_suffix(Png.get_default_suffix())
             with Image.open(old_path) as image:
                 image.save(
                     new_path,
                     Png.OUTPUT_FORMAT_STR,
                     compress_level=0,
                     exif=self.metadata.exif,
                     icc_profile=self.metadata.icc_profile,
```

### Comparing `picopt-3.3.3/picopt/handlers/webp_animated.py` & `picopt-3.3.4/picopt/handlers/webp_animated.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/handlers/zip.py` & `picopt-3.3.4/picopt/handlers/zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     PROGRAMS: dict[str, Optional[str]] = {ContainerHandler.INTERNAL: None}
 
     @classmethod
     def identify_format(cls, path: Path) -> Optional[FileFormat]:
         """Return the format if this handler can handle this path."""
         file_format = None
         suffix = path.suffix.lower()
-        if is_zipfile(path) and suffix == cls.output_suffix():
+        if is_zipfile(path) and suffix == cls.get_default_suffix():
             file_format = cls.OUTPUT_FILE_FORMAT
         elif is_rarfile(path) and suffix == cls.RAR_SUFFIX:
             file_format = cls.INPUT_FILE_FORMAT_RAR
         return file_format
 
     def _get_archive(self) -> Union[ZipFile, RarFile]:
         """Use the zipfile builtin for this archive."""
```

### Comparing `picopt-3.3.3/picopt/old_timestamps.py` & `picopt-3.3.4/picopt/old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/pillow/header.py` & `picopt-3.3.4/picopt/pillow/header.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/pillow/png_bit_depth.py` & `picopt-3.3.4/picopt/pillow/png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/pillow/webp_lossless.py` & `picopt-3.3.4/picopt/pillow/webp_lossless.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/stats.py` & `picopt-3.3.4/picopt/stats.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/picopt/walk.py` & `picopt-3.3.4/picopt/walk.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/pyproject.toml` & `picopt-3.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = ["poetry.core.masonry.api"]
 
 [tool.poetry]
 name = "picopt"
-version = "3.3.3"
+version = "3.3.4"
 description = "A multi format lossless image optimizer that uses external tools"
 license = "GPL-3.0-only"
 authors = ["AJ Slater <aj@slater.net>"]
 readme = "README.md"
 homepage = "https://github.com/ajslater/picopt"
 documentation = "https://github.com/ajslater/picopt"
 keywords = ["image", "png", "jpg", "cbz", "cbr"]
```

### Comparing `picopt-3.3.3/tests/__init__.py` & `picopt-3.3.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/integration/test_containers.py` & `picopt-3.3.4/tests/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/integration/test_images_dir.py` & `picopt-3.3.4/tests/integration/test_images_dir.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/integration/test_old_timestamps.py` & `picopt-3.3.4/tests/integration/test_old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/integration/test_one_container.py` & `picopt-3.3.4/tests/integration/test_one_container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/integration/test_timestamps.py` & `picopt-3.3.4/tests/integration/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/containers/igp-twss.epub` & `picopt-3.3.4/tests/test_files/containers/igp-twss.epub`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/containers/test_cbr.cbr` & `picopt-3.3.4/tests/test_files/containers/test_cbr.cbr`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/containers/test_cbz.cbz` & `picopt-3.3.4/tests/test_files/containers/test_cbz.cbz`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/containers/test_rar.rar` & `picopt-3.3.4/tests/test_files/containers/test_rar.rar`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/containers/test_zip.zip` & `picopt-3.3.4/tests/test_files/containers/test_zip.zip`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/07themecamplist.pdf` & `picopt-3.3.4/tests/test_files/images/07themecamplist.pdf`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/eight.tif` & `picopt-3.3.4/tests/test_files/images/eight.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/mri.tif` & `picopt-3.3.4/tests/test_files/images/mri.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_animated_gif.gif` & `picopt-3.3.4/tests/test_files/images/test_animated_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_animated_png.png` & `picopt-3.3.4/tests/test_files/images/test_animated_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_animated_webp.webp` & `picopt-3.3.4/tests/test_files/images/test_animated_webp.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_bmp.bmp` & `picopt-3.3.4/tests/test_files/images/test_bmp.bmp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_gif.gif` & `picopt-3.3.4/tests/test_files/images/test_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_jpg.jpg` & `picopt-3.3.4/tests/test_files/images/test_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_png.png` & `picopt-3.3.4/tests/test_files/images/test_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_png_16rgba.png` & `picopt-3.3.4/tests/test_files/images/test_png_16rgba.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_pnm.pnm` & `picopt-3.3.4/tests/test_files/images/test_pnm.pnm`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_pre-optimized_jpg.jpg` & `picopt-3.3.4/tests/test_files/images/test_pre-optimized_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_pre-optimized_png.png` & `picopt-3.3.4/tests/test_files/images/test_pre-optimized_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_webp_lossless.webp` & `picopt-3.3.4/tests/test_files/images/test_webp_lossless.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_webp_lossless_pre-optimized.webp` & `picopt-3.3.4/tests/test_files/images/test_webp_lossless_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_webp_lossy.webp` & `picopt-3.3.4/tests/test_files/images/test_webp_lossy.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/images/test_webp_lossy_pre-optimized.webp` & `picopt-3.3.4/tests/test_files/images/test_webp_lossy_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/test_files/invalid/test_mpeg.mpeg` & `picopt-3.3.4/tests/test_files/invalid/test_mpeg.mpeg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/unit/test_cli.py` & `picopt-3.3.4/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/tests/unit/test_png_bit_depth.py` & `picopt-3.3.4/tests/unit/test_png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.3/PKG-INFO` & `picopt-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopt
-Version: 3.3.3
+Version: 3.3.4
 Summary: A multi format lossless image optimizer that uses external tools
 Home-page: https://github.com/ajslater/picopt
 License: GPL-3.0-only
 Keywords: image,png,jpg,cbz,cbr
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
```

