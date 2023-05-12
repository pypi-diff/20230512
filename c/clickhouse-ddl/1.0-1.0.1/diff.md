# Comparing `tmp/clickhouse_ddl-1.0.tar.gz` & `tmp/clickhouse_ddl-1.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse_ddl-1.0.tar", last modified: Fri May 12 11:19:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

