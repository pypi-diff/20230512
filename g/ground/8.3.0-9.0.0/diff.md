# Comparing `tmp/ground-8.3.0.tar.gz` & `tmp/ground-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ground-8.3.0.tar", last modified: Fri Jan  6 22:14:48 2023, max compression
+gzip compressed data, was "ground-9.0.0.tar", last modified: Fri May 12 18:41:30 2023, max compression
```

## Comparing `ground-8.3.0.tar` & `ground-9.0.0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.574238 ground-8.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-06 22:14:26.000000 ground-8.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-06 22:14:26.000000 ground-8.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-01-06 22:14:48.574238 ground-8.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-01-06 22:14:26.000000 ground-8.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.554237 ground-8.3.0/ground/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-06 22:14:26.000000 ground-8.3.0/ground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86803 2023-01-06 22:14:26.000000 ground-8.3.0/ground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.554237 ground-8.3.0/ground/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/angular/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/angular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/angular/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/angular/exact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/angular/plain/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/angular/plain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/angular/robust/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/angular/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/boxed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/centroidal/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/centroidal/exact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/multisegment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/exact/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.558237 ground-8.3.0/ground/core/centroidal/plain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/multisegment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/plain/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/centroidal/robust/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/multisegment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/centroidal/robust/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/circular/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/circular/exact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/exact/point_point_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/circular/plain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/plain/point_point_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/circular/robust/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/circular/robust/point_point_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/geometries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/measured/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.562237 ground-8.3.0/ground/core/measured/exact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/exact/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/measured/plain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/plain/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/measured/robust/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/measured/robust/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/metric/
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/metric/exact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/exact/box.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/exact/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/exact/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/metric/plain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/plain/box.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/plain/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/plain/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.566238 ground-8.3.0/ground/core/metric/robust/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/robust/box.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/robust/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/metric/robust/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/robust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/rotation/
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/rotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/rotation/exact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/rotation/plain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/rotation/robust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/scaling/
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/scaling/exact.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/scaling/plain.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/scaling/robust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/segment/exact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/segment/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/translation/
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/translation/exact.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/translation/plain.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/translation/robust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/vector/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.570238 ground-8.3.0/ground/core/vector/exact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/exact/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/exact/dot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.574238 ground-8.3.0/ground/core/vector/plain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/plain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/plain/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/plain/dot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.574238 ground-8.3.0/ground/core/vector/robust/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/robust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/robust/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-06 22:14:26.000000 ground-8.3.0/ground/core/vector/robust/dot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-06 22:14:26.000000 ground-8.3.0/ground/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:14:48.554237 ground-8.3.0/ground.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-01-06 22:14:48.000000 ground-8.3.0/ground.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-01-06 22:14:48.000000 ground-8.3.0/ground.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 22:14:48.000000 ground-8.3.0/ground.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-06 22:14:48.000000 ground-8.3.0/ground.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-06 22:14:48.000000 ground-8.3.0/ground.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-06 22:14:26.000000 ground-8.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 22:14:48.574238 ground-8.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-06 22:14:26.000000 ground-8.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.249796 ground-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-12 18:41:19.000000 ground-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 18:41:19.000000 ground-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-12 18:41:30.249796 ground-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-12 18:41:19.000000 ground-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 18:41:19.000000 ground-9.0.0/ground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86519 2023-05-12 18:41:19.000000 ground-9.0.0/ground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/angular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/angular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/angular/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/angular/exact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/angular/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/angular/plain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/angular/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/angular/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/boxed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/centroidal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground/core/centroidal/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/multisegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/exact/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/centroidal/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/multisegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/plain/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/centroidal/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/multisegment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/centroidal/robust/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/circular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/circular/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/exact/point_point_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/circular/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/plain/point_point_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/circular/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/circular/robust/point_point_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/measured/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/measured/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/exact/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/measured/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/plain/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/measured/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/measured/robust/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/metric/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/exact/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/exact/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/exact/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/metric/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/plain/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/plain/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/plain/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.241796 ground-9.0.0/ground/core/metric/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/robust/box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/robust/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/metric/robust/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/robust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/rotation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/rotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/rotation/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/rotation/plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/rotation/robust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/scaling/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/scaling/plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/scaling/robust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/segment/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/segment/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/translation/
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/translation/exact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/translation/plain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/translation/robust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.245796 ground-9.0.0/ground/core/vector/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/exact/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/exact/dot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.249796 ground-9.0.0/ground/core/vector/plain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/plain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/plain/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/plain/dot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.249796 ground-9.0.0/ground/core/vector/robust/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/robust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/robust/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 18:41:19.000000 ground-9.0.0/ground/core/vector/robust/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-12 18:41:19.000000 ground-9.0.0/ground/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 18:41:30.237796 ground-9.0.0/ground.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-12 18:41:30.000000 ground-9.0.0/ground.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-12 18:41:30.000000 ground-9.0.0/ground.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 18:41:30.000000 ground-9.0.0/ground.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-12 18:41:30.000000 ground-9.0.0/ground.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 18:41:30.000000 ground-9.0.0/ground.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-12 18:41:19.000000 ground-9.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 18:41:30.249796 ground-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-12 18:41:19.000000 ground-9.0.0/setup.py
```

### Comparing `ground-8.3.0/LICENSE` & `ground-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/PKG-INFO` & `ground-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ground
-Version: 8.3.0
+Version: 9.0.0
 Summary: Basis of computational geometry.
 Home-page: https://github.com/lycantropos/ground/
 Download-URL: https://github.com/lycantropos/ground/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ground-8.3.0/README.md` & `ground-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/base.py` & `ground-9.0.0/ground/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import enum as _enum
 from contextvars import ContextVar as _ContextVar
