# Comparing `tmp/carefree-learn-0.4.2.tar.gz` & `tmp/carefree-learn-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-learn-0.4.2.tar", last modified: Sat May  6 05:29:58 2023, max compression
+gzip compressed data, was "carefree-learn-0.4.3.tar", last modified: Fri May 12 11:21:40 2023, max compression
```

## Comparing `carefree-learn-0.4.2.tar` & `carefree-learn-0.4.3.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/
--rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/LICENSE
--rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7575 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.240707 carefree-learn-0.4.2/carefree_learn.egg-info/
--rw-rw-rw-   0        0        0     7575 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10736 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      601 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 05:29:58.000000 carefree-learn-0.4.2/carefree_learn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.244708 carefree-learn-0.4.2/cflearn/
--rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.246707 carefree-learn-0.4.2/cflearn/api/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/api/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.2/cflearn/api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.247707 carefree-learn-0.4.2/cflearn/api/cv/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/cv/__init__.py
--rw-rw-rw-   0        0        0    58260 2023-04-20 12:00:25.000000 carefree-learn-0.4.2/cflearn/api/cv/diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.249709 carefree-learn-0.4.2/cflearn/api/cv/third_party/
--rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/blip.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.250708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/api.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.252708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/predictor.py
--rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/transforms.py
--rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.253707 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/
--rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
--rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/base.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.254708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.256708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/
--rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
--rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
--rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
--rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.258708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/
--rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
--rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
--rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.262708 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
--rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
--rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
--rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
--rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
--rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
--rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
--rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
--rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
--rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modifiers.py
--rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/ops.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.263707 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/utils/misc.py
--rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/isnet.py
--rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/lama.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.265708 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/api.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.269708 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/base_model.py
--rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/blocks.py
--rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/dpt_depth.py
--rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net.py
--rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
--rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/transforms.py
--rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/vit.py
--rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.270708 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/api.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.271708 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.274711 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/api.py
--rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/body.py
--rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/hand.py
--rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/model.py
--rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/util.py
--rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/api/cv/third_party/prompt.py
--rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.2/cflearn/api/cv/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.274711 carefree-learn-0.4.2/cflearn/api/ml/
--rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/ml/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/api/ml/ddr.py
--rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/api/schema.py
--rw-rw-rw-   0        0        0     5513 2023-04-20 04:16:04.000000 carefree-learn-0.4.2/cflearn/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.275712 carefree-learn-0.4.2/cflearn/api/zoo/
--rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.2/cflearn/api/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.276711 carefree-learn-0.4.2/cflearn/callbacks/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.2/cflearn/callbacks/classification.py
--rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.2/cflearn/callbacks/general.py
--rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.2/cflearn/callbacks/generator.py
--rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.277711 carefree-learn-0.4.2/cflearn/data/
--rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.2/cflearn/data/__init__.py
--rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.2/cflearn/data/array.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.278711 carefree-learn-0.4.2/cflearn/data/blocks/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.281711 carefree-learn-0.4.2/cflearn/data/blocks/cv/
--rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/crop.py
--rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/hwc_to_chw.py
--rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/image_folder.py
--rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/normalize.py
--rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/to_numpy.py
--rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/cv/tuple_to_batch.py
--rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/flatten.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.285712 carefree-learn-0.4.2/cflearn/data/blocks/ml/
--rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/__init__.py
--rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/file.py
--rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/gather.py
--rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/nan_handler.py
--rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/preprocessor.py
--rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/recognizer.py
--rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/schema.py
--rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.2/cflearn/data/blocks/ml/splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.286712 carefree-learn-0.4.2/cflearn/data/ml/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/ml/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.2/cflearn/data/ml/api.py
--rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/ml/datasets.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.287711 carefree-learn-0.4.2/cflearn/data/pytorch/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/data/pytorch/__init__.py
--rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.2/cflearn/data/pytorch/api.py
--rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.2/cflearn/data/pytorch/datasets.py
--rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.2/cflearn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.287711 carefree-learn-0.4.2/cflearn/dist/
--rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.289219 carefree-learn-0.4.2/cflearn/dist/ml/
--rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/ml/__init__.py
--rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/experiment.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.290223 carefree-learn-0.4.2/cflearn/dist/ml/runs/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/_utils.py
--rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/runs/basic.py
--rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/dist/ml/task.py
--rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/inference.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.292223 carefree-learn-0.4.2/cflearn/losses/
--rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/losses/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.2/cflearn/losses/basic.py
--rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/losses/gan.py
--rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.2/cflearn/losses/lpips.py
--rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/losses/vae.py
--rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.293223 carefree-learn-0.4.2/cflearn/misc/
--rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.2/cflearn/misc/__init__.py
--rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.2/cflearn/misc/available.json
--rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/misc/mixins.py
--rw-rw-rw-   0        0        0    42445 2023-04-12 11:55:25.000000 carefree-learn-0.4.2/cflearn/misc/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.294223 carefree-learn-0.4.2/cflearn/models/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/bases.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.295223 carefree-learn-0.4.2/cflearn/models/cv/
--rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.296223 carefree-learn-0.4.2/cflearn/models/cv/ae/
--rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/__init__.py
--rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/common.py
--rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/kl.py
--rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.2/cflearn/models/cv/ae/vq.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.297223 carefree-learn-0.4.2/cflearn/models/cv/classifier/
--rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/classifier/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/classifier/vanilla.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.301226 carefree-learn-0.4.2/cflearn/models/cv/decoder/
--rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/__init__.py
--rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/attn.py
--rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/schema.py
--rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan.py
--rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan_v2.py
--rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/vanilla.py
--rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/decoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.303223 carefree-learn-0.4.2/cflearn/models/cv/diffusion/
--rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.305222 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/
--rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/clip.py
--rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/rescaler.py
--rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/schema.py
--rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/ddpm.py
--rw-rw-rw-   0        0        0    10395 2023-04-20 06:47:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/ldm.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.309223 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/
--rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/basic.py
--rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/ddim.py
--rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/k_samplers.py
--rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/plms.py
--rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/schema.py
--rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/solver.py
--rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/utils.py
--rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/unet.py
--rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/diffusion/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.313223 carefree-learn-0.4.2/cflearn/models/cv/encoder/
--rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/attn.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.315224 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/
--rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/api.py
--rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/core.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.317223 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/
--rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/__init__.py
--rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/mobilenet.py
--rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/resnet.py
--rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/transformer.py
--rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/vgg.py
--rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/register.py
--rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/fnet.py
--rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/mixer.py
--rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/perceiver.py
--rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/pool_former.py
--rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/schema.py
--rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/transformer.py
--rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/vanilla.py
--rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/models/cv/encoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.319223 carefree-learn-0.4.2/cflearn/models/cv/gan/
--rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/__init__.py
--rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/discriminators.py
--rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/schema.py
--rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/gan/vanilla.py
--rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/general.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.320223 carefree-learn-0.4.2/cflearn/models/cv/translator/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/cv/translator/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/cv/translator/rrdb.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.321223 carefree-learn-0.4.2/cflearn/models/implicit/
--rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/implicit/__init__.py
--rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/models/implicit/siren.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.325223 carefree-learn-0.4.2/cflearn/models/ml/
--rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/base.py
--rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.2/cflearn/models/ml/ddr.py
--rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.2/cflearn/models/ml/encoders.py
--rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/fcnn.py
--rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/linear.py
--rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/mixed_stacked.py
--rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/nbm.py
--rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/ndt.py
--rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/rnn.py
--rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/ml/wnd.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.326223 carefree-learn-0.4.2/cflearn/models/multimodal/
--rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/multimodal/__init__.py
--rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.2/cflearn/models/multimodal/clip.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/multimodal/constants.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.2/cflearn/models/multimodal/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.327223 carefree-learn-0.4.2/cflearn/models/nlp/
--rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.328223 carefree-learn-0.4.2/cflearn/models/nlp/encoder/
--rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/constants.py
--rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/encoder/transformer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.329222 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/clip.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.331223 carefree-learn-0.4.2/cflearn/models/nlp/transformers/
--rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/core.py
--rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/opus.py
--rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/models/nlp/transformers/simbert.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.332224 carefree-learn-0.4.2/cflearn/models/schemas/
--rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.2/cflearn/models/schemas/__init__.py
--rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/models/schemas/custom.py
--rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/models/schemas/cv.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.334223 carefree-learn-0.4.2/cflearn/modules/
--rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.341222 carefree-learn-0.4.2/cflearn/modules/blocks/
--rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.2/cflearn/modules/blocks/__init__.py
--rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.2/cflearn/modules/blocks/activations.py
--rw-rw-rw-   0        0        0    22018 2023-04-12 11:14:32.000000 carefree-learn-0.4.2/cflearn/modules/blocks/attentions.py
--rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.2/cflearn/modules/blocks/common.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.343222 carefree-learn-0.4.2/cflearn/modules/blocks/convs/
--rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/__init__.py
--rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/basic.py
--rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.2/cflearn/modules/blocks/convs/residual.py
--rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.2/cflearn/modules/blocks/customs.py
--rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/modules/blocks/high_level.py
--rw-rw-rw-   0        0        0    14999 2023-04-12 13:33:59.000000 carefree-learn-0.4.2/cflearn/modules/blocks/hijacks.py
--rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.2/cflearn/modules/blocks/hooks.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.345223 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/
--rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/__init__.py
--rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/implementations/perceiver.py
--rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.349223 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/
--rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/__init__.py
--rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/api.py
--rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
--rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/poolers.py
--rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/schema.py
--rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/token_mixers.py
--rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/blocks/norms.py
--rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.2/cflearn/modules/blocks/utils.py
--rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.2/cflearn/modules/optimizers.py
--rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.2/cflearn/modules/schedulers.py
--rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/monitors.py
--rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.2/cflearn/parameters.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.351223 carefree-learn-0.4.2/cflearn/pipeline/
--rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/__init__.py
--rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.2/cflearn/pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.353222 carefree-learn-0.4.2/cflearn/pipeline/blocks/
--rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/__init__.py
--rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/basic.py
--rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/ml.py
--rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/blocks/utils.py
--rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.2/cflearn/pipeline/core.py
--rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/schema.py
--rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/pipeline/third_party.py
--rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/register.py
--rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.2/cflearn/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.354221 carefree-learn-0.4.2/cflearn/scripts/
--rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.2/cflearn/scripts/__init__.py
--rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/scripts/sd.py
--rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.2/cflearn/trainer.py
--rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/types.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.354221 carefree-learn-0.4.2/cflearn/zoo/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.225708 carefree-learn-0.4.2/cflearn/zoo/configs/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/ae/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.356221 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/
--rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f16.json
--rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f4.json
--rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.358222 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/
--rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f4.json
--rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f4_no_attn.json
--rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/ae/vq/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.358222 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/
--rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/default.json
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.361222 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/
--rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/default.json
--rw-rw-rw-   0        0        0      451 2023-04-04 04:59:57.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd.json
--rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
--rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
--rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
--rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/vq.json
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.224708 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.363222 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/
--rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/chinese.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/default.json
--rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/large.json
--rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.225708 carefree-learn-0.4.2/cflearn/zoo/configs/sr/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.364222 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/
--rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/anime.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/configs/sr/esr/default.json
--rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.2/cflearn/zoo/core.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:29:58.365221 carefree-learn-0.4.2/cflearn/zoo/models/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/models/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.2/cflearn/zoo/models/clip.py
--rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.2/cflearn/zoo/models/schema.py
--rw-rw-rw-   0        0        0      383 2023-05-06 05:29:58.370221 carefree-learn-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1702 2023-05-06 05:22:46.000000 carefree-learn-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.094033 carefree-learn-0.4.3/
+-rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7575 2023-05-12 11:21:40.095033 carefree-learn-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.967523 carefree-learn-0.4.3/carefree_learn.egg-info/
+-rw-rw-rw-   0        0        0     7575 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10736 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      635 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 11:21:39.000000 carefree-learn-0.4.3/carefree_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.971523 carefree-learn-0.4.3/cflearn/
+-rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.973523 carefree-learn-0.4.3/cflearn/api/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/api/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.3/cflearn/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.974523 carefree-learn-0.4.3/cflearn/api/cv/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/cv/__init__.py
+-rw-rw-rw-   0        0        0    61743 2023-05-09 10:43:21.000000 carefree-learn-0.4.3/cflearn/api/cv/diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.976523 carefree-learn-0.4.3/cflearn/api/cv/third_party/
+-rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/blip.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.977523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/api.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.978523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/predictor.py
+-rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/transforms.py
+-rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.980523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/
+-rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
+-rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/base.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.981523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.982524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/
+-rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
+-rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
+-rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
+-rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.984523 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/
+-rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
+-rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
+-rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.991524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
+-rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
+-rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
+-rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
+-rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
+-rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
+-rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
+-rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
+-rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modifiers.py
+-rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/ops.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.992524 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/utils/misc.py
+-rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/isnet.py
+-rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/lama.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.995524 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/__init__.py
+-rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.002524 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/base_model.py
+-rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/blocks.py
+-rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/dpt_depth.py
+-rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net.py
+-rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/transforms.py
+-rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/vit.py
+-rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.004524 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/api.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.006524 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.009525 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/api.py
+-rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/body.py
+-rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/hand.py
+-rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/model.py
+-rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/util.py
+-rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/api/cv/third_party/prompt.py
+-rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.3/cflearn/api/cv/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.010525 carefree-learn-0.4.3/cflearn/api/ml/
+-rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/ml/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/api/ml/ddr.py
+-rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/api/schema.py
+-rw-rw-rw-   0        0        0     5513 2023-04-20 04:16:04.000000 carefree-learn-0.4.3/cflearn/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.010525 carefree-learn-0.4.3/cflearn/api/zoo/
+-rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.3/cflearn/api/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.013526 carefree-learn-0.4.3/cflearn/callbacks/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.3/cflearn/callbacks/classification.py
+-rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.3/cflearn/callbacks/general.py
+-rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.3/cflearn/callbacks/generator.py
+-rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.014525 carefree-learn-0.4.3/cflearn/data/
+-rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.3/cflearn/data/__init__.py
+-rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.3/cflearn/data/array.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.015525 carefree-learn-0.4.3/cflearn/data/blocks/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.019526 carefree-learn-0.4.3/cflearn/data/blocks/cv/
+-rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/crop.py
+-rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/hwc_to_chw.py
+-rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/image_folder.py
+-rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/normalize.py
+-rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/to_numpy.py
+-rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/cv/tuple_to_batch.py
+-rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/flatten.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.022525 carefree-learn-0.4.3/cflearn/data/blocks/ml/
+-rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/__init__.py
+-rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/file.py
+-rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/gather.py
+-rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/nan_handler.py
+-rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/preprocessor.py
+-rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/recognizer.py
+-rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/schema.py
+-rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.3/cflearn/data/blocks/ml/splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.024031 carefree-learn-0.4.3/cflearn/data/ml/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/ml/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.3/cflearn/data/ml/api.py
+-rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/ml/datasets.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.026034 carefree-learn-0.4.3/cflearn/data/pytorch/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/data/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.3/cflearn/data/pytorch/api.py
+-rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.3/cflearn/data/pytorch/datasets.py
+-rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.3/cflearn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.026034 carefree-learn-0.4.3/cflearn/dist/
+-rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.027034 carefree-learn-0.4.3/cflearn/dist/ml/
+-rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/ml/__init__.py
+-rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/experiment.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.028034 carefree-learn-0.4.3/cflearn/dist/ml/runs/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/_utils.py
+-rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/runs/basic.py
+-rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/dist/ml/task.py
+-rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/inference.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.030033 carefree-learn-0.4.3/cflearn/losses/
+-rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/losses/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.3/cflearn/losses/basic.py
+-rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/losses/gan.py
+-rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.3/cflearn/losses/lpips.py
+-rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/losses/vae.py
+-rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.031033 carefree-learn-0.4.3/cflearn/misc/
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.3/cflearn/misc/__init__.py
+-rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.3/cflearn/misc/available.json
+-rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/misc/mixins.py
+-rw-rw-rw-   0        0        0    44325 2023-05-08 12:35:20.000000 carefree-learn-0.4.3/cflearn/misc/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.032033 carefree-learn-0.4.3/cflearn/models/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/bases.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.033034 carefree-learn-0.4.3/cflearn/models/cv/
+-rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.035035 carefree-learn-0.4.3/cflearn/models/cv/ae/
+-rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/__init__.py
+-rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/common.py
+-rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/kl.py
+-rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.3/cflearn/models/cv/ae/vq.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.036034 carefree-learn-0.4.3/cflearn/models/cv/classifier/
+-rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/classifier/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/classifier/vanilla.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.039034 carefree-learn-0.4.3/cflearn/models/cv/decoder/
+-rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/attn.py
+-rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/schema.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan.py
+-rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan_v2.py
+-rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/vanilla.py
+-rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/decoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.042034 carefree-learn-0.4.3/cflearn/models/cv/diffusion/
+-rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.044034 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/
+-rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/clip.py
+-rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/rescaler.py
+-rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/schema.py
+-rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/ddpm.py
+-rw-rw-rw-   0        0        0    10578 2023-05-08 12:33:49.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/ldm.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.047033 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/
+-rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/basic.py
+-rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/ddim.py
+-rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/k_samplers.py
+-rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/plms.py
+-rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/schema.py
+-rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/solver.py
+-rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/utils.py
+-rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/unet.py
+-rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/diffusion/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.051033 carefree-learn-0.4.3/cflearn/models/cv/encoder/
+-rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/attn.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.053034 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/
+-rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/api.py
+-rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/core.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.055034 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/
+-rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/__init__.py
+-rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/mobilenet.py
+-rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/resnet.py
+-rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/transformer.py
+-rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/vgg.py
+-rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/register.py
+-rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/fnet.py
+-rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/mixer.py
+-rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/perceiver.py
+-rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/pool_former.py
+-rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/schema.py
+-rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/transformer.py
+-rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/vanilla.py
+-rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/models/cv/encoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.057034 carefree-learn-0.4.3/cflearn/models/cv/gan/
+-rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/__init__.py
+-rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/discriminators.py
+-rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/schema.py
+-rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/gan/vanilla.py
+-rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/general.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.058033 carefree-learn-0.4.3/cflearn/models/cv/translator/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/cv/translator/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/cv/translator/rrdb.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.058033 carefree-learn-0.4.3/cflearn/models/implicit/
+-rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/implicit/__init__.py
+-rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/models/implicit/siren.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.063034 carefree-learn-0.4.3/cflearn/models/ml/
+-rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/base.py
+-rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.3/cflearn/models/ml/ddr.py
+-rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.3/cflearn/models/ml/encoders.py
+-rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/fcnn.py
+-rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/linear.py
+-rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/mixed_stacked.py
+-rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/nbm.py
+-rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/ndt.py
+-rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/rnn.py
+-rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/ml/wnd.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.064033 carefree-learn-0.4.3/cflearn/models/multimodal/
+-rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/multimodal/__init__.py
+-rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.3/cflearn/models/multimodal/clip.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/multimodal/constants.py
+-rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.3/cflearn/models/multimodal/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.064033 carefree-learn-0.4.3/cflearn/models/nlp/
+-rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.066033 carefree-learn-0.4.3/cflearn/models/nlp/encoder/
+-rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/constants.py
+-rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/encoder/transformer.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.067033 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/clip.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.069035 carefree-learn-0.4.3/cflearn/models/nlp/transformers/
+-rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/core.py
+-rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/opus.py
+-rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/models/nlp/transformers/simbert.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.070033 carefree-learn-0.4.3/cflearn/models/schemas/
+-rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.3/cflearn/models/schemas/__init__.py
+-rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/models/schemas/custom.py
+-rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/models/schemas/cv.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.071033 carefree-learn-0.4.3/cflearn/modules/
+-rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.076033 carefree-learn-0.4.3/cflearn/modules/blocks/
+-rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.3/cflearn/modules/blocks/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.3/cflearn/modules/blocks/activations.py
+-rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.3/cflearn/modules/blocks/attentions.py
+-rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.3/cflearn/modules/blocks/common.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.077033 carefree-learn-0.4.3/cflearn/modules/blocks/convs/
+-rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/__init__.py
+-rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/basic.py
+-rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.3/cflearn/modules/blocks/convs/residual.py
+-rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.3/cflearn/modules/blocks/customs.py
+-rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/modules/blocks/high_level.py
+-rw-rw-rw-   0        0        0    14999 2023-04-12 13:33:59.000000 carefree-learn-0.4.3/cflearn/modules/blocks/hijacks.py
+-rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.3/cflearn/modules/blocks/hooks.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.078033 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/
+-rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/__init__.py
+-rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/implementations/perceiver.py
+-rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.080033 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/
+-rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/__init__.py
+-rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/api.py
+-rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
+-rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/poolers.py
+-rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/schema.py
+-rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/token_mixers.py
+-rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/blocks/norms.py
+-rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.3/cflearn/modules/blocks/utils.py
+-rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.3/cflearn/modules/optimizers.py
+-rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.3/cflearn/modules/schedulers.py
+-rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/monitors.py
+-rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.3/cflearn/parameters.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.082034 carefree-learn-0.4.3/cflearn/pipeline/
+-rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/__init__.py
+-rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.3/cflearn/pipeline/api.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.084033 carefree-learn-0.4.3/cflearn/pipeline/blocks/
+-rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/__init__.py
+-rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/basic.py
+-rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/ml.py
+-rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/blocks/utils.py
+-rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.3/cflearn/pipeline/core.py
+-rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/schema.py
+-rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/pipeline/third_party.py
+-rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/register.py
+-rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.3/cflearn/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.084033 carefree-learn-0.4.3/cflearn/scripts/
+-rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.3/cflearn/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/scripts/sd.py
+-rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.3/cflearn/trainer.py
+-rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/types.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.085034 carefree-learn-0.4.3/cflearn/zoo/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.956523 carefree-learn-0.4.3/cflearn/zoo/configs/ae/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.087034 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/
+-rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f16.json
+-rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f4.json
+-rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.088033 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/
+-rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f4.json
+-rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f4_no_attn.json
+-rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/ae/vq/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.088033 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/
+-rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/default.json
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.091033 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/
+-rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/default.json
+-rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd.json
+-rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
+-rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
+-rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
+-rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/vq.json
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.092033 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/
+-rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/chinese.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/default.json
+-rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/large.json
+-rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:39.957523 carefree-learn-0.4.3/cflearn/zoo/configs/sr/
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.093033 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/
+-rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/anime.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/configs/sr/esr/default.json
+-rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.3/cflearn/zoo/core.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:21:40.094033 carefree-learn-0.4.3/cflearn/zoo/models/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/models/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.3/cflearn/zoo/models/clip.py
+-rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.3/cflearn/zoo/models/schema.py
+-rw-rw-rw-   0        0        0      383 2023-05-12 11:21:40.096033 carefree-learn-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1727 2023-05-12 11:17:01.000000 carefree-learn-0.4.3/setup.py
```

### Comparing `carefree-learn-0.4.2/LICENSE` & `carefree-learn-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/PKG-INFO` & `carefree-learn-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.3.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.2/README.md` & `carefree-learn-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/carefree_learn.egg-info/PKG-INFO` & `carefree-learn-0.4.3/carefree_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.2.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.3.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.2/carefree_learn.egg-info/SOURCES.txt` & `carefree-learn-0.4.3/carefree_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/carefree_learn.egg-info/requires.txt` & `carefree-learn-0.4.3/carefree_learn.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 albumentations
 pillow
 scikit-image
 scipy>=1.8.0
 opencv-python-headless
 timm
 salesforce-lavis
