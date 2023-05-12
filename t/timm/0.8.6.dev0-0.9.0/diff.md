# Comparing `tmp/timm-0.8.6.dev0.tar.gz` & `tmp/timm-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timm-0.8.6.dev0.tar", last modified: Thu Jan 12 05:34:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

