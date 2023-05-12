# Comparing `tmp/autogluon.cloud-0.2.1b20230511.tar.gz` & `tmp/autogluon.cloud-0.2.1b20230512-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autogluon.cloud-0.2.1b20230511.tar", last modified: Thu May 11 09:04:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