+from numbers import Rational as _Rational
 from typing import (Optional as _Optional,
                     Sequence as _Sequence,
                     Type as _Type,
                     Union as _Union)
 
 from reprit import serializers as _serializers
 from reprit.base import generate_repr as _generate_repr
@@ -1310,20 +1311,20 @@
         ...      Segment(Point(0, 0), Point(1, 0)), 0, 1)
         ...  == Segment(Point(0, 0), Point(0, 1)))
         True
         """
         return self._rotation.rotate_segment_around_origin(
                 segment, cosine, sine, self.point_cls, self.segment_cls)
 
-    def scale_contour(self,
-                      contour: _hints.Contour,
-                      factor_x: _hints.Scalar,
-                      factor_y: _hints.Scalar
-                      ) -> _Union[_hints.Contour, _hints.Multipoint,
-                                  _hints.Segment]:
+    def scale_contour(
+            self,
+            contour: _hints.Contour,
+            factor_x: _hints.Scalar,
+            factor_y: _hints.Scalar
+    ) -> _Union[_hints.Contour, _hints.Multipoint, _hints.Segment]:
         """
         Returns contour scaled by given factor.
 
         Time complexity:
             ``O(len(contour.vertices))``
         Memory complexity:
             ``O(len(contour.vertices))``
@@ -1386,20 +1387,20 @@
         ...  == Multipoint([Point(0, 0), Point(1, 1)]))
         True
         """
         return self._scaling.scale_multipoint(multipoint, factor_x, factor_y,
                                               self.multipoint_cls,
                                               self.point_cls)
 
-    def scale_multipolygon(self,
-                           multipolygon: _hints.Multipolygon,
-                           factor_x: _hints.Scalar,
-                           factor_y: _hints.Scalar
-                           ) -> _Union[_hints.Multipoint, _hints.Multipolygon,
-                                       _hints.Multisegment]:
+    def scale_multipolygon(
+            self,
+            multipolygon: _hints.Multipolygon,
+            factor_x: _hints.Scalar,
+            factor_y: _hints.Scalar
+    ) -> _Union[_hints.Multipoint, _hints.Multipolygon, _hints.Multisegment]:
         """
         Returns multipolygon scaled by given factor.
 
         Time complexity:
             ``O(vertices_count)``
         Memory complexity:
             ``O(vertices_count)``
