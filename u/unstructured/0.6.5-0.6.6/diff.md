# Comparing `tmp/unstructured-0.6.5.tar.gz` & `tmp/unstructured-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.5.tar", last modified: Wed May 10 04:48:50 2023, max compression
+gzip compressed data, was "unstructured-0.6.6.tar", last modified: Fri May 12 17:49:05 2023, max compression
```

## Comparing `unstructured-0.6.5.tar` & `unstructured-0.6.6.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-10 04:48:39.000000 unstructured-0.6.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-10 04:48:50.161395 unstructured-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-10 04:48:39.000000 unstructured-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 04:48:50.161395 unstructured-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-10 04:48:39.000000 unstructured-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.157395 unstructured-0.6.5/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-10 04:48:50.000000 unstructured-0.6.5/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.018533 unstructured-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-12 17:48:53.000000 unstructured-0.6.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-12 17:49:05.018533 unstructured-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-12 17:48:53.000000 unstructured-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-12 17:49:05.022533 unstructured-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-12 17:48:53.000000 unstructured-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.994531 unstructured-0.6.6/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.994531 unstructured-0.6.6/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-12 17:48:53.000000 unstructured-0.6.6/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10826 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.002532 unstructured-0.6.6/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.014532 unstructured-0.6.6/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:53.000000 unstructured-0.6.6/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.014532 unstructured-0.6.6/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:05.018533 unstructured-0.6.6/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-12 17:48:54.000000 unstructured-0.6.6/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:49:04.998531 unstructured-0.6.6/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 17:49:04.000000 unstructured-0.6.6/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.5/LICENSE.md` & `unstructured-0.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/PKG-INFO` & `unstructured-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.5
+Version: 0.6.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.5/README.md` & `unstructured-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/setup.py` & `unstructured-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.6/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.6/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/test_unstructured/test_utils.py` & `unstructured-0.6.6/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/cleaners/core.py` & `unstructured-0.6.6/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/cleaners/extract.py` & `unstructured-0.6.6/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/cleaners/translate.py` & `unstructured-0.6.6/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/documents/base.py` & `unstructured-0.6.6/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/documents/elements.py` & `unstructured-0.6.6/unstructured/documents/elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import datetime
 import hashlib
+import os
 import pathlib
 from abc import ABC
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 
 class NoID(ABC):
@@ -30,21 +32,31 @@
     # Text format metadata fields
     text_as_html: Optional[str] = None
 
     def __post_init__(self):
         if isinstance(self.filename, pathlib.Path):
             self.filename = str(self.filename)
 
+        if self.filename is not None:
+            self.filename = os.path.basename(self.filename)
+
     def to_dict(self):
         return {key: value for key, value in self.__dict__.items() if value is not None}
 
     @classmethod
     def from_dict(cls, input_dict):
         return cls(**input_dict)
 
