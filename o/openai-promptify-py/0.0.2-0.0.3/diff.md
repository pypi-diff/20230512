# Comparing `tmp/openai-promptify-py-0.0.2.tar.gz` & `tmp/openai_promptify_py-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-promptify-py-0.0.2.tar", last modified: Thu Apr 20 03:13:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