@@ -1452,20 +1453,20 @@
         """
         return self._scaling.scale_multipolygon(
                 multipolygon, factor_x, factor_y, self.contour_cls,
                 self.multipoint_cls, self.multipolygon_cls,
                 self.multisegment_cls, self.point_cls, self.polygon_cls,
                 self.segment_cls)
 
-    def scale_multisegment(self,
-                           multisegment: _hints.Multisegment,
-                           factor_x: _hints.Scalar,
-                           factor_y: _hints.Scalar
-                           ) -> _Union[_hints.Mix, _hints.Multipoint,
-                                       _hints.Multisegment]:
+    def scale_multisegment(
+            self,
+            multisegment: _hints.Multisegment,
+            factor_x: _hints.Scalar,
+            factor_y: _hints.Scalar
+    ) -> _Union[_hints.Mix, _hints.Multipoint, _hints.Multisegment]:
         """
         Returns multisegment scaled by given factor.
 
         Time complexity:
             ``O(len(multisegment.segments))``
         Memory complexity:
             ``O(len(multisegment.segments))``
@@ -1528,20 +1529,20 @@
         True
         >>> context.scale_point(Point(1, 1), 1, 1) == Point(1, 1)
         True
         """
         return self._scaling.scale_point(point, factor_x, factor_y,
                                          self.point_cls)
 
-    def scale_polygon(self,
-                      polygon: _hints.Polygon,
-                      factor_x: _hints.Scalar,
-                      factor_y: _hints.Scalar
-                      ) -> _Union[_hints.Multipoint, _hints.Polygon,
-                                  _hints.Segment]:
+    def scale_polygon(
+            self,
+            polygon: _hints.Polygon,
+            factor_x: _hints.Scalar,
+            factor_y: _hints.Scalar
+    ) -> _Union[_hints.Multipoint, _hints.Polygon, _hints.Segment]:
         """
         Returns polygon scaled by given factor.
 
         Time complexity:
             ``O(vertices_count)``
         Memory complexity:
             ``O(vertices_count)``
