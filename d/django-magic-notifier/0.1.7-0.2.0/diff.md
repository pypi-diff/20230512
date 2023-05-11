# Comparing `tmp/django-magic-notifier-0.1.7.tar.gz` & `tmp/django_magic_notifier-0.2.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magic-notifier-0.1.7.tar", last modified: Wed Sep 14 23:46:08 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

