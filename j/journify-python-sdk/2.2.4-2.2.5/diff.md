# Comparing `tmp/journify-python-sdk-2.2.4.tar.gz` & `tmp/journify_python_sdk-2.2.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "journify-python-sdk-2.2.4.tar", last modified: Thu May 11 13:44:52 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

