# Comparing `tmp/qeschema-1.4.0.tar.gz` & `tmp/qeschema-1.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qeschema-1.4.0.tar", last modified: Fri Apr 29 10:20:34 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

