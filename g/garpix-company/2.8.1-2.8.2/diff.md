# Comparing `tmp/garpix_company-2.8.1.tar.gz` & `tmp/garpix_company-2.8.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_company-2.8.1.tar", last modified: Thu May 11 11:02:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

