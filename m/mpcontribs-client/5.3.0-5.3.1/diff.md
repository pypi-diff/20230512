# Comparing `tmp/mpcontribs-client-5.3.0.tar.gz` & `tmp/mpcontribs_client-5.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.3.0.tar", last modified: Fri Apr 28 00:40:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

