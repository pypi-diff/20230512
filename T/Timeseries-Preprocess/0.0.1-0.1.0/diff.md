# Comparing `tmp/Timeseries-Preprocess-0.0.1.tar.gz` & `tmp/Timeseries_Preprocess-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Timeseries-Preprocess-0.0.1.tar", last modified: Sun Apr 23 15:47:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

