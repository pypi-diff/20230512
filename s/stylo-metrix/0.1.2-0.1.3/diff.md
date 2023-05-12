# Comparing `tmp/stylo_metrix-0.1.2.tar.gz` & `tmp/stylo_metrix-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stylo_metrix-0.1.2.tar", last modified: Mon May  8 07:21:30 2023, max compression
+gzip compressed data, was "stylo_metrix-0.1.3.tar", last modified: Fri May 12 08:34:41 2023, max compression
```

## Comparing `stylo_metrix-0.1.2.tar` & `stylo_metrix-0.1.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.600842 stylo_metrix-0.1.2/
--rw-rw-rw-   0        0        0    33095 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/LICENSE
--rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6790 2023-05-08 07:21:30.600842 stylo_metrix-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6307 2023-04-21 09:43:18.000000 stylo_metrix-0.1.2/README.md
--rw-rw-rw-   0        0        0      772 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      798 2023-05-08 07:21:30.600842 stylo_metrix-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:29.982940 stylo_metrix-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.074029 stylo_metrix-0.1.2/src/stylo_metrix/
--rw-rw-rw-   0        0        0      861 2023-05-04 07:11:21.000000 stylo_metrix-0.1.2/src/stylo_metrix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.122202 stylo_metrix-0.1.2/src/stylo_metrix/metrics/
--rw-rw-rw-   0        0        0      758 2023-03-15 13:04:26.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.215032 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/
--rw-rw-rw-   0        0        0     1157 2023-03-10 20:11:10.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/__init__.py
--rw-rw-rw-   0        0        0     5113 2023-03-15 13:30:46.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/distance_en.py
--rw-rw-rw-   0        0        0     1971 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/figures_of_speech.py
--rw-rw-rw-   0        0        0    13569 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/grammatical_forms.py
--rw-rw-rw-   0        0        0    16796 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/lexical_en.py
--rw-rw-rw-   0        0        0     4081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/parts_of_speech_en.py
--rw-rw-rw-   0        0        0     4464 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/psycholinguistics.py
--rw-rw-rw-   0        0        0     8324 2023-03-29 12:59:55.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/social_media.py
--rw-rw-rw-   0        0        0     7885 2023-03-29 12:59:55.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/syntactic_en.py
--rw-rw-rw-   0        0        0     4223 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/text_statistics.py
--rw-rw-rw-   0        0        0    12004 2023-04-06 13:12:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/verb_tenses_en.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.280084 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/
--rw-rw-rw-   0        0        0     1059 2023-03-10 19:52:40.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/descriptive.py
--rw-rw-rw-   0        0        0     5229 2023-04-06 13:10:29.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/grammatical_forms.py
--rw-rw-rw-   0        0        0     1336 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/graphical.py
--rw-rw-rw-   0        0        0    19983 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/inflection.py
--rw-rw-rw-   0        0        0     6373 2023-03-10 20:11:05.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/lexical.py
--rw-rw-rw-   0        0        0     6066 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/psycholinguistic.py
--rw-rw-rw-   0        0        0     2330 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/punctuation.py
--rw-rw-rw-   0        0        0     7377 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/syntactic.py
--rw-rw-rw-   0        0        0     5788 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/word_formation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.314781 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/
--rw-rw-rw-   0        0        0      944 2023-03-15 13:04:46.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/__init__.py
--rw-rw-rw-   0        0        0    17631 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/lexical_ukr.py
--rw-rw-rw-   0        0        0     4040 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py
--rw-rw-rw-   0        0        0     6598 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/syntactic_ukr.py
--rw-rw-rw-   0        0        0    10724 2023-03-28 08:06:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/verb_forms_ukr.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.330160 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/
--rw-rw-rw-   0        0        0       23 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.397264 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/
--rw-rw-rw-   0        0        0      987 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/custom_preprocessing.py
--rw-rw-rw-   0        0        0     8872 2023-03-10 19:46:18.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/dictionary_en.py
--rw-rw-rw-   0        0        0    44832 2023-04-06 13:12:03.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/grammar.py
--rw-rw-rw-   0        0        0     1909 2023-03-10 19:53:28.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/params.py
--rw-rw-rw-   0        0        0     3065 2023-03-29 12:59:55.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/pos_tagger.py
--rw-rw-rw-   0        0        0     3402 2023-03-10 19:46:18.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/psycholinguistics.py
--rw-rw-rw-   0        0        0     5020 2023-03-29 12:59:55.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/stylistic.py
--rw-rw-rw-   0        0        0     2321 2023-05-08 07:18:39.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/new_pipe.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.446749 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/
--rw-rw-rw-   0        0        0     1206 2023-03-15 11:55:34.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/__init__.py
--rw-rw-rw-   0        0        0     2213 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/matcher_component.py
--rw-rw-rw-   0        0        0     1931 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/params.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.474539 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/__init__.py
--rw-rw-rw-   0        0        0     4284 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py
--rw-rw-rw-   0        0        0     6232 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/pos.py
--rw-rw-rw-   0        0        0     3892 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pos_tagger.py
--rw-rw-rw-   0        0        0     1286 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/psycholinguistic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.489442 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/resources/
--rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/resources/__init__.py
--rw-rw-rw-   0        0        0   290924 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/resources/experimental_data.py
--rw-rw-rw-   0        0        0     1155 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/sentence_segmenter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.549335 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/
--rw-rw-rw-   0        0        0      833 2023-03-15 11:56:59.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/__init__.py
--rw-rw-rw-   0        0        0      386 2023-03-15 10:11:22.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/custom_preprocessing.py
--rw-rw-rw-   0        0        0     1128 2023-03-15 10:11:22.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/dictionary_ukr.py
--rw-rw-rw-   0        0        0     4715 2023-03-15 10:11:22.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/grammar_ukr.py
--rw-rw-rw-   0        0        0     1753 2023-03-15 10:11:22.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/params.py
--rw-rw-rw-   0        0        0     2232 2023-03-15 10:11:22.000000 stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.584866 stylo_metrix-0.1.2/src/stylo_metrix/structures/
--rw-rw-rw-   0        0        0      812 2023-03-10 19:12:54.000000 stylo_metrix-0.1.2/src/stylo_metrix/structures/__init__.py
--rw-rw-rw-   0        0        0     3184 2023-03-10 19:54:10.000000 stylo_metrix-0.1.2/src/stylo_metrix/structures/category.py
--rw-rw-rw-   0        0        0     2826 2023-03-10 19:54:30.000000 stylo_metrix-0.1.2/src/stylo_metrix/structures/language.py
--rw-rw-rw-   0        0        0     2691 2023-03-10 19:54:39.000000 stylo_metrix-0.1.2/src/stylo_metrix/structures/metric.py
--rw-rw-rw-   0        0        0     2575 2023-04-27 12:52:00.000000 stylo_metrix-0.1.2/src/stylo_metrix/structures/metrics_group.py
--rw-rw-rw-   0        0        0     3856 2023-05-08 07:11:31.000000 stylo_metrix-0.1.2/src/stylo_metrix/stylo_metrix.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.600842 stylo_metrix-0.1.2/src/stylo_metrix/tools/
--rw-rw-rw-   0        0        0       26 2023-03-10 19:46:18.000000 stylo_metrix-0.1.2/src/stylo_metrix/tools/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-05-08 07:02:40.000000 stylo_metrix-0.1.2/src/stylo_metrix/tools/metric_tools.py
--rw-rw-rw-   0        0        0     2175 2023-03-10 19:48:40.000000 stylo_metrix-0.1.2/src/stylo_metrix/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 07:21:30.114186 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/
--rw-rw-rw-   0        0        0     6790 2023-05-08 07:21:29.000000 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3067 2023-05-08 07:21:29.000000 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 07:21:29.000000 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-05-08 07:21:29.000000 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 07:21:29.000000 stylo_metrix-0.1.2/src/stylo_metrix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.119612 stylo_metrix-0.1.3/
+-rw-rw-rw-   0        0        0    33095 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6790 2023-05-12 08:34:41.119612 stylo_metrix-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6307 2023-04-21 09:43:18.000000 stylo_metrix-0.1.3/README.md
+-rw-rw-rw-   0        0        0      772 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      798 2023-05-12 08:34:41.122606 stylo_metrix-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.833444 stylo_metrix-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.867246 stylo_metrix-0.1.3/src/stylo_metrix/
+-rw-rw-rw-   0        0        0      868 2023-05-12 07:54:40.000000 stylo_metrix-0.1.3/src/stylo_metrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.893380 stylo_metrix-0.1.3/src/stylo_metrix/metrics/
+-rw-rw-rw-   0        0        0      758 2023-03-15 13:04:26.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.927703 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/
+-rw-rw-rw-   0        0        0     1157 2023-03-10 20:11:10.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/__init__.py
+-rw-rw-rw-   0        0        0     5113 2023-03-15 13:30:46.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/distance_en.py
+-rw-rw-rw-   0        0        0     1971 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/figures_of_speech.py
+-rw-rw-rw-   0        0        0    13569 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/grammatical_forms.py
+-rw-rw-rw-   0        0        0    16796 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/lexical_en.py
+-rw-rw-rw-   0        0        0     4081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/parts_of_speech_en.py
+-rw-rw-rw-   0        0        0     4464 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/psycholinguistics.py
+-rw-rw-rw-   0        0        0     8324 2023-03-29 12:59:55.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/social_media.py
+-rw-rw-rw-   0        0        0     7885 2023-03-29 12:59:55.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/syntactic_en.py
+-rw-rw-rw-   0        0        0     4223 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/text_statistics.py
+-rw-rw-rw-   0        0        0    12004 2023-04-06 13:12:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/verb_tenses_en.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.963037 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/
+-rw-rw-rw-   0        0        0     1059 2023-03-10 19:52:40.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/__init__.py
+-rw-rw-rw-   0        0        0     2997 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/descriptive.py
+-rw-rw-rw-   0        0        0     5229 2023-04-06 13:10:29.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/grammatical_forms.py
+-rw-rw-rw-   0        0        0     1336 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/graphical.py
+-rw-rw-rw-   0        0        0    19983 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/inflection.py
+-rw-rw-rw-   0        0        0     6373 2023-03-10 20:11:05.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/lexical.py
+-rw-rw-rw-   0        0        0     6066 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/psycholinguistic.py
+-rw-rw-rw-   0        0        0     2330 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/punctuation.py
+-rw-rw-rw-   0        0        0     7377 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/syntactic.py
+-rw-rw-rw-   0        0        0     5788 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/word_formation.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.986342 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/
+-rw-rw-rw-   0        0        0      944 2023-03-15 13:04:46.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/__init__.py
+-rw-rw-rw-   0        0        0    17631 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/lexical_ukr.py
+-rw-rw-rw-   0        0        0     4040 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py
+-rw-rw-rw-   0        0        0     6598 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/syntactic_ukr.py
+-rw-rw-rw-   0        0        0    10724 2023-03-28 08:06:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/verb_forms_ukr.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.997341 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/
+-rw-rw-rw-   0        0        0       23 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.029648 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/
+-rw-rw-rw-   0        0        0      987 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/custom_preprocessing.py
+-rw-rw-rw-   0        0        0     8872 2023-03-10 19:46:18.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/dictionary_en.py
+-rw-rw-rw-   0        0        0    44832 2023-04-06 13:12:03.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/grammar.py
+-rw-rw-rw-   0        0        0     1909 2023-03-10 19:53:28.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/params.py
+-rw-rw-rw-   0        0        0     3065 2023-03-29 12:59:55.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/pos_tagger.py
+-rw-rw-rw-   0        0        0     3402 2023-03-10 19:46:18.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/psycholinguistics.py
+-rw-rw-rw-   0        0        0     5020 2023-03-29 12:59:55.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/stylistic.py
+-rw-rw-rw-   0        0        0     2937 2023-05-12 08:33:10.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/new_pipe.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.051958 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/
+-rw-rw-rw-   0        0        0     1206 2023-03-15 11:55:34.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/__init__.py
+-rw-rw-rw-   0        0        0     2213 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/matcher_component.py
+-rw-rw-rw-   0        0        0     1931 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/params.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.062957 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/__init__.py
+-rw-rw-rw-   0        0        0     4284 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py
+-rw-rw-rw-   0        0        0     6232 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/pos.py
+-rw-rw-rw-   0        0        0     3892 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pos_tagger.py
+-rw-rw-rw-   0        0        0     1286 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/psycholinguistic.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.067132 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-15 12:10:08.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/resources/__init__.py
+-rw-rw-rw-   0        0        0   290924 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/resources/experimental_data.py
+-rw-rw-rw-   0        0        0     1155 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/sentence_segmenter.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.094304 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/
+-rw-rw-rw-   0        0        0      833 2023-03-15 11:56:59.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-03-15 10:11:22.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/custom_preprocessing.py
+-rw-rw-rw-   0        0        0     1128 2023-03-15 10:11:22.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/dictionary_ukr.py
+-rw-rw-rw-   0        0        0     4715 2023-03-15 10:11:22.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/grammar_ukr.py
+-rw-rw-rw-   0        0        0     1753 2023-03-15 10:11:22.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/params.py
+-rw-rw-rw-   0        0        0     2232 2023-03-15 10:11:22.000000 stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.100463 stylo_metrix-0.1.3/src/stylo_metrix/structures/
+-rw-rw-rw-   0        0        0      812 2023-03-10 19:12:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/structures/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-03-10 19:54:10.000000 stylo_metrix-0.1.3/src/stylo_metrix/structures/category.py
+-rw-rw-rw-   0        0        0     2826 2023-03-10 19:54:30.000000 stylo_metrix-0.1.3/src/stylo_metrix/structures/language.py
+-rw-rw-rw-   0        0        0     2691 2023-03-10 19:54:39.000000 stylo_metrix-0.1.3/src/stylo_metrix/structures/metric.py
+-rw-rw-rw-   0        0        0     2575 2023-04-27 12:52:00.000000 stylo_metrix-0.1.3/src/stylo_metrix/structures/metrics_group.py
+-rw-rw-rw-   0        0        0     4505 2023-05-12 08:33:54.000000 stylo_metrix-0.1.3/src/stylo_metrix/stylo_metrix.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:41.117607 stylo_metrix-0.1.3/src/stylo_metrix/tools/
+-rw-rw-rw-   0        0        0       26 2023-03-10 19:46:18.000000 stylo_metrix-0.1.3/src/stylo_metrix/tools/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-05-08 07:02:40.000000 stylo_metrix-0.1.3/src/stylo_metrix/tools/metric_tools.py
+-rw-rw-rw-   0        0        0     2175 2023-03-10 19:48:40.000000 stylo_metrix-0.1.3/src/stylo_metrix/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:34:40.890380 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/
+-rw-rw-rw-   0        0        0     6790 2023-05-12 08:34:40.000000 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3067 2023-05-12 08:34:40.000000 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 08:34:40.000000 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-05-12 08:34:40.000000 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-12 08:34:40.000000 stylo_metrix-0.1.3/src/stylo_metrix.egg-info/top_level.txt
```

### Comparing `stylo_metrix-0.1.2/LICENSE` & `stylo_metrix-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/PKG-INFO` & `stylo_metrix-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylo_metrix
-Version: 0.1.2
+Version: 0.1.3
 Summary: StyloMetrix tool
 Home-page: https://github.com/ZILiAT-NASK/StyloMetrix
 Author: ZILiAT-NASK, Adam Nowakowski
 Author-email: adam.nowakowski@nask.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stylo_metrix Version: 0.1.2 Summary: StyloMetrix
