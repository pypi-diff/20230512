# Comparing `tmp/generic-path-0.4.3.tar.gz` & `tmp/generic_path-0.4.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-path-0.4.3.tar", last modified: Thu May 11 13:17:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