+    def get_date(self) -> Optional[datetime.datetime]:
+        """Converts the date field to a datetime object."""
+        dt = None
+        if self.date is not None:
+            dt = datetime.datetime.fromisoformat(self.date)
+        return dt
+
 
 class Element(ABC):
     """An element is a section of a page in the document."""
 
     def __init__(
         self,
         element_id: Union[str, NoID] = NoID(),
```

### Comparing `unstructured-0.6.5/unstructured/documents/email_elements.py` & `unstructured-0.6.6/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/documents/html.py` & `unstructured-0.6.6/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/documents/xml.py` & `unstructured-0.6.6/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/file_utils/exploration.py` & `unstructured-0.6.6/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.6/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/file_utils/filetype.py` & `unstructured-0.6.6/unstructured/file_utils/filetype.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,27 +348,27 @@
 
     if file is not None:
         file.seek(0)
         file_content = file.read(4096)
         if isinstance(file_content, str):
             file_text = file_content
         else:
-            file_text = file_content.decode()
+            file_text = file_content.decode(errors="ignore")
         file.seek(0)
     elif filename is not None:
         with open(filename) as f:
             file_text = f.read()
 
     return re.match(LIST_OF_DICTS_PATTERN, file_text) is not None
 
 
 def _check_eml_from_buffer(file: IO) -> bool:
     """Checks if a text/plain file is actually a .eml file. Uses a regex pattern to see if the
     start of the file matches the typical pattern for a .eml file."""
     file.seek(0)
     file_content = file.read(4096)
     if isinstance(file_content, bytes):
-        file_head = file_content.decode("utf-8")
+        file_head = file_content.decode("utf-8", errors="ignore")
     else:
         file_head = file_content
 
     return EMAIL_HEAD_RE.match(file_head) is not None
```

### Comparing `unstructured-0.6.5/unstructured/file_utils/metadata.py` & `unstructured-0.6.6/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/azure.py` & `unstructured-0.6.6/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.6/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.6/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/git.py` & `unstructured-0.6.6/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/github.py` & `unstructured-0.6.6/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.6/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.6/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/local.py` & `unstructured-0.6.6/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.6/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/s3.py` & `unstructured-0.6.6/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/slack.py` & `unstructured-0.6.6/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.6/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.6/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/interfaces.py` & `unstructured-0.6.6/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/ingest/main.py` & `unstructured-0.6.6/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/nlp/english-words.txt` & `unstructured-0.6.6/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/nlp/english_words.py` & `unstructured-0.6.6/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/nlp/patterns.py` & `unstructured-0.6.6/unstructured/nlp/patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,19 @@
 # - skipping qa because we need the escape for the regex
 
 # Mapi ID example: 32.88.5467.123
 MAPI_ID_PATTERN = "[0-9]*\.[0-9]*\.[0-9]*\.[0-9]*;"  # noqa: W605 NOTE(harrell)
 # - skipping qa because we need the escape for the regex
 
 # Date, time, timezone example: Fri, 26 Mar 2021 11:04:09 +1200
-EMAIL_DATETIMETZ_PATTERN = "[a-zA-z]{3},\s[0-9]{2}\s[a-zA-Z]{3}\s[0-9]{4}\s[0-9]{2}:[0-9]{2}:[0-9]{2}\s[+0-9]{5}"  # noqa: W605,E501
 # NOTE(harrell) - skipping qa because we need the escape for the regex
+EMAIL_DATETIMETZ_PATTERN = (
+    r"[A-Za-z]{3},\s\d{1,2}\s[A-Za-z]{3}\s\d{4}\s\d{2}:\d{2}:\d{2}\s[+-]\d{4}"  # noqa: W605,E501
+)
+EMAIL_DATETIMETZ_PATTERN_RE = re.compile(EMAIL_DATETIMETZ_PATTERN)
 
 EMAIL_ADDRESS_PATTERN = "[a-z0-9\.\-+_]+@[a-z0-9\.\-+_]+\.[a-z]+"  # noqa: W605 NOTE(harrell)
 # - skipping qa because we need the escape for the regex
 
 
 ENDS_IN_PUNCT_PATTERN = r"[^\w\s]\Z"
 ENDS_IN_PUNCT_RE = re.compile(ENDS_IN_PUNCT_PATTERN)
```

### Comparing `unstructured-0.6.5/unstructured/nlp/tokenize.py` & `unstructured-0.6.6/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/__init__.py` & `unstructured-0.6.6/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/api.py` & `unstructured-0.6.6/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/auto.py` & `unstructured-0.6.6/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/common.py` & `unstructured-0.6.6/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/doc.py` & `unstructured-0.6.6/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/docx.py` & `unstructured-0.6.6/unstructured/partition/docx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os
 import tempfile
 from tempfile import SpooledTemporaryFile
 from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import docx
 import pypandoc
+from docx.oxml.shared import qn
+from docx.text.paragraph import Paragraph
+from docx.text.run import Run
+from tabulate import tabulate
 
 from unstructured.cleaners.core import clean_bullets
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
+    Table,
     Text,
     Title,
 )
 from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
