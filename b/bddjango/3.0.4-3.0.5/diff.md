# Comparing `tmp/bddjango-3.0.4.tar.gz` & `tmp/bddjango-3.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bddjango-3.0.4.tar", last modified: Fri May 12 01:53:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

