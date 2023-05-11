# Comparing `tmp/lockss_soap-0.8.0.dev2.tar.gz` & `tmp/lockss_soap-0.8.0.dev3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_soap-0.8.0.dev2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

