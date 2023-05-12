# Comparing `tmp/osais-1.0.40.tar.gz` & `tmp/osais-1.0.41-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-synb31yc\osais-1.0.40.tar", last modified: Thu May 11 10:41:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

