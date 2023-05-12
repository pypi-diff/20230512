# Comparing `tmp/pykingas-1.2.4.tar.gz` & `tmp/pykingas-2.0.0-cp39-none-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykingas-1.2.4.tar", last modified: Thu May 12 18:33:24 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

