# Comparing `tmp/deeplake-3.4.1.tar.gz` & `tmp/deeplake-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.4.1.tar", last modified: Tue May  9 10:10:40 2023, max compression
+gzip compressed data, was "deeplake-3.4.2.tar", last modified: Fri May 12 17:11:08 2023, max compression
```

## Comparing `deeplake-3.4.1.tar` & `deeplake-3.4.2.tar`

### file list

```diff
@@ -1,359 +1,359 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-05-09 10:06:24.000000 deeplake-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-09 10:06:24.000000 deeplake-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25285 2023-05-09 10:10:40.115128 deeplake-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24578 2023-05-09 10:06:24.000000 deeplake-3.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94061 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    79381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19170 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   109338 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   169710 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4242 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13294 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25667 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    49363 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7404 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    10116 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48823 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29082 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5373 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6781 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25806 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     4986 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.105128 deeplake-3.4.1/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4477 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34661 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    24791 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31017 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.115128 deeplake-3.4.1/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-05-09 10:06:24.000000 deeplake-3.4.1/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 10:10:40.095128 deeplake-3.4.1/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25285 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10849 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 10:10:39.000000 deeplake-3.4.1/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-09 10:10:40.115128 deeplake-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-09 10:06:24.000000 deeplake-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-05-12 17:09:29.000000 deeplake-3.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-12 17:09:29.000000 deeplake-3.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-12 17:11:08.234314 deeplake-3.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24578 2023-05-12 17:09:29.000000 deeplake-3.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94061 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    79704 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19170 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   109338 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   169757 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25667 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49363 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7404 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    10116 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49584 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29082 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.224314 deeplake-3.4.2/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25905 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22441 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34661 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    24791 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31017 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.234314 deeplake-3.4.2/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-05-12 17:09:29.000000 deeplake-3.4.2/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 17:11:08.214314 deeplake-3.4.2/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25285 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10849 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-12 17:11:08.000000 deeplake-3.4.2/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-12 17:11:08.244314 deeplake-3.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-05-12 17:09:29.000000 deeplake-3.4.2/setup.py
```

### Comparing `deeplake-3.4.1/LICENSE` & `deeplake-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/PKG-INFO` & `deeplake-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.4.1
+Version: 3.4.2
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.4.1 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.2 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.4.1/README.md` & `deeplake-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/__init__.py` & `deeplake-3.4.2/deeplake/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.4.1"
+__version__ = "3.4.2"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.4.1/deeplake/api/dataset.py` & `deeplake-3.4.2/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/info.py` & `deeplake-3.4.2/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/link.py` & `deeplake-3.4.2/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/link_tiled.py` & `deeplake-3.4.2/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/read.py` & `deeplake-3.4.2/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_access_method.py` & `deeplake-3.4.2/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_agreement.py` & `deeplake-3.4.2/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_api.py` & `deeplake-3.4.2/deeplake/api/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2453,7 +2453,20 @@
         # issue was when number of samples (flattened) was a multiple of length of tensor
         ds.abc.extend([[1, 2], [1, 2, 3], [1, 2, 3, 4]])
 
         with pytest.raises(DynamicTensorNumpyError):
             ds.abc.numpy()
 
         assert ds.abc.numpy(aslist=True) == [[1, 2], [1, 2, 3], [1, 2, 3, 4]]
