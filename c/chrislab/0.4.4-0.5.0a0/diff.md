# Comparing `tmp/chrislab-0.4.4.tar.gz` & `tmp/chrislab-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrislab-0.4.4.tar", last modified: Mon Mar 27 08:36:58 2023, max compression
+gzip compressed data, was "chrislab-0.5.0a0.tar", last modified: Fri May 12 08:09:10 2023, max compression
```

## Comparing `chrislab-0.4.4.tar` & `chrislab-0.5.0a0.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.435820 chrislab-0.4.4/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-03-27 07:49:21.000000 chrislab-0.4.4/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      880 2023-03-27 08:36:58.435820 chrislab-0.4.4/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-03-27 07:49:21.000000 chrislab-0.4.4/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-03-27 07:49:21.000000 chrislab-0.4.4/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1133 2023-03-27 08:36:58.435820 chrislab-0.4.4/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.375820 chrislab-0.4.4/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.423820 chrislab-0.4.4/src/chrislab/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.427820 chrislab-0.4.4/src/chrislab/common/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/common/__init__.py
--rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/common/downloader.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14529 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/common/tokenizer_korbert.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    13156 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/common/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.427820 chrislab-0.4.4/src/chrislab/language/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/converter.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/evaluater.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/finetuner.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/modeling.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/language/predictor.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.427820 chrislab-0.4.4/src/chrislab/ratsnlp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/ratsnlp/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5327 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/chrislab/ratsnlp/cli.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.423820 chrislab-0.4.4/src/chrislab.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      880 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)     1823 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      108 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      201 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-03-27 08:36:58.000000 chrislab-0.4.4/src/chrislab.egg-info/zip-safe
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.427820 chrislab-0.4.4/src/ratsnlp/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.431820 chrislab-0.4.4/src/ratsnlp/nlpbook/
--rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.431820 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/
--rw-rw-r--   0 chris     (1000) chris     (1000)      181 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5365 2023-03-27 08:12:25.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5677 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      647 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1740 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/classification/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/data_utils.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.431820 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/
--rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5379 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1280 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/generation/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/metrics.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.431820 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/
--rw-rw-r--   0 chris     (1000) chris     (1000)      149 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4726 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    12164 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      627 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1747 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/ner/task.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.435820 chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/
--rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2675 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/deploy.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:36:58.435820 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/
--rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/arguments.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17108 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/corpus.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/deploy.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2067 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/qa/task.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1176 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/trainer.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     8691 2023-03-27 07:49:21.000000 chrislab-0.4.4/src/ratsnlp/nlpbook/utils.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      832 2023-05-12 08:09:10.894961 chrislab-0.5.0a0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      291 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1095 2023-05-12 08:09:10.894961 chrislab-0.5.0a0/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.886961 chrislab-0.5.0a0/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.886961 chrislab-0.5.0a0/src/chrislab/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/chrislab/common/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/common/__init__.py
+-rwxrwxr-x   0 chris     (1000) chris     (1000)     7852 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/common/downloader.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14529 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/common/tokenizer_korbert.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    13164 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/common/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/chrislab/language/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1316 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14142 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/converter.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     9408 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/evaluater.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    39567 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/finetuner.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6833 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/modeling.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    14491 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/language/predictor.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/chrislab/ratsnlp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/ratsnlp/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10788 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/chrislab/ratsnlp/cli.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/chrislab.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      832 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1722 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      108 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      201 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       17 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 08:09:10.000000 chrislab-0.5.0a0/src/chrislab.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       70 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6249 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/arguments.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       59 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5626 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1715 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2246 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/data_utils.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      663 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      170 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4280 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5379 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      882 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1301 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      653 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/metrics.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    12004 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1802 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/task.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       62 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2675 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      641 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/deploy.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 08:09:10.890961 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      146 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4984 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/arguments.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    17108 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/corpus.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      639 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/deploy.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2088 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/task.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1253 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/trainer.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     8691 2023-05-12 07:41:54.000000 chrislab-0.5.0a0/src/ratsnlp/nlpbook/utils.py
```

### Comparing `chrislab-0.4.4/LICENSE` & `chrislab-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/PKG-INFO` & `chrislab-0.5.0a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.4.4
+Version: 0.5.0a0
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chrislab
```

### Comparing `chrislab-0.4.4/setup.cfg` & `chrislab-0.5.0a0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [metadata]
 name = chrislab