+xformers>=0.0.19
 
 [full]
 ftfy
 lmdb
 regex
 transformers
 albumentations
 pillow
 scikit-image
 scipy>=1.8.0
 opencv-python-headless
 timm
 salesforce-lavis
+xformers>=0.0.19
 onnx
 onnxruntime
 onnx-simplifier>=0.4.1
 open_clip_torch
 faiss-cpu
 protobuf==3.19.4
 ortools>=9.3.0
```

### Comparing `carefree-learn-0.4.2/cflearn/__init__.py` & `carefree-learn-0.4.3/cflearn/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/api.py` & `carefree-learn-0.4.3/cflearn/api/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/diffusion.py` & `carefree-learn-0.4.3/cflearn/api/cv/diffusion.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,14 +173,18 @@
 ) -> Optional[Tuple[int, int]]:
     if size is None:
         return None
     new_size = restrict_wh(*size, max_wh)
     return tuple(map(get_suitable_size, new_size, (anchor, anchor)))  # type: ignore
 
 
+def get_highres_steps(num_steps: int, fidelity: float) -> int:
+    return int(num_steps / min(1.0 - fidelity, 0.999))
+
+
 class DiffusionAPI(APIMixin):
     m: DDPM
     sampler: ISampler
     cond_model: Optional[nn.Module]
     first_stage: Optional[IAutoEncoder]
     latest_seed: int
     latest_variation_seed: Optional[int]
