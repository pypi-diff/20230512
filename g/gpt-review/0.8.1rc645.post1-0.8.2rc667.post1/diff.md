# Comparing `tmp/gpt-review-0.8.1rc645.post1.tar.gz` & `tmp/gpt_review-0.8.2rc667.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.1rc645.post1.tar", last modified: Thu May 11 17:34:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