-version = 0.4.4
+version = 0.5.0a
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrislab
 description = An advanced tool for doing experimental study.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = True
 packages = find:
 package_dir =
```

### Comparing `chrislab-0.4.4/src/chrislab/common/downloader.py` & `chrislab-0.5.0a0/src/chrislab/common/downloader.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/common/tokenizer_korbert.py` & `chrislab-0.5.0a0/src/chrislab/common/tokenizer_korbert.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/common/util.py` & `chrislab-0.5.0a0/src/chrislab/common/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from chrisbase.io import make_dir, files_info, dirs, exists_or, hr
 from chrisbase.io import prepend_to_global_path
 from chrisbase.io import running_file, run_command
 from chrisbase.time import now
 from chrisbase.util import number_only, NO, tupled, to_dataframe
 
 
-def working_gpus(gpus=None):
+def cuda_visible_devices(gpus=None):
     if gpus:
         os.environ["CUDA_DEVICE_ORDER"] = "PCI_BUS_ID"
         os.environ["CUDA_VISIBLE_DEVICES"] = gpus
     return os.environ.get("CUDA_VISIBLE_DEVICES")
 
 
 def num_cuda_devices():
```

### Comparing `chrislab-0.4.4/src/chrislab/language/cli.py` & `chrislab-0.5.0a0/src/chrislab/language/cli.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/language/converter.py` & `chrislab-0.5.0a0/src/chrislab/language/converter.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/language/evaluater.py` & `chrislab-0.5.0a0/src/chrislab/language/evaluater.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/language/finetuner.py` & `chrislab-0.5.0a0/src/chrislab/language/finetuner.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/language/modeling.py` & `chrislab-0.5.0a0/src/chrislab/language/modeling.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab/language/predictor.py` & `chrislab-0.5.0a0/src/chrislab/language/predictor.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/chrislab.egg-info/PKG-INFO` & `chrislab-0.5.0a0/src/chrislab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: chrislab
-Version: 0.4.4
+Version: 0.5.0a0
 Summary: An advanced tool for doing experimental study.
 Home-page: https://github.com/chrisjihee/chrislab
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chrislab
```

### Comparing `chrislab-0.4.4/src/chrislab.egg-info/SOURCES.txt` & `chrislab-0.5.0a0/src/chrislab.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -21,32 +21,30 @@
 src/chrislab/language/finetuner.py
 src/chrislab/language/modeling.py
 src/chrislab/language/predictor.py
 src/chrislab/ratsnlp/__init__.py
 src/chrislab/ratsnlp/cli.py
 src/ratsnlp/__init__.py
 src/ratsnlp/nlpbook/__init__.py
+src/ratsnlp/nlpbook/arguments.py
 src/ratsnlp/nlpbook/data_utils.py
+src/ratsnlp/nlpbook/deploy.py
 src/ratsnlp/nlpbook/metrics.py
 src/ratsnlp/nlpbook/trainer.py
 src/ratsnlp/nlpbook/utils.py
 src/ratsnlp/nlpbook/classification/__init__.py
-src/ratsnlp/nlpbook/classification/arguments.py
 src/ratsnlp/nlpbook/classification/corpus.py
-src/ratsnlp/nlpbook/classification/deploy.py
 src/ratsnlp/nlpbook/classification/task.py
 src/ratsnlp/nlpbook/generation/__init__.py
 src/ratsnlp/nlpbook/generation/arguments.py
 src/ratsnlp/nlpbook/generation/corpus.py
 src/ratsnlp/nlpbook/generation/deploy.py
 src/ratsnlp/nlpbook/generation/task.py
 src/ratsnlp/nlpbook/ner/__init__.py
-src/ratsnlp/nlpbook/ner/arguments.py
 src/ratsnlp/nlpbook/ner/corpus.py