+Metadata-Version: 2.1 Name: stylo_metrix Version: 0.1.3 Summary: StyloMetrix
 tool Home-page: https://github.com/ZILiAT-NASK/StyloMetrix Author: ZILiAT-NASK,
 Adam Nowakowski Author-email: adam.nowakowski@nask.pl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # StyloMetrix [StyloMetrix][NASK] ZakÅad InÅ¼ynierii Lingwistycznej i
 Anailzy Tekstu, NASK PIB ## ð Quick ð¡ Stylometry tool in beta version for
```

### Comparing `stylo_metrix-0.1.2/README.md` & `stylo_metrix-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/pyproject.toml` & `stylo_metrix-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/setup.cfg` & `stylo_metrix-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7479 6c6f 5f6d 6574 7269 780d   = stylo_metrix.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e32  .version = 0.1.2
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e33  .version = 0.1.3
 00000030: 0d0a 6175 7468 6f72 203d 205a 494c 6941  ..author = ZILiA
 00000040: 542d 4e41 534b 2c20 4164 616d 204e 6f77  T-NASK, Adam Now
 00000050: 616b 6f77 736b 690d 0a61 7574 686f 725f  akowski..author_
 00000060: 656d 6169 6c20 3d20 6164 616d 2e6e 6f77  email = adam.now
 00000070: 616b 6f77 736b 6940 6e61 736b 2e70 6c0d  akowski@nask.pl.
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2053  .description = S
 00000090: 7479 6c6f 4d65 7472 6978 2074 6f6f 6c0d  tyloMetrix tool.
