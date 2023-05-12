# Comparing `tmp/checksec.py-0.6.2.tar.gz` & `tmp/checksec_py-0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/checksec.py-0.6.2.tar", last modified: Wed Oct 13 21:49:49 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

