# Comparing `tmp/opentdf-1.2.2-cp39-cp39-win_amd64.whl.zip` & `tmp/opentdf-1.2.9a1476-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2718881 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat  5469696 b- defN 23-May-12 15:22 opentdf.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1674 b- defN 23-May-12 15:22 opentdf-1.2.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7129 b- defN 23-May-12 15:22 opentdf-1.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-12 15:22 opentdf-1.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-12 15:22 opentdf-1.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      472 b- defN 23-May-12 15:22 opentdf-1.2.2.dist-info/RECORD
-6 files, 5479079 bytes uncompressed, 2718033 bytes compressed:  50.4%
+Zip file size: 5450731 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-06 13:32 opentdf.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 21-Oct-06 13:32 opentdf-1.2.9a1476.dist-info/
+-rwxr-xr-x  2.0 unx 14935528 b- defN 21-Oct-06 13:32 opentdf.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      148 b- defN 21-Oct-06 13:32 opentdf-1.2.9a1476.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2184 b- defN 21-Oct-06 13:32 opentdf-1.2.9a1476.dist-info/METADATA
+-rw-rw-r--  2.0 unx      422 b- defN 21-Oct-06 13:32 opentdf-1.2.9a1476.dist-info/RECORD
+-rw-r--r--  2.0 unx        8 b- defN 21-Oct-06 13:32 opentdf-1.2.9a1476.dist-info/top_level.txt
+7 files, 14938290 bytes uncompressed, 5449721 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: opentdf.cp39-win_amd64.pyd
+Filename: opentdf.libs/
 Comment: 
 
-Filename: opentdf-1.2.2.dist-info/LICENSE
+Filename: opentdf-1.2.9a1476.dist-info/
 Comment: 
 
-Filename: opentdf-1.2.2.dist-info/METADATA
+Filename: opentdf.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: opentdf-1.2.2.dist-info/WHEEL
+Filename: opentdf-1.2.9a1476.dist-info/WHEEL
 Comment: 
 
-Filename: opentdf-1.2.2.dist-info/top_level.txt
+Filename: opentdf-1.2.9a1476.dist-info/METADATA
 Comment: 
 
-Filename: opentdf-1.2.2.dist-info/RECORD
+Filename: opentdf-1.2.9a1476.dist-info/RECORD
+Comment: 
+
+Filename: opentdf-1.2.9a1476.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

