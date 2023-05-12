# Comparing `tmp/machine_stats-2.5.7a0.tar.gz` & `tmp/machine_stats-2.5.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machine_stats-2.5.7a0.tar", last modified: Thu Jan  5 08:24:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

