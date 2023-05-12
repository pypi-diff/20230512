# Comparing `tmp/delia-1.1.0.tar.gz` & `tmp/delia-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.1.0.tar", last modified: Fri May  5 16:21:57 2023, max compression
+gzip compressed data, was "delia-1.1.1.tar", last modified: Fri May 12 19:34:15 2023, max compression
```

## Comparing `delia-1.1.0.tar` & `delia-1.1.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.944439 delia-1.1.0/
--rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    14855 2023-05-05 16:21:57.944439 delia-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    14223 2023-05-05 16:16:03.000000 delia-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.900353 delia-1.1.0/delia/
--rw-rw-rw-   0        0        0      583 2023-05-05 16:17:05.000000 delia-1.1.0/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.905819 delia-1.1.0/delia/databases/
--rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.1.0/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13270 2023-05-05 16:07:22.000000 delia-1.1.0/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.906828 delia-1.1.0/delia/extractors/
--rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.1.0/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14755 2023-05-05 16:07:22.000000 delia-1.1.0/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.909824 delia-1.1.0/delia/radiomics/
--rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.1.0/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    11691 2023-05-05 16:07:22.000000 delia-1.1.0/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.911006 delia-1.1.0/delia/readers/
--rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.1.0/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.912518 delia-1.1.0/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    10880 2023-05-05 16:07:22.000000 delia-1.1.0/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.915532 delia-1.1.0/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.916530 delia-1.1.0/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     4887 2022-11-15 18:06:34.000000 delia-1.1.0/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     7615 2022-11-15 18:06:34.000000 delia-1.1.0/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3783 2022-11-15 18:06:34.000000 delia-1.1.0/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      963 2022-11-03 14:49:27.000000 delia-1.1.0/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10002 2023-05-05 16:07:22.000000 delia-1.1.0/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.920074 delia-1.1.0/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.924066 delia-1.1.0/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.1.0/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.1.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.1.0/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.1.0/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.1.0/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.1.0/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.1.0/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.926067 delia-1.1.0/delia/transforms/
--rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.1.0/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    13213 2023-03-16 17:06:08.000000 delia-1.1.0/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.929686 delia-1.1.0/delia/transforms/array_space/
--rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.1.0/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     5103 2023-03-16 17:56:25.000000 delia-1.1.0/delia/transforms/array_space/matching_centroid_spatial_crop.py
--rw-rw-rw-   0        0        0     3132 2023-03-27 00:28:53.000000 delia-1.1.0/delia/transforms/array_space/matching_crop_foreground.py
--rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.1.0/delia/transforms/array_space/tools.py
--rw-rw-rw-   0        0        0     2562 2023-03-16 16:29:22.000000 delia-1.1.0/delia/transforms/array_space/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.931409 delia-1.1.0/delia/transforms/data/
--rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.1.0/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4594 2023-05-05 16:10:26.000000 delia-1.1.0/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1882 2022-11-15 18:06:34.000000 delia-1.1.0/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.935421 delia-1.1.0/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.1.0/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-03-27 00:36:22.000000 delia-1.1.0/delia/transforms/physical_space/matching_resample.py
--rw-rw-rw-   0        0        0     9826 2023-05-05 16:10:26.000000 delia-1.1.0/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3470 2022-11-15 18:06:34.000000 delia-1.1.0/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     3010 2023-03-16 16:29:21.000000 delia-1.1.0/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2430 2023-03-16 16:29:21.000000 delia-1.1.0/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.939066 delia-1.1.0/delia/utils/
--rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.1.0/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.1.0/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.1.0/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.1.0/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.903819 delia-1.1.0/delia.egg-info/
--rw-rw-rw-   0        0        0    14855 2023-05-05 16:21:57.000000 delia-1.1.0/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2252 2023-05-05 16:21:57.000000 delia-1.1.0/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 16:21:57.000000 delia-1.1.0/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-05 16:21:57.000000 delia-1.1.0/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-05 16:21:57.000000 delia-1.1.0/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 16:21:57.943063 delia-1.1.0/examples/
--rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.1.0/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.1.0/examples/env_examples.py
--rw-rw-rw-   0        0        0     3460 2023-05-04 17:50:21.000000 delia-1.1.0/examples/ex01.py
--rw-rw-rw-   0        0        0     3106 2022-11-16 14:39:31.000000 delia-1.1.0/examples/ex02.py
--rw-rw-rw-   0        0        0     2796 2023-05-05 14:37:22.000000 delia-1.1.0/examples/ex03.py
--rw-rw-rw-   0        0        0     5641 2022-11-15 18:06:34.000000 delia-1.1.0/examples/ex04.py
--rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 16:21:57.944983 delia-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-05 16:17:05.000000 delia-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.826714 delia-1.1.1/
+-rw-rw-rw-   0        0        0    11549 2022-03-24 18:12:27.000000 delia-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    14855 2023-05-12 19:34:15.826714 delia-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14223 2023-05-05 16:16:03.000000 delia-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.717804 delia-1.1.1/delia/
+-rw-rw-rw-   0        0        0      583 2023-05-12 19:33:13.000000 delia-1.1.1/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.724553 delia-1.1.1/delia/databases/
+-rw-rw-rw-   0        0        0       49 2022-11-08 03:00:14.000000 delia-1.1.1/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13270 2023-05-05 16:07:22.000000 delia-1.1.1/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.725571 delia-1.1.1/delia/extractors/
+-rw-rw-rw-   0        0        0      187 2023-05-04 17:50:19.000000 delia-1.1.1/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    14755 2023-05-05 16:07:22.000000 delia-1.1.1/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.730246 delia-1.1.1/delia/radiomics/
+-rw-rw-rw-   0        0        0      158 2023-05-04 17:50:19.000000 delia-1.1.1/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    11691 2023-05-05 16:07:22.000000 delia-1.1.1/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.732959 delia-1.1.1/delia/readers/
+-rw-rw-rw-   0        0        0       65 2022-11-08 03:03:57.000000 delia-1.1.1/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.736288 delia-1.1.1/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    10880 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.743658 delia-1.1.1/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.749970 delia-1.1.1/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     4887 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     7615 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     3783 2022-11-15 18:06:34.000000 delia-1.1.1/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      963 2022-11-03 14:49:27.000000 delia-1.1.1/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10002 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.757412 delia-1.1.1/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.768954 delia-1.1.1/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2042 2022-11-08 03:20:33.000000 delia-1.1.1/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     6278 2022-11-08 03:20:33.000000 delia-1.1.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2022-07-27 14:35:42.000000 delia-1.1.1/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2022-02-08 18:32:16.000000 delia-1.1.1/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     2801 2023-03-16 14:44:58.000000 delia-1.1.1/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-05-05 16:07:22.000000 delia-1.1.1/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.774518 delia-1.1.1/delia/transforms/
+-rw-rw-rw-   0        0        0      120 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    13213 2023-03-16 17:06:08.000000 delia-1.1.1/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.785193 delia-1.1.1/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0      293 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     5103 2023-03-16 17:56:25.000000 delia-1.1.1/delia/transforms/array_space/matching_centroid_spatial_crop.py
+-rw-rw-rw-   0        0        0     3132 2023-03-27 00:28:53.000000 delia-1.1.1/delia/transforms/array_space/matching_crop_foreground.py
+-rw-rw-rw-   0        0        0     1043 2023-03-16 16:39:24.000000 delia-1.1.1/delia/transforms/array_space/tools.py
+-rw-rw-rw-   0        0        0     2562 2023-03-16 16:29:22.000000 delia-1.1.1/delia/transforms/array_space/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.790192 delia-1.1.1/delia/transforms/data/
+-rw-rw-rw-   0        0        0      115 2023-03-16 15:36:25.000000 delia-1.1.1/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4594 2023-05-05 16:10:26.000000 delia-1.1.1/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1882 2022-11-15 18:06:34.000000 delia-1.1.1/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.802447 delia-1.1.1/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0      269 2023-03-27 00:27:35.000000 delia-1.1.1/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     3378 2023-05-12 19:28:03.000000 delia-1.1.1/delia/transforms/physical_space/matching_resample.py
+-rw-rw-rw-   0        0        0     9826 2023-05-05 16:10:26.000000 delia-1.1.1/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3712 2023-05-12 19:30:41.000000 delia-1.1.1/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     3010 2023-03-16 16:29:21.000000 delia-1.1.1/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2430 2023-03-16 16:29:21.000000 delia-1.1.1/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.811922 delia-1.1.1/delia/utils/
+-rw-rw-rw-   0        0        0       42 2022-11-08 03:52:44.000000 delia-1.1.1/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-03-16 14:44:58.000000 delia-1.1.1/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2022-03-25 22:07:08.000000 delia-1.1.1/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2022-11-08 03:00:14.000000 delia-1.1.1/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.723389 delia-1.1.1/delia.egg-info/
+-rw-rw-rw-   0        0        0    14855 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2252 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-12 19:34:15.000000 delia-1.1.1/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 19:34:15.824970 delia-1.1.1/examples/
+-rw-rw-rw-   0        0        0       38 2022-03-26 17:30:16.000000 delia-1.1.1/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2022-03-29 17:53:18.000000 delia-1.1.1/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3460 2023-05-12 19:24:41.000000 delia-1.1.1/examples/ex01.py
+-rw-rw-rw-   0        0        0     3106 2023-05-12 19:24:41.000000 delia-1.1.1/examples/ex02.py
+-rw-rw-rw-   0        0        0     2748 2023-05-12 19:28:03.000000 delia-1.1.1/examples/ex03.py
+-rw-rw-rw-   0        0        0     5641 2022-11-15 18:06:34.000000 delia-1.1.1/examples/ex04.py
+-rw-rw-rw-   0        0        0      108 2022-01-10 21:30:41.000000 delia-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 19:34:15.826714 delia-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-12 19:33:13.000000 delia-1.1.1/setup.py
```

### Comparing `delia-1.1.0/LICENSE` & `delia-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/PKG-INFO` & `delia-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.1.0
+Version: 1.1.1
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.1.0/README.md` & `delia-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/__init__.py` & `delia-1.1.1/delia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.1.0/delia/databases/patients_database.py` & `delia-1.1.1/delia/databases/patients_database.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/extractors/patients_data_extractor.py` & `delia-1.1.1/delia/extractors/patients_data_extractor.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/radiomics/radiomics_dataset.py` & `delia-1.1.1/delia/radiomics/radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/image/dicom_reader.py` & `delia-1.1.1/delia/readers/image/dicom_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.1.1/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.1.1/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.1.1/delia/readers/patient_data/patient_data_query_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.1.1/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/patient_data/patient_data_reader.py` & `delia-1.1.1/delia/readers/patient_data/patient_data_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.1.1/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.1.1/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/factories/segment.py` & `delia-1.1.1/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/factories/segmentation.py` & `delia-1.1.1/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/segmentation_context.py` & `delia-1.1.1/delia/readers/segmentation/segmentation_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/segmentation_reader.py` & `delia-1.1.1/delia/readers/segmentation/segmentation_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.1.1/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/applications.py` & `delia-1.1.1/delia/transforms/applications.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/array_space/matching_centroid_spatial_crop.py` & `delia-1.1.1/delia/transforms/array_space/matching_centroid_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.1.1/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/array_space/tools.py` & `delia-1.1.1/delia/transforms/array_space/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/array_space/transform.py` & `delia-1.1.1/delia/transforms/array_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/data/copy_segmentations.py` & `delia-1.1.1/delia/transforms/data/copy_segmentations.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/data/transform.py` & `delia-1.1.1/delia/transforms/data/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/physical_space/matching_resample.py` & `delia-1.1.1/delia/transforms/physical_space/matching_resample.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,47 +4,51 @@
 
     @Creation Date:     03/2022
     @Last modification: 03/2022
 
     @Description:       This file contains the MatchingResampled transform.
 """
 
-from typing import Dict, Hashable
+from typing import Callable, Dict, Hashable
 
 import SimpleITK as sitk
 
-from delia.transforms.physical_space.transform import PhysicalSpaceTransform, ImageData, KeysCollection
+from delia.transforms.physical_space.transform import PhysicalSpaceTransform, ImageData, KeysCollection, Mode
 
 
 class MatchingResampled(PhysicalSpaceTransform):
     """
     Resample matching images to the spacing, size, origin and direction of a given reference image.
     """
 
     def __init__(
             self,
             reference_image_key: str,
             matching_keys: KeysCollection,
+            interpolator: Callable = sitk.sitkBSpline,
     ):
         """
         Initializes images.
 
         Parameters
         ----------
         reference_image_key : str
             Key of the image from which the spacing, size, origin and direction are taken.
         matching_keys : KeysCollection
             Keys of the corresponding items to be transformed using the calculated coordinates of spatial bounding box
             for foreground on the image. Image keys are assumed to be arbitrary series keys defined in
             'series_descriptions'. For the label maps, the keys are organ names. Note that if 'series_descriptions' is
             None, the image keys are assumed to be modality names.
