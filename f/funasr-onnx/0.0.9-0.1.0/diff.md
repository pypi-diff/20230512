# Comparing `tmp/funasr_onnx-0.0.9.tar.gz` & `tmp/funasr_onnx-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr_onnx-0.0.9.tar", last modified: Fri May 12 02:20:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

