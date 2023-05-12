# Comparing `tmp/ml-swissknife-0.1.8.tar.gz` & `tmp/ml-swissknife-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-swissknife-0.1.8.tar", last modified: Fri Dec  9 23:19:28 2022, max compression
+gzip compressed data, was "ml-swissknife-0.1.9.tar", last modified: Sat Dec 10 00:23:21 2022, max compression
```

## Comparing `ml-swissknife-0.1.8.tar` & `ml-swissknife-0.1.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.282003 ml-swissknife-0.1.8/
--rw-r--r--   0 xuechenli   (501) staff       (20)     1067 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/LICENSE
--rw-r--r--   0 xuechenli   (501) staff       (20)      421 2022-12-09 23:19:28.282084 ml-swissknife-0.1.8/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     1142 2022-08-15 00:15:27.000000 ml-swissknife-0.1.8/README.md
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.261563 ml-swissknife-0.1.8/experiments/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.263041 ml-swissknife-0.1.8/experiments/dp_semisup/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/dp_semisup/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    19158 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/dp_semisup/gaussian_model.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.267293 ml-swissknife-0.1.8/experiments/ee364a/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     9402 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a10_4.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3546 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a11_8.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1793 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a14_4.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    25943 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a15_13.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2055 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a16_2.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      938 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a17_16.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1047 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a17_4.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3483 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a20_4.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2331 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a20_9.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1352 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a21_22.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      742 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a4_2.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5574 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a4_20.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1919 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a4_28.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      982 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a5_1.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1410 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a6_3.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      863 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/a6_9.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      804 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/a7_18.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      198 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/ee364a/common.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      428 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/ee364a/midterm.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.269307 ml-swissknife-0.1.8/experiments/explainx/
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.269493 ml-swissknife-0.1.8/experiments/explainx/BLIP/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/__init__.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.271646 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    17925 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2839 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_itm.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4179 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_nlvr.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    15407 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_pretrain.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    13111 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_retrieval.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     8305 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_vqa.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    41755 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/med.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    36199 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/nlvr_encoder.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    14070 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/BLIP/models/vit.py
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7484 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/celeba_check.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5010 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/colored_mnist.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1316 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/common.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.273078 ml-swissknife-0.1.8/experiments/explainx/launchers/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      840 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/analyze.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      655 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/feb2822.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1199 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/mar0222.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1246 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/mar1022.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1325 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/mar1122.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      812 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/launchers/waterbird_check.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    19894 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/loop.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2222 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/misc.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      457 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/numerical.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5090 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/run.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.274011 ml-swissknife-0.1.8/experiments/explainx/search_engine/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/search_engine/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     3307 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/search_engine/annotated_beam_scorer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    19206 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/search_engine/base.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    21732 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/search_engine/contrastive_captioner.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    41936 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/explainx/search_engine/mixture_captioner.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7979 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/explainx/waterbird_check.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.275649 ml-swissknife-0.1.8/experiments/priv_fair/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/priv_fair/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     7307 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/image_cls.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.276691 ml-swissknife-0.1.8/experiments/priv_fair/plots/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/priv_fair/plots/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2718 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/plots/acc_on_the_line.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2375 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/plots/pos_transfer.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2808 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/plots/priv_fair.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2638 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/plots/priv_fair_scale.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      505 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/priv_fair/shared.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4623 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/transfer_cifar.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    15184 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/priv_fair/transfer_cifar_v2.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.277734 ml-swissknife-0.1.8/experiments/simclrv2/
--rw-r--r--   0 xuechenli   (501) staff       (20)      296 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4943 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2/convert.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2017 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2/download.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6996 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2/resnet.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2413 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2/verify.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.278763 ml-swissknife-0.1.8/experiments/simclrv2_florian/
--rw-r--r--   0 xuechenli   (501) staff       (20)      139 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2_florian/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2258 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2_florian/download.py
--rw-r--r--   0 xuechenli   (501) staff       (20)      397 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2_florian/download_all.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    12181 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/experiments/simclrv2_florian/extract_simclr.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     6996 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/experiments/simclrv2_florian/resnet.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.280945 ml-swissknife-0.1.8/ml_swissknife/
--rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/ml_swissknife/__init__.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     5017 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/ml_swissknife/blocks.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1390 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/ml_swissknife/distributed_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)    12003 2022-07-06 06:26:05.000000 ml-swissknife-0.1.8/ml_swissknife/numerical.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     9684 2022-08-15 05:00:25.000000 ml-swissknife-0.1.8/ml_swissknife/numerical_distributed.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     2155 2022-12-09 23:18:51.000000 ml-swissknife-0.1.8/ml_swissknife/openai_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)   112008 2022-11-13 18:42:34.000000 ml-swissknife-0.1.8/ml_swissknife/utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     1950 2022-08-14 00:06:14.000000 ml-swissknife-0.1.8/ml_swissknife/wandb_utils.py
--rw-r--r--   0 xuechenli   (501) staff       (20)     4992 2022-11-15 07:16:55.000000 ml-swissknife-0.1.8/ml_swissknife/wrapper.py
-drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-09 23:19:28.281859 ml-swissknife-0.1.8/ml_swissknife.egg-info/
--rw-r--r--   0 xuechenli   (501) staff       (20)      421 2022-12-09 23:19:28.000000 ml-swissknife-0.1.8/ml_swissknife.egg-info/PKG-INFO
--rw-r--r--   0 xuechenli   (501) staff       (20)     3253 2022-12-09 23:19:28.000000 ml-swissknife-0.1.8/ml_swissknife.egg-info/SOURCES.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)        1 2022-12-09 23:19:28.000000 ml-swissknife-0.1.8/ml_swissknife.egg-info/dependency_links.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)      190 2022-12-09 23:19:28.000000 ml-swissknife-0.1.8/ml_swissknife.egg-info/requires.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       26 2022-12-09 23:19:28.000000 ml-swissknife-0.1.8/ml_swissknife.egg-info/top_level.txt
--rw-r--r--   0 xuechenli   (501) staff       (20)       79 2022-12-09 23:19:28.282406 ml-swissknife-0.1.8/setup.cfg
--rw-r--r--   0 xuechenli   (501) staff       (20)      952 2022-12-09 23:18:51.000000 ml-swissknife-0.1.8/setup.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.108483 ml-swissknife-0.1.9/
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1067 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/LICENSE
+-rw-r--r--   0 xuechenli   (501) staff       (20)      421 2022-12-10 00:23:21.108564 ml-swissknife-0.1.9/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1142 2022-08-15 00:15:27.000000 ml-swissknife-0.1.9/README.md
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.089017 ml-swissknife-0.1.9/experiments/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.090417 ml-swissknife-0.1.9/experiments/dp_semisup/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/dp_semisup/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    19158 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/dp_semisup/gaussian_model.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.094997 ml-swissknife-0.1.9/experiments/ee364a/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     9402 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a10_4.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3546 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a11_8.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1793 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a14_4.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    25943 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a15_13.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2055 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a16_2.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      938 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a17_16.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1047 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a17_4.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3483 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a20_4.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2331 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a20_9.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1352 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a21_22.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      742 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a4_2.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5574 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a4_20.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1919 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a4_28.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      982 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a5_1.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1410 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a6_3.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      863 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/a6_9.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      804 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/a7_18.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      198 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/ee364a/common.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      428 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/ee364a/midterm.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.097248 ml-swissknife-0.1.9/experiments/explainx/
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.097414 ml-swissknife-0.1.9/experiments/explainx/BLIP/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/__init__.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.099576 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    17925 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2839 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_itm.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4179 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_nlvr.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    15407 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_pretrain.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    13111 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_retrieval.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     8305 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_vqa.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    41755 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/med.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    36199 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/nlvr_encoder.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    14070 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/BLIP/models/vit.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7484 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/celeba_check.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5010 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/colored_mnist.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1316 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/common.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.100745 ml-swissknife-0.1.9/experiments/explainx/launchers/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      840 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/analyze.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      655 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/feb2822.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1199 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/mar0222.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1246 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/mar1022.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1325 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/mar1122.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      812 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/launchers/waterbird_check.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    19894 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/loop.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2222 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/misc.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      457 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/numerical.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5090 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/run.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.101610 ml-swissknife-0.1.9/experiments/explainx/search_engine/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/search_engine/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3307 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/search_engine/annotated_beam_scorer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    19206 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/search_engine/base.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    21732 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/search_engine/contrastive_captioner.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    41936 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/explainx/search_engine/mixture_captioner.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7979 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/explainx/waterbird_check.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.103023 ml-swissknife-0.1.9/experiments/priv_fair/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/priv_fair/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     7307 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/image_cls.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.103905 ml-swissknife-0.1.9/experiments/priv_fair/plots/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/priv_fair/plots/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2718 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/plots/acc_on_the_line.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2375 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/plots/pos_transfer.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2808 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/plots/priv_fair.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2638 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/plots/priv_fair_scale.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      505 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/priv_fair/shared.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4623 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/transfer_cifar.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    15184 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/priv_fair/transfer_cifar_v2.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.104832 ml-swissknife-0.1.9/experiments/simclrv2/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      296 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4943 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2/convert.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2017 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2/download.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6996 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2/resnet.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2413 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2/verify.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.105632 ml-swissknife-0.1.9/experiments/simclrv2_florian/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      139 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2_florian/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2258 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2_florian/download.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)      397 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2_florian/download_all.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12181 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/experiments/simclrv2_florian/extract_simclr.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     6996 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/experiments/simclrv2_florian/resnet.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.107526 ml-swissknife-0.1.9/ml_swissknife/
+-rw-r--r--   0 xuechenli   (501) staff       (20)        0 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/ml_swissknife/__init__.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     5017 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/ml_swissknife/blocks.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1390 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/ml_swissknife/distributed_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)    12003 2022-07-06 06:26:05.000000 ml-swissknife-0.1.9/ml_swissknife/numerical.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     9684 2022-08-15 05:00:25.000000 ml-swissknife-0.1.9/ml_swissknife/numerical_distributed.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     2507 2022-12-10 00:22:18.000000 ml-swissknife-0.1.9/ml_swissknife/openai_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)   112008 2022-11-13 18:42:34.000000 ml-swissknife-0.1.9/ml_swissknife/utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     1950 2022-08-14 00:06:14.000000 ml-swissknife-0.1.9/ml_swissknife/wandb_utils.py
+-rw-r--r--   0 xuechenli   (501) staff       (20)     4992 2022-11-15 07:16:55.000000 ml-swissknife-0.1.9/ml_swissknife/wrapper.py
+drwxr-xr-x   0 xuechenli   (501) staff       (20)        0 2022-12-10 00:23:21.108358 ml-swissknife-0.1.9/ml_swissknife.egg-info/
+-rw-r--r--   0 xuechenli   (501) staff       (20)      421 2022-12-10 00:23:21.000000 ml-swissknife-0.1.9/ml_swissknife.egg-info/PKG-INFO
+-rw-r--r--   0 xuechenli   (501) staff       (20)     3253 2022-12-10 00:23:21.000000 ml-swissknife-0.1.9/ml_swissknife.egg-info/SOURCES.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)        1 2022-12-10 00:23:21.000000 ml-swissknife-0.1.9/ml_swissknife.egg-info/dependency_links.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)      190 2022-12-10 00:23:21.000000 ml-swissknife-0.1.9/ml_swissknife.egg-info/requires.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       26 2022-12-10 00:23:21.000000 ml-swissknife-0.1.9/ml_swissknife.egg-info/top_level.txt
+-rw-r--r--   0 xuechenli   (501) staff       (20)       79 2022-12-10 00:23:21.108874 ml-swissknife-0.1.9/setup.cfg
+-rw-r--r--   0 xuechenli   (501) staff       (20)      960 2022-12-10 00:20:58.000000 ml-swissknife-0.1.9/setup.py
```

### Comparing `ml-swissknife-0.1.8/LICENSE` & `ml-swissknife-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/README.md` & `ml-swissknife-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/dp_semisup/gaussian_model.py` & `ml-swissknife-0.1.9/experiments/dp_semisup/gaussian_model.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a10_4.py` & `ml-swissknife-0.1.9/experiments/ee364a/a10_4.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a11_8.py` & `ml-swissknife-0.1.9/experiments/ee364a/a11_8.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a14_4.py` & `ml-swissknife-0.1.9/experiments/ee364a/a14_4.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a15_13.py` & `ml-swissknife-0.1.9/experiments/ee364a/a15_13.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a16_2.py` & `ml-swissknife-0.1.9/experiments/ee364a/a16_2.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a17_16.py` & `ml-swissknife-0.1.9/experiments/ee364a/a17_16.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a17_4.py` & `ml-swissknife-0.1.9/experiments/ee364a/a17_4.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a20_4.py` & `ml-swissknife-0.1.9/experiments/ee364a/a20_4.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a20_9.py` & `ml-swissknife-0.1.9/experiments/ee364a/a20_9.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a21_22.py` & `ml-swissknife-0.1.9/experiments/ee364a/a21_22.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a4_2.py` & `ml-swissknife-0.1.9/experiments/ee364a/a4_2.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a4_20.py` & `ml-swissknife-0.1.9/experiments/ee364a/a4_20.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a4_28.py` & `ml-swissknife-0.1.9/experiments/ee364a/a4_28.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a5_1.py` & `ml-swissknife-0.1.9/experiments/ee364a/a5_1.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a6_3.py` & `ml-swissknife-0.1.9/experiments/ee364a/a6_3.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a6_9.py` & `ml-swissknife-0.1.9/experiments/ee364a/a6_9.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/ee364a/a7_18.py` & `ml-swissknife-0.1.9/experiments/ee364a/a7_18.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_itm.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_itm.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_nlvr.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_nlvr.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_pretrain.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_retrieval.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_retrieval.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/blip_vqa.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/blip_vqa.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/med.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/med.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/nlvr_encoder.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/nlvr_encoder.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/BLIP/models/vit.py` & `ml-swissknife-0.1.9/experiments/explainx/BLIP/models/vit.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/celeba_check.py` & `ml-swissknife-0.1.9/experiments/explainx/celeba_check.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/colored_mnist.py` & `ml-swissknife-0.1.9/experiments/explainx/colored_mnist.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/common.py` & `ml-swissknife-0.1.9/experiments/explainx/common.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/analyze.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/analyze.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/feb2822.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/feb2822.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/mar0222.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/mar0222.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/mar1022.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/mar1022.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/mar1122.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/mar1122.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/launchers/waterbird_check.py` & `ml-swissknife-0.1.9/experiments/explainx/launchers/waterbird_check.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/loop.py` & `ml-swissknife-0.1.9/experiments/explainx/loop.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/misc.py` & `ml-swissknife-0.1.9/experiments/explainx/misc.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/run.py` & `ml-swissknife-0.1.9/experiments/explainx/run.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/search_engine/annotated_beam_scorer.py` & `ml-swissknife-0.1.9/experiments/explainx/search_engine/annotated_beam_scorer.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/search_engine/base.py` & `ml-swissknife-0.1.9/experiments/explainx/search_engine/base.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/search_engine/contrastive_captioner.py` & `ml-swissknife-0.1.9/experiments/explainx/search_engine/contrastive_captioner.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/search_engine/mixture_captioner.py` & `ml-swissknife-0.1.9/experiments/explainx/search_engine/mixture_captioner.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/explainx/waterbird_check.py` & `ml-swissknife-0.1.9/experiments/explainx/waterbird_check.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/image_cls.py` & `ml-swissknife-0.1.9/experiments/priv_fair/image_cls.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/plots/acc_on_the_line.py` & `ml-swissknife-0.1.9/experiments/priv_fair/plots/acc_on_the_line.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/plots/pos_transfer.py` & `ml-swissknife-0.1.9/experiments/priv_fair/plots/pos_transfer.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/plots/priv_fair.py` & `ml-swissknife-0.1.9/experiments/priv_fair/plots/priv_fair.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/plots/priv_fair_scale.py` & `ml-swissknife-0.1.9/experiments/priv_fair/plots/priv_fair_scale.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/transfer_cifar.py` & `ml-swissknife-0.1.9/experiments/priv_fair/transfer_cifar.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/priv_fair/transfer_cifar_v2.py` & `ml-swissknife-0.1.9/experiments/priv_fair/transfer_cifar_v2.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2/convert.py` & `ml-swissknife-0.1.9/experiments/simclrv2/convert.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2/download.py` & `ml-swissknife-0.1.9/experiments/simclrv2/download.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2/resnet.py` & `ml-swissknife-0.1.9/experiments/simclrv2/resnet.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2/verify.py` & `ml-swissknife-0.1.9/experiments/simclrv2/verify.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2_florian/download.py` & `ml-swissknife-0.1.9/experiments/simclrv2_florian/download.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2_florian/extract_simclr.py` & `ml-swissknife-0.1.9/experiments/simclrv2_florian/extract_simclr.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/experiments/simclrv2_florian/resnet.py` & `ml-swissknife-0.1.9/experiments/simclrv2_florian/resnet.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/blocks.py` & `ml-swissknife-0.1.9/ml_swissknife/blocks.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/distributed_utils.py` & `ml-swissknife-0.1.9/ml_swissknife/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/numerical.py` & `ml-swissknife-0.1.9/ml_swissknife/numerical.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/numerical_distributed.py` & `ml-swissknife-0.1.9/ml_swissknife/numerical_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/openai_utils.py` & `ml-swissknife-0.1.9/ml_swissknife/openai_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Light wrapper around OpenAI API.
 
 Should not rewrite these multiple times for different projects...