+
+
+def test_iterate_with_groups(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("x/y/z")
+
+    ds["x/y/z"].extend(list(range(100)))
+
+    for i, sample in enumerate(ds):
+        assert sample["x/y"].z.is_iteration == True
+
+    for i, sample in enumerate(ds):
+        assert sample["x/y/z"].is_iteration == True
```

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.4.2/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.4.2/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.4.2/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.4.2/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_dataset.py` & `deeplake-3.4.2/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_dicom.py` & `deeplake-3.4.2/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_downsample.py` & `deeplake-3.4.2/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_events.py` & `deeplake-3.4.2/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_grayscale.py` & `deeplake-3.4.2/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_info.py` & `deeplake-3.4.2/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.4.2/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_json.py` & `deeplake-3.4.2/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_link.py` & `deeplake-3.4.2/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.4.2/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_linking.py` & `deeplake-3.4.2/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_mesh.py` & `deeplake-3.4.2/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_meta.py` & `deeplake-3.4.2/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_nifti.py` & `deeplake-3.4.2/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_none.py` & `deeplake-3.4.2/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.4.2/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_pickle.py` & `deeplake-3.4.2/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.4.2/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_polygons.py` & `deeplake-3.4.2/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_pop.py` & `deeplake-3.4.2/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_readonly.py` & `deeplake-3.4.2/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_rechunk.py` & `deeplake-3.4.2/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_reset.py` & `deeplake-3.4.2/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_sample_info.py` & `deeplake-3.4.2/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_text.py` & `deeplake-3.4.2/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_update_samples.py` & `deeplake-3.4.2/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_video.py` & `deeplake-3.4.2/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tests/test_views.py` & `deeplake-3.4.2/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/api/tiled.py` & `deeplake-3.4.2/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/structured/base.py` & `deeplake-3.4.2/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/structured/dataframe.py` & `deeplake-3.4.2/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.4.2/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.4.2/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.4.2/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.4.2/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/base.py` & `deeplake-3.4.2/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.4.2/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.4.2/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.4.2/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.4.2/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.4.2/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.4.2/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/util.py` & `deeplake-3.4.2/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.4.2/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.4.2/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/cli/auth.py` & `deeplake-3.4.2/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/cli/test_cli.py` & `deeplake-3.4.2/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/client/client.py` & `deeplake-3.4.2/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/client/config.py` & `deeplake-3.4.2/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/client/log.py` & `deeplake-3.4.2/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/client/test_client.py` & `deeplake-3.4.2/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/client/utils.py` & `deeplake-3.4.2/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/compression.py` & `deeplake-3.4.2/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/constants.py` & `deeplake-3.4.2/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/base_chunk.py` & `deeplake-3.4.2/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.4.2/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.4.2/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.4.2/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.4.2/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.4.2/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.4.2/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/chunk_engine.py` & `deeplake-3.4.2/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compression.py` & `deeplake-3.4.2/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compute/process.py` & `deeplake-3.4.2/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compute/provider.py` & `deeplake-3.4.2/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compute/ray.py` & `deeplake-3.4.2/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compute/serial.py` & `deeplake-3.4.2/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/compute/thread.py` & `deeplake-3.4.2/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/__init__.py` & `deeplake-3.4.2/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/dataset.py` & `deeplake-3.4.2/deeplake/core/dataset/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,14 +485,15 @@
                     index=self.index,
                     group_index=posixpath.join(self.group_index, item),
                     read_only=self.read_only,
                     token=self._token,
                     verbose=False,
                     version_state=self.version_state,
                     path=self.path,
+                    is_iteration=is_iteration,
                     link_creds=self.link_creds,
                     pad_tensors=self._pad_tensors,
                     enabled_tensors=self.enabled_tensors,
                     view_base=self._view_base or self,
                     libdeeplake_dataset=self.libdeeplake_dataset,
                 )
             elif "/" in item:
```

### Comparing `deeplake-3.4.1/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.4.2/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.4.2/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.4.2/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/invalid_view.py` & `deeplake-3.4.2/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/dataset/view_entry.py` & `deeplake-3.4.2/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/fast_forwarding.py` & `deeplake-3.4.2/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/index/index.py` & `deeplake-3.4.2/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/io.py` & `deeplake-3.4.2/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/ipc.py` & `deeplake-3.4.2/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/link_creds.py` & `deeplake-3.4.2/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/linked_chunk_engine.py` & `deeplake-3.4.2/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/linked_sample.py` & `deeplake-3.4.2/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/linked_tiled_sample.py` & `deeplake-3.4.2/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/lock.py` & `deeplake-3.4.2/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/dataset_meta.py` & `deeplake-3.4.2/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.4.2/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.4.2/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.4.2/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/creds.py` & `deeplake-3.4.2/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/pad.py` & `deeplake-3.4.2/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/sequence.py` & `deeplake-3.4.2/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/shape.py` & `deeplake-3.4.2/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/encode/tile.py` & `deeplake-3.4.2/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/meta/tensor_meta.py` & `deeplake-3.4.2/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/partial_reader.py` & `deeplake-3.4.2/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/partial_sample.py` & `deeplake-3.4.2/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/polygon.py` & `deeplake-3.4.2/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/query/autocomplete.py` & `deeplake-3.4.2/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/query/filter.py` & `deeplake-3.4.2/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/query/query.py` & `deeplake-3.4.2/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/sample.py` & `deeplake-3.4.2/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/serialize.py` & `deeplake-3.4.2/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.4.2/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/gcs.py` & `deeplake-3.4.2/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/google_drive.py` & `deeplake-3.4.2/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/local.py` & `deeplake-3.4.2/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/lru_cache.py` & `deeplake-3.4.2/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/memory.py` & `deeplake-3.4.2/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/provider.py` & `deeplake-3.4.2/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/storage/s3.py` & `deeplake-3.4.2/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tensor.py` & `deeplake-3.4.2/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tensor_link.py` & `deeplake-3.4.2/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/test_serialize.py` & `deeplake-3.4.2/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_compression.py` & `deeplake-3.4.2/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_compute.py` & `deeplake-3.4.2/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.4.2/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_io.py` & `deeplake-3.4.2/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_locking.py` & `deeplake-3.4.2/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_readonly.py` & `deeplake-3.4.2/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tests/test_serialize.py` & `deeplake-3.4.2/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/deserialize.py` & `deeplake-3.4.2/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/optimizer.py` & `deeplake-3.4.2/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.4.2/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/serialize.py` & `deeplake-3.4.2/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.4.2/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/tiling/test_serialize.py` & `deeplake-3.4.2/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/transform/test_transform.py` & `deeplake-3.4.2/deeplake/core/transform/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     get_default_tensor_diff,
     get_default_dataset_diff,
 )
 from deeplake.util.remove_cache import remove_memory_cache
 from deeplake.util.check_installation import ray_installed
 from deeplake.util.exceptions import (
     AllSamplesSkippedError,
+    EmptyTensorError,
     InvalidOutputDatasetError,
     TransformError,
 )
 from deeplake.tests.common import parametrize_num_workers
 from deeplake.util.transform import get_pbar_description
 import deeplake
 import gc