-src/ratsnlp/nlpbook/ner/deploy.py
 src/ratsnlp/nlpbook/ner/task.py
 src/ratsnlp/nlpbook/paircls/__init__.py
 src/ratsnlp/nlpbook/paircls/corpus.py
 src/ratsnlp/nlpbook/paircls/deploy.py
 src/ratsnlp/nlpbook/qa/__init__.py
 src/ratsnlp/nlpbook/qa/arguments.py
 src/ratsnlp/nlpbook/qa/corpus.py
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/classification/arguments.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/arguments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import os
 from dataclasses import dataclass, field
 from pathlib import Path
+from typing import List
 
 import pandas as pd
 from dataclasses_json import DataClassJsonMixin
+from pytorch_lightning.accelerators import Accelerator
+from pytorch_lightning.strategies import Strategy
 
 from chrisbase.io import ProjectEnv
 from chrisbase.io import files, make_parent_dir, out_hr, out_table
 from chrisbase.util import to_dataframe
 
 
 @dataclass
-class ClassificationArguments(DataClassJsonMixin):
+class NLUArguments(DataClassJsonMixin):
     def env_data(self) -> ProjectEnv:
         if isinstance(self.env, ProjectEnv):
             return self.env
         else:
             return ProjectEnv.from_dict(self.env)
 
     def env_dict(self) -> dict:
         if isinstance(self.env, DataClassJsonMixin):
             return self.env.to_dict()
         else:
             return self.env
 
     def __post_init__(self):
         self.env = self.env_data()
-        self.working_config_file = self.env.running_file.with_suffix('.json').name
         self.downstream_model_home = Path(self.downstream_model_home)
 
     env: ProjectEnv | dict = field(
         metadata={"help": "current project environment"}
     )
     pretrained_model_path: Path | str | None = field(
         default="beomi/kcbert-base",
@@ -40,33 +42,32 @@
         default=None,
         metadata={"help": "root directory of output model and working config"}
     )
     downstream_model_file: str | None = field(
         default=None,
         metadata={"help": "filename or filename format of output model"}
     )
