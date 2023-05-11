# Comparing `tmp/padacioso-0.2.1a1.tar.gz` & `tmp/padacioso-0.2.1a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padacioso-0.2.1a1.tar", last modified: Sat May  6 22:28:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

