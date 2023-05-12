# Comparing `tmp/openmetadata_managed_apis-1.0.1.1.tar.gz` & `tmp/openmetadata_managed_apis-1.0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.0.1.1.tar", last modified: Wed May 10 12:37:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