-    downstream_task_name: str = field(
-        default="document-classification",
+    downstream_task_name: str | None = field(
+        default=None,
         metadata={"help": "name of downstream task"}
     )
+    working_config_file: str | None = field(
+        default=None,
+        metadata={"help": "filename of current config"}
+    )
     max_seq_length: int = field(
         default=128,
         metadata={"help": "The maximum total input sequence length after tokenization. "
                           "Sequences longer than this will be truncated, sequences shorter will be padded."}
     )
-    working_config_file: str | None = field(
-        init=False,
-        metadata={"help": "filename of current config"}
-    )
 
     def save_working_config(self, to: Path | str = None) -> Path:
         self.env = self.env_dict()
-        config_file = make_parent_dir(to) if to \
-            else make_parent_dir(self.downstream_model_home / self.working_config_file)
-        config_file.write_text(self.to_json(default=str, ensure_ascii=False, indent=2))
+        config_file = to if to else self.downstream_model_home.parent / self.working_config_file
+        make_parent_dir(config_file).write_text(self.to_json(default=str, ensure_ascii=False, indent=2))
         return config_file
 
     def as_dataframe(self):
         columns = [self.__class__.__name__, "value"]
         return pd.concat([
             to_dataframe(data_prefix="env", raw=self.env, columns=columns),
             to_dataframe(data_exclude="env", raw=self, columns=columns),
@@ -76,20 +77,24 @@
         out_hr(c='-')
         out_table(self.as_dataframe())
         out_hr(c='-')
         return self
 
 
 @dataclass
-class ClassificationTrainArguments(ClassificationArguments):
+class NLUTrainerArguments(NLUArguments):
     def __post_init__(self):
         super().__post_init__()
+        self.downstream_data_home = Path(self.downstream_data_home)
+        if not self.working_config_file:
+            self.working_config_file = self.downstream_model_home \
+                .with_stem(self.downstream_model_home.stem + "=train") \
+                .with_suffix('.json').name
         if not self.save_top_k:
             self.save_top_k = self.epochs
-        self.downstream_data_home = Path(self.downstream_data_home)
 
     downstream_data_home: Path | str | None = field(
         default="/content/Korpora",
         metadata={"help": "root of downstream data"}
     )
     downstream_data_name: str | None = field(
         default=None,
@@ -131,24 +136,40 @@
         default=32,
         metadata={"help": "batch size. if 0, let lightening find the best batch size"}
     )
     cpu_workers: int = field(
         default=os.cpu_count(),
         metadata={"help": "number of CPU workers"}
     )
-    fp16: bool = field(
-        default=False,
-        metadata={"help": "enable train on floating point 16"}
+    accelerator: str | Accelerator = field(
+        default="auto",
+        metadata={"help": 'accelerator types ("cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto")'}
+    )
+    precision: str | int = field(
+        default="32-true",
+        metadata={"help": "floating-point precision type"}
+    )
+    strategy: str | Strategy = field(
+        default="auto",
+        metadata={"help": 'training strategies'}
+    )
+    devices: List[int] | str | int = field(
+        default="auto",
+        metadata={"help": 'devices to use'}
     )
 
 
 @dataclass
-class ClassificationDeployArguments(ClassificationArguments):
+class NLUServerArguments(NLUArguments):
     def __post_init__(self):
         super().__post_init__()
+        assert self.downstream_model_home.exists(), f"downstream_model_home does not exist: {self.downstream_model_home}"
+        assert self.downstream_model_home.is_dir(), f"downstream_model_home is not a directory: {self.downstream_model_home}"
+        if not self.working_config_file:
+            self.working_config_file = self.downstream_model_home \
+                .with_stem(self.downstream_model_home.stem + "=serve") \
+                .with_suffix('.json').name
         if not self.downstream_model_file:
-            assert self.downstream_model_home.exists() and self.downstream_model_home.is_dir(), \
-                f"downstream_model_path is not a directory: {self.downstream_model_home}"
             ckpt_files = files(self.downstream_model_home / "*.ckpt")
             ckpt_files = sorted([x for x in ckpt_files if "temp" not in str(x) and "tmp" not in str(x)], key=str)
             assert len(ckpt_files) > 0, f"No checkpoint file in {self.downstream_model_home}"
             self.downstream_model_file = ckpt_files[-1].name
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/classification/corpus.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/corpus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import os
 import csv
-import time
-import torch
 import logging
-from filelock import FileLock
+import os
+import time
 from dataclasses import dataclass
 from typing import List, Optional
+
+import torch
+from filelock import FileLock
 from torch.utils.data.dataset import Dataset
-from transformers import PreTrainedTokenizer
-from ratsnlp.nlpbook.classification.arguments import ClassificationTrainArguments
 
+from ratsnlp.nlpbook import NLUTrainerArguments
+from transformers import PreTrainedTokenizer
 
 logger = logging.getLogger("ratsnlp")
 
 
 @dataclass
 class ClassificationExample:
     text_a: str
@@ -53,15 +54,15 @@
     def num_labels(self):
         return len(self.get_labels())
 
 
 def _convert_examples_to_classification_features(
         examples: List[ClassificationExample],
         tokenizer: PreTrainedTokenizer,
-        args: ClassificationTrainArguments,
+        args: NLUTrainerArguments,
         label_list: List[str],
 ):
     label_map = {label: i for i, label in enumerate(label_list)}
     labels = [label_map[example.label] for example in examples]
 
     logger.info(
         "tokenize sentences, it could take a lot of time..."
@@ -97,15 +98,15 @@
     return features
 
 
 class ClassificationDataset(Dataset):
 
     def __init__(
             self,
-            args: ClassificationTrainArguments,
+            args: NLUTrainerArguments,
             tokenizer: PreTrainedTokenizer,
             corpus,
             mode: Optional[str] = "train",
             convert_examples_to_features_fn=_convert_examples_to_classification_features,
     ):
         if corpus is not None:
             self.corpus = corpus
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/classification/deploy.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from flask import Flask, request, jsonify, render_template
 
 
-def get_web_service_app(inference_fn, ngrok_home=None):
+def get_web_service_app(inference_fn, template_file, ngrok_home=None):
     app = Flask(__name__, template_folder='')
     if ngrok_home:
         from flask_ngrok import run_with_ngrok
         run_with_ngrok(app, home=ngrok_home)
     else:
         from flask_cors import CORS
         CORS(app)
 
     @app.route('/')
     def index():
-        return render_template('index.html')
+        return render_template(template_file)
 
     @app.route('/api', methods=['POST'])
     def api():
         query_sentence = request.json
         output_data = inference_fn(query_sentence)
         response = jsonify(output_data)
         return response
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/classification/task.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,47 @@
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from lightning import LightningModule
-from ratsnlp.nlpbook.classification.arguments import ClassificationTrainArguments
+from ratsnlp.nlpbook import NLUTrainerArguments
 from ratsnlp.nlpbook.metrics import accuracy
-from transformers import PreTrainedModel
+from ratsnlp.nlpbook.ner import NER_PAD_ID
+from transformers import BertPreTrainedModel
 
 
-class ClassificationTask(LightningModule):
+class NERTask(LightningModule):
 
     def __init__(self,
-                 model: PreTrainedModel,
-                 args: ClassificationTrainArguments,
-    ):
+                 model: BertPreTrainedModel,
+                 args: NLUTrainerArguments,
+                 ):
         super().__init__()
         self.model = model
         self.args = args
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning_rate)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'lr_scheduler': scheduler,
         }
 
     def training_step(self, inputs, batch_idx):
-        # outputs: SequenceClassifierOutput
+        # outputs: TokenClassifierOutput
         outputs = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
-        acc = accuracy(preds, labels)
+        acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
         self.log("loss", outputs.loss, prog_bar=False, logger=True, on_step=True, on_epoch=False)
         self.log("acc", acc, prog_bar=True, logger=True, on_step=True, on_epoch=False)
         return outputs.loss
 
     def validation_step(self, inputs, batch_idx):
-        # outputs: SequenceClassifierOutput
+        # outputs: TokenClassifierOutput
         outputs = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
-        acc = accuracy(preds, labels)
+        acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
         self.log("val_loss", outputs.loss, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         self.log("val_acc", acc, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         return outputs.loss
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/data_utils.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/generation/arguments.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/generation/corpus.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/generation/deploy.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/deploy.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/generation/task.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/generation/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from lightning import LightningModule
 from ratsnlp.nlpbook.generation.arguments import GenerationTrainArguments
 from transformers import PreTrainedModel
 
 
 class GenerationTask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
                  args: GenerationTrainArguments,
-    ):
+                 ):
         super().__init__()
         self.model = model
         self.args = args
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning_rate)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/metrics.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/metrics.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/ner/corpus.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/ner/corpus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+import logging
 import os
 import re
 import time
+from dataclasses import dataclass
+from typing import List, Optional
+
 import torch
-import logging
 from filelock import FileLock
-from typing import List, Optional
-from dataclasses import dataclass
-from transformers import BertTokenizer
 from torch.utils.data.dataset import Dataset
-from ratsnlp.nlpbook.ner import NERTrainArguments
-from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
+from ratsnlp.nlpbook import NLUTrainerArguments
+from transformers import BertTokenizer
+from transformers.tokenization_utils_base import PaddingStrategy, TruncationStrategy
 
 logger = logging.getLogger("ratsnlp")
 
-
 # 자체 제작 NER 코퍼스 기준의 레이블 시퀀스를 만들기 위한 ID 체계
 # 나 는 삼성 에 입사 했다
 # O O 기관 O O O > [CLS] O O 기관 O O O [SEP] [PAD] [PAD] ...
 NER_CLS_TOKEN = "[CLS]"
 NER_SEP_TOKEN = "[SEP]"
 NER_PAD_TOKEN = "[PAD]"
 NER_MASK_TOKEN = "[MASK]"
@@ -39,40 +39,40 @@
     label_ids: Optional[List[int]] = None
 
 
 class NERCorpus:
 
     def __init__(
             self,
-            args: NERTrainArguments
+            args: NLUTrainerArguments
     ):
         self.args = args
 
     def get_examples(self, data_root_path, mode):
         data_fpath = os.path.join(data_root_path, f"{mode}.txt")
         logger.info(f"loading {mode} data... LOOKING AT {data_fpath}")
         examples = []
         for line in open(data_fpath, "r", encoding="utf-8").readlines():
             text, label = line.split("\u241E")
             examples.append(NERExample(text=text, label=label))
         return examples
 
     def get_labels(self):
         label_map_path = os.path.join(
-            self.args.downstream_model_dir,
+            self.args.downstream_model_home,
             "label_map.txt",
         )
         if not os.path.exists(label_map_path):
             logger.info("processing NER tag dictionary...")
-            os.makedirs(self.args.downstream_model_dir, exist_ok=True)
+            os.makedirs(self.args.downstream_model_home, exist_ok=True)
             ner_tags = []
             regex_ner = re.compile('<(.+?):[A-Z]{3}>')
             train_corpus_path = os.path.join(
-                self.args.downstream_corpus_root_dir,
-                self.args.downstream_corpus_name,
+                self.args.downstream_data_home,
+                self.args.downstream_data_name,
                 "train.txt",
             )
             target_sentences = [line.split("\u241E")[1].strip()
                                 for line in open(train_corpus_path, "r", encoding="utf-8").readlines()]
             for target_sentence in target_sentences:
                 regex_filter_res = regex_ner.finditer(target_sentence)
                 for match_item in regex_filter_res:
@@ -200,82 +200,82 @@
     label_ids = [label_map[label] for label in label_sequence]
     return label_ids
 
 
 def _convert_examples_to_ner_features(
         examples: List[NERExample],
         tokenizer: BertTokenizer,
-        args: NERTrainArguments,
+        args: NLUTrainerArguments,
         label_list: List[str],
         cls_token_at_end: Optional[bool] = False,
-    ):
-        """
-        `cls_token_at_end` define the location of the CLS token:
-                - False (Default, BERT/XLM pattern): [CLS] + A + [SEP] + B + [SEP]
-                - True (XLNet/GPT pattern): A + [SEP] + B + [SEP] + [CLS]
-        """
-        label_map = {label: i for i, label in enumerate(label_list)}
-        id_to_label = {i: label for i, label in enumerate(label_list)}
-
-        features = []
-        for example in examples:
-            tokens = tokenizer.tokenize(example.text)
-            inputs = tokenizer._encode_plus(
-                tokens,
-                max_length=args.max_seq_length,
-                truncation_strategy=TruncationStrategy.LONGEST_FIRST,
-                padding_strategy=PaddingStrategy.MAX_LENGTH,
-            )
-            label_ids = _process_target_sentence(
-                tokens=tokens,
-                origin_sentence=example.text,
-                target_sentence=example.label,
-                max_length=args.max_seq_length,
-                label_map=label_map,
-                tokenizer=tokenizer,
-                cls_token_at_end=cls_token_at_end,
-            )
-            features.append(NERFeatures(**inputs, label_ids=label_ids))
+):
+    """
+    `cls_token_at_end` define the location of the CLS token:
+            - False (Default, BERT/XLM pattern): [CLS] + A + [SEP] + B + [SEP]
+            - True (XLNet/GPT pattern): A + [SEP] + B + [SEP] + [CLS]
+    """
+    label_map = {label: i for i, label in enumerate(label_list)}
+    id_to_label = {i: label for i, label in enumerate(label_list)}
+
+    features = []
+    for example in examples:
+        tokens = tokenizer.tokenize(example.text)
+        inputs = tokenizer._encode_plus(
+            tokens,
+            max_length=args.max_seq_length,
+            truncation_strategy=TruncationStrategy.LONGEST_FIRST,
+            padding_strategy=PaddingStrategy.MAX_LENGTH,
+        )
+        label_ids = _process_target_sentence(
+            tokens=tokens,
+            origin_sentence=example.text,
+            target_sentence=example.label,
+            max_length=args.max_seq_length,
+            label_map=label_map,
+            tokenizer=tokenizer,
+            cls_token_at_end=cls_token_at_end,
+        )
+        features.append(NERFeatures(**inputs, label_ids=label_ids))
 
