# Comparing `tmp/ink_extensions-1.3.0.tar.gz` & `tmp/ink_extensions-1.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ink_extensions-1.3.0.tar", last modified: Thu May 11 22:01:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

