# Comparing `tmp/justa-0.0.1.dev1.tar.gz` & `tmp/justa-0.0.1.dev2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justa-0.0.1.dev1.tar", last modified: Wed May 10 07:36:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