@@ -1545,7 +1546,32 @@
 
     assert len(ds2) == 11
     np.testing.assert_array_equal(ds2.abc[:10].numpy(), ds.abc.numpy())
     np.testing.assert_array_equal(ds2.abc[10].numpy(), np.zeros((0,)))
     np.testing.assert_array_equal(ds2.xyz.numpy(), ds.xyz.numpy())
 
     ds2.delete()
+
+
+def test_ds_append_empty(local_ds):
+    @deeplake.compute
+    def upload(stuff, ds):
+        ds.append(stuff, append_empty=True)
+
+    with local_ds as ds:
+        ds.create_tensor("images", htype="image", sample_compression="png")
+        ds.create_tensor("label1", htype="class_label")
+        ds.create_tensor("label2", htype="class_label")
+
+    samples = [
+        {"images": np.random.randint(0, 255, (10, 10, 3), dtype=np.uint8), "label1": 1}
+        for _ in range(20)
+    ]
+
+    upload().eval(samples, ds, num_workers=TRANSFORM_TEST_NUM_WORKERS)
+
+    with pytest.raises(EmptyTensorError):
+        ds.label2.numpy()
+
+    ds.label2.append(1)
+
+    np.testing.assert_array_equal(ds.label2[:20].numpy(), np.array([]).reshape((20, 0)))
```

### Comparing `deeplake-3.4.1/deeplake/core/transform/transform.py` & `deeplake-3.4.2/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/transform/transform_dataset.py` & `deeplake-3.4.2/deeplake/core/transform/transform_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from deeplake.util.exceptions import SampleAppendError, TensorDoesNotExistError
 from deeplake.core.transform.transform_tensor import TransformTensor
 from deeplake.core.linked_tiled_sample import LinkedTiledSample
-from deeplake.util.exceptions import SampleAppendError
 from deeplake.core.partial_sample import PartialSample
 from deeplake.core.linked_sample import LinkedSample
 from deeplake.core.sample import Sample
 from deeplake.core.tensor import Tensor
 from deeplake.constants import MB
 
 
@@ -55,20 +55,30 @@
         self.idx = item
         return self
 
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
-    def append(self, sample):
-        if len(set(map(len, (self[k] for k in sample)))) != 1:
-            raise ValueError("All tensors are expected to have the same length.")
+    def append(self, sample, skip_ok=False, append_empty=False):
+        if skip_ok:
+            raise ValueError(
+                "`skip_ok` is not supported for `ds.append` in transforms. Use `skip_ok` parameter of the `eval` method instead."
+            )
 
-        for k, v in sample.items():
-            self[k].append(v)
+        if len(set(map(len, (self[k] for k in sample)))) != 1:
+            raise ValueError(
+                "All tensors are expected to have the same length before `ds.append`."
+            )
+
+        for k in self.tensors:
+            if k in sample:
+                self[k].append(sample[k])
+            elif append_empty:
+                self[k].append(None)
 
     def item_added(self, item):
         if isinstance(item, Sample):
             sizeof_item = len(item.buffer)
         elif isinstance(item, LinkedSample):
             sizeof_item = len(item.path)
         elif isinstance(item, np.ndarray):
