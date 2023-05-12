# Comparing `tmp/drb-extractor-1.0.2.tar.gz` & `tmp/drb_extractor-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-extractor-1.0.2.tar", last modified: Thu Feb  9 09:25:24 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