+        interpolator : Callable
+            The interpolator to be used for resampling the images. Default = sitk.sitkBSpline.
         """
         keys = [key for key in matching_keys] + [reference_image_key]
         super().__init__(keys=keys)
         self._reference_image_key = reference_image_key
+        self._interpolator = interpolator
 
     def __call__(self, data: Dict[str, ImageData]) -> Dict[Hashable, sitk.Image]:
         """
         Resamples matching itk images to the spacing, size, origin and direction of a given reference image.
 
         Parameters
         ----------
@@ -61,13 +65,27 @@
         reference_image = None
         for key in self.key_iterator(d):
             if key == self._reference_image_key:
                 reference_image = d[key].simple_itk_image
 
         for key in self.key_iterator(d):
             if key != self._reference_image_key:
-                d[key] = sitk.Resample(d[key].simple_itk_image, reference_image)
+
+                if self._mode == Mode.NONE:
+                    raise AssertionError("Transform mode must be set before __call__.")
+                elif self._mode == Mode.IMAGE:
+                    interpolator = self._interpolator
+                elif self._mode == Mode.SEGMENTATION:
+                    interpolator = sitk.sitkNearestNeighbor
+                else:
+                    raise ValueError("Unknown transform mode.")
+
+                d[key] = sitk.Resample(
+                    image1=d[key].simple_itk_image,
+                    referenceImage=reference_image,
+                    interpolator=interpolator
+                )
 
         return d
 
 
 MatchingResampleD = MatchingResampleDict = MatchingResampled