```

### Comparing `ground-8.3.0/ground/core/angular/__init__.py` & `ground-9.0.0/ground/core/angular/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/angular/exact/__init__.py` & `ground-9.0.0/ground/core/angular/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/angular/plain/__init__.py` & `ground-9.0.0/ground/core/angular/plain/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/angular/robust/__init__.py` & `ground-9.0.0/ground/core/angular/robust/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/boxed.py` & `ground-9.0.0/ground/core/boxed.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/__init__.py` & `ground-9.0.0/ground/core/centroidal/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/contour.py` & `ground-9.0.0/ground/core/centroidal/exact/contour.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/multipoint.py` & `ground-9.0.0/ground/core/centroidal/exact/multipoint.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/multipolygon.py` & `ground-9.0.0/ground/core/centroidal/exact/multipolygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/multisegment.py` & `ground-9.0.0/ground/core/centroidal/exact/multisegment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/polygon.py` & `ground-9.0.0/ground/core/centroidal/exact/polygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/exact/region.py` & `ground-9.0.0/ground/core/centroidal/exact/region.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/contour.py` & `ground-9.0.0/ground/core/centroidal/plain/contour.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/multipoint.py` & `ground-9.0.0/ground/core/centroidal/plain/multipoint.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/multipolygon.py` & `ground-9.0.0/ground/core/centroidal/plain/multipolygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/multisegment.py` & `ground-9.0.0/ground/core/centroidal/plain/multisegment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/polygon.py` & `ground-9.0.0/ground/core/centroidal/plain/polygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/plain/region.py` & `ground-9.0.0/ground/core/centroidal/plain/region.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/contour.py` & `ground-9.0.0/ground/core/centroidal/robust/contour.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/multipoint.py` & `ground-9.0.0/ground/core/centroidal/robust/multipoint.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/multipolygon.py` & `ground-9.0.0/ground/core/centroidal/robust/multipolygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/multisegment.py` & `ground-9.0.0/ground/core/centroidal/robust/multisegment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/polygon.py` & `ground-9.0.0/ground/core/centroidal/robust/polygon.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/centroidal/robust/region.py` & `ground-9.0.0/ground/core/centroidal/robust/region.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/circular/__init__.py` & `ground-9.0.0/ground/core/circular/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/circular/exact/point_point_point.py` & `ground-9.0.0/ground/core/circular/exact/point_point_point.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/circular/plain/point_point_point.py` & `ground-9.0.0/ground/core/circular/plain/point_point_point.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/discrete.py` & `ground-9.0.0/ground/core/discrete.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/enums.py` & `ground-9.0.0/ground/core/enums.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/geometries.py` & `ground-9.0.0/ground/core/geometries.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/hints.py` & `ground-9.0.0/ground/core/hints.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/measured/__init__.py` & `ground-9.0.0/ground/core/measured/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/measured/exact/region.py` & `ground-9.0.0/ground/core/measured/exact/region.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/measured/robust/region.py` & `ground-9.0.0/ground/core/measured/robust/region.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/__init__.py` & `ground-9.0.0/ground/core/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/exact/box.py` & `ground-9.0.0/ground/core/metric/exact/box.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/exact/segment.py` & `ground-9.0.0/ground/core/metric/exact/segment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/plain/box.py` & `ground-9.0.0/ground/core/metric/plain/box.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/plain/segment.py` & `ground-9.0.0/ground/core/metric/plain/segment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/robust/box.py` & `ground-9.0.0/ground/core/metric/robust/box.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/metric/robust/segment.py` & `ground-9.0.0/ground/core/metric/robust/segment.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/packing.py` & `ground-9.0.0/ground/core/packing.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/primitive.py` & `ground-9.0.0/ground/core/primitive.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/robust.py` & `ground-9.0.0/ground/core/robust.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/rotation/__init__.py` & `ground-9.0.0/ground/core/rotation/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/rotation/exact.py` & `ground-9.0.0/ground/core/rotation/exact.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/rotation/plain.py` & `ground-9.0.0/ground/core/rotation/plain.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/rotation/robust.py` & `ground-9.0.0/ground/core/rotation/robust.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/scaling/__init__.py` & `ground-9.0.0/ground/core/scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/segment/__init__.py` & `ground-9.0.0/ground/core/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/segment/exact.py` & `ground-9.0.0/ground/core/segment/exact.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/segment/plain.py` & `ground-9.0.0/ground/core/segment/plain.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/translation/__init__.py` & `ground-9.0.0/ground/core/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/vector/__init__.py` & `ground-9.0.0/ground/core/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/vector/exact/cross.py` & `ground-9.0.0/ground/core/vector/exact/cross.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/core/vector/exact/dot.py` & `ground-9.0.0/ground/core/vector/exact/dot.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground/hints.py` & `ground-9.0.0/ground/hints.py`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/ground.egg-info/PKG-INFO` & `ground-9.0.0/ground.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ground
-Version: 8.3.0
+Version: 9.0.0
 Summary: Basis of computational geometry.
 Home-page: https://github.com/lycantropos/ground/
 Download-URL: https://github.com/lycantropos/ground/archive/master.zip
 Author: Azat Ibrakov
 Author-email: azatibrakov@gmail.com
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ground-8.3.0/ground.egg-info/SOURCES.txt` & `ground-9.0.0/ground.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ground-8.3.0/setup.py` & `ground-9.0.0/setup.py`

 * *Files identical despite different names*

