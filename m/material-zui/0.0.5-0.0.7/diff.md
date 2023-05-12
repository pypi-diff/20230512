# Comparing `tmp/material_zui-0.0.5.tar.gz` & `tmp/material_zui-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material_zui-0.0.5.tar", last modified: Thu May  4 09:24:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

