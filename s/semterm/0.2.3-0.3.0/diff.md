# Comparing `tmp/semterm-0.2.3.tar.gz` & `tmp/semterm-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semterm-0.2.3.tar", last modified: Sat May  6 06:52:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

