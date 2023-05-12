# Comparing `tmp/mmkit-features-0.0.1a1.tar.gz` & `tmp/mmkit-features-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmkit-features-0.0.1a1.tar", last modified: Sat Jun  4 15:30:19 2022, max compression
+gzip compressed data, was "mmkit-features-0.0.1a2.tar", last modified: Fri May 12 03:50:07 2023, max compression
```

## Comparing `mmkit-features-0.0.1a1.tar` & `mmkit-features-0.0.1a2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.906748 mmkit-features-0.0.1a1/
--rw-rw-rw-   0        0        0     1086 2022-05-03 10:02:28.000000 mmkit-features-0.0.1a1/LICENSE
--rw-rw-rw-   0        0        0      227 2022-05-08 14:24:59.000000 mmkit-features-0.0.1a1/MANIFEST.in
--rw-rw-rw-   0        0        0     4242 2022-06-04 15:30:19.906748 mmkit-features-0.0.1a1/PKG-INFO
--rw-rw-rw-   0        0        0     3022 2022-06-04 15:25:14.000000 mmkit-features-0.0.1a1/README.md
--rw-rw-rw-   0        0        0       81 2022-06-04 15:30:19.909743 mmkit-features-0.0.1a1/setup.cfg
--rw-rw-rw-   0        0        0     8924 2022-06-04 15:29:27.000000 mmkit-features-0.0.1a1/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.851101 mmkit-features-0.0.1a1/src/
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/
--rw-rw-rw-   0        0        0      896 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/LSTHM.py
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/__init__.py
--rw-rw-rw-   0        0        0      862 2021-10-15 08:37:34.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/test.py
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/__init__.py
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/blank.py
--rw-rw-rw-   0        0        0     8936 2021-10-30 16:06:21.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/computational_sequence.py
--rw-rw-rw-   0        0        0     9591 2021-10-27 16:10:39.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/computational_sequence_x.py
--rw-rw-rw-   0        0        0    20045 2021-10-15 06:18:55.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dataset.py
--rw-rw-rw-   0        0        0     1536 2021-10-15 06:17:18.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/download_ops.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dynamic_fusion_graph/
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dynamic_fusion_graph/__init__.py
--rw-rw-rw-   0        0        0     4959 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dynamic_fusion_graph/model.py
--rw-rw-rw-   0        0        0     8630 2021-10-30 16:04:25.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/file_ops.py
--rw-rw-rw-   0        0        0     4043 2021-10-16 18:18:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/integrity_check.py
--rw-rw-rw-   0        0        0     3586 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/log.py
--rw-rw-rw-   0        0        0      609 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/metadataconfigs.py
--rw-rw-rw-   0        0        0    16127 2022-05-08 06:54:01.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/mm_features_lib.py
--rw-rw-rw-   0        0        0     3720 2021-10-30 04:06:50.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/mm_features_node.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/multiple_attention/
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/multiple_attention/__init__.py
--rw-rw-rw-   0        0        0     3463 2021-10-15 08:31:50.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/multiple_attention/model.py
--rw-rw-rw-   0        0        0     1417 2021-10-15 07:30:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/read_mosi_h5_file.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/recurrent_fusion/
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/recurrent_fusion/__init__.py
--rw-rw-rw-   0        0        0     2179 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/recurrent_fusion/model.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.853448 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/tensor_fusion/
--rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/tensor_fusion/__init__.py
--rw-rw-rw-   0        0        0     2297 2021-10-15 08:24:48.000000 mmkit-features-0.0.1a1/src/mmkfeatures/fusion/tensor_fusion/model.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/graph/
--rw-rw-rw-   0        0        0        0 2022-05-22 16:57:15.000000 mmkit-features-0.0.1a1/src/mmkfeatures/graph/__init__.py
--rw-rw-rw-   0        0        0    12743 2022-05-22 13:59:02.000000 mmkit-features-0.0.1a1/src/mmkfeatures/graph/cgan_node.py
--rw-rw-rw-   0        0        0     6533 2022-05-28 23:17:30.000000 mmkit-features-0.0.1a1/src/mmkfeatures/graph/cnn_node.py
--rw-rw-rw-   0        0        0    37328 2022-05-28 23:17:29.000000 mmkit-features-0.0.1a1/src/mmkfeatures/graph/gan_node.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/image/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/__init__.py
--rw-rw-rw-   0        0        0     4090 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/bow_extractor.py
--rw-rw-rw-   0        0        0     2041 2019-07-01 23:17:45.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/clutering_model.py
--rw-rw-rw-   0        0        0     2227 2021-10-27 06:28:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/color_descriptor.py
--rw-rw-rw-   0        0        0     2215 2021-10-30 06:30:53.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/conv_autoencoder.py
--rw-rw-rw-   0        0        0     2310 2022-05-09 16:39:58.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/deep_extractor.py
--rw-rw-rw-   0        0        0     3472 2022-05-09 16:40:14.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/extractor.py
--rw-rw-rw-   0        0        0     9997 2021-10-30 10:24:27.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/image_autoencocer_builder.py
--rw-rw-rw-   0        0        0     4544 2021-10-16 11:58:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/image_features_wrapper.py
--rw-rw-rw-   0        0        0     5060 2021-10-13 16:56:16.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/image_model.py
--rw-rw-rw-   0        0        0     1157 2021-10-15 15:59:23.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/image_processing.py
--rw-rw-rw-   0        0        0     1551 2021-10-30 05:01:51.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/image_searcher.py
--rw-rw-rw-   0        0        0     2562 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/image/lbp_extractor.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/index/
--rw-rw-rw-   0        0        0        0 2022-05-08 03:05:14.000000 mmkit-features-0.0.1a1/src/mmkfeatures/index/__init__.py
--rw-rw-rw-   0        0        0     8691 2022-05-08 04:08:49.000000 mmkit-features-0.0.1a1/src/mmkfeatures/index/index_inverted_op.py
--rw-rw-rw-   0        0        0     8172 2022-05-08 07:01:03.000000 mmkit-features-0.0.1a1/src/mmkfeatures/index/index_positional_op.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/models/
--rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/
--rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/
--rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/__init__.py
--rw-rw-rw-   0        0        0     3481 2021-10-15 09:22:27.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/char_cnn_rnn.py
--rw-rw-rw-   0        0        0     1773 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_gru.py
--rw-rw-rw-   0        0        0      986 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_rnn.py
--rw-rw-rw-   0        0        0     1023 2021-10-15 10:22:30.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/multi_model_dataset.py
--rw-rw-rw-   0        0        0     7700 2021-10-15 10:22:02.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/train.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.869068 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/
--rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/__init__.py
--rw-rw-rw-   0        0        0     1872 2021-06-21 17:00:58.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/models.py
--rw-rw-rw-   0        0        0     4869 2021-10-15 10:23:01.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/train.py
--rw-rw-rw-   0        0        0     3710 2021-10-15 10:51:08.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/image_text_feature_wrapper.py
--rw-rw-rw-   0        0        0      341 2021-06-24 07:54:47.000000 mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/result_analysis.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/speech/
--rw-rw-rw-   0        0        0    10728 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/MFCC.py
--rw-rw-rw-   0        0        0      987 2020-09-03 17:26:41.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/Volume.py
--rw-rw-rw-   0        0        0      529 2020-09-03 17:26:41.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/ZeroCR.py
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/__init__.py
--rw-rw-rw-   0        0        0     3932 2022-05-10 08:34:08.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/audio_features_wrapper.py
--rw-rw-rw-   0        0        0    10302 2021-10-14 09:03:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/feature_extraction_functions.py
--rw-rw-rw-   0        0        0     5988 2021-10-14 09:05:18.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/sigproc.py
--rw-rw-rw-   0        0        0     6725 2021-11-07 05:42:14.000000 mmkit-features-0.0.1a1/src/mmkfeatures/speech/speech_toolkit.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/text/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/text/__init__.py
--rw-rw-rw-   0        0        0    15117 2021-10-15 05:21:28.000000 mmkit-features-0.0.1a1/src/mmkfeatures/text/featurization.py
--rw-rw-rw-   0        0        0    12556 2021-04-08 17:50:38.000000 mmkit-features-0.0.1a1/src/mmkfeatures/text/structures.py
--rw-rw-rw-   0        0        0     4817 2022-05-10 02:20:08.000000 mmkit-features-0.0.1a1/src/mmkfeatures/text/text_features_wrapper.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/__init__.py
--rw-rw-rw-   0        0        0     3905 2021-10-13 13:16:31.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/extract.py
--rw-rw-rw-   0        0        0     1809 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/model.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/configs/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/i3d/
--rw-rw-rw-   0        0        0        0 2022-05-10 04:43:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/i3d/__init__.py
--rw-rw-rw-   0        0        0    11433 2022-05-10 04:54:58.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/i3d/extract_i3d.py
--rw-rw-rw-   0        0        0     4076 2022-05-10 04:45:04.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/main.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/pwc/
--rw-rw-rw-   0        0        0        0 2022-05-10 04:24:37.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/pwc/__init__.py
--rw-rw-rw-   0        0        0     7396 2022-05-10 05:00:20.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/pwc/extract_pwc.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/r21d/
--rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/r21d/__init__.py
--rw-rw-rw-   0        0        0     5846 2022-05-10 04:04:05.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/r21d/extract_r21d.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/resnet/
--rw-rw-rw-   0        0        0        0 2022-05-10 04:06:19.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/resnet/__init__.py
--rw-rw-rw-   0        0        0     7208 2022-05-10 04:43:15.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/resnet/extract_resnet.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.884689 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/vggish/
--rw-rw-rw-   0        0        0       57 2021-12-22 08:00:26.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/vggish/__init__.py
--rw-rw-rw-   0        0        0     3834 2022-05-10 04:45:17.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/models/vggish/extract_vggish.py
--rw-rw-rw-   0        0        0     1255 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/preprocessing.py
--rw-rw-rw-   0        0        0      794 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/random_sequence_shuffler.py
--rw-rw-rw-   0        0        0     6052 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/resnext.py
--rw-rw-rw-   0        0        0      642 2021-10-14 10:36:19.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/run.py
--rw-rw-rw-   0        0        0     3388 2021-10-14 11:23:50.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/run_single_video.py
--rw-rw-rw-   0        0        0     4010 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/video_features_wrapper.py
--rw-rw-rw-   0        0        0     2751 2021-10-13 10:33:48.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/video_loader.py
--rw-rw-rw-   0        0        0     1285 2021-11-07 06:57:28.000000 mmkit-features-0.0.1a1/src/mmkfeatures/video/video_toolkit.py
-drwxrwxrwx   0        0        0        0 2022-06-04 15:30:19.905720 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/
--rw-rw-rw-   0        0        0     4242 2022-06-04 15:30:19.000000 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4456 2022-06-04 15:30:19.000000 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-04 15:30:19.000000 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2022-06-04 15:30:19.000000 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-06-04 15:30:19.000000 mmkit-features-0.0.1a1/src/mmkit_features.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.215589 mmkit-features-0.0.1a2/
+-rw-rw-rw-   0        0        0     1086 2023-05-12 02:35:26.000000 mmkit-features-0.0.1a2/LICENSE
+-rw-rw-rw-   0        0        0      227 2022-05-08 14:24:59.000000 mmkit-features-0.0.1a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7696 2023-05-12 03:50:07.215589 mmkit-features-0.0.1a2/PKG-INFO
+-rw-rw-rw-   0        0        0     5383 2023-05-12 03:49:35.000000 mmkit-features-0.0.1a2/README.md
+-rw-rw-rw-   0        0        0       81 2023-05-12 03:50:07.226039 mmkit-features-0.0.1a2/setup.cfg
+-rw-rw-rw-   0        0        0     9114 2023-05-12 02:42:55.000000 mmkit-features-0.0.1a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/
+-rw-rw-rw-   0        0        0      896 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/LSTHM.py
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/__init__.py
+-rw-rw-rw-   0        0        0      862 2021-10-15 08:37:34.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/test.py
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/__init__.py
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/blank.py
+-rw-rw-rw-   0        0        0     8936 2021-10-30 16:06:21.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/computational_sequence.py
+-rw-rw-rw-   0        0        0     9591 2021-10-27 16:10:39.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/computational_sequence_x.py
+-rw-rw-rw-   0        0        0    20045 2021-10-15 06:18:55.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dataset.py
+-rw-rw-rw-   0        0        0     1536 2021-10-15 06:17:18.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/download_ops.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dynamic_fusion_graph/
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dynamic_fusion_graph/__init__.py
+-rw-rw-rw-   0        0        0     4959 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dynamic_fusion_graph/model.py
+-rw-rw-rw-   0        0        0     8630 2021-10-30 16:04:25.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/file_ops.py
+-rw-rw-rw-   0        0        0     4043 2021-10-16 18:18:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/integrity_check.py
+-rw-rw-rw-   0        0        0     3586 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/log.py
+-rw-rw-rw-   0        0        0      609 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/metadataconfigs.py
+-rw-rw-rw-   0        0        0    16127 2022-05-08 06:54:01.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/mm_features_lib.py
+-rw-rw-rw-   0        0        0     3720 2021-10-30 04:06:50.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/mm_features_node.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/multiple_attention/
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/multiple_attention/__init__.py
+-rw-rw-rw-   0        0        0     3463 2021-10-15 08:31:50.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/multiple_attention/model.py
+-rw-rw-rw-   0        0        0     1417 2021-10-15 07:30:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/read_mosi_h5_file.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/recurrent_fusion/
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/recurrent_fusion/__init__.py
+-rw-rw-rw-   0        0        0     2179 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/recurrent_fusion/model.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.153016 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/tensor_fusion/
+-rw-rw-rw-   0        0        0        0 2021-10-09 15:13:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/tensor_fusion/__init__.py
+-rw-rw-rw-   0        0        0     2297 2021-10-15 08:24:48.000000 mmkit-features-0.0.1a2/src/mmkfeatures/fusion/tensor_fusion/model.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/graph/
+-rw-rw-rw-   0        0        0        0 2022-05-22 16:57:15.000000 mmkit-features-0.0.1a2/src/mmkfeatures/graph/__init__.py
+-rw-rw-rw-   0        0        0    12743 2022-05-22 13:59:02.000000 mmkit-features-0.0.1a2/src/mmkfeatures/graph/cgan_node.py
+-rw-rw-rw-   0        0        0     6533 2022-05-28 23:17:30.000000 mmkit-features-0.0.1a2/src/mmkfeatures/graph/cnn_node.py
+-rw-rw-rw-   0        0        0    37328 2022-05-28 23:17:29.000000 mmkit-features-0.0.1a2/src/mmkfeatures/graph/gan_node.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/image/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/__init__.py
+-rw-rw-rw-   0        0        0     4090 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/bow_extractor.py
+-rw-rw-rw-   0        0        0     2041 2019-07-01 23:17:45.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/clutering_model.py
+-rw-rw-rw-   0        0        0     2227 2021-10-27 06:28:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/color_descriptor.py
+-rw-rw-rw-   0        0        0     2215 2021-10-30 06:30:53.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     2310 2022-05-09 16:39:58.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/deep_extractor.py
+-rw-rw-rw-   0        0        0     3472 2022-05-09 16:40:14.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/extractor.py
+-rw-rw-rw-   0        0        0     9997 2021-10-30 10:24:27.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/image_autoencocer_builder.py
+-rw-rw-rw-   0        0        0     4544 2021-10-16 11:58:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/image_features_wrapper.py
+-rw-rw-rw-   0        0        0     5060 2021-10-13 16:56:16.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/image_model.py
+-rw-rw-rw-   0        0        0     1157 2021-10-15 15:59:23.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/image_processing.py
+-rw-rw-rw-   0        0        0     1551 2021-10-30 05:01:51.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/image_searcher.py
+-rw-rw-rw-   0        0        0     2562 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/image/lbp_extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/index/
+-rw-rw-rw-   0        0        0        0 2022-05-08 03:05:14.000000 mmkit-features-0.0.1a2/src/mmkfeatures/index/__init__.py
+-rw-rw-rw-   0        0        0     8691 2022-05-08 04:08:49.000000 mmkit-features-0.0.1a2/src/mmkfeatures/index/index_inverted_op.py
+-rw-rw-rw-   0        0        0     8172 2022-05-08 07:01:03.000000 mmkit-features-0.0.1a2/src/mmkfeatures/index/index_positional_op.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/models/
+-rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/
+-rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.168640 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/
+-rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/__init__.py
+-rw-rw-rw-   0        0        0     3481 2021-10-15 09:22:27.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/char_cnn_rnn.py
+-rw-rw-rw-   0        0        0     1773 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_gru.py
+-rw-rw-rw-   0        0        0      986 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_rnn.py
+-rw-rw-rw-   0        0        0     1023 2021-10-15 10:22:30.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/multi_model_dataset.py
+-rw-rw-rw-   0        0        0     7700 2021-10-15 10:22:02.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/train.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/
+-rw-rw-rw-   0        0        0        0 2021-01-23 09:47:00.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/__init__.py
+-rw-rw-rw-   0        0        0     1872 2021-06-21 17:00:58.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/models.py
+-rw-rw-rw-   0        0        0     4869 2021-10-15 10:23:01.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/train.py
+-rw-rw-rw-   0        0        0     3710 2021-10-15 10:51:08.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/image_text_feature_wrapper.py
+-rw-rw-rw-   0        0        0      341 2021-06-24 07:54:47.000000 mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/result_analysis.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/speech/
+-rw-rw-rw-   0        0        0    10728 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/MFCC.py
+-rw-rw-rw-   0        0        0      987 2020-09-03 17:26:41.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/Volume.py
+-rw-rw-rw-   0        0        0      529 2020-09-03 17:26:41.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/ZeroCR.py
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/__init__.py
+-rw-rw-rw-   0        0        0     3932 2022-05-10 08:34:08.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/audio_features_wrapper.py
+-rw-rw-rw-   0        0        0    10302 2021-10-14 09:03:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/feature_extraction_functions.py
+-rw-rw-rw-   0        0        0     5988 2021-10-14 09:05:18.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/sigproc.py
+-rw-rw-rw-   0        0        0     6725 2021-11-07 05:42:14.000000 mmkit-features-0.0.1a2/src/mmkfeatures/speech/speech_toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/text/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/text/__init__.py
+-rw-rw-rw-   0        0        0    15117 2021-10-15 05:21:28.000000 mmkit-features-0.0.1a2/src/mmkfeatures/text/featurization.py
+-rw-rw-rw-   0        0        0    12556 2021-04-08 17:50:38.000000 mmkit-features-0.0.1a2/src/mmkfeatures/text/structures.py
+-rw-rw-rw-   0        0        0     4817 2022-05-10 02:20:08.000000 mmkit-features-0.0.1a2/src/mmkfeatures/text/text_features_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/video/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/__init__.py
+-rw-rw-rw-   0        0        0     3905 2021-10-13 13:16:31.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/extract.py
+-rw-rw-rw-   0        0        0     1809 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/model.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/configs/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/i3d/
+-rw-rw-rw-   0        0        0        0 2022-05-10 04:43:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/i3d/__init__.py
+-rw-rw-rw-   0        0        0    11433 2022-05-10 04:54:58.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/i3d/extract_i3d.py
+-rw-rw-rw-   0        0        0     4076 2022-05-10 04:45:04.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/main.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.184267 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/pwc/
+-rw-rw-rw-   0        0        0        0 2022-05-10 04:24:37.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/pwc/__init__.py
+-rw-rw-rw-   0        0        0     7396 2022-05-10 05:00:20.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/pwc/extract_pwc.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.199891 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/r21d/
+-rw-rw-rw-   0        0        0        0 2021-10-14 17:03:54.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/r21d/__init__.py
+-rw-rw-rw-   0        0        0     5846 2022-05-10 04:04:05.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/r21d/extract_r21d.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.199891 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/resnet/
+-rw-rw-rw-   0        0        0        0 2022-05-10 04:06:19.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/resnet/__init__.py
+-rw-rw-rw-   0        0        0     7208 2022-05-10 04:43:15.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/resnet/extract_resnet.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.199891 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/vggish/
+-rw-rw-rw-   0        0        0       57 2021-12-22 08:00:26.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/vggish/__init__.py
+-rw-rw-rw-   0        0        0     3834 2022-05-10 04:45:17.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/models/vggish/extract_vggish.py
+-rw-rw-rw-   0        0        0     1255 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/preprocessing.py
+-rw-rw-rw-   0        0        0      794 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/random_sequence_shuffler.py
+-rw-rw-rw-   0        0        0     6052 2020-07-05 09:09:37.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/resnext.py
+-rw-rw-rw-   0        0        0      642 2021-10-14 10:36:19.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/run.py
+-rw-rw-rw-   0        0        0     3388 2021-10-14 11:23:50.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/run_single_video.py
+-rw-rw-rw-   0        0        0     4010 2021-10-14 17:04:57.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/video_features_wrapper.py
+-rw-rw-rw-   0        0        0     2751 2021-10-13 10:33:48.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/video_loader.py
+-rw-rw-rw-   0        0        0     1285 2021-11-07 06:57:28.000000 mmkit-features-0.0.1a2/src/mmkfeatures/video/video_toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:50:07.199891 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/
+-rw-rw-rw-   0        0        0     7696 2023-05-12 03:50:06.000000 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4456 2023-05-12 03:50:07.000000 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:50:06.000000 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2023-05-12 03:50:06.000000 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-12 03:50:06.000000 mmkit-features-0.0.1a2/src/mmkit_features.egg-info/top_level.txt
```

### Comparing `mmkit-features-0.0.1a1/LICENSE` & `mmkit-features-0.0.1a2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 The Python Packaging Authority
+Copyright (c) 2023 The Python Packaging Authority
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mmkit-features-0.0.1a1/setup.py` & `mmkit-features-0.0.1a2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A setuptools based setup module.
 