```

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .stylo_metrix import StyloMetrix
 from .tools.metric_tools import get_all_categories, get_all_metrics, custom_metric
 from .structures import Metric, Category
-import utils
+from . import utils
```

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/distance_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/distance_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/figures_of_speech.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/figures_of_speech.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/grammatical_forms.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/grammatical_forms.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/lexical_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/lexical_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/parts_of_speech_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/parts_of_speech_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/psycholinguistics.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/psycholinguistics.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/social_media.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/social_media.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/syntactic_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/syntactic_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/text_statistics.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/text_statistics.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/en/verb_tenses_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/en/verb_tenses_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/descriptive.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/descriptive.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/grammatical_forms.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/grammatical_forms.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/graphical.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/graphical.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/inflection.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/inflection.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/lexical.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/lexical.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/psycholinguistic.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/psycholinguistic.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/punctuation.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/punctuation.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/syntactic.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/syntactic.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/pl/word_formation.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/pl/word_formation.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/lexical_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/lexical_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/parts_of_speech_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/syntactic_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/syntactic_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/metrics/ukr/verb_forms_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/metrics/ukr/verb_forms_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/custom_preprocessing.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/custom_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/dictionary_en.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/dictionary_en.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/grammar.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/grammar.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/params.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/params.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/pos_tagger.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/psycholinguistics.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/psycholinguistics.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/en/stylistic.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/en/stylistic.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/matcher_component.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/matcher_component.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/params.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/params.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/dictionary_pl.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pl_nask/pos.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pl_nask/pos.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/pos_tagger.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/pos_tagger.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/psycholinguistic.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/psycholinguistic.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/resources/experimental_data.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/resources/experimental_data.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/pl/sentence_segmenter.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/pl/sentence_segmenter.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/dictionary_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/dictionary_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/grammar_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/grammar_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/params.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/params.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py` & `stylo_metrix-0.1.3/src/stylo_metrix/pipeline/ukr/pos_tagger_ukr.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/structures/__init__.py` & `stylo_metrix-0.1.3/src/stylo_metrix/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/structures/category.py` & `stylo_metrix-0.1.3/src/stylo_metrix/structures/category.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/structures/language.py` & `stylo_metrix-0.1.3/src/stylo_metrix/structures/language.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/structures/metric.py` & `stylo_metrix-0.1.3/src/stylo_metrix/structures/metric.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/structures/metrics_group.py` & `stylo_metrix-0.1.3/src/stylo_metrix/structures/metrics_group.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/tools/metric_tools.py` & `stylo_metrix-0.1.3/src/stylo_metrix/tools/metric_tools.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix/utils.py` & `stylo_metrix-0.1.3/src/stylo_metrix/utils.py`

 * *Files identical despite different names*

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix.egg-info/PKG-INFO` & `stylo_metrix-0.1.3/src/stylo_metrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stylo-metrix
-Version: 0.1.2
+Version: 0.1.3
 Summary: StyloMetrix tool
 Home-page: https://github.com/ZILiAT-NASK/StyloMetrix
 Author: ZILiAT-NASK, Adam Nowakowski
 Author-email: adam.nowakowski@nask.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stylo-metrix Version: 0.1.2 Summary: StyloMetrix
+Metadata-Version: 2.1 Name: stylo-metrix Version: 0.1.3 Summary: StyloMetrix
 tool Home-page: https://github.com/ZILiAT-NASK/StyloMetrix Author: ZILiAT-NASK,
 Adam Nowakowski Author-email: adam.nowakowski@nask.pl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # StyloMetrix [StyloMetrix][NASK] ZakÅad InÅ¼ynierii Lingwistycznej i
 Anailzy Tekstu, NASK PIB ## ð Quick ð¡ Stylometry tool in beta version for
```

### Comparing `stylo_metrix-0.1.2/src/stylo_metrix.egg-info/SOURCES.txt` & `stylo_metrix-0.1.3/src/stylo_metrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

