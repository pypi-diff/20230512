# Comparing `tmp/pyright-1.1.307.tar.gz` & `tmp/pyright-1.1.308-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyright-1.1.307.tar", last modified: Wed May 10 09:22:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

