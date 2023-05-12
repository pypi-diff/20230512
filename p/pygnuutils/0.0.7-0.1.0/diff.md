# Comparing `tmp/pygnuutils-0.0.7.tar.gz` & `tmp/pygnuutils-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnuutils-0.0.7.tar", last modified: Sat Apr 22 21:14:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

