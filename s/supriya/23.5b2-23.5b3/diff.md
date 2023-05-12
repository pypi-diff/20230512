# Comparing `tmp/supriya-23.5b2.tar.gz` & `tmp/supriya-23.5b3-cp310-cp310-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supriya-23.5b2.tar", last modified: Thu May 11 16:51:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