```

### Comparing `deeplake-3.4.1/deeplake/core/transform/transform_tensor.py` & `deeplake-3.4.2/deeplake/core/transform/transform_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,17 @@
             not isinstance(item, (LinkedSample, LinkedTiledSample, Tensor))
             and item is not None
         ):
             shape = getattr(item, "shape", None)  # verify sample
 
     def append(self, item):
         """Adds an item to the tensor."""
+        if self.is_group:
+            raise TensorDoesNotExistError(self.name)
         try:
-            if self.is_group:
-                raise TensorDoesNotExistError(self.name)
-
             # optimization applicable only if extending
             self.non_numpy_only()
 
             self._verify_item(item)
             self.items.append(item)
             self._item_added(item)
         except Exception as e:
```

### Comparing `deeplake-3.4.1/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.4.2/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/version_control/commit_diff.py` & `deeplake-3.4.2/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/version_control/commit_node.py` & `deeplake-3.4.2/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.4.2/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/version_control/test_merge.py` & `deeplake-3.4.2/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/core/version_control/test_version_control.py` & `deeplake-3.4.2/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.4.2/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/dataloader.py` & `deeplake-3.4.2/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.4.2/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.4.2/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/test_pytorch.py` & `deeplake-3.4.2/deeplake/enterprise/test_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import deeplake
 import numpy as np
 import pytest
 from deeplake.util.exceptions import EmptyTensorError, TensorDoesNotExistError
 
 from deeplake.util.remove_cache import get_base_storage
 from deeplake.core.index.index import IndexEntry
-from deeplake.tests.common import requires_torch, requires_libdeeplake
+from deeplake.tests.common import (
+    requires_torch,
+    requires_libdeeplake,
+    convert_data_according_to_torch_version,
+)
 from deeplake.core.dataset import Dataset
 from deeplake.constants import KB
 
 from PIL import Image  # type: ignore
 
 try:
     from torch.utils.data._utils.collate import default_collate
@@ -454,15 +458,15 @@
         hub_cloud_ds.image.extend(
             [deeplake.read(compressed_image_paths["jpeg"][0])] * 5
         )
 
     ptds = hub_cloud_ds.dataloader().pytorch(decode_method={"image": "tobytes"})
 
     for i, batch in enumerate(ptds):
-        image = batch["image"]
+        image = convert_data_according_to_torch_version(batch["image"])
         assert isinstance(image, bytes)
         if i < 5 and not compression:
             np.testing.assert_array_equal(
                 np.frombuffer(image, dtype=np.uint8).reshape(10, 10, 3),
                 i * np.ones((10, 10, 3), dtype=np.uint8),
             )
         elif i >= 5 and compression:
```

### Comparing `deeplake-3.4.1/deeplake/enterprise/test_query.py` & `deeplake-3.4.2/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.4.2/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/enterprise/util.py` & `deeplake-3.4.2/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/hooks.py` & `deeplake-3.4.2/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/htype.py` & `deeplake-3.4.2/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.4.2/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.4.2/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/pytorch/common.py` & `deeplake-3.4.2/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.4.2/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.4.2/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.4.2/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,18 @@
                 from torch import Tensor as TorchTensor
             else:
                 return 0
         except ImportError:
             return 0
         if isinstance(sample, TorchTensor):
             return 1
+        elif isinstance(sample, bytes):
+            return 0
+        elif isinstance(sample, str):
+            return 0
         elif isinstance(sample, dict):
             return sum(self._num_torch_tensors(tensor) for tensor in sample.values())
         elif isinstance(sample, Sequence):
             return sum(self._num_torch_tensors(tensor) for tensor in sample)
         else:
             return 0
```

### Comparing `deeplake-3.4.1/deeplake/integrations/tf/common.py` & `deeplake-3.4.2/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.4.2/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.4.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/integrations/wandb/wandb.py` & `deeplake-3.4.2/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/tests/cache_fixtures.py` & `deeplake-3.4.2/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/tests/client_fixtures.py` & `deeplake-3.4.2/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/tests/common.py` & `deeplake-3.4.2/deeplake/tests/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,13 +138,11 @@
         _register_link_transform(self.name, self.func)
 
     def __exit__(self, *args, **kwargs):
         _unregister_link_transform(self.name)
 
 
 def convert_data_according_to_torch_version(batch):
-    import torch
-
-    if torch.__version__ < "2.0.0":
+    if isinstance(batch, List):
         return batch[0]
     else:
         return batch