```

### Comparing `delia-1.1.0/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.1.1/delia/transforms/physical_space/pet_to_suv.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/physical_space/resample.py` & `delia-1.1.1/delia/transforms/physical_space/resample.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
     @Creation Date:     10/2022
     @Last modification: 11/2022
 
     @Description:       This file contains the Resampled transform.
 """
 
-from typing import Dict, Hashable, Tuple
+from typing import Callable, Dict, Hashable, Tuple
 
 import SimpleITK as sitk
 import numpy as np
 
 from delia.transforms.physical_space.transform import PhysicalSpaceTransform, ImageData, KeysCollection, Mode
 
 
@@ -20,30 +20,34 @@
     """
     Resample an itk_image to new out_spacing.
     """
 
     def __init__(
             self,
             keys: KeysCollection,
-            out_spacing: Tuple[float, float, float] = (1.0, 1.0, 1.0)
+            out_spacing: Tuple[float, float, float] = (1.0, 1.0, 1.0),
+            interpolator: Callable = sitk.sitkBSpline,
     ):
         """
         Initialize output spacing.
 
         Parameters
         ----------
         keys : KeysCollection
             Keys of the corresponding items to be transformed. Image keys are assumed to be arbitrary series keys
             defined in 'series_descriptions'. For the label maps, the keys are organ names. Note that if
             'series_descriptions' is None, the image keys are assumed to be modality names.
         out_spacing : Tuple[int, int, int], default = (1.0, 1.0, 1.0)
             The desired spacing in the physical space. Default = (1.0 mm, 1.0 mm, 1.0 mm).