@@ -346,14 +350,29 @@
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         callback: Optional[Callable[[Tensor], Tensor]] = None,
         batch_size: Optional[int] = None,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
+        o_kw_backup = dict(
+            seed=seed,
+            variations=variations,
+            alpha=alpha,
+            cond=cond,
+            cond_concat=cond_concat,
+            unconditional_cond=unconditional_cond,
+            hint=hint,
+            hint_start=hint_start,
+            num_steps=num_steps,
+            clip_output=clip_output,
+            callback=callback,
+            batch_size=batch_size,
+            verbose=verbose,
+        )
         if batch_size is None:
             batch_size = num_samples
         registered_custom = False
         if self.cond_model is not None:
             clip_skip = kwargs.get(
                 "clip_skip",
                 0 if self.clip_skip is None else self.clip_skip,
@@ -408,21 +427,23 @@
                 self.sampler,
                 "unconditional_cond",
                 None,
             )
             uncond = self.get_cond(unconditional_cond).to(self.device)
             self.sampler.uncond = uncond.clone()
             self.sampler.unconditional_cond = uncond.clone()
+        highres_info = kwargs.get("highres_info")
         with eval_context(self.m):
             with self.amp_context:
                 for i, batch in enumerate(iterator):
                     # from the 2nd batch forward, we need to re-generate new seeds
                     if i >= 1:
                         seed = new_seed()
                     i_kw = shallow_copy_dict(kw)
