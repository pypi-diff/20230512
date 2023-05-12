# Comparing `tmp/matplotlibs-8.8.8.1.tar.gz` & `tmp/matplotlibs-8.8.8.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlibs-8.8.8.1.tar", last modified: Thu May 11 22:54:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

