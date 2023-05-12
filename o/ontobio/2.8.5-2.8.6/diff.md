# Comparing `tmp/ontobio-2.8.5.tar.gz` & `tmp/ontobio-2.8.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ontobio-2.8.5.tar", last modified: Mon Apr 24 19:08:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

