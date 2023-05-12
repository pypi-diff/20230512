# Comparing `tmp/PythonCoordinates-0.5.8.tar.gz` & `tmp/PythonCoordinates-0.5.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonCoordinates-0.5.8.tar", last modified: Wed May 10 17:03:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

