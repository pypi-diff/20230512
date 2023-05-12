# Comparing `tmp/aiida-project-0.3.0.tar.gz` & `tmp/aiida_project-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-project-0.3.0.tar", last modified: Fri Apr 21 23:23:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

