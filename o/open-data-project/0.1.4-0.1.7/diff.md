# Comparing `tmp/open_data_project-0.1.4.tar.gz` & `tmp/open_data_project-0.1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_data_project-0.1.4.tar", last modified: Sat May  6 13:10:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

