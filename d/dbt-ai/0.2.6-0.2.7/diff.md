# Comparing `tmp/dbt-ai-0.2.6.tar.gz` & `tmp/dbt_ai-0.2.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.2.6.tar", last modified: Fri May 12 00:19:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

