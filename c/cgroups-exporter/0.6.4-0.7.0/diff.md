# Comparing `tmp/cgroups-exporter-0.6.4.tar.gz` & `tmp/cgroups_exporter-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgroups-exporter-0.6.4.tar", last modified: Fri Sep 30 09:55:47 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

