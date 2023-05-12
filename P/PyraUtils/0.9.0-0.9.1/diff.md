# Comparing `tmp/PyraUtils-0.9.0.tar.gz` & `tmp/PyraUtils-0.9.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyraUtils-0.9.0.tar", last modified: Mon Apr 10 08:09:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