+                    i_kw_backup = shallow_copy_dict(i_kw)
                     i_cond = batch[INPUT_KEY].to(self.device)
                     i_n = len(i_cond)
                     repeat = (
                         lambda t: t
                         if t.shape[0] == i_n
                         else t.repeat_interleave(i_n, dim=0)
                     )
@@ -502,15 +523,37 @@
                         else:
                             i_cond = {
                                 CROSS_ATTN_KEY: i_cond,
                                 CONTROL_HINT_KEY: hint,
                                 CONTROL_HINT_START_KEY: hint_start,
                             }
                     with switch_sampler_context(self, i_kw.get("sampler")):
+                        if highres_info is not None:
+                            # highres workaround
+                            i_kw["return_latent"] = True
                         i_sampled = self.m.decode(i_z, cond=i_cond, **i_kw)
+                        if highres_info is not None:
+                            i_z = self._get_highres_latent(i_sampled, highres_info)
+                            fidelity = highres_info["fidelity"]
+                            if num_steps is None:
+                                num_steps = self.sampler.default_steps
+                            i_num_steps = get_highres_steps(num_steps, fidelity)
+                            i_kw_backup.pop("highres_info", None)
+                            i_kw_backup.update(o_kw_backup)
+                            i_kw_backup["fidelity"] = fidelity
+                            i_kw_backup["num_steps"] = i_num_steps
+                            i_kw_backup["decode_callback"] = self.empty_cuda_cache
+                            self.empty_cuda_cache()
+                            i_sampled = self._img2img(i_z, export_path, **i_kw_backup)
+                            if original_size is not None:
+                                upscale_factor = highres_info["upscale_factor"]
+                                original_size = (
+                                    round(original_size[0] * upscale_factor),
+                                    round(original_size[1] * upscale_factor),
+                                )
                     sampled.append(i_sampled.cpu().float())
         if uncond_backup is not None:
             self.sampler.uncond = uncond_backup
         if unconditional_cond_backup is not None:
             self.sampler.unconditional_cond = unconditional_cond_backup
         concat = torch.cat(sampled, dim=0)
         if clip_output:
