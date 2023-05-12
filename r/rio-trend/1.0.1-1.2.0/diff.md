# Comparing `tmp/rio-trend-1.0.1.tar.gz` & `tmp/rio_trend-1.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-trend-1.0.1.tar", last modified: Fri Jan  6 16:56:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