+        interpolator : Callable
+            The interpolator to be used for resampling the images. Default = sitk.sitkBSpline.
         """
         super().__init__(keys=keys)
         self._out_spacing = out_spacing
+        self._interpolator = interpolator
 
     def __call__(self, data: Dict[str, ImageData]) -> Dict[Hashable, sitk.Image]:
         """
         Resample an itk_image to new out_spacing.
 
         Parameters
         ----------
@@ -76,15 +80,15 @@
             resample.SetOutputOrigin(original_itk_image.GetOrigin())
             resample.SetTransform(sitk.Transform())
             resample.SetDefaultPixelValue(original_itk_image.GetPixelIDValue())
 
             if self._mode == Mode.NONE:
                 raise AssertionError("Transform mode must be set before __call__.")
             elif self._mode == Mode.IMAGE:
-                resample.SetInterpolator(sitk.sitkLinear)
+                resample.SetInterpolator(self._interpolator)
             elif self._mode == Mode.SEGMENTATION:
                 resample.SetInterpolator(sitk.sitkNearestNeighbor)
             else:
                 raise ValueError("Unknown transform mode.")
 
             resampled_image = resample.Execute(original_itk_image)
```

### Comparing `delia-1.1.0/delia/transforms/physical_space/transform.py` & `delia-1.1.1/delia/transforms/physical_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/transforms/tools.py` & `delia-1.1.1/delia/transforms/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/utils/data_model.py` & `delia-1.1.1/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/utils/tools.py` & `delia-1.1.1/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia/utils/transforms_history.py` & `delia-1.1.1/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/delia.egg-info/PKG-INFO` & `delia-1.1.1/delia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.1.0
+Version: 1.1.1
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.1.0/delia.egg-info/SOURCES.txt` & `delia-1.1.1/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/examples/env_examples.py` & `delia-1.1.1/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/examples/ex01.py` & `delia-1.1.1/examples/ex01.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
             [
                 ResampleD(keys=["CT_THORAX", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
                 MatchingCentroidSpatialCropD(
                     segmentation_key="Heart",
                     matching_keys=["CT_THORAX"],
                     roi_size=(96, 96, 96)
                 ),
-                PETtoSUVD(keys=["TEP"]),
+                PETtoSUVD(keys=["PET"]),
                 KeepLargestConnectedComponentD(keys=["Heart"]),
-                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="TEP")
+                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PET")
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                    Perform on-thy-fly tasks on images                                       #
     # ----------------------------------------------------------------------------------------------------------- #
```

### Comparing `delia-1.1.0/examples/ex02.py` & `delia-1.1.1/examples/ex02.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
         series_descriptions="data/radiomics_series_descriptions.json",
         transforms=Compose(
             [
-                PETtoSUVD(keys=["TEP"]),
-                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="TEP")
+                PETtoSUVD(keys=["PET"]),
+                CopySegmentationsD(segmented_image_key="CT_THORAX", unsegmented_image_key="PET")
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #       Extract radiomics features of the CT image from the segmentation of the heart made on the CT image    #
     # ----------------------------------------------------------------------------------------------------------- #
@@ -57,9 +57,9 @@
         path_to_params="features_extractor_params_PT.yaml",
         geometryTolerance=1e-4
     )
 
     PT_radiomics_dataset.create(
         patients_data_extractor=patients_data_extractor,
         organ="Heart",
-        image_name="TEP"
+        image_name="PET"
     )
```

### Comparing `delia-1.1.0/examples/ex03.py` & `delia-1.1.1/examples/ex03.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 """
 
 import env_examples  # Modifies path, DO NOT REMOVE
 
 from delia.databases import PatientsDatabase
 from delia.extractors import PatientsDataExtractor
 from delia.transforms import (
+    MatchingResampleD,
     PETtoSUVD,
     ResampleD
 )
 from monai.transforms import (
     CenterSpatialCropD,
     Compose,
-    ScaleIntensityD,
-    ThresholdIntensityD
+    ScaleIntensityRangeD
 )
 
 
 if __name__ == "__main__":
     # ----------------------------------------------------------------------------------------------------------- #
     #                                         Logs Setup (Optional)                                               #
     # ----------------------------------------------------------------------------------------------------------- #
@@ -30,20 +30,19 @@
     #                                      Create patients data extractor                                         #
     # ----------------------------------------------------------------------------------------------------------- #
     patients_data_extractor = PatientsDataExtractor(
         path_to_patients_folder="data/patients",
         series_descriptions="data/series_descriptions.json",
         transforms=Compose(
             [
-                ResampleD(keys=["CT_THORAX", "TEP", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
-                CenterSpatialCropD(keys=["CT_THORAX", "TEP", "Heart"], roi_size=(1000, 160, 160)),
-                ThresholdIntensityD(keys=["CT_THORAX"], threshold=-250, above=True, cval=-250),
-                ThresholdIntensityD(keys=["CT_THORAX"], threshold=500, above=False, cval=500),
-                ScaleIntensityD(keys=["CT_THORAX"], minv=0, maxv=1),
-                PETtoSUVD(keys=["TEP"])
+                ResampleD(keys=["CT_THORAX", "PET", "Heart"], out_spacing=(1.5, 1.5, 1.5)),
+                MatchingResampleD(reference_image_key="CT_THORAX", matching_keys=["PET", "Heart"]),
+                CenterSpatialCropD(keys=["CT_THORAX", "PET", "Heart"], roi_size=(1000, 160, 160)),
+                ScaleIntensityRangeD(keys=["CT_THORAX"], a_min=-250, a_max=500, b_min=0, b_max=1, clip=True),
+                PETtoSUVD(keys=["PET"])
             ]
         )
     )
 
     # ----------------------------------------------------------------------------------------------------------- #
     #                                                Create database                                              #
     # ----------------------------------------------------------------------------------------------------------- #
```

### Comparing `delia-1.1.0/examples/ex04.py` & `delia-1.1.1/examples/ex04.py`

 * *Files identical despite different names*

### Comparing `delia-1.1.0/setup.py` & `delia-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.1.0",
+    version="1.1.1",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