@@ -752,14 +795,32 @@
         else:
             res = read_image(image, max_wh, anchor=anchor)
             image = res.image
             original_size = res.original_size
             if alpha is None:
                 alpha = res.alpha
         z = self._get_z(image)
+        highres_info = kwargs.pop("highres_info", None)
+        if highres_info is not None:
+            z = self._get_highres_latent(z, highres_info)
+            if num_steps is None:
+                num_steps = self.sampler.default_steps
+            num_steps = get_highres_steps(num_steps, fidelity)
+            upscale_factor = highres_info["upscale_factor"]
+            original_size = (
+                round(original_size[0] * upscale_factor),
+                round(original_size[1] * upscale_factor),
+            )
+            if alpha is not None:
+                with torch.no_grad():
+                    alpha = F.interpolate(
+                        torch.from_numpy(alpha),
+                        original_size[::-1],
+                        mode="nearest",
+                    ).numpy()
         return self._img2img(
             z,
             export_path,
             fidelity=fidelity,
             original_size=original_size,  # type: ignore
             alpha=alpha,
             cond=cond,
@@ -1257,14 +1318,23 @@
                 cond=cond,
                 num_steps=num_steps,
                 clip_output=clip_output,
                 verbose=verbose,
                 **kwargs,
             )
 
+    def _get_highres_latent(self, z: Tensor, highres_info: Dict[str, Any]) -> Tensor:
+        upscale_factor = highres_info["upscale_factor"]
+        shrink_factor = self.size_info.factor
+        max_wh = round(highres_info["max_wh"] / shrink_factor)
+        h, w = z.shape[-2:]
+        upscaled = round(w * upscale_factor), round(h * upscale_factor)
+        w, h = get_size(upscaled, 64 // shrink_factor, max_wh)  # type: ignore
+        return F.interpolate(z, size=(h, w), mode="bilinear", antialias=False)
+
 
 def offset_cnet_weights(
     d: tensor_dict_type,
     *,
     api: Optional[DiffusionAPI] = None,
     base_md: Optional[tensor_dict_type] = None,
 ) -> tensor_dict_type:
```

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/blip.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/blip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/api.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/predictor.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/inference/transforms.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/inference/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/mconfigs/base.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/mconfigs/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/dih_model.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/dih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/modeling/unet.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/modeling/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/iharm/model/ops.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/iharm/model/ops.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/isnet.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/isnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/lama.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/lama.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/api.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/blocks.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/dpt_depth.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/midas_net_custom.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/transforms.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/core/vit.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/core/vit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/midas/utils.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/midas/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/api.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/mlsd/utils.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/api.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/body.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/body.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/hand.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/model.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/openpose/util.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/openpose/util.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/third_party/prompt.py` & `carefree-learn-0.4.3/cflearn/api/cv/third_party/prompt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/cv/translator.py` & `carefree-learn-0.4.3/cflearn/api/cv/translator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/ml/ddr.py` & `carefree-learn-0.4.3/cflearn/api/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/schema.py` & `carefree-learn-0.4.3/cflearn/api/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/utils.py` & `carefree-learn-0.4.3/cflearn/api/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/api/zoo/__init__.py` & `carefree-learn-0.4.3/cflearn/api/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/callbacks/classification.py` & `carefree-learn-0.4.3/cflearn/callbacks/classification.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/callbacks/general.py` & `carefree-learn-0.4.3/cflearn/callbacks/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/callbacks/generator.py` & `carefree-learn-0.4.3/cflearn/callbacks/generator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/constants.py` & `carefree-learn-0.4.3/cflearn/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/array.py` & `carefree-learn-0.4.3/cflearn/data/array.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/cv/crop.py` & `carefree-learn-0.4.3/cflearn/data/blocks/cv/crop.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/cv/image_folder.py` & `carefree-learn-0.4.3/cflearn/data/blocks/cv/image_folder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/cv/normalize.py` & `carefree-learn-0.4.3/cflearn/data/blocks/cv/normalize.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/cv/to_numpy.py` & `carefree-learn-0.4.3/cflearn/data/blocks/cv/to_numpy.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/cv/tuple_to_batch.py` & `carefree-learn-0.4.3/cflearn/data/blocks/cv/tuple_to_batch.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/file.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/file.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/gather.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/gather.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/nan_handler.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/nan_handler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/preprocessor.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/preprocessor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/recognizer.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/recognizer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/blocks/ml/splitter.py` & `carefree-learn-0.4.3/cflearn/data/blocks/ml/splitter.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/ml/api.py` & `carefree-learn-0.4.3/cflearn/data/ml/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/ml/datasets.py` & `carefree-learn-0.4.3/cflearn/data/ml/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/pytorch/api.py` & `carefree-learn-0.4.3/cflearn/data/pytorch/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/pytorch/datasets.py` & `carefree-learn-0.4.3/cflearn/data/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/data/utils.py` & `carefree-learn-0.4.3/cflearn/data/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/dist/ml/experiment.py` & `carefree-learn-0.4.3/cflearn/dist/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/dist/ml/runs/_utils.py` & `carefree-learn-0.4.3/cflearn/dist/ml/runs/_utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/dist/ml/task.py` & `carefree-learn-0.4.3/cflearn/dist/ml/task.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/inference.py` & `carefree-learn-0.4.3/cflearn/inference.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/losses/basic.py` & `carefree-learn-0.4.3/cflearn/losses/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/losses/gan.py` & `carefree-learn-0.4.3/cflearn/losses/gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/losses/lpips.py` & `carefree-learn-0.4.3/cflearn/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/losses/vae.py` & `carefree-learn-0.4.3/cflearn/losses/vae.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/metrics.py` & `carefree-learn-0.4.3/cflearn/metrics.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/misc/available.json` & `carefree-learn-0.4.3/cflearn/misc/available.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/misc/mixins.py` & `carefree-learn-0.4.3/cflearn/misc/mixins.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/misc/toolkit.py` & `carefree-learn-0.4.3/cflearn/misc/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,37 +369,100 @@
         show_or_save(export_path)
 
 
 # dl
 
 
 pt2_sdp_attn = getattr(F, "scaled_dot_product_attention", None)
+warnings = set()
 
 
-def sdp_attn(
+def warn_once(message: str, *, key: Optional[str] = None) -> None:
+    key = key or message
+    if key not in warnings:
+        print_warning(message)
+        warnings.add(key)
+
+
+def try_run_xformers_sdp_attn(
+    q: Tensor,
+    k: Tensor,
+    v: Tensor,
+    training: bool,
+    mask: Optional[Tensor] = None,
+    p: Optional[float] = None,
+) -> Optional[Tensor]:
+    try:
+        import xformers.ops
+
+        if p is None:
+            p = 0.0
+        return xformers.ops.memory_efficient_attention(q, k, v, mask, p)
+    except Exception as err:
+        warn_once(f"failed to run `xformers` sdp attn: {err}")
+        return None
+
+
+def _sdp_attn(
     q: Tensor,
     k: Tensor,
     v: Tensor,
     training: bool,
     mask: Optional[Tensor] = None,
     dropout: Optional[float] = None,
 ) -> Tensor:
+    q = q.contiguous()
+    k = k.contiguous()
+    v = v.contiguous()
     if pt2_sdp_attn is not None:
         dropout = dropout if training else None
         dropout = 0.0 if dropout is None else dropout
         return pt2_sdp_attn(q, k, v, mask, dropout)
     raw_weights = q @ k.transpose(-2, -1) / math.sqrt(k.shape[-1])
     if mask is not None:
         raw_weights.masked_fill_(~mask, float("-inf"))
     weights = F.softmax(raw_weights, dim=-1)
     if training and dropout is not None and 0.0 < dropout < 1.0:
         weights = F.dropout(weights, dropout)
     return weights @ v
 
 
+def sdp_attn(
+    q: Tensor,
+    k: Tensor,
+    v: Tensor,
+    training: bool,
+    mask: Optional[Tensor] = None,
+    dropout: Optional[float] = None,
+    split_chunk: Optional[int] = None,
+) -> Tensor:
+    q = q.contiguous()
+    k = k.contiguous()
+    v = v.contiguous()
+    try_xformers = try_run_xformers_sdp_attn(q, k, v, training, mask, dropout)
+    if try_xformers is not None:
+        return try_xformers
+    size = q.shape[0]
+    if split_chunk is None:
+        if mask is not None and len(mask.shape) == 3:
+            b = mask.shape[0]
+            mask = mask.view(b, -1)
+            mask = mask[:, None, :].repeat(size // b, 1, 1)
+        return _sdp_attn(q, k, v, training, mask)
+    if mask is not None:
+        msg = "`mask` is not supported yet when `attn_split_chunk` is enabled"
+        raise ValueError(msg)
+    tq = q.shape[1]
+    net = torch.zeros(size, tq, v.shape[2], dtype=q.dtype, device=q.device)
+    for i in range(0, size, split_chunk):
+        end = i + split_chunk
+        net[i:end] = _sdp_attn(q[i:end], k[i:end], v[i:end], training, dropout=dropout)
+    return net
+
+
 def get_tensors(inp: Union[str, tensor_dict_type]) -> tensor_dict_type:
     if isinstance(inp, str):
         if inp.endswith(".safetensors"):
             inp = load_file(inp)
         else:
             inp = torch.load(inp, map_location="cpu")
     if "state_dict" in inp:
```

### Comparing `carefree-learn-0.4.2/cflearn/models/bases.py` & `carefree-learn-0.4.3/cflearn/models/bases.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/ae/common.py` & `carefree-learn-0.4.3/cflearn/models/cv/ae/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/ae/kl.py` & `carefree-learn-0.4.3/cflearn/models/cv/ae/kl.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/ae/vq.py` & `carefree-learn-0.4.3/cflearn/models/cv/ae/vq.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/classifier/vanilla.py` & `carefree-learn-0.4.3/cflearn/models/cv/classifier/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/attn.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/schema.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/style_gan_v2.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/style_gan_v2.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/vanilla.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/decoder/vqgan.py` & `carefree-learn-0.4.3/cflearn/models/cv/decoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/clip.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/rescaler.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/rescaler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/cond_models/schema.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/cond_models/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/ddpm.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/ldm.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/ldm.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,19 @@
             z,
             cond=cond,
             num_steps=num_steps,
             start_step=start_step,
             verbose=verbose,
             **kwargs,
         )
