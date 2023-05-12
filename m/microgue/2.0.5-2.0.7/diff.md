# Comparing `tmp/microgue-2.0.5.tar.gz` & `tmp/microgue-2.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-2.0.5.tar", last modified: Tue May  9 14:30:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

