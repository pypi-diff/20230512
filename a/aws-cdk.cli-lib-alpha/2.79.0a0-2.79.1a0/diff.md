# Comparing `tmp/aws-cdk.cli-lib-alpha-2.79.0a0.tar.gz` & `tmp/aws_cdk.cli_lib_alpha-2.79.1a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src077221208/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.79.0a0.tar", last modified: Wed May 10 11:36:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

