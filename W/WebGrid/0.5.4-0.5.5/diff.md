# Comparing `tmp/WebGrid-0.5.4.tar.gz` & `tmp/WebGrid-0.5.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebGrid-0.5.4.tar", last modified: Mon May  8 14:10:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

