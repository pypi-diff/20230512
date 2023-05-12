# Comparing `tmp/ogc_na-0.2.4.tar.gz` & `tmp/ogc_na-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.2.4.tar", last modified: Thu May 11 16:45:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

