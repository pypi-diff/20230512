# Comparing `tmp/lupin-grognard-2.0.0.dev2.tar.gz` & `tmp/lupin_grognard-2.0.0.dev3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-2.0.0.dev2.tar", last modified: Fri May 12 07:38:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

