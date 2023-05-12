# Comparing `tmp/mattlib-1.1.3.tar.gz` & `tmp/mattlib-1.1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattlib-1.1.3.tar", last modified: Fri May 12 00:07:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

