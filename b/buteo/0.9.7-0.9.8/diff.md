# Comparing `tmp/buteo-0.9.7.tar.gz` & `tmp/buteo-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buteo-0.9.7.tar", last modified: Fri May 12 11:18:57 2023, max compression
+gzip compressed data, was "buteo-0.9.8.tar", last modified: Fri May 12 13:35:34 2023, max compression
```

## Comparing `buteo-0.9.7.tar` & `buteo-0.9.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.7/LICENSE
--rw-r--r--   0        0        0     4779 2023-05-09 11:35:41.351219 buteo-0.9.7/buteo/__init__.py
--rw-r--r--   0        0        0      222 2023-05-09 11:50:06.491154 buteo-0.9.7/buteo/ai/__init__.py
--rw-r--r--   0        0        0     9723 2023-05-12 11:16:29.988305 buteo-0.9.7/buteo/ai/augmentation.py
--rw-r--r--   0        0        0    28002 2023-05-09 12:27:55.018873 buteo-0.9.7/buteo/ai/augmentation_funcs.py
--rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.7/buteo/ai/augmentation_utils.py
--rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.7/buteo/ai/encoding.py
--rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.7/buteo/ai/scalers.py
--rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.7/buteo/ai/selection.py
--rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.7/buteo/array/__init__.py
--rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.7/buteo/array/color.py
--rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.7/buteo/array/convolution.py
--rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.7/buteo/array/convolution_distance.py
--rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.7/buteo/array/convolution_funcs.py
--rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.7/buteo/array/convolution_kernels.py
--rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.7/buteo/array/edge_detection.py
--rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.7/buteo/array/fill.py
--rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.7/buteo/array/filters.py
--rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.7/buteo/array/morphology.py
--rw-r--r--   0        0        0    31304 2023-05-12 08:46:36.605401 buteo-0.9.7/buteo/array/patches.py
--rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.7/buteo/array/timeseries.py
--rw-r--r--   0        0        0     2819 2023-05-09 11:52:21.206628 buteo-0.9.7/buteo/array/utils_array.py
--rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.7/buteo/eo/__init__.py
--rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/L2A_GIPP.xml
--rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/step_01_backstatter.xml
--rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/step_01_coherence.xml
--rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/step_02_backscatter.xml
--rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/step_02_backscatter_speckle.xml
--rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.7/buteo/eo/graphs/step_02_coherence.xml
--rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.7/buteo/eo/s1_preprocess.py
--rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.7/buteo/eo/s1_utils.py
--rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.7/buteo/eo/s2_indices.py
--rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.7/buteo/eo/s2_utils.py
--rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.7/buteo/raster/__init__.py
--rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.7/buteo/raster/align.py
--rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.7/buteo/raster/borders.py
--rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.7/buteo/raster/clip.py
--rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.7/buteo/raster/coordinates.py
--rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.7/buteo/raster/core_offsets.py
--rw-r--r--   0        0        0    18432 2023-05-10 07:50:31.889375 buteo-0.9.7/buteo/raster/core_raster.py
--rw-r--r--   0        0        0    37055 2023-05-12 11:11:07.920206 buteo-0.9.7/buteo/raster/core_raster_io.py
--rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.7/buteo/raster/core_stack.py
--rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.7/buteo/raster/datatype.py
--rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.7/buteo/raster/dem.py
--rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.7/buteo/raster/grid.py
--rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.7/buteo/raster/metadata.py
--rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.7/buteo/raster/nodata.py
--rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.7/buteo/raster/proximity.py
--rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.7/buteo/raster/reproject.py
--rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.7/buteo/raster/resample.py
--rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.7/buteo/raster/shift.py
--rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.7/buteo/raster/vectorize.py
--rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.7/buteo/utils/__init__.py
--rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.7/buteo/utils/utils_aux.py
--rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.7/buteo/utils/utils_base.py
--rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.7/buteo/utils/utils_bbox.py
--rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.7/buteo/utils/utils_gdal.py
--rw-r--r--   0        0        0     8848 2023-05-12 08:52:50.076953 buteo-0.9.7/buteo/utils/utils_io.py
--rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.7/buteo/utils/utils_path.py
--rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.7/buteo/utils/utils_projection.py
--rw-r--r--   0        0        0    16744 2023-05-09 10:16:56.513576 buteo-0.9.7/buteo/utils/utils_translate.py
--rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.7/buteo/vector/__init__.py
--rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.7/buteo/vector/buffer.py
--rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.7/buteo/vector/clip.py
--rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/convert_parts.py
--rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.7/buteo/vector/core_vector.py
--rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/dissolve.py
--rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.7/buteo/vector/grid.py
--rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/intersect.py
--rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/merge.py
--rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/metadata.py
--rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.7/buteo/vector/rasterize.py
--rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.7/buteo/vector/reproject.py
--rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.7/buteo/vector/shapes.py
--rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.7/buteo/vector/split.py
--rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.7/buteo/vector/zonal_statistics.py
--rw-r--r--   0        0        0      785 2023-05-12 11:16:57.781452 buteo-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.7/readme.md
--rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-03-07 09:20:18.869934 buteo-0.9.8/LICENSE
+-rw-r--r--   0        0        0     4779 2023-05-09 11:35:41.351219 buteo-0.9.8/buteo/__init__.py
+-rw-r--r--   0        0        0      222 2023-05-09 11:50:06.491154 buteo-0.9.8/buteo/ai/__init__.py
+-rw-r--r--   0        0        0     9723 2023-05-12 11:16:29.988305 buteo-0.9.8/buteo/ai/augmentation.py
+-rw-r--r--   0        0        0    28002 2023-05-09 12:27:55.018873 buteo-0.9.8/buteo/ai/augmentation_funcs.py
+-rw-r--r--   0        0        0     5632 2023-04-28 10:13:19.277505 buteo-0.9.8/buteo/ai/augmentation_utils.py
+-rw-r--r--   0        0        0    12666 2023-04-27 12:08:41.855227 buteo-0.9.8/buteo/ai/encoding.py
+-rw-r--r--   0        0        0    13346 2023-04-27 12:10:59.465989 buteo-0.9.8/buteo/ai/scalers.py
+-rw-r--r--   0        0        0     7952 2023-05-04 12:07:45.359917 buteo-0.9.8/buteo/ai/selection.py
+-rw-r--r--   0        0        0      408 2023-05-03 11:12:45.284473 buteo-0.9.8/buteo/array/__init__.py
+-rw-r--r--   0        0        0     5365 2023-05-02 12:17:14.771058 buteo-0.9.8/buteo/array/color.py
+-rw-r--r--   0        0        0    16282 2023-05-05 12:25:08.221262 buteo-0.9.8/buteo/array/convolution.py
+-rw-r--r--   0        0        0     3808 2023-05-08 13:11:10.703319 buteo-0.9.8/buteo/array/convolution_distance.py
+-rw-r--r--   0        0        0    12279 2023-04-30 17:19:03.247105 buteo-0.9.8/buteo/array/convolution_funcs.py
+-rw-r--r--   0        0        0    15308 2023-05-03 14:21:39.376562 buteo-0.9.8/buteo/array/convolution_kernels.py
+-rw-r--r--   0        0        0     2634 2023-05-03 14:18:12.376178 buteo-0.9.8/buteo/array/edge_detection.py
+-rw-r--r--   0        0        0     4090 2023-05-03 14:09:36.372639 buteo-0.9.8/buteo/array/fill.py
+-rw-r--r--   0        0        0    10639 2023-05-05 12:27:09.566352 buteo-0.9.8/buteo/array/filters.py
+-rw-r--r--   0        0        0     7902 2023-05-05 12:33:39.152123 buteo-0.9.8/buteo/array/morphology.py
+-rw-r--r--   0        0        0    31384 2023-05-12 13:33:23.446975 buteo-0.9.8/buteo/array/patches.py
+-rw-r--r--   0        0        0     2513 2023-05-03 14:16:07.383138 buteo-0.9.8/buteo/array/timeseries.py
+-rw-r--r--   0        0        0     2819 2023-05-09 11:52:21.206628 buteo-0.9.8/buteo/array/utils_array.py
+-rw-r--r--   0        0        0      155 2023-04-12 12:14:08.281651 buteo-0.9.8/buteo/eo/__init__.py
+-rw-r--r--   0        0        0     5677 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/L2A_GIPP.xml
+-rw-r--r--   0        0        0     3552 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_01_backstatter.xml
+-rw-r--r--   0        0        0    12077 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_01_coherence.xml
+-rw-r--r--   0        0        0     3572 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_backscatter.xml
+-rw-r--r--   0        0        0     4299 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_backscatter_speckle.xml
+-rw-r--r--   0        0        0     3712 2022-08-16 15:39:47.000000 buteo-0.9.8/buteo/eo/graphs/step_02_coherence.xml
+-rw-r--r--   0        0        0    10510 2023-05-08 18:31:03.565806 buteo-0.9.8/buteo/eo/s1_preprocess.py
+-rw-r--r--   0        0        0     2133 2023-05-03 09:56:32.765943 buteo-0.9.8/buteo/eo/s1_utils.py
+-rw-r--r--   0        0        0     9188 2023-05-03 09:56:39.496000 buteo-0.9.8/buteo/eo/s2_indices.py
+-rw-r--r--   0        0        0    12465 2023-05-08 15:14:09.972611 buteo-0.9.8/buteo/eo/s2_utils.py
+-rw-r--r--   0        0        0      497 2023-05-05 06:20:35.014620 buteo-0.9.8/buteo/raster/__init__.py
+-rw-r--r--   0        0        0    16663 2023-05-08 13:09:19.688308 buteo-0.9.8/buteo/raster/align.py
+-rw-r--r--   0        0        0     7299 2023-05-05 17:25:56.416262 buteo-0.9.8/buteo/raster/borders.py
+-rw-r--r--   0        0        0    13523 2023-05-08 15:16:27.420173 buteo-0.9.8/buteo/raster/clip.py
+-rw-r--r--   0        0        0     1510 2023-05-08 06:54:59.813075 buteo-0.9.8/buteo/raster/coordinates.py
+-rw-r--r--   0        0        0     9674 2023-05-05 10:46:19.677097 buteo-0.9.8/buteo/raster/core_offsets.py
+-rw-r--r--   0        0        0    18432 2023-05-10 07:50:31.889375 buteo-0.9.8/buteo/raster/core_raster.py
+-rw-r--r--   0        0        0    37055 2023-05-12 11:11:07.920206 buteo-0.9.8/buteo/raster/core_raster_io.py
+-rw-r--r--   0        0        0    10157 2023-05-05 12:25:08.222263 buteo-0.9.8/buteo/raster/core_stack.py
+-rw-r--r--   0        0        0     7431 2023-05-08 07:41:05.893227 buteo-0.9.8/buteo/raster/datatype.py
+-rw-r--r--   0        0        0     8331 2023-05-08 08:18:57.689620 buteo-0.9.8/buteo/raster/dem.py
+-rw-r--r--   0        0        0     6231 2023-05-08 07:52:34.295257 buteo-0.9.8/buteo/raster/grid.py
+-rw-r--r--   0        0        0     4079 2023-05-08 13:07:43.602719 buteo-0.9.8/buteo/raster/metadata.py
+-rw-r--r--   0        0        0     8386 2023-05-08 09:51:45.634002 buteo-0.9.8/buteo/raster/nodata.py
+-rw-r--r--   0        0        0     6167 2023-05-08 13:49:35.641110 buteo-0.9.8/buteo/raster/proximity.py
+-rw-r--r--   0        0        0     9300 2023-05-08 11:56:10.990154 buteo-0.9.8/buteo/raster/reproject.py
+-rw-r--r--   0        0        0    10673 2023-05-08 13:04:45.244156 buteo-0.9.8/buteo/raster/resample.py
+-rw-r--r--   0        0        0     8041 2023-05-08 13:37:41.583753 buteo-0.9.8/buteo/raster/shift.py
+-rw-r--r--   0        0        0     4318 2023-05-08 13:48:24.329191 buteo-0.9.8/buteo/raster/vectorize.py
+-rw-r--r--   0        0        0      298 2023-05-03 14:19:58.866941 buteo-0.9.8/buteo/utils/__init__.py
+-rw-r--r--   0        0        0     4536 2023-05-05 12:25:22.517045 buteo-0.9.8/buteo/utils/utils_aux.py
+-rw-r--r--   0        0        0     9459 2023-05-05 12:26:38.230306 buteo-0.9.8/buteo/utils/utils_base.py
+-rw-r--r--   0        0        0    33937 2023-05-07 07:53:13.792610 buteo-0.9.8/buteo/utils/utils_bbox.py
+-rw-r--r--   0        0        0    28852 2023-05-09 07:50:41.612053 buteo-0.9.8/buteo/utils/utils_gdal.py
+-rw-r--r--   0        0        0     8848 2023-05-12 08:52:50.076953 buteo-0.9.8/buteo/utils/utils_io.py
+-rw-r--r--   0        0        0    28485 2023-05-08 09:46:50.435511 buteo-0.9.8/buteo/utils/utils_path.py
+-rw-r--r--   0        0        0    18880 2023-05-08 14:44:59.714163 buteo-0.9.8/buteo/utils/utils_projection.py
+-rw-r--r--   0        0        0    16744 2023-05-09 10:16:56.513576 buteo-0.9.8/buteo/utils/utils_translate.py
+-rw-r--r--   0        0        0      377 2023-05-08 15:17:25.536089 buteo-0.9.8/buteo/vector/__init__.py
+-rw-r--r--   0        0        0     5661 2023-05-09 08:20:47.551957 buteo-0.9.8/buteo/vector/buffer.py
+-rw-r--r--   0        0        0     6639 2023-05-09 08:45:14.629449 buteo-0.9.8/buteo/vector/clip.py
+-rw-r--r--   0        0        0    13506 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/convert_parts.py
+-rw-r--r--   0        0        0    24435 2023-05-09 08:19:00.716883 buteo-0.9.8/buteo/vector/core_vector.py
+-rw-r--r--   0        0        0     6187 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/dissolve.py
+-rw-r--r--   0        0        0      263 2023-05-02 12:27:13.705244 buteo-0.9.8/buteo/vector/grid.py
+-rw-r--r--   0        0        0     6529 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/intersect.py
+-rw-r--r--   0        0        0     1926 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/merge.py
+-rw-r--r--   0        0        0     7523 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/metadata.py
+-rw-r--r--   0        0        0     6936 2023-05-08 15:13:20.218015 buteo-0.9.8/buteo/vector/rasterize.py
+-rw-r--r--   0        0        0     4870 2023-05-09 09:04:48.200349 buteo-0.9.8/buteo/vector/reproject.py
+-rw-r--r--   0        0        0     6973 2023-05-08 15:13:20.210020 buteo-0.9.8/buteo/vector/shapes.py
+-rw-r--r--   0        0        0     2637 2023-05-09 08:37:35.507047 buteo-0.9.8/buteo/vector/split.py
+-rw-r--r--   0        0        0    18080 2023-05-08 07:22:45.435592 buteo-0.9.8/buteo/vector/zonal_statistics.py
+-rw-r--r--   0        0        0      785 2023-05-12 13:33:46.713793 buteo-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     4710 2023-04-23 13:45:46.888099 buteo-0.9.8/readme.md
+-rw-r--r--   0        0        0     5170 1970-01-01 00:00:00.000000 buteo-0.9.8/PKG-INFO
```

### Comparing `buteo-0.9.7/LICENSE` & `buteo-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/__init__.py` & `buteo-0.9.8/buteo/__init__.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/augmentation.py` & `buteo-0.9.8/buteo/ai/augmentation.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/augmentation_funcs.py` & `buteo-0.9.8/buteo/ai/augmentation_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/augmentation_utils.py` & `buteo-0.9.8/buteo/ai/augmentation_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/encoding.py` & `buteo-0.9.8/buteo/ai/encoding.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/scalers.py` & `buteo-0.9.8/buteo/ai/scalers.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/ai/selection.py` & `buteo-0.9.8/buteo/ai/selection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/color.py` & `buteo-0.9.8/buteo/array/color.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/convolution.py` & `buteo-0.9.8/buteo/array/convolution.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/convolution_distance.py` & `buteo-0.9.8/buteo/array/convolution_distance.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/convolution_funcs.py` & `buteo-0.9.8/buteo/array/convolution_funcs.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/convolution_kernels.py` & `buteo-0.9.8/buteo/array/convolution_kernels.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/edge_detection.py` & `buteo-0.9.8/buteo/array/edge_detection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/fill.py` & `buteo-0.9.8/buteo/array/fill.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/filters.py` & `buteo-0.9.8/buteo/array/filters.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/morphology.py` & `buteo-0.9.8/buteo/array/morphology.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/patches.py` & `buteo-0.9.8/buteo/array/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -704,19 +704,18 @@
 
     # Get the list of offsets for both x and y dimensions
     offsets = _get_offsets(tile_size, n_offsets)
 
     if border_check:
         borders_y, borders_x = _borders_are_necessary_list(arr, tile_size, offsets)
 
