# Comparing `tmp/flask-useful-0.2.1.tar.gz` & `tmp/flask_useful-0.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-useful-0.2.1.tar", last modified: Tue May  9 11:08:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