-MMKit-Features: A Python library to extract and fuse multimodal features for deep learning.
+MMKit-Features: A multimodal architecture to build multimodal knowledge graphs with flexible multimodal feature extraction and dynamic multimodal concept generation.
 
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
@@ -32,20 +32,20 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.1a1',  # Required
+    version='0.0.1a2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='A Python library to extract, store and fuse multimodal features for deep learning',  # Optional
+    description='A multimodal architecture to build multimodal knowledge graphs with flexible multimodal feature extraction and dynamic multimodal concept generation.',  # Optional
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
@@ -126,15 +126,15 @@
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    packages=find_packages(where='src',exclude=["data","examples"]),  # Required
+    packages=find_packages(where='src',exclude=["data","examples","examples-graph","third_party_examples","tests"]),  # Required
 
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
     python_requires='>=3.6, <4',
```

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/LSTHM.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/LSTHM.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/LSTHM/test.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/LSTHM/test.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/computational_sequence.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/computational_sequence.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/computational_sequence_x.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/computational_sequence_x.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dataset.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dataset.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/download_ops.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/download_ops.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/dynamic_fusion_graph/model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/dynamic_fusion_graph/model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/file_ops.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/file_ops.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/integrity_check.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/integrity_check.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/log.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/log.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/metadataconfigs.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/metadataconfigs.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/mm_features_lib.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/mm_features_lib.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/mm_features_node.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/mm_features_node.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/multiple_attention/model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/multiple_attention/model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/read_mosi_h5_file.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/read_mosi_h5_file.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/recurrent_fusion/model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/recurrent_fusion/model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/fusion/tensor_fusion/model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/fusion/tensor_fusion/model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/graph/cgan_node.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/graph/cgan_node.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/graph/cnn_node.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/graph/cnn_node.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/graph/gan_node.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/graph/gan_node.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/bow_extractor.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/bow_extractor.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/clutering_model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/clutering_model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/color_descriptor.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/color_descriptor.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/conv_autoencoder.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/deep_extractor.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/deep_extractor.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/extractor.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/extractor.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/image_autoencocer_builder.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/image_autoencocer_builder.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/image_features_wrapper.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/image_features_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/image_model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/image_model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/image_processing.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/image_processing.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/image_searcher.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/image_searcher.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/image/lbp_extractor.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/image/lbp_extractor.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/index/index_inverted_op.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/index/index_inverted_op.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/index/index_positional_op.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/index/index_positional_op.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/char_cnn_rnn.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/char_cnn_rnn.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_gru.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_gru.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_rnn.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/fixed_rnn.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/multi_model_dataset.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/multi_model_dataset.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/char_embedding/train.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/char_embedding/train.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/models.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/models.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/train.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/conv_autoencoder/train.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/models/image_text_fusion/image_text_feature_wrapper.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/models/image_text_fusion/image_text_feature_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/MFCC.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/MFCC.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/Volume.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/Volume.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/ZeroCR.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/ZeroCR.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/audio_features_wrapper.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/audio_features_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/feature_extraction_functions.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/feature_extraction_functions.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/sigproc.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/sigproc.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/speech/speech_toolkit.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/speech/speech_toolkit.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/text/featurization.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/text/featurization.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/text/structures.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/text/structures.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/text/text_features_wrapper.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/text/text_features_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/extract.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/extract.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/model.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/model.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/i3d/extract_i3d.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/i3d/extract_i3d.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/main.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/main.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/pwc/extract_pwc.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/pwc/extract_pwc.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/r21d/extract_r21d.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/r21d/extract_r21d.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/resnet/extract_resnet.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/resnet/extract_resnet.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/models/vggish/extract_vggish.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/models/vggish/extract_vggish.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/preprocessing.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/random_sequence_shuffler.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/random_sequence_shuffler.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/resnext.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/resnext.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/run.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/run.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/run_single_video.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/run_single_video.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/video_features_wrapper.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/video_features_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/video_loader.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/video_loader.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkfeatures/video/video_toolkit.py` & `mmkit-features-0.0.1a2/src/mmkfeatures/video/video_toolkit.py`

 * *Files identical despite different names*

### Comparing `mmkit-features-0.0.1a1/src/mmkit_features.egg-info/SOURCES.txt` & `mmkit-features-0.0.1a2/src/mmkit_features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