-        if borders_y:
-            offsets.append((arr.shape[0] - tile_size, 0))
-        if borders_x:
+        # TODO: Investigate how to handle smarter. Currently we might get duplicates.
+        if borders_y or borders_x:
             offsets.append((0, arr.shape[1] - tile_size))
-        if borders_y and borders_x:
+            offsets.append((arr.shape[0] - tile_size, 0))
             offsets.append((arr.shape[0] - tile_size, arr.shape[1] - tile_size))
 
     # Initialize an empty list to store the generated patches
     patches = []
 
     # Iterate through the offsets and generate patches for each offset
     for offset in offsets:
@@ -772,19 +771,18 @@
 
     # Get the list of offsets for both x and y dimensions
     offsets = _get_offsets(tile_size, n_offsets)
 
     if border_check:
         borders_y, borders_x = _borders_are_necessary_list(arr, tile_size, offsets)
 
-        if borders_y:
-            offsets.append((arr.shape[0] - tile_size, 0))
-        if borders_x:
+        # TODO: Investigate how to handle smarter. Currently we might get duplicates.
+        if borders_y or borders_x:
             offsets.append((0, arr.shape[1] - tile_size))
-        if borders_y and borders_x:
+            offsets.append((arr.shape[0] - tile_size, 0))
             offsets.append((arr.shape[0] - tile_size, arr.shape[1] - tile_size))
 
     # Test output dimensions of prediction
     test_patch = arr[np.newaxis, :tile_size, :tile_size, :]
     test_prediction = callback(test_patch)
     test_shape = test_prediction.shape
