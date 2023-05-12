# Comparing `tmp/polly-validator-0.0.1.tar.gz` & `tmp/polly_validator-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polly-validator-0.0.1.tar", last modified: Wed Feb  1 13:27:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