+        if kwargs.get("return_latent", False):
+            return latent
+        callback = kwargs.get("decode_callback")
+        if callback is not None:
+            callback()
         net = self._from_latent(latent)
         return net
 
     def _preprocess(self, net: Tensor, *, deterministic: bool = False) -> Tensor:
         net = self.first_stage.encode(net)
         if isinstance(net, GaussianDistribution):
             net = net.mode() if deterministic else net.sample()
```

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/basic.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/ddim.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/k_samplers.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/k_samplers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/plms.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/schema.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/solver.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/solver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/samplers/utils.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/unet.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/diffusion/utils.py` & `carefree-learn-0.4.3/cflearn/models/cv/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/attn.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/api.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/core.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/resnet.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/transformer.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/models/vgg.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/models/vgg.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/backbone/register.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/backbone/register.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/fnet.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/fnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/mixer.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/mixer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/perceiver.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/pool_former.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/pool_former.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/schema.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/transformer.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/vanilla.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/encoder/vqgan.py` & `carefree-learn-0.4.3/cflearn/models/cv/encoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/gan/discriminators.py` & `carefree-learn-0.4.3/cflearn/models/cv/gan/discriminators.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/gan/schema.py` & `carefree-learn-0.4.3/cflearn/models/cv/gan/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/gan/vanilla.py` & `carefree-learn-0.4.3/cflearn/models/cv/gan/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/general.py` & `carefree-learn-0.4.3/cflearn/models/cv/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/cv/translator/rrdb.py` & `carefree-learn-0.4.3/cflearn/models/cv/translator/rrdb.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/implicit/siren.py` & `carefree-learn-0.4.3/cflearn/models/implicit/siren.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/base.py` & `carefree-learn-0.4.3/cflearn/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/ddr.py` & `carefree-learn-0.4.3/cflearn/models/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/encoders.py` & `carefree-learn-0.4.3/cflearn/models/ml/encoders.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/fcnn.py` & `carefree-learn-0.4.3/cflearn/models/ml/fcnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/linear.py` & `carefree-learn-0.4.3/cflearn/models/ml/linear.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/mixed_stacked.py` & `carefree-learn-0.4.3/cflearn/models/ml/mixed_stacked.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/nbm.py` & `carefree-learn-0.4.3/cflearn/models/ml/nbm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/ndt.py` & `carefree-learn-0.4.3/cflearn/models/ml/ndt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/rnn.py` & `carefree-learn-0.4.3/cflearn/models/ml/rnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/ml/wnd.py` & `carefree-learn-0.4.3/cflearn/models/ml/wnd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/multimodal/clip.py` & `carefree-learn-0.4.3/cflearn/models/multimodal/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/multimodal/schema.py` & `carefree-learn-0.4.3/cflearn/models/multimodal/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/encoder/transformer.py` & `carefree-learn-0.4.3/cflearn/models/nlp/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/clip.py` & `carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/tokenizers/schema.py` & `carefree-learn-0.4.3/cflearn/models/nlp/tokenizers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/transformers/core.py` & `carefree-learn-0.4.3/cflearn/models/nlp/transformers/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/transformers/opus.py` & `carefree-learn-0.4.3/cflearn/models/nlp/transformers/opus.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/nlp/transformers/simbert.py` & `carefree-learn-0.4.3/cflearn/models/nlp/transformers/simbert.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/schemas/custom.py` & `carefree-learn-0.4.3/cflearn/models/schemas/custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/models/schemas/cv.py` & `carefree-learn-0.4.3/cflearn/models/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/__init__.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/activations.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/activations.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/attentions.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/attentions.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,31 +547,17 @@
 
         # (B * head, Tq, dim)
         q = self.transpose(q)
         # (B * head, Tc, dim)
         k = self.transpose(k)
         v = self.transpose(v)
 
-        if self.attn_split_chunk is None:
-            if mask is not None:
-                mask = mask.view(b, -1)
-                mask = mask[:, None, :].repeat(self.num_heads, 1, 1)
-                mask = ~mask
-            net = sdp_attn(q, k, v, self.training, mask)
-        else:
-            if mask is not None:
-                msg = "`mask` is not supported yet when `attn_split_chunk` is enabled"
-                raise ValueError(msg)
-            size = b * self.num_heads
-            # (B * head, Tq, dim)
-            net = torch.zeros(size, tq, v.shape[2], dtype=q.dtype, device=q.device)
-            for i in range(0, size, self.attn_split_chunk):
-                end = i + self.attn_split_chunk
-                net[i:end] = sdp_attn(q[i:end], k[i:end], v[i:end], self.training)
-
+        if mask is not None:
+            mask = ~mask
+        net = sdp_attn(q, k, v, self.training, mask, split_chunk=self.attn_split_chunk)
         # (B, head, Tq, dim)
         net = net.reshape(b, self.num_heads, tq, dq // self.num_heads)
         # (B, Tq, head, dim)
         net = net.permute(0, 2, 1, 3).contiguous()
         # (B, Tq, D)
         net = net.view(b, tq, dq)
         # (B, Tq, Dq)
```

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/common.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/convs/basic.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/convs/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/convs/residual.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/convs/residual.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/customs.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/customs.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/high_level.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/high_level.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/hijacks.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/hijacks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/hooks.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/hooks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/implementations/perceiver.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/implementations/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mappings.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mappings.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/api.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/channel_mixers.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/channel_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/poolers.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/poolers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/schema.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/mixed_stacks/token_mixers.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/mixed_stacks/token_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/norms.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/norms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/blocks/utils.py` & `carefree-learn-0.4.3/cflearn/modules/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/optimizers.py` & `carefree-learn-0.4.3/cflearn/modules/optimizers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/modules/schedulers.py` & `carefree-learn-0.4.3/cflearn/modules/schedulers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/monitors.py` & `carefree-learn-0.4.3/cflearn/monitors.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/parameters.py` & `carefree-learn-0.4.3/cflearn/parameters.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/api.py` & `carefree-learn-0.4.3/cflearn/pipeline/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/blocks/basic.py` & `carefree-learn-0.4.3/cflearn/pipeline/blocks/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/blocks/ml.py` & `carefree-learn-0.4.3/cflearn/pipeline/blocks/ml.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/blocks/utils.py` & `carefree-learn-0.4.3/cflearn/pipeline/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/core.py` & `carefree-learn-0.4.3/cflearn/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/pipeline/third_party.py` & `carefree-learn-0.4.3/cflearn/pipeline/third_party.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/schema.py` & `carefree-learn-0.4.3/cflearn/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/scripts/sd.py` & `carefree-learn-0.4.3/cflearn/scripts/sd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/trainer.py` & `carefree-learn-0.4.3/cflearn/trainer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/types.py` & `carefree-learn-0.4.3/cflearn/types.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/configs/ae/kl/f4.json` & `carefree-learn-0.4.3/cflearn/zoo/configs/ae/kl/f4.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ddpm/default.json` & `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ddpm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/default.json` & `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/configs/diffusion/ldm/vq.json` & `carefree-learn-0.4.3/cflearn/zoo/configs/diffusion/ldm/vq.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/configs/multimodal/clip/chinese.json` & `carefree-learn-0.4.3/cflearn/zoo/configs/multimodal/clip/chinese.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/core.py` & `carefree-learn-0.4.3/cflearn/zoo/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/cflearn/zoo/models/clip.py` & `carefree-learn-0.4.3/cflearn/zoo/models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.2/setup.py` & `carefree-learn-0.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.4.2"
+VERSION = "0.4.3"
 DESCRIPTION = "Deep Learning with PyTorch made easy"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 cv_requires = [
     "ftfy",
     "lmdb",
@@ -17,14 +17,15 @@
     "scikit-image",
     "scipy>=1.8.0",
     "opencv-python-headless",
 ]
 cv_full_requires = cv_requires + [
     "timm",
     "salesforce-lavis",
+    "xformers>=0.0.19",
 ]
 onnx_requires = [
     "onnx",
     "onnxruntime",
     "onnx-simplifier>=0.4.1",
 ]
```