-        for i, example in enumerate(examples[:5]):
-            logger.info("*** Example ***")
-            logger.info("sentence: %s" % (example.text))
-            logger.info("target: %s" % (example.label))
-            logger.info("tokens: %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
-            logger.info("label: %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
-            logger.info("features: %s" % features[i])
+    for i, example in enumerate(examples[:5]):
+        logger.info("*** Example ***")
+        logger.info("sentence: %s" % (example.text))
+        logger.info("target: %s" % (example.label))
+        logger.info("tokens: %s" % (" ".join(tokenizer.convert_ids_to_tokens(features[i].input_ids))))
+        logger.info("label: %s" % (" ".join([id_to_label[label_id] for label_id in features[i].label_ids])))
+        logger.info("features: %s" % features[i])
 
-        return features
+    return features
 
 
 class NERDataset(Dataset):
 
     def __init__(
             self,
-            args: NERTrainArguments,
+            args: NLUTrainerArguments,
             tokenizer: BertTokenizer,
             corpus: NERCorpus,
             mode: Optional[str] = "train",
             convert_examples_to_features_fn=_convert_examples_to_ner_features,
     ):
         if corpus is not None:
             self.corpus = corpus
         else:
             raise KeyError("corpus is not valid")
         if not mode in ["train", "val", "test"]:
             raise KeyError(f"mode({mode}) is not a valid split name")
         # Load data features from cache or dataset file
         cached_features_file = os.path.join(
-            args.downstream_corpus_root_dir,
-            args.downstream_corpus_name,
+            args.downstream_data_home,
+            args.downstream_data_name,
             "cached_{}_{}_{}_{}_{}".format(
                 mode,
                 tokenizer.__class__.__name__,
                 str(args.max_seq_length),
-                args.downstream_corpus_name,
+                args.downstream_data_name,
                 args.downstream_task_name,
             ),
         )
 
         # Make sure only the first process in distributed training processes the dataset,
         # and the others will use the cache.
         lock_path = cached_features_file + ".lock"
@@ -285,16 +285,16 @@
                 start = time.time()
                 self.features = torch.load(cached_features_file)
                 logger.info(
                     f"Loading features from cached file {cached_features_file} [took %.3f s]", time.time() - start
                 )
             else:
                 corpus_path = os.path.join(
-                    args.downstream_corpus_root_dir,
-                    args.downstream_corpus_name,
+                    args.downstream_data_home,
+                    args.downstream_data_name,
                 )
                 logger.info(f"Creating features from dataset file at {corpus_path}")
                 examples = self.corpus.get_examples(corpus_path, mode)
                 self.features = convert_examples_to_features_fn(
                     examples,
                     tokenizer,
                     args,
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/ner/deploy.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 
     @app.route('/')
     def index():
         return render_template('index.html')
 
     @app.route('/api', methods=['POST'])
     def api():
-        query_sentence = request.json
-        output_data = inference_fn(query_sentence)
+        query = request.json
+        output_data = inference_fn(query["premise"], query["hypothesis"])
         response = jsonify(output_data)
         return response
 
     return app
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/ner/task.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/classification/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from lightning import LightningModule
+from ratsnlp.nlpbook import NLUTrainerArguments
 from ratsnlp.nlpbook.metrics import accuracy
-from ratsnlp.nlpbook.ner import NERTrainArguments, NER_PAD_ID
-from transformers import BertPreTrainedModel
+from transformers import PreTrainedModel
 
 
-class NERTask(LightningModule):
+class ClassificationTask(LightningModule):
 
     def __init__(self,
-                 model: BertPreTrainedModel,
-                 args: NERTrainArguments,
-    ):
+                 model: PreTrainedModel,
+                 args: NLUTrainerArguments,
+                 ):
         super().__init__()
         self.model = model
         self.args = args
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning_rate)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
         return {
             'optimizer': optimizer,
             'scheduler': scheduler,
         }
 
     def training_step(self, inputs, batch_idx):
-        # outputs: TokenClassifierOutput
+        # outputs: SequenceClassifierOutput
         outputs = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
-        acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
+        acc = accuracy(preds, labels)
         self.log("loss", outputs.loss, prog_bar=False, logger=True, on_step=True, on_epoch=False)
         self.log("acc", acc, prog_bar=True, logger=True, on_step=True, on_epoch=False)
         return outputs.loss
 
     def validation_step(self, inputs, batch_idx):
-        # outputs: TokenClassifierOutput
+        # outputs: SequenceClassifierOutput
         outputs = self.model(**inputs)
         preds = outputs.logits.argmax(dim=-1)
         labels = inputs["labels"]
-        acc = accuracy(preds, labels, ignore_index=NER_PAD_ID)
+        acc = accuracy(preds, labels)
         self.log("val_loss", outputs.loss, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         self.log("val_acc", acc, prog_bar=True, logger=True, on_step=False, on_epoch=True)
         return outputs.loss
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/corpus.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/paircls/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/paircls/deploy.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/deploy.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,12 +14,12 @@
     @app.route('/')
     def index():
         return render_template('index.html')
 
     @app.route('/api', methods=['POST'])
     def api():
         query = request.json
-        output_data = inference_fn(query["premise"], query["hypothesis"])
+        output_data = inference_fn(query["question"], query["context"])
         response = jsonify(output_data)
         return response
 
     return app
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/qa/arguments.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/arguments.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/qa/corpus.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/corpus.py`

 * *Files identical despite different names*

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/qa/task.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/qa/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+from pytorch_lightning import LightningModule
 from torch.optim import AdamW
 from torch.optim.lr_scheduler import ExponentialLR
 
-from lightning import LightningModule
 from ratsnlp.nlpbook.metrics import accuracy
 from ratsnlp.nlpbook.qa import QATrainArguments
 from transformers import PreTrainedModel
 
 
 class QATask(LightningModule):
 
     def __init__(self,
                  model: PreTrainedModel,
                  args: QATrainArguments,
-    ):
+                 ):
         super().__init__()
         self.model = model
         self.args = args
 
     def configure_optimizers(self):
         optimizer = AdamW(self.parameters(), lr=self.args.learning_rate)
         scheduler = ExponentialLR(optimizer, gamma=0.9)
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/trainer.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/trainer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 import torch
 
-from lightning import Trainer
-from lightning.pytorch.callbacks import ModelCheckpoint
-from ratsnlp.nlpbook.classification.arguments import ClassificationTrainArguments
+from pytorch_lightning import Trainer
+from pytorch_lightning.callbacks import ModelCheckpoint
+from ratsnlp.nlpbook.arguments import NLUTrainerArguments
 
 
-def get_trainer(args: ClassificationTrainArguments, return_trainer_only=True):
+def get_trainer(args: NLUTrainerArguments, return_trainer_only=True):
     ckpt_path = os.path.abspath(args.downstream_model_home)
     os.makedirs(ckpt_path, exist_ok=True)
     checkpoint_callback = ModelCheckpoint(
         dirpath=ckpt_path,
         filename=args.downstream_model_file,
         save_top_k=args.save_top_k,
         monitor=args.monitor.split()[1],
@@ -19,16 +19,17 @@
     )
     trainer = Trainer(
         max_epochs=args.epochs,
         fast_dev_run=args.test_mode,
         num_sanity_val_steps=None if args.test_mode else 0,
         callbacks=[checkpoint_callback],
         default_root_dir=ckpt_path,
-        # For GPU Setup
         deterministic=torch.cuda.is_available() and args.seed is not None,
-        devices=torch.cuda.device_count() if torch.cuda.is_available() else None,
-        precision=16 if args.fp16 else 32,
+        accelerator=args.accelerator if args.accelerator else None,
+        precision=args.precision if args.precision else 32,
+        strategy=args.strategy if not args.strategy else None,
+        devices=args.devices if not args.devices else None,
     )
     if return_trainer_only:
         return trainer
     else:
         return checkpoint_callback, trainer
```

### Comparing `chrislab-0.4.4/src/ratsnlp/nlpbook/utils.py` & `chrislab-0.5.0a0/src/ratsnlp/nlpbook/utils.py`

 * *Files identical despite different names*