```

### Comparing `deeplake-3.4.1/deeplake/tests/dataset_fixtures.py` & `deeplake-3.4.2/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/tests/path_fixtures.py` & `deeplake-3.4.2/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/tests/storage_fixtures.py` & `deeplake-3.4.2/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/access_method.py` & `deeplake-3.4.2/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/agreement.py` & `deeplake-3.4.2/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/array_list.py` & `deeplake-3.4.2/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/assert_byte_indexes.py` & `deeplake-3.4.2/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/auto.py` & `deeplake-3.4.2/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/bugout_reporter.py` & `deeplake-3.4.2/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/cache_chain.py` & `deeplake-3.4.2/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/casting.py` & `deeplake-3.4.2/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/check_latest_version.py` & `deeplake-3.4.2/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/chunk_engine.py` & `deeplake-3.4.2/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/class_label.py` & `deeplake-3.4.2/deeplake/util/class_label.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import OrderedDict, defaultdict
 from typing import List
 
 from deeplake.util.hash import hash_str_to_int32
+from deeplake.util.exceptions import EmptyTensorError
 from deeplake.client.log import logger
 import numpy as np
 import deeplake
 
 
 def convert_to_idx(samples, class_names: List[str]):
     class_idx = {class_names[i]: i for i in range(len(class_names))}
@@ -80,16 +81,19 @@
     @deeplake.compute
     def class_label_sync(
         hash_tensor_sample,
         samples_out,
         label_tensor: str,
         hash_idx_map,
     ):
-        hashes = hash_tensor_sample.numpy().tolist()
-        idxs = convert_hash_to_idx(hashes, hash_idx_map)
+        try:
+            hashes = hash_tensor_sample.numpy().tolist()
+            idxs = convert_hash_to_idx(hashes, hash_idx_map)
+        except EmptyTensorError:
+            idxs = None
         samples_out[label_tensor].append(idxs)
 
     for tensor, temp_tensor in label_temp_tensors.items():
         if len(ds[temp_tensor]) == 0:
             ds.delete_tensor(temp_tensor, large_ok=True)
         else:
             try:
```

### Comparing `deeplake-3.4.1/deeplake/util/compute.py` & `deeplake-3.4.2/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/connect_dataset.py` & `deeplake-3.4.2/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/dataset.py` & `deeplake-3.4.2/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/diff.py` & `deeplake-3.4.2/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/downsample.py` & `deeplake-3.4.2/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/encoder.py` & `deeplake-3.4.2/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/exceptions.py` & `deeplake-3.4.2/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/exif.py` & `deeplake-3.4.2/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/from_tfds.py` & `deeplake-3.4.2/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/htype.py` & `deeplake-3.4.2/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/image.py` & `deeplake-3.4.2/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/invalid_view_op.py` & `deeplake-3.4.2/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/iteration_warning.py` & `deeplake-3.4.2/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/json.py` & `deeplake-3.4.2/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/keys.py` & `deeplake-3.4.2/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/link.py` & `deeplake-3.4.2/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/logging.py` & `deeplake-3.4.2/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/merge.py` & `deeplake-3.4.2/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/modified.py` & `deeplake-3.4.2/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/notebook.py` & `deeplake-3.4.2/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/mesh.py` & `deeplake-3.4.2/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.4.2/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.4.2/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.4.2/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.4.2/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/path.py` & `deeplake-3.4.2/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/pretty_print.py` & `deeplake-3.4.2/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/remove_cache.py` & `deeplake-3.4.2/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/scheduling.py` & `deeplake-3.4.2/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/shape_interval.py` & `deeplake-3.4.2/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/spinner.py` & `deeplake-3.4.2/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/split.py` & `deeplake-3.4.2/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/storage.py` & `deeplake-3.4.2/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tag.py` & `deeplake-3.4.2/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/testing.py` & `deeplake-3.4.2/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_auto.py` & `deeplake-3.4.2/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.4.2/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.4.2/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_read.py` & `deeplake-3.4.2/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.4.2/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_split.py` & `deeplake-3.4.2/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/tests/test_version_control.py` & `deeplake-3.4.2/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/transform.py` & `deeplake-3.4.2/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/version_control.py` & `deeplake-3.4.2/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/util/video.py` & `deeplake-3.4.2/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/visualizer/video_streaming.py` & `deeplake-3.4.2/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake/visualizer/visualizer.py` & `deeplake-3.4.2/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake.egg-info/PKG-INFO` & `deeplake-3.4.2/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.4.1
+Version: 3.4.2
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.4.1 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.4.2 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
```

### Comparing `deeplake-3.4.1/deeplake.egg-info/SOURCES.txt` & `deeplake-3.4.2/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/deeplake.egg-info/requires.txt` & `deeplake-3.4.2/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.4.1/setup.py` & `deeplake-3.4.2/setup.py`

 * *Files identical despite different names*