```

### Comparing `buteo-0.9.7/buteo/array/timeseries.py` & `buteo-0.9.8/buteo/array/timeseries.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/array/utils_array.py` & `buteo-0.9.8/buteo/array/utils_array.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/L2A_GIPP.xml` & `buteo-0.9.8/buteo/eo/graphs/L2A_GIPP.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/step_01_backstatter.xml` & `buteo-0.9.8/buteo/eo/graphs/step_01_backstatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/step_01_coherence.xml` & `buteo-0.9.8/buteo/eo/graphs/step_01_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/step_02_backscatter.xml` & `buteo-0.9.8/buteo/eo/graphs/step_02_backscatter.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/step_02_backscatter_speckle.xml` & `buteo-0.9.8/buteo/eo/graphs/step_02_backscatter_speckle.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/graphs/step_02_coherence.xml` & `buteo-0.9.8/buteo/eo/graphs/step_02_coherence.xml`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/s1_preprocess.py` & `buteo-0.9.8/buteo/eo/s1_preprocess.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/s1_utils.py` & `buteo-0.9.8/buteo/eo/s1_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/s2_indices.py` & `buteo-0.9.8/buteo/eo/s2_indices.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/eo/s2_utils.py` & `buteo-0.9.8/buteo/eo/s2_utils.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/align.py` & `buteo-0.9.8/buteo/raster/align.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/borders.py` & `buteo-0.9.8/buteo/raster/borders.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/clip.py` & `buteo-0.9.8/buteo/raster/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/coordinates.py` & `buteo-0.9.8/buteo/raster/coordinates.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/core_offsets.py` & `buteo-0.9.8/buteo/raster/core_offsets.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/core_raster.py` & `buteo-0.9.8/buteo/raster/core_raster.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/core_raster_io.py` & `buteo-0.9.8/buteo/raster/core_raster_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/core_stack.py` & `buteo-0.9.8/buteo/raster/core_stack.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/datatype.py` & `buteo-0.9.8/buteo/raster/datatype.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/dem.py` & `buteo-0.9.8/buteo/raster/dem.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/grid.py` & `buteo-0.9.8/buteo/raster/grid.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/metadata.py` & `buteo-0.9.8/buteo/raster/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/nodata.py` & `buteo-0.9.8/buteo/raster/nodata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/proximity.py` & `buteo-0.9.8/buteo/raster/proximity.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/reproject.py` & `buteo-0.9.8/buteo/raster/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/resample.py` & `buteo-0.9.8/buteo/raster/resample.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/shift.py` & `buteo-0.9.8/buteo/raster/shift.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/raster/vectorize.py` & `buteo-0.9.8/buteo/raster/vectorize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_aux.py` & `buteo-0.9.8/buteo/utils/utils_aux.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_base.py` & `buteo-0.9.8/buteo/utils/utils_base.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_bbox.py` & `buteo-0.9.8/buteo/utils/utils_bbox.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_gdal.py` & `buteo-0.9.8/buteo/utils/utils_gdal.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_io.py` & `buteo-0.9.8/buteo/utils/utils_io.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_path.py` & `buteo-0.9.8/buteo/utils/utils_path.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_projection.py` & `buteo-0.9.8/buteo/utils/utils_projection.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/utils/utils_translate.py` & `buteo-0.9.8/buteo/utils/utils_translate.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/buffer.py` & `buteo-0.9.8/buteo/vector/buffer.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/clip.py` & `buteo-0.9.8/buteo/vector/clip.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/convert_parts.py` & `buteo-0.9.8/buteo/vector/convert_parts.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/core_vector.py` & `buteo-0.9.8/buteo/vector/core_vector.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/dissolve.py` & `buteo-0.9.8/buteo/vector/dissolve.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/intersect.py` & `buteo-0.9.8/buteo/vector/intersect.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/merge.py` & `buteo-0.9.8/buteo/vector/merge.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/metadata.py` & `buteo-0.9.8/buteo/vector/metadata.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/rasterize.py` & `buteo-0.9.8/buteo/vector/rasterize.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/reproject.py` & `buteo-0.9.8/buteo/vector/reproject.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/shapes.py` & `buteo-0.9.8/buteo/vector/shapes.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/split.py` & `buteo-0.9.8/buteo/vector/split.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/buteo/vector/zonal_statistics.py` & `buteo-0.9.8/buteo/vector/zonal_statistics.py`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/pyproject.toml` & `buteo-0.9.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.8.0", "numba>=0.57.0", "psutil>=5.9.5", "PyYAML>=6.0", "tqdm>=4.65.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "buteo"
-version = "0.9.7"
+version = "0.9.8"
 authors = [
   { name="Casper Fibaek", email="casperfibaek@gmail.com" },
 ]
 description = "Tools for merging Geospatial Analysis and AI."
 readme = "readme.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `buteo-0.9.7/readme.md` & `buteo-0.9.8/readme.md`

 * *Files identical despite different names*

### Comparing `buteo-0.9.7/PKG-INFO` & `buteo-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buteo
-Version: 0.9.7
+Version: 0.9.8
 Summary: Tools for merging Geospatial Analysis and AI.
 Author-email: Casper Fibaek <casperfibaek@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