@@ -57,14 +62,43 @@
     "Quote": Text,  # TODO(robinson) - add quote element type
     "Subtitle": Title,
     "TOCHeading": Title,
     "Title": Title,
 }
 
 
+def _get_paragraph_runs(paragraph):
+    """
+    Get hyperlink text from a paragraph object.
+    Without this, the default runs function skips over hyperlinks.
+
+    Args:
+        paragraph (Paragraph): A Paragraph object.
+
+    Returns:
+        list: A list of Run objects.
+    """
+
+    # Recursively get runs.
+    def _get_runs(node, parent):
+        for child in node:
+            # If the child is a run, yield a Run object
+            if child.tag == qn("w:r"):
+                yield Run(child, parent)
+            # If the child is a hyperlink, search for runs within it recursively
+            if child.tag == qn("w:hyperlink"):
+                yield from _get_runs(child, parent)
+
+    return list(_get_runs(paragraph._element, paragraph))
+
+
+# Add the runs property to the Paragraph class
+Paragraph.runs = property(lambda self: _get_paragraph_runs(self))
+
+
 def partition_docx(
     filename: Optional[str] = None,
     file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
@@ -88,23 +122,55 @@
     elif file is not None:
         document = docx.Document(
             spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file)),
         )
 
     metadata_filename = metadata_filename or filename
     elements: List[Element] = []
-    for paragraph in document.paragraphs:
-        element = _paragraph_to_element(paragraph)
-        if element is not None:
-            element.metadata = ElementMetadata(filename=metadata_filename)
-            elements.append(element)
+    table_index = 0
+
+    for element_item in document.element.body:
+        if element_item.tag.endswith("tbl"):
+            table = document.tables[table_index]
+            html_table = _convert_table_to_text(table, as_html=True)
+            text_table = _convert_table_to_text(table, as_html=False)
+            element = Table(text_table)
+            if element is not None:
+                element.metadata = ElementMetadata(filename=metadata_filename)
+                element.metadata = ElementMetadata(text_as_html=html_table)
+                elements.append(element)
+            table_index += 1
+        elif element_item.tag.endswith("p"):
+            paragraph = docx.text.paragraph.Paragraph(element_item, document)
+            para_element: Optional[Text] = _paragraph_to_element(paragraph)
+            if para_element is not None:
+                para_element.metadata = ElementMetadata(filename=metadata_filename)
+                elements.append(para_element)
 
     return elements
 
 
+def _convert_table_to_text(table, as_html):
+    """
+    Convert a table object from a Word document to an HTML table string using the tabulate library.
+
+    Args:
+        table (Table): A Table object.
+        as_html (bool): Whether to return the table as an HTML string (True) or a
+            plain text string (False)
+
+    Returns:
+        str: An table string representation of the input table.
+    """
+    fmt = "html" if as_html else "plain"
+    headers = [cell.text for cell in table.rows[0].cells]
+    data = [[cell.text for cell in row.cells] for row in table.rows[1:]]
+    return tabulate(data, headers=headers, tablefmt=fmt)
+
+
 def _paragraph_to_element(paragraph: docx.text.paragraph.Paragraph) -> Optional[Text]:
     """Converts a docx Paragraph object into the appropriate unstructured document element.
     If the paragraph style is "Normal" or unknown, we try to predict the element type from the
     raw text."""
     text = paragraph.text
     style_name = paragraph.style and paragraph.style.name  # .style can be None
```

### Comparing `unstructured-0.6.5/unstructured/partition/email.py` & `unstructured-0.6.6/unstructured/partition/email.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 from unstructured.documents.email_elements import (
     MetaData,
     ReceivedInfo,
     Recipient,
     Sender,
     Subject,
 )
+from unstructured.logger import logger
+from unstructured.nlp.patterns import EMAIL_DATETIMETZ_PATTERN_RE
 from unstructured.partition.html import partition_html
 from unstructured.partition.text import partition_text, split_by_paragraph
 
 VALID_CONTENT_SOURCES: Final[List[str]] = ["text/html", "text/plain"]
 
 
 def _parse_received_data(data: str) -> List[Element]:
@@ -85,15 +87,15 @@
             elements += _parse_received_data(item[1])
         else:
             elements.append(MetaData(name=item[0], text=item[1]))
 
     return elements
 
 
-def build_email_metadata(msg: Message) -> ElementMetadata:
+def build_email_metadata(msg: Message, filename: Optional[str]) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the email."""
     header_dict = dict(msg.raw_items())
     email_date = header_dict.get("Date")
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = header_dict.get("To")
@@ -105,20 +107,29 @@
         sent_to = [recipient.strip() for recipient in sent_to.split(",")]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=header_dict.get("Subject"),
         date=email_date,
+        filename=filename,
     )
 
 
-def convert_to_iso_8601(time: str) -> str:
+def convert_to_iso_8601(time: str) -> Optional[str]:
     """Converts the datetime from the email output to ISO-8601 format."""
-    datetime_object = datetime.datetime.strptime(time, "%a, %d %b %Y %H:%M:%S %z")
+    cleaned_time = clean_extra_whitespace(time)
+    regex_match = EMAIL_DATETIMETZ_PATTERN_RE.search(cleaned_time)
+    if regex_match is None:
+        logger.warning(f"{time} did not match RFC-2822 format. Unable to extract the time.")
+        return None
+
+    start, end = regex_match.span()
+    dt_string = cleaned_time[start:end]
+    datetime_object = datetime.datetime.strptime(dt_string, "%a, %d %b %Y %H:%M:%S %z")
     return datetime_object.isoformat()
 
 
 def extract_attachment_info(
     message: Message,
     output_dir: Optional[str] = None,
 ) -> List[Dict[str, str]]:
@@ -264,12 +275,11 @@
             elements.insert(idx + 1, image_info)
 
     header: List[Element] = []
     if include_headers:
         header = partition_email_header(msg)
     all_elements = header + elements
 
-    metadata = build_email_metadata(msg)
-    metadata.filename = filename
+    metadata = build_email_metadata(msg, filename=filename)
     for element in all_elements:
         element.metadata = metadata
     return all_elements
```

### Comparing `unstructured-0.6.5/unstructured/partition/epub.py` & `unstructured-0.6.6/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/html.py` & `unstructured-0.6.6/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/image.py` & `unstructured-0.6.6/unstructured/partition/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     filename: str = "",
     file: Optional[bytes] = None,
     url: Optional[str] = None,
     template: Optional[str] = None,
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
-    strategy: str = "hi_res",
+    strategy: str = "auto",
 ) -> List[Element]:
     """Parses an image into a list of interpreted elements.
 
     Parameters
     ----------
     filename
         A string defining the target filename path.
```

### Comparing `unstructured-0.6.5/unstructured/partition/json.py` & `unstructured-0.6.6/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/md.py` & `unstructured-0.6.6/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/msg.py` & `unstructured-0.6.6/unstructured/partition/msg.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,23 +35,22 @@
 
     text = msg_obj.body
     if "<html>" in text or "</div>" in text:
         elements = partition_html(text=text)
     else:
         elements = partition_text(text=text)
 
-    metadata = build_msg_metadata(msg_obj)
-    metadata.filename = filename
+    metadata = build_msg_metadata(msg_obj, filename)
     for element in elements:
         element.metadata = metadata
 
     return elements
 
 
-def build_msg_metadata(msg_obj: msg_parser.MsOxMessage) -> ElementMetadata:
+def build_msg_metadata(msg_obj: msg_parser.MsOxMessage, filename: Optional[str]) -> ElementMetadata:
     """Creates an ElementMetadata object from the header information in the emai."""
     email_date = getattr(msg_obj, "sent_date", None)
     if email_date is not None:
         email_date = convert_to_iso_8601(email_date)
 
     sent_from = getattr(msg_obj, "sender", None)
     if sent_from is not None:
@@ -62,14 +61,15 @@
         sent_to = [str(recipient) for recipient in sent_to]
 
     return ElementMetadata(
         sent_to=sent_to,
         sent_from=sent_from,
         subject=getattr(msg_obj, "subject", None),
         date=email_date,
+        filename=filename,
     )
 
 
 def extract_msg_attachment_info(
     filename: str,
     file: Optional[IO] = None,
     output_dir: Optional[str] = None,
```

### Comparing `unstructured-0.6.5/unstructured/partition/odt.py` & `unstructured-0.6.6/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/pdf.py` & `unstructured-0.6.6/unstructured/partition/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def partition_pdf(
     filename: str = "",
     file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
-    strategy: str = "hi_res",
+    strategy: str = "auto",
     infer_table_structure: bool = False,
     encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf document into a list of interpreted elements.
     Parameters
     ----------
@@ -90,15 +90,15 @@
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = "https://ml.unstructured.io/",
     template: str = "layout/pdf",
     token: Optional[str] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
-    strategy: str = "hi_res",
+    strategy: str = "auto",
     infer_table_structure: bool = False,
     encoding: str = "utf-8",
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Parses a pdf or image document into a list of interpreted elements."""
     if url is None:
         # TODO(alan): Extract information about the filetype to be processed from the template
@@ -112,14 +112,15 @@
             out_template = None
 
         strategy = determine_pdf_or_image_strategy(
             strategy,
             filename=filename,
             file=file,
             is_image=is_image,
+            infer_table_structure=infer_table_structure,
         )
 
         if strategy == "hi_res":
             # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
```

### Comparing `unstructured-0.6.5/unstructured/partition/ppt.py` & `unstructured-0.6.6/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/pptx.py` & `unstructured-0.6.6/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/rtf.py` & `unstructured-0.6.6/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/strategies.py` & `unstructured-0.6.6/unstructured/partition/strategies.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 from pdfminer.utils import open_filename
 
 from unstructured.logger import logger
 from unstructured.partition.common import exactly_one
 from unstructured.utils import dependency_exists
 
 VALID_STRATEGIES: Dict[str, List[str]] = {
+    "auto": [
+        "pdf",
+        "image",
+    ],
     "hi_res": [
         "pdf",
         "image",
     ],
     "ocr_only": [
         "pdf",
         "image",
@@ -58,27 +62,37 @@
 
 
 def determine_pdf_or_image_strategy(
     strategy: str,
     filename: str = "",
     file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
+    infer_table_structure: bool = False,
 ):
     """Determines what strategy to use for processing PDFs or images, accounting for fallback
     logic if some dependencies are not available."""
     pytesseract_installed = dependency_exists("pytesseract")
     detectron2_installed = dependency_exists("detectron2")
 
     if is_image:
         validate_strategy(strategy, "image")
         pdf_text_extractable = False
     else:
         validate_strategy(strategy, "pdf")
         pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
 
+    if strategy == "auto":
+        if is_image:
+            strategy = _determine_image_auto_strategy(infer_table_structure=infer_table_structure)
+        else:
+            strategy = _determine_pdf_auto_strategy(
+                pdf_text_extractable=pdf_text_extractable,
+                infer_table_structure=infer_table_structure,
+            )
+
     if file is not None:
         file.seek(0)  # type: ignore
 
     if all([not detectron2_installed, not pytesseract_installed, not pdf_text_extractable]):
         raise ValueError(
             "detectron2 is not installed, pytesseract is not installed "
             "and the text of the PDF is not extractable. "
@@ -117,7 +131,33 @@
             logger.warning("Falling back to partitioning with fast.")
             return "fast"
         else:
             logger.warning("Falling back to partitioning with hi_res.")
             return "hi_res"
 
     return strategy
+
+
+def _determine_image_auto_strategy(infer_table_structure: bool = False):
+    """If "auto" is passed in as the strategy, determines what strategy to use
+    for images."""
+    if infer_table_structure is True:
+        return "hi_res"
+    else:
+        return "ocr_only"
+
+
+def _determine_pdf_auto_strategy(
+    pdf_text_extractable: bool = True,
+    infer_table_structure: bool = False,
+):
+    """If "auto" is passed in as the strategy, determines what strategy to use
+    for PDFs."""
+    # NOTE(robinson) - Currrently "hi_res" is the only stategy where
+    # infer_table_structure is used.
+    if infer_table_structure:
+        return "hi_res"
+
+    if pdf_text_extractable:
+        return "fast"
+    else:
+        return "ocr_only"
```

### Comparing `unstructured-0.6.5/unstructured/partition/text.py` & `unstructured-0.6.6/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/partition/text_type.py` & `unstructured-0.6.6/unstructured/partition/text_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final  # pragma: nocover
 else:
     from typing import Final
 
 from unstructured.cleaners.core import remove_punctuation
-from unstructured.logger import logger
+from unstructured.logger import trace_logger
 from unstructured.nlp.english_words import ENGLISH_WORDS
 from unstructured.nlp.patterns import (
     ENDS_IN_PUNCT_RE,
     UNICODE_BULLETS_RE,
     US_CITY_STATE_ZIP_RE,
     US_PHONE_NUMBERS_RE,
 )
@@ -53,42 +53,42 @@
         accurate partitioning and off for faster processing.
     """
     _language_checks = os.environ.get("UNSTRUCTURED_LANGUAGE_CHECKS")
     if _language_checks is not None:
         language_checks = _language_checks.lower() == "true"
 
     if len(text) == 0:
-        logger.debug("Not narrative. Text is empty.")
+        trace_logger.detail("Not narrative. Text is empty.")  # type: ignore
         return False
 
     if text.isnumeric():
-        logger.debug(f"Not narrative. Text is all numeric:\n\n{text}")
+        trace_logger.detail(f"Not narrative. Text is all numeric:\n\n{text}")  # type: ignore
         return False
 
     language = os.environ.get("UNSTRUCTURED_LANGUAGE", language)
     if language == "en" and language_checks and not contains_english_word(text):
         return False
 
     # NOTE(robinson): it gets read in from the environment as a string so we need to
     # cast it to a float
     cap_threshold = float(
         os.environ.get("UNSTRUCTURED_NARRATIVE_TEXT_CAP_THRESHOLD", cap_threshold),
     )
     if exceeds_cap_ratio(text, threshold=cap_threshold):
-        logger.debug(f"Not narrative. Text exceeds cap ratio {cap_threshold}:\n\n{text}")
+        trace_logger.detail(f"Not narrative. Text exceeds cap ratio {cap_threshold}:\n\n{text}")  # type: ignore # noqa: E501
         return False
 
     non_alpha_threshold = float(
         os.environ.get("UNSTRUCTURED_NARRATIVE_TEXT_NON_ALPHA_THRESHOLD", non_alpha_threshold),
     )
     if under_non_alpha_ratio(text, threshold=non_alpha_threshold):
         return False
 
     if (sentence_count(text, 3) < 2) and (not contains_verb(text)) and language == "en":
-        logger.debug(f"Not narrative. Text does not contain a verb:\n\n{text}")
+        trace_logger.detail(f"Not narrative. Text does not contain a verb:\n\n{text}")  # type: ignore # noqa: E501
         return False
 
     return True
 
 
 def is_possible_title(
     text: str,
@@ -117,15 +117,15 @@
         accurate partitioning and off for faster processing.
     """
     _language_checks = os.environ.get("UNSTRUCTURED_LANGUAGE_CHECKS")
     if _language_checks is not None:
         language_checks = _language_checks.lower() == "true"
 
     if len(text) == 0:
-        logger.debug("Not a title. Text is empty.")
+        trace_logger.detail("Not a title. Text is empty.")  # type: ignore
         return False
 
     if text.isupper() and ENDS_IN_PUNCT_RE.search(text) is not None:
         return False
 
     title_max_word_length = int(
         os.environ.get("UNSTRUCTURED_TITLE_MAX_WORD_LENGTH", title_max_word_length),
@@ -146,22 +146,24 @@
         return False
 
     language = os.environ.get("UNSTRUCTURED_LANGUAGE", language)
     if language == "en" and not contains_english_word(text) and language_checks:
         return False
 
     if text.isnumeric():
-        logger.debug(f"Not a title. Text is all numeric:\n\n{text}")
+        trace_logger.detail(f"Not a title. Text is all numeric:\n\n{text}")  # type: ignore
         return False
 
     # NOTE(robinson) - The min length is to capture content such as "ITEM 1A. RISK FACTORS"
     # that sometimes get tokenized as separate sentences due to the period, but are still
     # valid titles
     if sentence_count(text, min_length=sentence_min_length) > 1:
-        logger.debug(f"Not a title. Text is longer than {sentence_min_length} sentences:\n\n{text}")
+        trace_logger.detail(  # type: ignore
+            f"Not a title. Text is longer than {sentence_min_length} sentences:\n\n{text}",
+        )
         return False
 
     return True
 
 
 def is_bulleted_text(text: str) -> bool:
     """Checks to see if the section of text is part of a bulleted list."""
@@ -219,15 +221,15 @@
     """
     sentences = sent_tokenize(text)
     count = 0
     for sentence in sentences:
         sentence = remove_punctuation(sentence)
         words = [word for word in word_tokenize(sentence) if word != "."]
         if min_length and len(words) < min_length:
-            logger.debug(
+            trace_logger.detail(  # type: ignore
                 f"Skipping sentence because does not exceed {min_length} word tokens\n"
                 f"{sentence}",
             )
             continue
         count += 1
     return count
```

### Comparing `unstructured-0.6.5/unstructured/staging/argilla.py` & `unstructured-0.6.6/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/base.py` & `unstructured-0.6.6/unstructured/staging/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,27 +18,31 @@
     "type",
     "text",
     "element_id",
     "coordinates",
     "filename",
     "page_number",
     "url",
+    "sent_from",
+    "sent_to",
+    "subject",
+    "sender",
 ]
 
 
-def convert_to_isd(elements: List[Element]) -> List[Dict[str, str]]:
+def convert_to_isd(elements: List[Element]) -> List[Dict[str, Any]]:
     """Represents the document elements as an Initial Structured Document (ISD)."""
     isd: List[Dict[str, str]] = []
     for element in elements:
         section = element.to_dict()
         isd.append(section)
     return isd
 
 
-def convert_to_dict(elements: List[Element]) -> List[Dict[str, str]]:
+def convert_to_dict(elements: List[Element]) -> List[Dict[str, Any]]:
     """Converts a list of elements into a dictionary."""
     return convert_to_isd(elements)
 
 
 def elements_to_json(
     elements: List[Element],
     filename: Optional[str] = None,
@@ -123,14 +127,19 @@
     # NOTE(robinson) - flatten metadata and add it to the table
     for row in rows:
         metadata = row.pop("metadata")
         for key, value in metadata.items():
             if key in TABLE_FIELDNAMES:
                 row[key] = value
 
+        if row.get("sent_from"):
+            row["sender"] = row.get("sent_from")
+            if type(row["sender"]) == list:
+                row["sender"] = row["sender"][0]
+
     with io.StringIO() as buffer:
         csv_writer = csv.DictWriter(buffer, fieldnames=TABLE_FIELDNAMES)
         csv_writer.writeheader()
         csv_writer.writerows(rows)
         return buffer.getvalue()
```

### Comparing `unstructured-0.6.5/unstructured/staging/baseplate.py` & `unstructured-0.6.6/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/datasaur.py` & `unstructured-0.6.6/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/huggingface.py` & `unstructured-0.6.6/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/label_box.py` & `unstructured-0.6.6/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/label_studio.py` & `unstructured-0.6.6/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/staging/prodigy.py` & `unstructured-0.6.6/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured/utils.py` & `unstructured-0.6.6/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.5/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.6/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.5
+Version: 0.6.6
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.5 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.6 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.5/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.6/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