+
+For reference:
+    https://beta.openai.com/docs/api-reference/completions/create
 """
 import dataclasses
 import logging
 import math
 import sys
 import time
-from typing import Union, Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import openai
 import tqdm
 
 
 @dataclasses.dataclass
 class DecodingArguments(object):
@@ -26,15 +29,16 @@
     # stop: Optional[Tuple[str, ...]] = ("}\n\nstatic", "}\n\n/*")
 
 
 def _openai_completion(
     model_name, prompts: Union[str, list, tuple], decoding_args, sleep_time=2, batch_size=1,
     max_batches=sys.maxsize,  # This should only be used during testing.
 ):
-    if isinstance(prompts, str):
+    is_single_prompt = isinstance(prompts, str)
+    if is_single_prompt:
         prompts = [prompts]
 
     num_prompts = len(prompts)
     prompt_batches = [
         prompts[batch_id * batch_size: (batch_id + 1) * batch_size]
         for batch_id in range(int(math.ceil(num_prompts / batch_size)))
     ]
@@ -62,8 +66,14 @@
                 )
                 completions.extend(completion_batch.choices)
                 break
             except Exception as e:
                 logging.warning('Hit request rate limit; retrying...')
                 time.sleep(sleep_time)  # Annoying rate limit on requests.
 
+    if is_single_prompt and decoding_args.n == 1:
+        completions, = completions  # Return non-tuple if only 1 input and 1 generation.
     return completions
+
+
+# Keep the private function for backwards compat.
+openai_completion = _openai_completion
```

### Comparing `ml-swissknife-0.1.8/ml_swissknife/utils.py` & `ml-swissknife-0.1.9/ml_swissknife/utils.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/wandb_utils.py` & `ml-swissknife-0.1.9/ml_swissknife/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife/wrapper.py` & `ml-swissknife-0.1.9/ml_swissknife/wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-swissknife-0.1.8/ml_swissknife.egg-info/SOURCES.txt` & `ml-swissknife-0.1.9/ml_swissknife.egg-info/SOURCES.txt`

 * *Files identical despite different names*

