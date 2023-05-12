# Comparing `tmp/motion_python-0.1.39.tar.gz` & `tmp/motion_python-0.1.40-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.39.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

