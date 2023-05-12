# Comparing `tmp/lmqg-0.0.8.tar.gz` & `tmp/lmqg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmqg-0.0.8.tar", last modified: Fri Feb 10 13:53:48 2023, max compression
+gzip compressed data, was "lmqg-0.1.0.tar", last modified: Fri May 12 17:50:07 2023, max compression
```

## Comparing `lmqg-0.0.8.tar` & `lmqg-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.481049 lmqg-0.0.8/
--rw-r--r--   0 asahi      (501) staff       (20)    19917 2021-10-29 09:59:07.000000 lmqg-0.0.8/LICENSE
--rw-r--r--   0 asahi      (501) staff       (20)    10754 2023-02-10 13:53:48.481300 lmqg-0.0.8/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     9958 2023-02-10 10:28:27.000000 lmqg-0.0.8/README.md
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.444673 lmqg-0.0.8/lmqg/
--rw-r--r--   0 asahi      (501) staff       (20)      242 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    12555 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.452325 lmqg-0.0.8/lmqg/automatic_evaluation_tool/
--rw-r--r--   0 asahi      (501) staff       (20)      256 2022-12-04 12:31:54.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/__init__.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.457937 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/
--rw-r--r--   0 asahi      (501) staff       (20)       66 2022-05-20 15:17:04.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    11181 2022-05-20 15:17:04.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/score.py
--rw-r--r--   0 asahi      (501) staff       (20)    11657 2022-09-03 23:52:23.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/scorer.py
--rw-r--r--   0 asahi      (501) staff       (20)    29393 2022-05-20 15:17:04.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/utils.py
--rw-r--r--   0 asahi      (501) staff       (20)      732 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bertscore.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.462676 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/
--rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2155 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/bleu.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     8721 2022-02-18 17:28:54.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.464422 lmqg-0.0.8/lmqg/automatic_evaluation_tool/meteor/
--rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/meteor/__init__.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     7124 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/meteor/meteor.py
--rw-r--r--   0 asahi      (501) staff       (20)     6909 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/moverscore.py
--rw-r--r--   0 asahi      (501) staff       (20)     3748 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py
--rwxr-xr-x   0 asahi      (501) staff       (20)     4510 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/rouge.py
--rw-r--r--   0 asahi      (501) staff       (20)      884 2022-02-18 17:28:54.000000 lmqg-0.0.8/lmqg/automatic_evaluation_tool/text_normalization.py
--rw-r--r--   0 asahi      (501) staff       (20)     2747 2022-12-05 11:07:21.000000 lmqg-0.0.8/lmqg/data.py
--rw-r--r--   0 asahi      (501) staff       (20)     1018 2022-05-20 15:17:04.000000 lmqg-0.0.8/lmqg/exceptions.py
--rw-r--r--   0 asahi      (501) staff       (20)    15623 2022-12-05 11:07:21.000000 lmqg-0.0.8/lmqg/grid_searcher.py
--rw-r--r--   0 asahi      (501) staff       (20)     5726 2023-02-04 21:25:17.000000 lmqg-0.0.8/lmqg/inference_api.py
--rw-r--r--   0 asahi      (501) staff       (20)    34900 2023-02-10 13:53:27.000000 lmqg-0.0.8/lmqg/language_model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.471899 lmqg-0.0.8/lmqg/lmqg_cl/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-09-03 23:52:23.000000 lmqg-0.0.8/lmqg/lmqg_cl/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3413 2022-12-05 11:07:21.000000 lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation.py
--rw-r--r--   0 asahi      (501) staff       (20)     5292 2022-12-05 11:07:21.000000 lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     4297 2023-02-10 10:28:27.000000 lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py
--rw-r--r--   0 asahi      (501) staff       (20)     9018 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qag.py
--rw-r--r--   0 asahi      (501) staff       (20)     6982 2022-12-04 12:31:54.000000 lmqg-0.0.8/lmqg/lmqg_cl/model_finetuning.py
--rw-r--r--   0 asahi      (501) staff       (20)     3120 2022-10-04 10:28:52.000000 lmqg-0.0.8/lmqg/lmqg_cl/push_to_hf.py
--rw-r--r--   0 asahi      (501) staff       (20)    61040 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/lmqg_cl/readme_template.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.479830 lmqg-0.0.8/lmqg/qa_evaluation_tool/
--rw-r--r--   0 asahi      (501) staff       (20)       93 2022-12-04 12:31:54.000000 lmqg-0.0.8/lmqg/qa_evaluation_tool/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3714 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py
--rwxr-xr-x   0 asahi      (501) staff       (20)    22361 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/qa_evaluation_tool/run_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     4741 2022-12-04 12:31:54.000000 lmqg-0.0.8/lmqg/qa_evaluation_tool/trainer_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)    22310 2022-12-04 12:31:54.000000 lmqg-0.0.8/lmqg/qa_evaluation_tool/utils_qa.py
--rw-r--r--   0 asahi      (501) staff       (20)     3102 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/spacy_module.py
--rw-r--r--   0 asahi      (501) staff       (20)    11877 2023-02-04 14:23:33.000000 lmqg-0.0.8/lmqg/trainer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-02-10 13:53:48.447840 lmqg-0.0.8/lmqg.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)    10754 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)     1583 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)      459 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/entry_points.txt
--rw-r--r--   0 asahi      (501) staff       (20)      255 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        5 2023-02-10 13:53:48.000000 lmqg-0.0.8/lmqg.egg-info/top_level.txt
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-02-10 13:53:48.482120 lmqg-0.0.8/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     2782 2023-02-10 13:53:43.000000 lmqg-0.0.8/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.623651 lmqg-0.1.0/
+-rw-r--r--   0 asahi      (501) staff       (20)    19917 2021-10-29 09:59:07.000000 lmqg-0.1.0/LICENSE
+-rw-r--r--   0 asahi      (501) staff       (20)    16475 2023-05-12 17:50:07.623802 lmqg-0.1.0/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)    15679 2023-05-12 17:49:30.000000 lmqg-0.1.0/README.md
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.589243 lmqg-0.1.0/lmqg/
+-rw-r--r--   0 asahi      (501) staff       (20)      382 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    12897 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/automatic_evaluation.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.600200 lmqg-0.1.0/lmqg/automatic_evaluation_tool/
+-rw-r--r--   0 asahi      (501) staff       (20)      256 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/__init__.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.605095 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/
+-rw-r--r--   0 asahi      (501) staff       (20)       66 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    11181 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/score.py
+-rw-r--r--   0 asahi      (501) staff       (20)    11657 2022-09-03 23:52:23.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/scorer.py
+-rw-r--r--   0 asahi      (501) staff       (20)    29393 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/utils.py
+-rw-r--r--   0 asahi      (501) staff       (20)      732 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bertscore.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.608409 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/
+-rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2155 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     8721 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.610530 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/
+-rwxr-xr-x   0 asahi      (501) staff       (20)       21 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/__init__.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     7124 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/meteor.py
+-rw-r--r--   0 asahi      (501) staff       (20)      840 2023-02-26 10:57:31.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor.py
+-rw-r--r--   0 asahi      (501) staff       (20)     6909 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/moverscore.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3748 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)     4510 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/rouge.py
+-rw-r--r--   0 asahi      (501) staff       (20)      884 2022-02-18 17:28:54.000000 lmqg-0.1.0/lmqg/automatic_evaluation_tool/text_normalization.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2747 2022-12-05 11:07:21.000000 lmqg-0.1.0/lmqg/data.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1018 2022-05-20 15:17:04.000000 lmqg-0.1.0/lmqg/exceptions.py
+-rw-r--r--   0 asahi      (501) staff       (20)    16244 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/grid_searcher.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7082 2023-02-22 13:09:46.000000 lmqg-0.1.0/lmqg/inference_api.py
+-rw-r--r--   0 asahi      (501) staff       (20)    35965 2023-03-15 21:59:59.000000 lmqg-0.1.0/lmqg/language_model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.616950 lmqg-0.1.0/lmqg/lmqg_cl/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-09-03 23:52:23.000000 lmqg-0.1.0/lmqg/lmqg_cl/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3645 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5582 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4648 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py
+-rw-r--r--   0 asahi      (501) staff       (20)     9719 2023-03-06 13:07:50.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qag.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7295 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/lmqg_cl/model_finetuning.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1913 2023-03-06 12:09:53.000000 lmqg-0.1.0/lmqg/lmqg_cl/push_to_hf.py
+-rw-r--r--   0 asahi      (501) staff       (20)    61040 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/lmqg_cl/readme_template.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.622685 lmqg-0.1.0/lmqg/qa_evaluation_tool/
+-rw-r--r--   0 asahi      (501) staff       (20)       93 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3999 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py
+-rwxr-xr-x   0 asahi      (501) staff       (20)    22361 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/run_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4741 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/trainer_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)    22310 2022-12-04 12:31:54.000000 lmqg-0.1.0/lmqg/qa_evaluation_tool/utils_qa.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3102 2023-02-04 14:23:33.000000 lmqg-0.1.0/lmqg/spacy_module.py
+-rw-r--r--   0 asahi      (501) staff       (20)    12421 2023-02-12 10:54:29.000000 lmqg-0.1.0/lmqg/trainer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-05-12 17:50:07.592882 lmqg-0.1.0/lmqg.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)    16475 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)     1624 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      516 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/entry_points.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      279 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        5 2023-05-12 17:50:07.000000 lmqg-0.1.0/lmqg.egg-info/top_level.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-05-12 17:50:07.624288 lmqg-0.1.0/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     2900 2023-05-12 17:50:04.000000 lmqg-0.1.0/setup.py
```

### Comparing `lmqg-0.0.8/LICENSE` & `lmqg-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/PKG-INFO` & `lmqg-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,175 @@
-Metadata-Version: 2.1
-Name: lmqg
-Version: 0.0.8
-Summary: Language Model for Question Generation.
-Home-page: https://github.com/asahi417/lm-question-generation
-Author: Asahi Ushio
-Author-email: asahi1992ushio@gmail.com
-License: MIT License
-Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.0.8.tar.gz
-Keywords: language model,question-answering,question-generation
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: api
-License-File: LICENSE
-
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/lmqg/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/lmqg.svg)](https://badge.fury.io/py/lmqg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 [![PyPI status](https://img.shields.io/pypi/status/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 
-# Generative Language Models for Paragraph-Level Question Generation
+# Question and Answer Generation with Language Models
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qg_diagram.png" width="500">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qag.png" width="400">
+  <br><em> Figure 1: Three distinct QAG approaches. </em>
 </p>
 
-This is the official repository of the paper
-["Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 main conference"](https://aclanthology.org/2022.emnlp-main.42/).
-This repository includes following contents:
-- ***QG-Bench***, the first ever multilingual/multidomain QG benchmark.
-- ***Multilingual/multidomain QG models*** fine-tuned on QG-Bench.
-- A python library ***`lmqg`*** developed for question generation in python as well as QG model fine-tuning/evaluation.
-- ***AutoQG***, a web application hosting QG models where user can test the model output interactively. 
-
-### Table of Contents  
-1. **[QG-Bench: multilingual & multidomain QG datasets (+ fine-tuned models)](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md)**
-2. **[LMQG: python library to fine-tune/evaluate QG model](#lmqg-language-model-for-question-generation-)**
-3. **[AutoQG: web application hosting multilingual QG models](#autoqg)**
-4. **[RestAPI: run model prediction via restAPI](#rest-api-with-huggingface-inference-api)**
+The `lmqg` is a python library for question and answer generation (QAG) with language models (LMs). Here, we consider 
+paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
+question and answer pairs on the context. With `lmqg`, you can do following things:
+- [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
+- [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
+- [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
+- [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
+ 
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
+
+### A bit more about QAG models 📝
+Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
+and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
+where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
+The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
+Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
+In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
+and the quality of the generated question and answer pairs depend on language.
+All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
+To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
-Please cite following paper if you use any resource:
-```
-@inproceedings{ushio-etal-2022-generative,
-    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
-    author = "Ushio, Asahi  and
-        Alva-Manchego, Fernando  and
-        Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
-    month = dec,
-    year = "2022",
-    address = "Abu Dhabi, U.A.E.",
-    publisher = "Association for Computational Linguistics",
-}
-```
+### Is QAG different from Question Generation (QG)? 🤔
 
-## LMQG: Language Model for Question Generation 🚀
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
+  <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
+</p>
+
+All the functionalities support question generation as well. Our QG model assumes user to specify an answer in addition to a context,
+and the QG model will generate a question that is answerable by the answer given the context (see Figure 2 for a comparison of QAG and QG).
+To know more about QG, please check [our EMNLP 2022 paper](https://aclanthology.org/2022.emnlp-main.42/) that describes the QG models more in detail.
+
+
+## Get Started 🚀
 
-The `lmqg` is a python library to fine-tune seq2seq language models ([T5](https://arxiv.org/pdf/1910.10683.pdf), [BART](https://arxiv.org/pdf/1910.13461.pdf)) 
-on the question generation task and provide an API to host the model prediction via [huggingface](https://huggingface.co/).
 Let's install `lmqg` via pip first.
 ```shell
 pip install lmqg
 ```
 
-### Generate Question & Answer
+## Generate Question & Answer
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
 
-- ***Generate Question on Answers:*** This is a basic usecase of our QG models, where user provides a paragraph and an answer to generate a question that is answerable by the answer given the paragraph.
-See [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#qg-models) for the available models.
+The main functionality of `lmqg` is to generate question and answer pairs on a given context with a handy api.
+The available models for each QAG class can be found at [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md#qag).
 
+- ***QAG with End2end or Multitask Models:*** The end2end QAG models are fine-tuned to generate a list of QA pairs with a single inference, 
+  so it is the fastest class among our QAG models. Meanwhile, multitask QAG models breakdown the QAG task into QG and AE, where they 
+  parse each sentence to get the answer with AE, and generate question on each answer with QG. Multitask QAG potentially generate more QA pairs than end2end QAG, but 
+  inference takes a few times more than end2end models. Both models can be used as following 
+  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg')
+model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
+    ("What did many of Turner's paintings depict?", 'the countryside around Oxford'),
+    ("What is one of Turner's best known pictures?", 'a view of the city of Oxford from Hinksey Hill')
+]
+```
+
+- ***QAG with Pipeline Models:*** The pipeline QAG is similar to multitask QAG, but the QG and AE models are independently fine-tuned, unlike 
+  multitask QAG that fine-tunes QG and AE jointly. Pipeline QAG can improve the performance in some cases, but it is as heavy as multitask QAG with 
+  more storage consuming due to the two models loaded. The pipeline QAG can be used as following. The `model` and `model_ae` are the QG and AE models respectively.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is another name for William Turner?', 'William Turner of Oxford'),
+    ("What did many of William Turner's paintings depict around Oxford?", 'the countryside'),
+    ('From what hill is a view of the city of Oxford taken?', 'Hinksey Hill.')
+]
+```
+
+- ***QG only:*** The QG model can be used as following. The `model` is the QG model. See the [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md), 
+a multilingual QG benchmark, for the list of available QG models.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg')
+
 # a list of paragraph
 context = [
     "William Turner was an English painter who specialised in watercolour landscapes",
     "William Turner was an English painter who specialised in watercolour landscapes"
 ]
 # a list of answer (same size as the context)
 answer = [
     "William Turner",
     "English"
 ]
 # model prediction
 question = model.generate_q(list_context=context, list_answer=answer)
-print(question)
+pprint(question)
 [
-    'Who was an English painter who specialised in watercolour landscapes?',
-    'What nationality was William Turner?'
+  'Who was an English painter who specialised in watercolour landscapes?',
+  'What nationality was William Turner?'
 ]
-```
+``` 
+
+- ***AE only:*** The QG model can be used as following. The `model` is the QG model.
 
-- ***Generate Question & Answer Pairs:*** Instead of specifying an answer, user can let QG model to generate an answer on the paragraph, and generate question on it sequentially.
-This functionality is only available for the QG models fine-tuned with answer extraction see [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#models-with-answer-extraction) for the full list of models with answer extraction (model alias usually has a suffix of `-qg-ae`).
-  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg-ae')
-# paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+model = TransformersQG(model='lmqg/t5-base-squad-ae')
 # model prediction
-question_answer = model.generate_qa(context)
-# the output is a list of tuple (question, answer)
-print(question_answer)
-[
-    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
-    ("What was William Turner's nickname?", 'William Turner of Oxford'),
-    ("What did many of Turner's paintings depict around Oxford?", 'countryside'),
-    ("What is one of William Turner's best known paintings?", 'a view of the city of Oxford')
-]
+answer = model.generate_a("William Turner was an English painter who specialised in watercolour landscapes")
+pprint(answer)
+['William Turner']
 ```
 
+## AutoQG
 
-### Model Evaluation
-The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
-From command line, run following command 
-```shell
-lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
-Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
-```shell
-lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
-([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
-Check `lmqg-eval -h` to display all the options.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
+</p>
+
+***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QAG models.
+
+## Model Development
+The `lmqg` also provides a command line interface to fine-tune and evaluate QG, AE, and QAG models.
 
 ### Model Training
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/grid_search.png" width="650">
 </p>
 
-To fine-tune QG model, we employ a two-stage hyper-parameter optimization, described as above diagram.
+To fine-tune QG (or AE, QAG) model, we employ a two-stage hyper-parameter optimization, described as above diagram.
 Following command is to run the fine-tuning with parameter optimization.
 ```shell
 lmqg-train-search -c "tmp_ckpt" -d "lmqg/qg_squad" -m "t5-small" -b 64 --epoch-partial 5 -e 15 --language "en" --n-max-config 1 \
   -g 2 4 --lr 1e-04 5e-04 1e-03 --label-smoothing 0 0.15
 ```
 Check `lmqg-train-search -h` to display all the options.
 
@@ -163,26 +188,33 @@
     lr=[1e-04, 5e-04, 1e-03],
     label_smoothing=[0, 0.15]
 )
 trainer.run()
 ```
 
 
-## AutoQG
-
-<p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
-</p>
+### Model Evaluation
+The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
+From command line, run following command 
+```shell
+lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
+Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
+```shell
+lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
+([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
+Check `lmqg-eval -h` to display all the options.
 
-***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QG models.
-The QG models are listed at the [QG-Bench page](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
 
 ## Rest API with huggingface inference API
 
-We provide a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
+Finally, `lmqg` provides a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
 ```shell
 pip install lmqg[api]
 ```
 Swagger UI is available at [`http://127.0.0.1:8088/docs`](http://127.0.0.1:8088/docs), when you run the app locally (replace the address by your server address).
 
 ### Build
 - Build/Run Local (command line):
@@ -215,14 +247,55 @@
   "qa": [
     {"question": "Who founded Nintendo Karuta?", "answer": "Fusajiro Yamauchi"},
     {"question": "When did Nintendo distribute its first video game console, the Color TV-Game?", "answer": "1977"}
   ]
 }
 ```
 
-## Misc
-Following link is useful if you need to reproduce the results in our paper.
-- [Model Fine-tuning/Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qg_model_training)
-- [QA based Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qa_based_evaluation)
-- [NQG model baseline](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/nqg_baseline)
+## Citation
+Please cite following paper if you use any resource and see the code to reproduce the model if needed.
 
+- [***Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 Main***](https://aclanthology.org/2022.emnlp-main.42/): The QG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2022_emnlp_qg)).
+```
+@inproceedings{ushio-etal-2022-generative,
+    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
+    month = dec,
+    year = "2022",
+    address = "Abu Dhabi, U.A.E.",
+    publisher = "Association for Computational Linguistics",
+}
+```
 
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+```
+@inproceedings{ushio-etal-2023-tba,
+    title = "TBA",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+
+```
+@inproceedings{ushio-etal-2023-a-practical-toolkit
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
```

### Comparing `lmqg-0.0.8/README.md` & `lmqg-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,197 @@
+Metadata-Version: 2.1
+Name: lmqg
+Version: 0.1.0
+Summary: Language Model for Question Generation.
+Home-page: https://github.com/asahi417/lm-question-generation
+Author: Asahi Ushio
+Author-email: asahi1992ushio@gmail.com
+License: MIT License
+Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.0.tar.gz
+Keywords: language model,question-answering,question-generation
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: api
+License-File: LICENSE
+
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/lmqg/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/lmqg.svg)](https://badge.fury.io/py/lmqg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 [![PyPI status](https://img.shields.io/pypi/status/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 
-# Generative Language Models for Paragraph-Level Question Generation
+# Question and Answer Generation with Language Models
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qg_diagram.png" width="500">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qag.png" width="400">
+  <br><em> Figure 1: Three distinct QAG approaches. </em>
 </p>
 
-This is the official repository of the paper
-["Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 main conference"](https://aclanthology.org/2022.emnlp-main.42/).
-This repository includes following contents:
-- ***QG-Bench***, the first ever multilingual/multidomain QG benchmark.
-- ***Multilingual/multidomain QG models*** fine-tuned on QG-Bench.
-- A python library ***`lmqg`*** developed for question generation in python as well as QG model fine-tuning/evaluation.
-- ***AutoQG***, a web application hosting QG models where user can test the model output interactively. 
-
-### Table of Contents  
-1. **[QG-Bench: multilingual & multidomain QG datasets (+ fine-tuned models)](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md)**
-2. **[LMQG: python library to fine-tune/evaluate QG model](#lmqg-language-model-for-question-generation-)**
-3. **[AutoQG: web application hosting multilingual QG models](#autoqg)**
-4. **[RestAPI: run model prediction via restAPI](#rest-api-with-huggingface-inference-api)**
+The `lmqg` is a python library for question and answer generation (QAG) with language models (LMs). Here, we consider 
+paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
+question and answer pairs on the context. With `lmqg`, you can do following things:
+- [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
+- [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
+- [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
+- [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
+ 
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
+
+### A bit more about QAG models 📝
+Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
+and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
+where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
+The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
+Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
+In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
+and the quality of the generated question and answer pairs depend on language.
+All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
+To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
-Please cite following paper if you use any resource:
-```
-@inproceedings{ushio-etal-2022-generative,
-    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
-    author = "Ushio, Asahi  and
-        Alva-Manchego, Fernando  and
-        Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
-    month = dec,
-    year = "2022",
-    address = "Abu Dhabi, U.A.E.",
-    publisher = "Association for Computational Linguistics",
-}
-```
+### Is QAG different from Question Generation (QG)? 🤔
 
-## LMQG: Language Model for Question Generation 🚀
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
+  <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
+</p>
+
+All the functionalities support question generation as well. Our QG model assumes user to specify an answer in addition to a context,
+and the QG model will generate a question that is answerable by the answer given the context (see Figure 2 for a comparison of QAG and QG).
+To know more about QG, please check [our EMNLP 2022 paper](https://aclanthology.org/2022.emnlp-main.42/) that describes the QG models more in detail.
+
+
+## Get Started 🚀
 
-The `lmqg` is a python library to fine-tune seq2seq language models ([T5](https://arxiv.org/pdf/1910.10683.pdf), [BART](https://arxiv.org/pdf/1910.13461.pdf)) 
-on the question generation task and provide an API to host the model prediction via [huggingface](https://huggingface.co/).
 Let's install `lmqg` via pip first.
 ```shell
 pip install lmqg
 ```
 
-### Generate Question & Answer
+## Generate Question & Answer
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
 
-- ***Generate Question on Answers:*** This is a basic usecase of our QG models, where user provides a paragraph and an answer to generate a question that is answerable by the answer given the paragraph.
-See [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#qg-models) for the available models.
+The main functionality of `lmqg` is to generate question and answer pairs on a given context with a handy api.
+The available models for each QAG class can be found at [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md#qag).
 
+- ***QAG with End2end or Multitask Models:*** The end2end QAG models are fine-tuned to generate a list of QA pairs with a single inference, 
+  so it is the fastest class among our QAG models. Meanwhile, multitask QAG models breakdown the QAG task into QG and AE, where they 
+  parse each sentence to get the answer with AE, and generate question on each answer with QG. Multitask QAG potentially generate more QA pairs than end2end QAG, but 
+  inference takes a few times more than end2end models. Both models can be used as following 
+  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg')
+model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
+    ("What did many of Turner's paintings depict?", 'the countryside around Oxford'),
+    ("What is one of Turner's best known pictures?", 'a view of the city of Oxford from Hinksey Hill')
+]
+```
+
+- ***QAG with Pipeline Models:*** The pipeline QAG is similar to multitask QAG, but the QG and AE models are independently fine-tuned, unlike 
+  multitask QAG that fine-tunes QG and AE jointly. Pipeline QAG can improve the performance in some cases, but it is as heavy as multitask QAG with 
+  more storage consuming due to the two models loaded. The pipeline QAG can be used as following. The `model` and `model_ae` are the QG and AE models respectively.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is another name for William Turner?', 'William Turner of Oxford'),
+    ("What did many of William Turner's paintings depict around Oxford?", 'the countryside'),
+    ('From what hill is a view of the city of Oxford taken?', 'Hinksey Hill.')
+]
+```
+
+- ***QG only:*** The QG model can be used as following. The `model` is the QG model. See the [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md), 
+a multilingual QG benchmark, for the list of available QG models.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg')
+
 # a list of paragraph
 context = [
     "William Turner was an English painter who specialised in watercolour landscapes",
     "William Turner was an English painter who specialised in watercolour landscapes"
 ]
 # a list of answer (same size as the context)
 answer = [
     "William Turner",
     "English"
 ]
 # model prediction
 question = model.generate_q(list_context=context, list_answer=answer)
-print(question)
+pprint(question)
 [
-    'Who was an English painter who specialised in watercolour landscapes?',
-    'What nationality was William Turner?'
+  'Who was an English painter who specialised in watercolour landscapes?',
+  'What nationality was William Turner?'
 ]
-```
+``` 
+
+- ***AE only:*** The QG model can be used as following. The `model` is the QG model.
 
-- ***Generate Question & Answer Pairs:*** Instead of specifying an answer, user can let QG model to generate an answer on the paragraph, and generate question on it sequentially.
-This functionality is only available for the QG models fine-tuned with answer extraction see [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#models-with-answer-extraction) for the full list of models with answer extraction (model alias usually has a suffix of `-qg-ae`).
-  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg-ae')
-# paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+model = TransformersQG(model='lmqg/t5-base-squad-ae')
 # model prediction
-question_answer = model.generate_qa(context)
-# the output is a list of tuple (question, answer)
-print(question_answer)
-[
-    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
-    ("What was William Turner's nickname?", 'William Turner of Oxford'),
-    ("What did many of Turner's paintings depict around Oxford?", 'countryside'),
-    ("What is one of William Turner's best known paintings?", 'a view of the city of Oxford')
-]
+answer = model.generate_a("William Turner was an English painter who specialised in watercolour landscapes")
+pprint(answer)
+['William Turner']
 ```
 
+## AutoQG
 
-### Model Evaluation
-The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
-From command line, run following command 
-```shell
-lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
-Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
-```shell
-lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
-([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
-Check `lmqg-eval -h` to display all the options.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
+</p>
+
+***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QAG models.
+
+## Model Development
+The `lmqg` also provides a command line interface to fine-tune and evaluate QG, AE, and QAG models.
 
 ### Model Training
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/grid_search.png" width="650">
 </p>
 
-To fine-tune QG model, we employ a two-stage hyper-parameter optimization, described as above diagram.
+To fine-tune QG (or AE, QAG) model, we employ a two-stage hyper-parameter optimization, described as above diagram.
 Following command is to run the fine-tuning with parameter optimization.
 ```shell
 lmqg-train-search -c "tmp_ckpt" -d "lmqg/qg_squad" -m "t5-small" -b 64 --epoch-partial 5 -e 15 --language "en" --n-max-config 1 \
   -g 2 4 --lr 1e-04 5e-04 1e-03 --label-smoothing 0 0.15
 ```
 Check `lmqg-train-search -h` to display all the options.
 
@@ -141,26 +210,33 @@
     lr=[1e-04, 5e-04, 1e-03],
     label_smoothing=[0, 0.15]
 )
 trainer.run()
 ```
 
 
-## AutoQG
-
-<p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
-</p>
+### Model Evaluation
+The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
+From command line, run following command 
+```shell
+lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
+Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
+```shell
+lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
+([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
+Check `lmqg-eval -h` to display all the options.
 
-***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QG models.
-The QG models are listed at the [QG-Bench page](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
 
 ## Rest API with huggingface inference API
 
-We provide a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
+Finally, `lmqg` provides a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
 ```shell
 pip install lmqg[api]
 ```
 Swagger UI is available at [`http://127.0.0.1:8088/docs`](http://127.0.0.1:8088/docs), when you run the app locally (replace the address by your server address).
 
 ### Build
 - Build/Run Local (command line):
@@ -193,12 +269,57 @@
   "qa": [
     {"question": "Who founded Nintendo Karuta?", "answer": "Fusajiro Yamauchi"},
     {"question": "When did Nintendo distribute its first video game console, the Color TV-Game?", "answer": "1977"}
   ]
 }
 ```
 
-## Misc
-Following link is useful if you need to reproduce the results in our paper.
-- [Model Fine-tuning/Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qg_model_training)
-- [QA based Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qa_based_evaluation)
-- [NQG model baseline](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/nqg_baseline)
+## Citation
+Please cite following paper if you use any resource and see the code to reproduce the model if needed.
+
+- [***Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 Main***](https://aclanthology.org/2022.emnlp-main.42/): The QG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2022_emnlp_qg)).
+```
+@inproceedings{ushio-etal-2022-generative,
+    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
+    month = dec,
+    year = "2022",
+    address = "Abu Dhabi, U.A.E.",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+```
+@inproceedings{ushio-etal-2023-tba,
+    title = "TBA",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+
+```
+@inproceedings{ushio-etal-2023-a-practical-toolkit
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+
```

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation.py` & `lmqg-0.1.0/lmqg/automatic_evaluation.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,17 @@
              output_type: str = 'question',
              prediction_aggregation: str = 'first',
              prediction_level: str = None,
              data_caches: Dict = None,
              bleu_only: bool = False,
              overwrite: bool = False,
              use_auth_token: bool = False,
+             torch_dtype=None,
+             device_map: str = None,
+             low_cpu_mem_usage: bool = False,
              language: str = 'en',
              test_split: str = 'test',
              validation_split: str = 'validation'):
     """ Evaluate question-generation model """
     reference_files = get_reference_files(dataset_path, dataset_name)
     if prediction_level is None:
         valid_prediction_level = [k.split('-')[0] for k in reference_files.keys()]
@@ -199,15 +202,19 @@
 
     if model is not None:
         lm = TransformersQG(model,
                             max_length=max_length,
                             max_length_output=max_length_output,
                             drop_overflow_error_text=False,
                             skip_overflow_error=True,
-                            language=language)
+                            language=language,
+                            use_auth_token=use_auth_token,
+                            torch_dtype=torch_dtype,
+                            device_map=device_map,
+                            low_cpu_mem_usage=low_cpu_mem_usage)
         lm.eval()
 
         def get_model_prediction_file(split, _input_type, _output_type):
             path = pj(
                 export_dir,
                 f'samples.{split}.hyp.{_input_type}.{_output_type}.{dataset_path.replace("/", "_")}.{dataset_name}.txt')
             raw_input, _ = get_dataset(
```

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/score.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/score.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/scorer.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/scorer.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bert_score/utils.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bert_score/utils.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bertscore.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bertscore.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/bleu.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/bleu/bleu_scorer.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/meteor/meteor.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/meteor/meteor.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/moverscore.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/moverscore.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/rouge.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/rouge.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/automatic_evaluation_tool/text_normalization.py` & `lmqg-0.1.0/lmqg/automatic_evaluation_tool/text_normalization.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/data.py` & `lmqg-0.1.0/lmqg/data.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/exceptions.py` & `lmqg-0.1.0/lmqg/exceptions.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/grid_searcher.py` & `lmqg-0.1.0/lmqg/grid_searcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,25 @@
             tmp = ''.join(random.choice(string.ascii_lowercase) for _ in range(length))
     return tmp
 
 
 class GridSearcher:
     """ Grid search (epoch, batch, lr, random_seed, label_smoothing) """
 
-    def __init__(self, checkpoint_dir: str, dataset_path: str = "asahi417/qg_squad", dataset_name: str = "default",
+    def __init__(self, checkpoint_dir: str, dataset_path: str = "lmqg/qg_squad", dataset_name: str = "default",
                  input_types: List or str = 'paragraph_answer', output_types: List or str = 'question',
                  prefix_types: List or str = 'qg', model: str = 't5-small', fp16: bool = False,
                  gradient_accumulation_steps: List or int = 4, metric: str = 'validation/Bleu_4',
                  epoch: int = 10, epoch_partial: int = 2, n_max_config: int = 5, max_length: int = 512,
                  max_length_eval: int = None, max_length_output: int = 32, max_length_output_eval: int = None,
                  prediction_aggregation: str = 'first', prediction_level: str = 'sentence',
                  batch: int = 128, batch_eval: int = 32, n_beams_eval: int = 4, lr: List or float = 1e-4,
                  label_smoothing: List or float = None, random_seed: List or int = 42, language: str = 'en',
-                 normalize: bool = True, use_auth_token: bool = False):
+                 normalize: bool = True, use_auth_token: bool = False, torch_dtype=None, device_map: str = None,
+                 low_cpu_mem_usage: bool = False):
 
         # evaluation configs
         max_length_eval = max_length if max_length_eval is None else max_length_eval
         max_length_output_eval = max_length_output if max_length_output_eval is None else max_length_output_eval
         self.eval_config = {
             'max_length_eval': max_length_eval, 'max_length_output_eval': max_length_output_eval,
             'n_beams_eval': n_beams_eval, 'prediction_aggregation': prediction_aggregation,
@@ -58,14 +59,18 @@
         # dynamic config
         self.epoch = epoch
         self.epoch_partial = epoch_partial
         self.batch_eval = batch_eval
         self.checkpoint_dir = checkpoint_dir
         self.n_max_config = n_max_config
         self.use_auth_token = use_auth_token
+        self.torch_dtype = torch_dtype
+        self.device_map = device_map
+        self.low_cpu_mem_usage = low_cpu_mem_usage
+
         self.split, self.metric = metric.split('/')
 
         self.dynamic_config = {
             'lr': to_list(lr),
             'label_smoothing': to_list(label_smoothing),
             'random_seed': to_list(random_seed),
             'gradient_accumulation_steps': to_list(gradient_accumulation_steps),
@@ -200,15 +205,17 @@
                 model_ckpt = get_random_string(exclude=ckpt_name_exist + ckpt_name_made)
                 checkpoint_dir = pj(self.checkpoint_dir, f'model_{model_ckpt}')
             else:
                 raise ValueError(f'duplicated checkpoints are found: \n {duplicated_ckpt}')
 
             if not os.path.exists(pj(checkpoint_dir, f'epoch_{self.epoch_partial}')):
                 trainer = Trainer(
-                    checkpoint_dir=checkpoint_dir, disable_log=True, use_auth_token=self.use_auth_token, **config)
+                    checkpoint_dir=checkpoint_dir, disable_log=True, use_auth_token=self.use_auth_token,
+                    device_map=self.device_map, low_cpu_mem_usage=self.low_cpu_mem_usage, torch_dtype=self.torch_dtype,
+                    **config)
                 trainer.train(
                     epoch_partial=self.epoch_partial, epoch_save=1, interval=interval)
 
             checkpoints.append(checkpoint_dir)
 
         metrics = {}
         for n, checkpoint_dir in enumerate(checkpoints):
@@ -238,15 +245,17 @@
         ###########
         metrics = metrics[:min(len(metrics), self.n_max_config)]
         checkpoints = []
         for n, (checkpoint_dir_model, _metric) in enumerate(metrics):
             logging.info(f'## 2nd RUN: Configuration {n}/{len(metrics)}: {self.split}/{self.metric} = {_metric}')
             model_ckpt = os.path.dirname(checkpoint_dir_model)
             if not os.path.exists(pj(model_ckpt, f'epoch_{self.epoch}')):
-                trainer = Trainer(checkpoint_dir=model_ckpt, disable_log=True, use_auth_token=self.use_auth_token)
+                trainer = Trainer(
+                    checkpoint_dir=model_ckpt, disable_log=True, use_auth_token=self.use_auth_token,
+                    device_map=self.device_map, low_cpu_mem_usage=self.low_cpu_mem_usage, torch_dtype=self.torch_dtype)
                 trainer.train(epoch_save=1, interval=interval)
 
             checkpoints.append(model_ckpt)
 
         metrics = {}
         for n, checkpoint_dir in enumerate(checkpoints):
             logging.info(f'## 2nd RUN (EVAL): Configuration {n}/{len(checkpoints)} ##')
@@ -281,15 +290,16 @@
                 config['epoch'] = epoch
                 with open(pj(best_model_dir, 'trainer_config.additional_training.json'), 'w') as f:
                     json.dump(config, f)
                 checkpoint_dir_model = pj(best_model_dir, f'epoch_{epoch}')
                 if not os.path.exists(checkpoint_dir_model):
                     trainer = Trainer(
                         checkpoint_dir=best_model_dir, config_file='trainer_config.additional_training.json',
-                        disable_log=True, use_auth_token=self.use_auth_token)
+                        disable_log=True, use_auth_token=self.use_auth_token, device_map=self.device_map,
+                        low_cpu_mem_usage=self.low_cpu_mem_usage, torch_dtype=self.torch_dtype)
                     trainer.train(epoch_save=1, interval=interval)
                 logging.info(f'## 3rd RUN (EVAL): epoch {epoch} ##')
                 metric = evaluator(checkpoint_dir_model)
                 tmp_metric_score = metric[self.split][self.metric]
                 metric_list.append([epoch, tmp_metric_score])
                 logging.info(f'\t tmp metric: {tmp_metric_score}')
                 if best_metric_score > tmp_metric_score:
```

### Comparing `lmqg-0.0.8/lmqg/inference_api.py` & `lmqg-0.1.0/lmqg/inference_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,81 +56,107 @@
         top_p: float = 0.9,
         use_gpu: bool = False,
         is_qag: bool = None,
         add_prefix_qg: bool = None,
         add_prefix_answer: bool = None,
         splitting_symbol: str = '|',
         question_prefix: str = "question: ",
-        answer_prefix: str = ", answer: "):
+        answer_prefix: str = ", answer: ",
+        split_level: str = "paragraph"):
 
     logging.info('initialize TransformersQGInferenceAPI')
     is_qag = model_qg.endswith('qag') if is_qag is None else is_qag
     add_prefix_qg = transformers.AutoConfig.from_pretrained(model_qg).add_prefix if add_prefix_qg is None else add_prefix_qg
+
+    qa = []
+    qa_hash = []
     if is_qag:
         assert input_answer is None
-        input_text = f"{TASK_PREFIX['qag'] if add_prefix_qg else None}: {input_text}"
-        input_text = f"{TASK_PREFIX['qag']}: {input_text}" if add_prefix_qg else input_text
-        output = call_api(
-            input_text=input_text,
-            api_token=api_token,
-            model=model_qg,
-            max_length=max_length,
-            do_sample=do_sample,
-            num_beams=num_beams,
-            use_gpu=use_gpu,
-            top_p=top_p)
-
-        qa = []
-        for raw_string in output[0]['generated_text'].split(splitting_symbol):
-            if len(raw_string.split(answer_prefix)) != 2 or question_prefix not in raw_string:
-                logging.info(f"invalid prediction: {raw_string}")
-            else:
-                q, a = raw_string.split(answer_prefix)
-                a = re.sub(r'\A\s+', '', a)
-                a = re.sub(r'\s+\Z', '', a)
-                q = q.replace(question_prefix, "")
-                q = re.sub(r'\A\s+', '', q)
-                q = re.sub(r'\s+\Z', '', q)
-                qa.append({'question': q, 'answer': a})
+        if split_level is None or split_level == "paragraph":
+            input_text = [input_text]
+        elif split_level == "sentence":
+            input_text = spacy.sentence(input_text)
+        else:
+            raise ValueError(f"split_level must be one of ['paragraph', 'sentence'], got {split_level}")
+        for x in input_text:
+            x = f"{TASK_PREFIX['qag'] if add_prefix_qg else None}: {x}"
+            x = f"{TASK_PREFIX['qag']}: {x}" if add_prefix_qg else x
+            output = call_api(
+                input_text=x, api_token=api_token, model=model_qg, max_length=max_length, do_sample=do_sample,
+                num_beams=num_beams, use_gpu=use_gpu, top_p=top_p)
+
+            for raw_string in output[0]['generated_text'].split(splitting_symbol):
+                if len(raw_string.split(answer_prefix)) != 2 or question_prefix not in raw_string:
+                    logging.info(f"invalid prediction: {raw_string}")
+                else:
+                    if raw_string.replace(" ", "").lower() in qa_hash:
+                        continue
+                    qa_hash.append(raw_string.replace(" ", "").lower())
+                    q, a = raw_string.split(answer_prefix)
+                    a = re.sub(r'\A\s+', '', a)
+                    a = re.sub(r'\s+\Z', '', a)
+                    q = q.replace(question_prefix, "")
+                    q = re.sub(r'\A\s+', '', q)
+                    q = re.sub(r'\s+\Z', '', q)
+                    qa.append({'question': q, 'answer': a})
     else:
-
         if input_answer is None or len(input_answer) == 0:
+
             assert spacy is not None
             logging.info(f"answer extraction: {spacy.algorithm if model_ae is None else model_ae}")
             if model_ae is None:  # keyword extraction
                 input_answer = spacy.keyword(input_text)
             else:
                 add_prefix_ae = transformers.AutoConfig.from_pretrained(model_ae).add_prefix if add_prefix_answer is None else add_prefix_answer
-                batch = [highlight_sentence(input_text, i, TASK_PREFIX['ae'] if add_prefix_ae else None) for i in spacy.sentence(input_text)]
+                if split_level is None or split_level == "paragraph":
+                    batch = [highlight_sentence(input_text, i, TASK_PREFIX['ae'] if add_prefix_ae else None) for i in spacy.sentence(input_text)]
+                elif split_level == "sentence":
+                    batch = [highlight_sentence(i, i, TASK_PREFIX['ae'] if add_prefix_ae else None) for i in spacy.sentence(input_text)]
+                else:
+                    raise ValueError(f"split_level must be one of ['paragraph', 'sentence'], got {split_level}")
+
                 output = call_api(
                     input_text=batch,
                     api_token=api_token,
                     model=model_ae,
                     max_length=max_length,
                     do_sample=do_sample,
                     num_beams=num_beams,
                     use_gpu=use_gpu,
                     top_p=top_p)
                 input_answer = list(filter(None, [clean(i['generated_text']) for i in output]))  # remove None
-                input_answer = list(filter(lambda x: x in input_text, input_answer))  # remove answers not in input_text
+                input_answer = list(filter(lambda _x: _x in input_text, input_answer))  # remove answers not in input_text
                 if len(input_answer) == 0:
                     raise AnswerNotFoundError(input_text)
 
         logging.info("generate question")
         input_answer = [input_answer] if type(input_answer) is str else input_answer
-        batch = [highlight_sentence(input_text, i, TASK_PREFIX['qg'] if add_prefix_qg else None) for i in input_answer]
+        batch = [highlight_sentence(input_text, i, None) for i in input_answer]
+        if split_level is not None and split_level == "sentence":
+            batch = [[_i for _i in spacy.sentence(i) if _i.count(ADDITIONAL_SP_TOKENS['hl']) == 2] for i in batch]
+            batch = [i[0] for i in batch if len(i) > 0]
+            if len(batch) == 0:
+                raise AnswerNotFoundError(input_text)
+        if add_prefix_qg:
+            batch = [f"{TASK_PREFIX['qg']}: {i}" for i in batch]
         output = call_api(
             input_text=batch,
             api_token=api_token,
             model=model_qg,
             max_length=max_length,
             do_sample=do_sample,
             num_beams=num_beams,
             top_p=top_p,
             use_gpu=use_gpu)
-        question = [i['generated_text'] for i in output]
-        assert len(question) == len(input_answer), f"{question} != {input_answer}"
-        qa = [{'question': q, 'answer': a} for q, a in zip(question, input_answer)]
+        for i, a in zip(output, input_answer):
+
+            q = i['generated_text']
+            raw_string = f"{q}, {a}".replace(" ", "").lower()
+            if raw_string in qa_hash:
+                continue
+            qa_hash.append(raw_string)
+            qa.append({'question': q, 'answer': a})
+
         logging.info(f"complete process: {len(output)} qa pairs generated")
     return qa
```

### Comparing `lmqg-0.0.8/lmqg/language_model.py` & `lmqg-0.1.0/lmqg/language_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,20 @@
     try:
         urllib.request.urlopen(host)
         return True
     except:
         return False
 
 
-def load_language_model(model_name, cache_dir: str = None, use_auth_token: bool = False):
+def load_language_model(model_name,
+                        cache_dir: str = None,
+                        use_auth_token: bool = False,
+                        torch_dtype=None,
+                        device_map: str = None,
+                        low_cpu_mem_usage: bool = False):
     """ load language model from huggingface model hub """
     # tokenizer
     local_files_only = not internet_connection()
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         model_name, cache_dir=cache_dir, local_files_only=local_files_only, use_auth_token=use_auth_token)
     config = transformers.AutoConfig.from_pretrained(
         model_name, local_files_only=local_files_only, cache_dir=cache_dir, use_auth_token=use_auth_token)
@@ -85,16 +90,22 @@
         model_class = transformers.BartForConditionalGeneration.from_pretrained
     elif config.model_type == 'mbart':
         model_class = transformers.MBartForConditionalGeneration.from_pretrained
     elif config.model_type == 'switch_transformers':
         model_class = transformers.SwitchTransformersForConditionalGeneration.from_pretrained
     else:
         raise ValueError(f'unsupported model type: {config.model_type}')
-    model = model_class(
-        model_name, config=config, cache_dir=cache_dir, local_files_only=local_files_only, use_auth_token=use_auth_token)
+
+    param = {'config': config, "local_files_only": local_files_only, "use_auth_token": use_auth_token,
+             "low_cpu_mem_usage": low_cpu_mem_usage, "cache_dir": cache_dir}
+    if torch_dtype is not None:
+        param['torch_dtype'] = torch_dtype
+    if device_map is not None:
+        param['device_map'] = device_map
+    model = model_class(model_name, **param)
     # add new special tokens to the tokenizer and the model if they don't have it
     tokenizer.add_special_tokens({'additional_special_tokens': list(ADDITIONAL_SP_TOKENS.values())})
     model.resize_token_embeddings(len(tokenizer))
     return tokenizer, model, config
 
 
 def label_smoothed_loss(logits, labels, epsilon):
@@ -215,15 +226,18 @@
                     raise ExceedMaxLengthError(self.max_length)
                 return None  # remove overflow text
             if output_sequence is not None:
                 if len(self.tokenizer.encode(output_sequence)) > self.max_length_output:
                     if not self.drop_overflow_error_text:  # raise error for overflow text
                         raise ExceedMaxLengthError(self.max_length)
                     return None  # remove overflow text
-        encode = self.tokenizer.encode_plus(input_sequence, **self.param_in)
+        if type(self.tokenizer) is transformers.models.mbart.tokenization_mbart_fast.MBartTokenizerFast:
+            encode = self.tokenizer(input_sequence, **self.param_in)
+        else:
+            encode = self.tokenizer(text_target=input_sequence, **self.param_in)
         if output_sequence is not None:
             encode['labels'] = self.tokenizer.encode(output_sequence, **self.param_out)
         return encode
 
 
 class TransformersQG:
     """ Transformers Language Model for Question Generation. """
@@ -240,14 +254,17 @@
                  language: str = 'en',
                  label_smoothing: float = None,
                  skip_overflow_error: bool = False,
                  drop_overflow_error_text: bool = False,
                  drop_highlight_error_text: bool = False,
                  drop_answer_error_text: bool = False,
                  use_auth_token: bool = False,
+                 torch_dtype=None,
+                 device_map: str = None,
+                 low_cpu_mem_usage: bool = False,
                  is_qg: bool = None,
                  is_qag: bool = None,
                  is_qa: bool = None,
                  is_ae: bool = None):
         """ Transformers Language Model for Question Generation.
 
         @param model: Model alias or path to local model file.
@@ -285,15 +302,17 @@
         self.skip_overflow_error = skip_overflow_error
         self.drop_highlight_error_text = drop_highlight_error_text
         self.drop_answer_error_text = drop_answer_error_text
         self.model_name_ae = model_ae
         self.max_length_ae = max_length_ae
         self.max_length_output_ae = max_length_output_ae
         # load model
-        self.tokenizer, self.model, config = load_language_model(self.model_name, cache_dir=cache_dir, use_auth_token=use_auth_token)
+        self.tokenizer, self.model, config = load_language_model(
+            self.model_name, cache_dir=cache_dir, use_auth_token=use_auth_token, device_map=device_map,
+            torch_dtype=torch_dtype, low_cpu_mem_usage=low_cpu_mem_usage)
         if 'add_prefix' not in config.to_dict().keys():
             # this means the model is not fine-tuned
             # assert add_prefix, '`add_prefix` is required for non-fine-tuned models'
             self.add_prefix = add_prefix
         else:
             self.add_prefix = config.add_prefix
 
@@ -333,14 +352,21 @@
         if self.model_ae is not None:
             self.model_ae.to(self.device)
         logging.info(f'Model `{self.model_name}`')
         logging.info(f'\t * Num of GPU in use: {torch.cuda.device_count()}')
         logging.info(f'\t * Prefix: {self.add_prefix}')
         logging.info(f'\t * Language: {language} (ignore at the training phase)')
 
+    def push_to_hub(self, repo_id):
+        if self.parallel:
+            self.model.module.push_to_hub(repo_id)
+        else:
+            self.model.push_to_hub(repo_id)
+        self.tokenizer.push_to_hub(repo_id)
+
     def generate_qa_end2end(self,
                             list_context: str or List,
                             batch_size: int = None,
                             num_beams: int = 4,
                             cache_path: str = None,
                             splitting_symbol: str = '|',
                             question_prefix: str = "question: ",
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation.py` & `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     parser.add_argument('-o', '--output-type', help='', default='question', type=str)
     parser.add_argument('-l', '--language', help='', default='en', type=str)
     parser.add_argument('--test-split', help='the name of test split', default='test', type=str)
     parser.add_argument('--validation-split', help='the name of validation split', default='validation', type=str)
     parser.add_argument('--overwrite', help='', action='store_true')
     parser.add_argument('--bleu-only', help='', action='store_true')
     parser.add_argument('--use-auth-token', help='', action='store_true')
+    parser.add_argument('--device-map', help='', default=None, type=str)
+    parser.add_argument('--low-cpu-mem-usage', help='', action='store_true')
     parser.add_argument('--prediction-aggregation', default=None, type=str)
     parser.add_argument('--prediction-level', default=None, type=str)
-
     return parser.parse_args()
 
 
 def main():
     opt = get_options()
     prediction_aggregation = 'first' if opt.prediction_aggregation is None else opt.prediction_aggregation
     prediction_level = 'sentence'  # qg
@@ -61,10 +62,12 @@
         output_type=opt.output_type,
         prediction_aggregation=prediction_aggregation,
         prediction_level=prediction_level,
         overwrite=opt.overwrite,
         language=opt.language,
         bleu_only=opt.bleu_only,
         use_auth_token=opt.use_auth_token,
+        device_map=opt.device_map,
+        low_cpu_mem_usage=opt.low_cpu_mem_usage
     )
     print(json.dumps(metric, indent=4, sort_keys=True))
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qa.py` & `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     parser.add_argument('--dataset-name', help='huggingface datasets name', default='default', type=str)
     parser.add_argument('--test-split', help='the name of test split', default='test', type=str)
     parser.add_argument('--validation-split', help='the name of validation split', default='validation', type=str)
     parser.add_argument('--n-beams', default=4, type=int)
     parser.add_argument('--batch-size', default=16, type=int)
     parser.add_argument('-l', '--language', help='', default='en', type=str)
     parser.add_argument('--use-auth-token', help='', action='store_true')
+    parser.add_argument('--device-map', help='', default=None, type=str)
+    parser.add_argument('--low-cpu-mem-usage', help='', action='store_true')
     parser.add_argument('-e', '--export-dir', required=True, type=str)
     parser.add_argument('--hyp-test', default=None, type=str)
     parser.add_argument('--hyp-dev', default=None, type=str)
     parser.add_argument('--overwrite-prediction', help='', action='store_true')
     parser.add_argument('--overwrite-metric', help='', action='store_true')
     parser.add_argument('-i', '--input-type', help='', default='paragraph_question', type=str)
     parser.add_argument('-o', '--output-type', help='', default='answer', type=str)
@@ -44,15 +46,17 @@
         if opt.model_checkpoint is not None:
             _model = TransformersQG(opt.model_checkpoint,
                                     skip_overflow_error=True,
                                     drop_answer_error_text=True,
                                     language=opt.language,
                                     max_length=opt.max_length,
                                     max_length_output=opt.max_length_output,
-                                    use_auth_token=opt.use_auth_token)
+                                    use_auth_token=opt.use_auth_token,
+                                    device_map=opt.device_map,
+                                    low_cpu_mem_usage=opt.low_cpu_mem_usage)
             _model.eval()
             return _model
         raise ValueError(f"require `-m` or `--model-checkpoint`")
 
     metric_file = f"{opt.export_dir}/metric.first.answer.{opt.input_type}.{opt.output_type}." \
                   f"{opt.dataset_path.replace('/', '_')}.{opt.dataset_name}.json"
     if os.path.exists(metric_file):
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py` & `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qa_based_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,26 @@
     parser.add_argument('-n', '--anchor-data-name', default='new_wiki', type=str)
     parser.add_argument('--use-reference-answer', action='store_true')
     parser.add_argument('--overwrite', action='store_true')
     parser.add_argument('-b', '--batch-size', default=256, type=int)
     parser.add_argument('-e', '--export-dir', default='tmp_output', type=str)
     parser.add_argument('--max-length', default=512, type=int, help='')
     parser.add_argument('--max-length-output', default=64, type=int, help='')
+    parser.add_argument('--use-auth-token', help='', action='store_true')
+    parser.add_argument('--device-map', help='', default=None, type=str)
+    parser.add_argument('--low-cpu-mem-usage', help='', action='store_true')
     opt = parser.parse_args()
     generate_qa_pairs(
         model_qg=opt.model_qg,
         model_ae=opt.model_ae,
         language=opt.language,
         anchor_data=opt.anchor_data,
         anchor_data_name=opt.anchor_data_name,
         use_reference_answer=opt.use_reference_answer,
         batch_size=opt.batch_size,
         export_dir=opt.export_dir,
         overwrite=opt.overwrite,
         max_length=opt.max_length,
-        max_length_output=opt.max_length)
+        max_length_output=opt.max_length,
+        use_auth_token=opt.use_auth_token,
+        device_map=opt.device_map,
+        low_cpu_mem_usage=opt.low_cpu_mem_usage)
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/model_evaluation_qag.py` & `lmqg-0.1.0/lmqg/lmqg_cl/model_evaluation_qag.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,25 @@
     parser.add_argument('--dataset-name', help='huggingface datasets name', default='default', type=str)
     parser.add_argument('--test-split', help='the name of test split', default='test', type=str)
     parser.add_argument('--validation-split', help='the name of validation split', default='validation', type=str)
     parser.add_argument('--n-beams', default=4, type=int)
     parser.add_argument('--batch-size', default=16, type=int)
     parser.add_argument('-l', '--language', help='', default='en', type=str)
     parser.add_argument('--use-auth-token', help='', action='store_true')
+    parser.add_argument('--device-map', help='', default=None, type=str)
+    parser.add_argument('--low-cpu-mem-usage', help='', action='store_true')
     parser.add_argument('-e', '--export-dir', required=True, type=str)
     parser.add_argument('--hyp-test', default=None, type=str)
     parser.add_argument('--hyp-dev', default=None, type=str)
     parser.add_argument('--overwrite-prediction', help='', action='store_true')
     parser.add_argument('--overwrite-metric', help='', action='store_true')
     parser.add_argument('--use-reference-answer', action='store_true')
+    parser.add_argument('--is-qa', help='', action='store_true')
+    parser.add_argument('--is-ae', help='', action='store_true')
+    parser.add_argument('--is-qag', help='', action='store_true')
     return parser.parse_args()
 
 
 def main():
     opt = get_options()
     os.makedirs(opt.export_dir, exist_ok=True)
     metrics = [
@@ -61,21 +66,26 @@
         (BERTScore(language=opt.language), "BERTScore"),
         (MoverScore(language=opt.language), 'MoverScore')
     ]
 
     def load_model():
         if opt.model is not None:
             _model = TransformersQG(opt.model,
+                                    is_ae=None if opt.is_ae else True,
+                                    is_qg=None if opt.is_qg else True,
+                                    is_qag=None if opt.is_qag else True,
                                     model_ae=opt.model_ae,
                                     skip_overflow_error=True,
                                     drop_answer_error_text=True,
                                     language=opt.language,
                                     max_length=opt.max_length,
                                     max_length_output=opt.max_length_output,
-                                    use_auth_token=opt.use_auth_token)
+                                    use_auth_token=opt.use_auth_token,
+                                    device_map=opt.device_map,
+                                    low_cpu_mem_usage=opt.low_cpu_mem_usage)
             _model.eval()
             return _model
         raise ValueError(f"require `-m` or `--model`")
 
     if opt.model_ae is not None:
         metric_file = f"{opt.export_dir}/metric.first.answer.paragraph.questions_answers." \
                       f"{opt.dataset_path.replace('/', '_')}.{opt.dataset_name}." \
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/model_finetuning.py` & `lmqg-0.1.0/lmqg/lmqg_cl/model_finetuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
                         help='prefix type (`qg`/`ae`) which should be specified for T5 but not for mT5, BART, or mBART',
                         nargs='+', default=None, type=str)
     parser.add_argument('-m', '--model', help='pretrained language model', default='facebook/bart-large', type=str)
     parser.add_argument('-e', '--epoch', help='epoch', default=8, type=int)
     parser.add_argument('-b', '--batch', help='batch size', default=128, type=int)
     parser.add_argument('--fp16', help='fp16', action='store_true')
     parser.add_argument('--use-auth-token', help='', action='store_true')
+    parser.add_argument('--device-map', help='', default=None, type=str)
+    parser.add_argument('--low-cpu-mem-usage', help='', action='store_true')
     parser.add_argument('--max-length', default=512, type=int, help='max sequence length for input sequence')
     parser.add_argument('--max-length-output', default=32, type=int, help='max sequence length for output sequence')
     parser.add_argument('--interval', default=50, type=int)
     return parser
 
 
 def arguments_training(parser):
@@ -85,15 +87,17 @@
         lr=opt.lr,
         batch=opt.batch,
         max_length=opt.max_length,
         max_length_output=opt.max_length_output,
         fp16=opt.fp16,
         gradient_accumulation_steps=opt.gradient_accumulation_steps,
         label_smoothing=opt.label_smoothing,
-        use_auth_token=opt.use_auth_token)
+        use_auth_token=opt.use_auth_token,
+        device_map=opt.device_map,
+        low_cpu_mem_usage=opt.low_cpu_mem_usage)
     trainer.train(interval=opt.interval, epoch_save=opt.epoch_save)
 
 
 def main_training_search():
     parser = argparse.ArgumentParser(description='Fine-tuning on QG with Grid Search.')
     parser = arguments(parser)
     parser = arguments_training_search(parser)
@@ -124,11 +128,12 @@
         batch_eval=opt.batch_eval,
         n_beams_eval=opt.n_beams_eval,
         prediction_aggregation=opt.prediction_aggregation,
         prediction_level=opt.prediction_level,
         max_length_output_eval=opt.max_length_output_eval,
         max_length_eval=opt.max_length_eval,
         language=opt.language,
-        use_auth_token=opt.use_auth_token
-    )
+        use_auth_token=opt.use_auth_token,
+        device_map=opt.device_map,
+        low_cpu_mem_usage=opt.low_cpu_mem_usage)
     trainer.run(interval=opt.interval, overwrite=opt.overwrite)
```

### Comparing `lmqg-0.0.8/lmqg/lmqg_cl/readme_template.py` & `lmqg-0.1.0/lmqg/lmqg_cl/readme_template.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py` & `lmqg-0.1.0/lmqg/qa_evaluation_tool/generate_pseudo_qa_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,30 +14,38 @@
         anchor_data: str = 'lmqg/qa_squadshifts',
         anchor_data_name: str = 'new_wiki',
         use_reference_answer: bool = False,
         batch_size: int = 256,
         export_dir: str = None,
         overwrite: bool = False,
         max_length: int = 512,
-        max_length_output: int = 256):
+        max_length_output: int = 256,
+        use_auth_token: bool = False,
+        torch_dtype=None,
+        device_map: str = None,
+        low_cpu_mem_usage: bool = False):
 
     logging.info(f'generate QA pairs from {anchor_data} with {model_qg}')
     data = load_dataset(anchor_data) if anchor_data_name is None else load_dataset(anchor_data, anchor_data_name)
 
     if export_dir is not None:
         os.makedirs(export_dir, exist_ok=True)
 
     model = TransformersQG(
         model=model_qg,
         model_ae=model_ae,
         language=language,
         skip_overflow_error=True,
         drop_answer_error_text=True,
         max_length=max_length,
-        max_length_output=max_length_output)
+        max_length_output=max_length_output,
+        use_auth_token=use_auth_token,
+        torch_dtype=torch_dtype,
+        device_map=device_map,
+        low_cpu_mem_usage=low_cpu_mem_usage)
 
     logging.info(f"Export dir: {export_dir}")
     full_output = {}
     for _split in data:
 
         logging.info(f'running prediction on {_split}')
         if export_dir is not None:
```

### Comparing `lmqg-0.0.8/lmqg/qa_evaluation_tool/run_qa.py` & `lmqg-0.1.0/lmqg/qa_evaluation_tool/run_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/qa_evaluation_tool/trainer_qa.py` & `lmqg-0.1.0/lmqg/qa_evaluation_tool/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/qa_evaluation_tool/utils_qa.py` & `lmqg-0.1.0/lmqg/qa_evaluation_tool/utils_qa.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/spacy_module.py` & `lmqg-0.1.0/lmqg/spacy_module.py`

 * *Files identical despite different names*

### Comparing `lmqg-0.0.8/lmqg/trainer.py` & `lmqg-0.1.0/lmqg/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,17 +78,23 @@
                  lr: float = 1e-4,
                  fp16: bool = False,
                  random_seed: int = 42,
                  gradient_accumulation_steps: int = 4,
                  label_smoothing: float = None,
                  disable_log: bool = False,
                  config_file: str = 'trainer_config.json',
-                 use_auth_token: bool = False):
+                 use_auth_token: bool = False,
+                 torch_dtype=None,
+                 device_map: str = None,
+                 low_cpu_mem_usage: bool = False):
         logging.info('initialize model trainer')
         self.use_auth_token = use_auth_token
+        self.torch_dtype = torch_dtype
+        self.device_map = device_map
+        self.low_cpu_mem_usage = low_cpu_mem_usage
         # config
         self.config = Config(
             config_file=config_file, checkpoint_dir=checkpoint_dir, dataset_path=dataset_path, dataset_name=dataset_name,
             input_types=input_types, output_types=output_types, prefix_types=prefix_types, model=model,
             max_length=max_length, max_length_output=max_length_output, epoch=epoch, batch=batch, lr=lr, fp16=fp16,
             random_seed=random_seed, gradient_accumulation_steps=gradient_accumulation_steps,
             label_smoothing=label_smoothing)
@@ -114,30 +120,31 @@
             for epoch in epochs:
                 try:
                     path = pj(self.config.checkpoint_dir, f"epoch_{epoch}")
                     logging.info(f'load checkpoint from {path}')
                     self.model = TransformersQG(
                         model=path, max_length=self.config.max_length, max_length_output=self.config.max_length_output,
                         label_smoothing=self.config.label_smoothing, add_prefix=add_prefix,
-                        drop_overflow_error_text=True
-                    )
+                        drop_overflow_error_text=True, use_auth_token=self.use_auth_token, device_map=self.device_map,
+                        low_cpu_mem_usage=self.low_cpu_mem_usage, torch_dtype=self.torch_dtype)
                     self.optimizer = self.setup_optimizer(epoch)
                     self.current_epoch = epoch
                     assert self.current_epoch <= self.config.epoch, 'model training is done'
                     flag = True
                 except Exception:
                     logging.exception(f'error at loading checkpoint {ckpts}')
                 if flag:
                     break
         if not flag:
             logging.info(f'initialize checkpoint with {self.config.model}')
             self.model = TransformersQG(
                 model=self.config.model, max_length=self.config.max_length,
                 max_length_output=self.config.max_length_output, add_prefix=add_prefix,
-                drop_overflow_error_text=True)
+                drop_overflow_error_text=True, use_auth_token=self.use_auth_token,
+                device_map=self.device_map, low_cpu_mem_usage=self.low_cpu_mem_usage, torch_dtype=self.torch_dtype)
             self.optimizer = self.setup_optimizer()
             self.current_epoch = 0
 
         # GPU mixture precision
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.config.fp16)
 
         # cached data folder
```

### Comparing `lmqg-0.0.8/lmqg.egg-info/PKG-INFO` & `lmqg-0.1.0/lmqg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lmqg
-Version: 0.0.8
+Version: 0.1.0
 Summary: Language Model for Question Generation.
 Home-page: https://github.com/asahi417/lm-question-generation
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT License
-Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/asahi417/lm-question-generation/archive/v0.1.0.tar.gz
 Keywords: language model,question-answering,question-generation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -21,130 +21,177 @@
 License-File: LICENSE
 
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/lmqg/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/lmqg.svg)](https://badge.fury.io/py/lmqg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 [![PyPI status](https://img.shields.io/pypi/status/lmqg.svg)](https://pypi.python.org/pypi/lmqg/)
 
-# Generative Language Models for Paragraph-Level Question Generation
+# Question and Answer Generation with Language Models
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qg_diagram.png" width="500">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/qag.png" width="400">
+  <br><em> Figure 1: Three distinct QAG approaches. </em>
 </p>
 
-This is the official repository of the paper
-["Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 main conference"](https://aclanthology.org/2022.emnlp-main.42/).
-This repository includes following contents:
-- ***QG-Bench***, the first ever multilingual/multidomain QG benchmark.
-- ***Multilingual/multidomain QG models*** fine-tuned on QG-Bench.
-- A python library ***`lmqg`*** developed for question generation in python as well as QG model fine-tuning/evaluation.
-- ***AutoQG***, a web application hosting QG models where user can test the model output interactively. 
-
-### Table of Contents  
-1. **[QG-Bench: multilingual & multidomain QG datasets (+ fine-tuned models)](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md)**
-2. **[LMQG: python library to fine-tune/evaluate QG model](#lmqg-language-model-for-question-generation-)**
-3. **[AutoQG: web application hosting multilingual QG models](#autoqg)**
-4. **[RestAPI: run model prediction via restAPI](#rest-api-with-huggingface-inference-api)**
+The `lmqg` is a python library for question and answer generation (QAG) with language models (LMs). Here, we consider 
+paragraph-level QAG, where user will provide a context (paragraph or document), and the model will generate a list of 
+question and answer pairs on the context. With `lmqg`, you can do following things:
+- [***Generation in One Line of Code:***](https://github.com/asahi417/lm-question-generation#generate-question--answer) Generate questions and answers in *8* languages (en/fr/ja/ko/ru/it/es/de).
+- [***Model Training/Evaluation:***](https://github.com/asahi417/lm-question-generation#model-development) Train & evaluate your own QG/QAG models.
+- [***QAG & QG Model Hosting:***](https://github.com/asahi417/lm-question-generation#rest-api-with-huggingface-inference-api) Host your QAG models on a web application or a restAPI server.
+- [***AutoQG:***](https://github.com/asahi417/lm-question-generation/tree/master#autoqg) Online web service to generate questions and answers with our models.
+ 
+***Update May 2023:*** Two papers got accepted by ACL 2023 ([QAG at finding](https://asahiushio.com/files/paper_2023_acl_qag.pdf), [LMQG at system demonstration](https://asahiushio.com/files/paper_2023_acl_demo.pdf)). \
+***Update Oct 2022:*** Our [QG paper](https://aclanthology.org/2022.emnlp-main.42/) got accepted by EMNLP main 2022.
+
+### A bit more about QAG models 📝
+Our QAG models can be grouped into three types: **Pipeline**, **Multitask**, 
+and **End2end** (see Figure 1). The **Pipeline** consists of question generation (QG) and answer extraction (AE) models independently,
+where AE will parse all the sentences in the context to extract answers, and QG will generate questions on the answers.
+The **Multitask** follows same architecture as the **Pipeline**, but the QG and AE models are shared model fine-tuned jointly.
+Finally, **End2end** model will generate a list of question and answer pairs in an end-to-end manner.
+In practice, **Pipeline** and **Multitask** generate more question and answer pairs, while **End2end** generates less but a few times faster, 
+and the quality of the generated question and answer pairs depend on language.
+All types are available in the *8* diverse languages (en/fr/ja/ko/ru/it/es/de) via `lmqg`, and the models are all shared on HuggingFace (see the [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md)).
+To know more about QAG, please check [our ACL 2023 paper](https://asahiushio.com/files/paper_2023_acl_qag.pdf) that describes the QAG models and reports a complete performance comparison of each QAG models in every language.
 
-Please cite following paper if you use any resource:
-```
-@inproceedings{ushio-etal-2022-generative,
-    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
-    author = "Ushio, Asahi  and
-        Alva-Manchego, Fernando  and
-        Camacho-Collados, Jose",
-    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
-    month = dec,
-    year = "2022",
-    address = "Abu Dhabi, U.A.E.",
-    publisher = "Association for Computational Linguistics",
-}
-```
+### Is QAG different from Question Generation (QG)? 🤔
 
-## LMQG: Language Model for Question Generation 🚀
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/example.png" width="700">
+  <br><em> Figure 2: An example of QAG (a) and QG (b). </em>
+</p>
+
+All the functionalities support question generation as well. Our QG model assumes user to specify an answer in addition to a context,
+and the QG model will generate a question that is answerable by the answer given the context (see Figure 2 for a comparison of QAG and QG).
+To know more about QG, please check [our EMNLP 2022 paper](https://aclanthology.org/2022.emnlp-main.42/) that describes the QG models more in detail.
+
+
+## Get Started 🚀
 
-The `lmqg` is a python library to fine-tune seq2seq language models ([T5](https://arxiv.org/pdf/1910.10683.pdf), [BART](https://arxiv.org/pdf/1910.13461.pdf)) 
-on the question generation task and provide an API to host the model prediction via [huggingface](https://huggingface.co/).
 Let's install `lmqg` via pip first.
 ```shell
 pip install lmqg
 ```
 
-### Generate Question & Answer
+## Generate Question & Answer
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/13izkdp2l7G2oeh_fwL7xJdR_67HMK_hQ?usp=sharing)
 
-- ***Generate Question on Answers:*** This is a basic usecase of our QG models, where user provides a paragraph and an answer to generate a question that is answerable by the answer given the paragraph.
-See [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#qg-models) for the available models.
+The main functionality of `lmqg` is to generate question and answer pairs on a given context with a handy api.
+The available models for each QAG class can be found at [model card](https://github.com/asahi417/lm-question-generation/blob/master/MODEL_CARD.md#qag).
 
+- ***QAG with End2end or Multitask Models:*** The end2end QAG models are fine-tuned to generate a list of QA pairs with a single inference, 
+  so it is the fastest class among our QAG models. Meanwhile, multitask QAG models breakdown the QAG task into QG and AE, where they 
+  parse each sentence to get the answer with AE, and generate question on each answer with QG. Multitask QAG potentially generate more QA pairs than end2end QAG, but 
+  inference takes a few times more than end2end models. Both models can be used as following 
+  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg')
+model = TransformersQG('lmqg/t5-base-squad-qag') # or TransformersQG(model='lmqg/t5-base-squad-qg-ae') 
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is William Turner often known as?', 'William Turner of Oxford or just Turner of Oxford'),
+    ("What did many of Turner's paintings depict?", 'the countryside around Oxford'),
+    ("What is one of Turner's best known pictures?", 'a view of the city of Oxford from Hinksey Hill')
+]
+```
+
+- ***QAG with Pipeline Models:*** The pipeline QAG is similar to multitask QAG, but the QG and AE models are independently fine-tuned, unlike 
+  multitask QAG that fine-tunes QG and AE jointly. Pipeline QAG can improve the performance in some cases, but it is as heavy as multitask QAG with 
+  more storage consuming due to the two models loaded. The pipeline QAG can be used as following. The `model` and `model_ae` are the QG and AE models respectively.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg', model_ae='lmqg/t5-base-squad-ae')  
+# paragraph to generate pairs of question and answer
+context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+# model prediction
+question_answer = model.generate_qa(context)
+# the output is a list of tuple (question, answer)
+pprint(question_answer)
+[
+    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
+    ('What is another name for William Turner?', 'William Turner of Oxford'),
+    ("What did many of William Turner's paintings depict around Oxford?", 'the countryside'),
+    ('From what hill is a view of the city of Oxford taken?', 'Hinksey Hill.')
+]
+```
+
+- ***QG only:*** The QG model can be used as following. The `model` is the QG model. See the [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md), 
+a multilingual QG benchmark, for the list of available QG models.
+  
+```python
+from pprint import pprint
+from lmqg import TransformersQG
+
+# initialize model
+model = TransformersQG(model='lmqg/t5-base-squad-qg')
+
 # a list of paragraph
 context = [
     "William Turner was an English painter who specialised in watercolour landscapes",
     "William Turner was an English painter who specialised in watercolour landscapes"
 ]
 # a list of answer (same size as the context)
 answer = [
     "William Turner",
     "English"
 ]
 # model prediction
 question = model.generate_q(list_context=context, list_answer=answer)
-print(question)
+pprint(question)
 [
-    'Who was an English painter who specialised in watercolour landscapes?',
-    'What nationality was William Turner?'
+  'Who was an English painter who specialised in watercolour landscapes?',
+  'What nationality was William Turner?'
 ]
-```
+``` 
+
+- ***AE only:*** The QG model can be used as following. The `model` is the QG model.
 
-- ***Generate Question & Answer Pairs:*** Instead of specifying an answer, user can let QG model to generate an answer on the paragraph, and generate question on it sequentially.
-This functionality is only available for the QG models fine-tuned with answer extraction see [MODEL CARD](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md#models-with-answer-extraction) for the full list of models with answer extraction (model alias usually has a suffix of `-qg-ae`).
-  
 ```python
+from pprint import pprint
 from lmqg import TransformersQG
+
 # initialize model
-model = TransformersQG(language='en', model='lmqg/t5-large-squad-qg-ae')
-# paragraph to generate pairs of question and answer
-context = "William Turner was an English painter who specialised in watercolour landscapes. He is often known as William Turner of Oxford or just Turner of Oxford to distinguish him from his contemporary, J. M. W. Turner. Many of Turner's paintings depicted the countryside around Oxford. One of his best known pictures is a view of the city of Oxford from Hinksey Hill."
+model = TransformersQG(model='lmqg/t5-base-squad-ae')
 # model prediction
-question_answer = model.generate_qa(context)
-# the output is a list of tuple (question, answer)
-print(question_answer)
-[
-    ('Who was an English painter who specialised in watercolour landscapes?', 'William Turner'),
-    ("What was William Turner's nickname?", 'William Turner of Oxford'),
-    ("What did many of Turner's paintings depict around Oxford?", 'countryside'),
-    ("What is one of William Turner's best known paintings?", 'a view of the city of Oxford')
-]
+answer = model.generate_a("William Turner was an English painter who specialised in watercolour landscapes")
+pprint(answer)
+['William Turner']
 ```
 
+## AutoQG
 
-### Model Evaluation
-The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
-From command line, run following command 
-```shell
-lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
-Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
-```shell
-lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
-```
-The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
-([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
-Check `lmqg-eval -h` to display all the options.
+<p align="center">
+  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
+</p>
+
+***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QAG models.
+
+## Model Development
+The `lmqg` also provides a command line interface to fine-tune and evaluate QG, AE, and QAG models.
 
 ### Model Training
 <p align="center">
   <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/grid_search.png" width="650">
 </p>
 
-To fine-tune QG model, we employ a two-stage hyper-parameter optimization, described as above diagram.
+To fine-tune QG (or AE, QAG) model, we employ a two-stage hyper-parameter optimization, described as above diagram.
 Following command is to run the fine-tuning with parameter optimization.
 ```shell
 lmqg-train-search -c "tmp_ckpt" -d "lmqg/qg_squad" -m "t5-small" -b 64 --epoch-partial 5 -e 15 --language "en" --n-max-config 1 \
   -g 2 4 --lr 1e-04 5e-04 1e-03 --label-smoothing 0 0.15
 ```
 Check `lmqg-train-search -h` to display all the options.
 
@@ -163,26 +210,33 @@
     lr=[1e-04, 5e-04, 1e-03],
     label_smoothing=[0, 0.15]
 )
 trainer.run()
 ```
 
 
-## AutoQG
-
-<p align="center">
-  <img src="https://raw.githubusercontent.com/asahi417/lm-question-generation/master/assets/autoqg.gif" width="500">
-</p>
+### Model Evaluation
+The evaluation tool reports `BLEU4`, `ROUGE-L`, `METEOR`, `BERTScore`, and `MoverScore` following [QG-Bench](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
+From command line, run following command 
+```shell
+lmqg-eval -m "lmqg/t5-large-squad-qg" -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+where `-m` is a model alias on huggingface or path to local checkpoint, `-e` is the directly to export the metric file, `-d` is the dataset to evaluate, and `-l` is the language of the test set.
+Instead of running model prediction, you can provide a prediction file instead to avoid computing it each time.
+```shell
+lmqg-eval --hyp-test '{your prediction file}' -e "./eval_metrics" -d "lmqg/qg_squad" -l "en"
+```
+The prediction file should be a text file of model generation in each line in the order of `test` split in the target dataset
+([sample](https://huggingface.co/lmqg/t5-large-squad/raw/main/eval/samples.validation.hyp.paragraph_sentence.question.lmqg_qg_squad.default.txt)).
+Check `lmqg-eval -h` to display all the options.
 
-***AutoQG ([https://autoqg.net](https://autoqg.net/))*** is a free web application hosting our QG models.
-The QG models are listed at the [QG-Bench page](https://github.com/asahi417/lm-question-generation/blob/master/QG_BENCH.md).
 
 ## Rest API with huggingface inference API
 
-We provide a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
+Finally, `lmqg` provides a rest API which hosts the model inference through huggingface inference API. You need huggingface API token to run your own API and install dependencies as below.
 ```shell
 pip install lmqg[api]
 ```
 Swagger UI is available at [`http://127.0.0.1:8088/docs`](http://127.0.0.1:8088/docs), when you run the app locally (replace the address by your server address).
 
 ### Build
 - Build/Run Local (command line):
@@ -215,14 +269,57 @@
   "qa": [
     {"question": "Who founded Nintendo Karuta?", "answer": "Fusajiro Yamauchi"},
     {"question": "When did Nintendo distribute its first video game console, the Color TV-Game?", "answer": "1977"}
   ]
 }
 ```
 
-## Misc
-Following link is useful if you need to reproduce the results in our paper.
-- [Model Fine-tuning/Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qg_model_training)
-- [QA based Evaluation](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/qa_based_evaluation)
-- [NQG model baseline](https://github.com/asahi417/lm-question-generation/tree/master/misc/emnlp_2022/nqg_baseline)
+## Citation
+Please cite following paper if you use any resource and see the code to reproduce the model if needed.
+
+- [***Generative Language Models for Paragraph-Level Question Generation, EMNLP 2022 Main***](https://aclanthology.org/2022.emnlp-main.42/): The QG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2022_emnlp_qg)).
+```
+@inproceedings{ushio-etal-2022-generative,
+    title = "{G}enerative {L}anguage {M}odels for {P}aragraph-{L}evel {Q}uestion {G}eneration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
+    month = dec,
+    year = "2022",
+    address = "Abu Dhabi, U.A.E.",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+- [***An Empirical Comparison of LM-based Question and Answer Generation Methods, ACL 2022 Finding***](https://asahiushio.com/files/paper_2023_acl_qag.pdf): The QAG models ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+```
+@inproceedings{ushio-etal-2023-tba,
+    title = "TBA",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
+
+- [***A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration***](https://asahiushio.com/files/paper_2023_acl_demo.pdf): The library and demo ([code to reproduce experiments](https://github.com/asahi417/lm-question-generation/tree/master/misc/2023_acl_qag)).
+
+```
+@inproceedings{ushio-etal-2023-a-practical-toolkit
+    title = "A Practical Toolkit for Multilingual Question and Answer Generation, ACL 2022, System Demonstration",
+    author = "Ushio, Asahi  and
+        Alva-Manchego, Fernando  and
+        Camacho-Collados, Jose",
+    booktitle = "Proceedings of the 61th Annual Meeting of the Association for Computational Linguistics: System Demonstrations",
+    month = Jul,
+    year = "2023",
+    address = "Toronto, Canada",
+    publisher = "Association for Computational Linguistics",
+}
+```
```

### Comparing `lmqg-0.0.8/lmqg.egg-info/SOURCES.txt` & `lmqg-0.1.0/lmqg.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 lmqg.egg-info/SOURCES.txt
 lmqg.egg-info/dependency_links.txt
 lmqg.egg-info/entry_points.txt
 lmqg.egg-info/requires.txt
 lmqg.egg-info/top_level.txt
 lmqg/automatic_evaluation_tool/__init__.py
 lmqg/automatic_evaluation_tool/bertscore.py
+lmqg/automatic_evaluation_tool/meteor.py
 lmqg/automatic_evaluation_tool/moverscore.py
 lmqg/automatic_evaluation_tool/qa_aligned_f1_score.py
 lmqg/automatic_evaluation_tool/rouge.py
 lmqg/automatic_evaluation_tool/text_normalization.py
 lmqg/automatic_evaluation_tool/bert_score/__init__.py
 lmqg/automatic_evaluation_tool/bert_score/score.py
 lmqg/automatic_evaluation_tool/bert_score/scorer.py
```

### Comparing `lmqg-0.0.8/setup.py` & `lmqg-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
-VERSION = '0.0.8'
+VERSION = '0.1.0'
 NAME = 'lmqg'
 LICENSE = 'MIT License'
 setup(
     name=NAME,
     packages=find_packages(exclude=['tests', 'misc', 'asset']),
     version=VERSION,
     license=LICENSE,
@@ -44,32 +44,35 @@
         'pytextrank',
         "torch",
         "tqdm",
         "requests",
         "pandas",
         "numpy",
         "transformers>=4.26.1",
-        "huggingface-hub",
+        "huggingface-hub>=0.12.0",
         # "transformers<=4.21.2",  # push-to-model is not working for latest version
         # "huggingface-hub<=0.9.1",
         "sentencepiece",
         "datasets",
         "spacy",
         'sudachipy',
         'sudachidict_core',
         'bert-score',
         'pyemd',  # to compute moverscore
         'evaluate',
         "wandb",
         "ray",
-        "ray[tune]"
+        "ray[tune]",
+        "nltk",
+        "accelerate"
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
+            'lmqg-train = lmqg.lmqg_cl.model_finetuning:main_training',
             'lmqg-train-search = lmqg.lmqg_cl.model_finetuning:main_training_search',
             'lmqg-eval = lmqg.lmqg_cl.model_evaluation:main',
             'lmqg-eval-qag = lmqg.lmqg_cl.model_evaluation_qag:main',
             'lmqg-eval-qa = lmqg.lmqg_cl.model_evaluation_qa:main',
             'lmqg-push-to-hf = lmqg.lmqg_cl.push_to_hf:main',
             'lmqg-generate-qa = lmqg.lmqg_cl.model_evaluation_qa_based_metric:main_generate_qa_pair',
             'lmqg-qae = lmqg.lmqg_cl.model_evaluation_qa_based_metric:main_qa_model_training'
```

