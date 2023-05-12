# Comparing `tmp/tootstagram-0.0.5.tar.gz` & `tmp/tootstagram-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstagram-0.0.5.tar", last modified: Thu May  4 11:18:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

