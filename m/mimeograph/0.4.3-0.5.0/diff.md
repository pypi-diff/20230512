# Comparing `tmp/mimeograph-0.4.3.tar.gz` & `tmp/mimeograph-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.4.3.tar", last modified: Wed May 10 10:07:29 2023, max compression
+gzip compressed data, was "mimeograph-0.5.0.tar", last modified: Fri May 12 09:59:04 2023, max compression
```

## Comparing `mimeograph-0.4.3.tar` & `mimeograph-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.3/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.3/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    23631 2023-05-10 10:07:29.948366 mimeograph-0.4.3/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    21275 2023-05-10 10:02:21.000000 mimeograph-0.4.3/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     3529 2023-05-10 10:07:21.000000 mimeograph-0.4.3/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-10 10:07:29.948366 mimeograph-0.4.3/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1327 2023-05-10 10:07:21.000000 mimeograph-0.4.3/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1660 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4224 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17737 2023-05-10 10:07:21.000000 mimeograph-0.4.3/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      589 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3111 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    29911 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1323 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2135 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2814 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      892 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    16065 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5091 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1533 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5515 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5763 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2120 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5479 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     8025 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/mimeo_db.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      868 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1640 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    22917 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4028 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      651 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      357 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-08 08:24:08.000000 mimeograph-0.4.3/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-08 08:24:08.000000 mimeograph-0.4.3/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      778 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-08 08:24:10.000000 mimeograph-0.4.3/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.3/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-08 08:24:13.000000 mimeograph-0.4.3/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1030 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     2063 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1412 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    24474 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    20016 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    23631 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1826 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1794 2023-05-10 04:50:43.000000 mimeograph-0.4.3/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      514 2023-05-10 04:50:43.000000 mimeograph-0.4.3/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.5.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-05-11 05:33:09.000000 mimeograph-0.5.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23377 2023-05-12 09:59:04.042522 mimeograph-0.5.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21021 2023-05-12 09:42:23.000000 mimeograph-0.5.0/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3692 2023-05-12 09:58:54.000000 mimeograph-0.5.0/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-12 09:59:04.042522 mimeograph-0.5.0/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1327 2023-05-12 09:58:54.000000 mimeograph-0.5.0/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-11 13:41:23.000000 mimeograph-0.5.0/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1660 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4283 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17274 2023-05-12 09:58:54.000000 mimeograph-0.5.0/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.034522 mimeograph-0.5.0/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      589 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3111 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    28118 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1402 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2135 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2364 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3032 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1018 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16065 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5091 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1533 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5515 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5763 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2120 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5479 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8025 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/database/mimeo_db.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      981 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1117 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1640 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    24152 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.038522 mimeograph-0.5.0/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4028 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      651 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1525 2023-05-12 09:42:23.000000 mimeograph-0.5.0/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      357 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-08 08:24:08.000000 mimeograph-0.5.0/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-08 08:24:08.000000 mimeograph-0.5.0/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      778 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.5.0/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1030 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2063 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1412 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    24474 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20016 2023-05-11 05:33:09.000000 mimeograph-0.5.0/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23377 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1854 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      212 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-12 09:59:04.000000 mimeograph-0.5.0/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-12 09:59:04.042522 mimeograph-0.5.0/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1828 2023-05-12 09:42:23.000000 mimeograph-0.5.0/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      514 2023-05-11 05:33:09.000000 mimeograph-0.5.0/tests/test_tools.py
```

### Comparing `mimeograph-0.4.3/LICENSE` & `mimeograph-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/PKG-INFO` & `mimeograph-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.3
+Version: 0.5.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,16 @@
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Mimeo (Mimeograph)
 
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
-[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
+[![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
@@ -191,15 +192,14 @@
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
-|              | `--http-auth`       | overwrite the `output/auth` property                                 |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
 |              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
@@ -221,15 +221,14 @@
 | `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
 | `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
 | `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
 | `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
 | `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
 | `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
 | `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
 | `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
 | `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
```

### Comparing `mimeograph-0.4.3/README.md` & `mimeograph-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Mimeo (Mimeograph)
 
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
-[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
+[![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
@@ -141,15 +142,14 @@
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
-|              | `--http-auth`       | overwrite the `output/auth` property                                 |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
 |              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
@@ -171,15 +171,14 @@
 | `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
 | `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
 | `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
 | `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
 | `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
 | `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
 | `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
 | `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
 | `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
```

### Comparing `mimeograph-0.4.3/pyproject.toml` & `mimeograph-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimeograph"
-version = "0.4.3"
+version = "0.5.0"
 description = "Generate data based on a simple template"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = "T.A. Programming Svcs.", email = "tomasz.maciej.aniolowski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -25,32 +25,50 @@
     "Topic :: Database",
     "Topic :: Software Development",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities",
 ]
 keywords = ["mimeograph", "mimeo", "generate", "generator", "data", "xml"]
 dependencies = [
-    "requests",
+    "aiohttp",
+    "aiofiles",
     "pandas",
     "pyyaml",
     "haggis"
 ]
 
 [project.urls]
 GitHub = "https://github.com/TomaszAniolowski/mimeo"
 
 [project.optional-dependencies]
-dev = ["bumpver", "build", "twine", "ruff", "isort", "pytest", "pytest-cov", "responses"]
-test = ["pytest", "pytest-cov", "responses"]
+dev = [
+    "bumpver",
+    "build",
+    "twine",
+    "ruff",
+    "isort",
+    "requests",
+    "pytest",
+    "pytest-cov",
+    "aioresponses",
+    "pytest-aioresponses",
+    "pytest-asyncio"
+]
+test = [
+    "pytest",
+    "pytest-cov",
+    "pytest-aioresponses",
+    "pytest-asyncio"
+]
 
 [project.scripts]
 mimeo = "mimeo.__main__:main"
 
 [tool.bumpver]
-current_version = "0.4.3"
+current_version = "0.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} to {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `mimeograph-0.4.3/src/mimeo/__init__.py` & `mimeograph-0.5.0/src/mimeo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     from mimeo import MimeoConfig, Mimeograph
 """
 from __future__ import annotations
 
 from .config import MimeoConfig
 from .mimeo import Mimeograph
 
-__version__ = "0.4.3"
+__version__ = "0.5.0"
 __all__ = ["MimeoConfig", "Mimeograph"]
```

### Comparing `mimeograph-0.4.3/src/mimeo/cli/__init__.py` & `mimeograph-0.5.0/src/mimeo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/cli/exc.py` & `mimeograph-0.5.0/src/mimeo/cli/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/cli/job.py` & `mimeograph-0.5.0/src/mimeo/cli/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 It exports a single class:
     * MimeoJob
         A class representing a single Mimeo processing job.
 """
 from __future__ import annotations
 
+import asyncio
 import json
 import logging
 from argparse import Namespace
 from os import walk
 from pathlib import Path
 
 from mimeo import MimeoConfig, Mimeograph
@@ -49,15 +50,17 @@
         which are: (1) parsing the configuration and (2) processing
         it.
         """
         self._customize_log_level(self._args)
         logger.info("Starting a Mimeo job")
         for config_path in self._get_config_paths(self._args.paths):
             mimeo_config = self._get_mimeo_config(config_path, self._args)
-            Mimeograph(mimeo_config).process()
+            asyncio.run(
+                Mimeograph(mimeo_config).process(),
+            )
 
     @staticmethod
     def _customize_log_level(
             args,
     ):
         """Customize the log level based on command line arguments."""
         if args.silent:
```

### Comparing `mimeograph-0.4.3/src/mimeo/cli/parsers.py` & `mimeograph-0.5.0/src/mimeo/cli/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,14 @@
                                 overwrite the output/username property
           -P PASSWORD, --http-password PASSWORD
                                 overwrite the output/password property
           --http-method METHOD
                                 overwrite the output/method property
           --http-protocol PROTOCOL
                                 overwrite the output/protocol property
-          --http-auth AUTH
-                                overwrite the output/auth property
           -e ENVIRONMENT, --http-env ENVIRONMENT
                                 overwrite the output http properties using a mimeo
                                 env configuration
           --http-envs-file PATH
                                 use a custom environments file
                                 (by default: mimeo.envs.json)
 
@@ -97,15 +95,15 @@
             self,
     ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.4.3")
+            version="%(prog)s v0.5.0")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
     def _add_mimeo_configuration_arguments(
@@ -179,19 +177,14 @@
             help="overwrite the output/method property")
         mimeo_config_args.add_argument(
             "--http-protocol",
             type=str,
             metavar="PROTOCOL",
             help="overwrite the output/protocol property")
         mimeo_config_args.add_argument(
-            "--http-auth",
-            type=str,
-            metavar="AUTH",
-            help="overwrite the output/auth property")
-        mimeo_config_args.add_argument(
             "-e",
             "--http-env",
             type=str,
             metavar="ENVIRONMENT",
             help="overwrite the output http properties using a mimeo env configuration")
         mimeo_config_args.add_argument(
             "--http-envs-file",
@@ -227,15 +220,14 @@
     parse_config() -> MimeoConfig
         Parse a Mimeo Configuration using Mimeo arguments.
     """
 
     _ENVIRONMENT_PROPS = [MimeoConfig.OUTPUT_PROTOCOL_KEY,
                           MimeoConfig.OUTPUT_HOST_KEY,
                           MimeoConfig.OUTPUT_PORT_KEY,
-                          MimeoConfig.OUTPUT_AUTH_KEY,
                           MimeoConfig.OUTPUT_USERNAME_KEY,
                           MimeoConfig.OUTPUT_PASSWORD_KEY]
 
     _ENTRY_PATH_KEY = "entry_path"
     _GET_VALUE_KEY = "get_value"
     _ARGS_MAPPING = {
         "output": {
@@ -263,18 +255,14 @@
             "entry_path": [MimeoConfig.OUTPUT_KEY,
                            MimeoConfig.OUTPUT_METHOD_KEY],
         },
         "http_protocol": {
             "entry_path": [MimeoConfig.OUTPUT_KEY,
                            MimeoConfig.OUTPUT_PROTOCOL_KEY],
         },
-        "http_auth": {
-            "entry_path": [MimeoConfig.OUTPUT_KEY,
-                           MimeoConfig.OUTPUT_AUTH_KEY],
-        },
         "http_host": {
             "entry_path": [MimeoConfig.OUTPUT_KEY,
                            MimeoConfig.OUTPUT_HOST_KEY],
         },
         "http_port": {
             "entry_path": [MimeoConfig.OUTPUT_KEY,
                            MimeoConfig.OUTPUT_PORT_KEY],
```

### Comparing `mimeograph-0.4.3/src/mimeo/config/__init__.py` & `mimeograph-0.5.0/src/mimeo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/config/exc.py` & `mimeograph-0.5.0/src/mimeo/config/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/config/mimeo_config.py` & `mimeograph-0.5.0/src/mimeo/config/mimeo_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,14 @@
         A Mimeo Configuration http protocol key
     OUTPUT_HOST_KEY : str
         A Mimeo Configuration http host key
     OUTPUT_PORT_KEY : str
         A Mimeo Configuration http port key
     OUTPUT_ENDPOINT_KEY : str
         A Mimeo Configuration http endpoint key
-    OUTPUT_AUTH_KEY : str
-        A Mimeo Configuration http auth key
     OUTPUT_USERNAME_KEY : str
         A Mimeo Configuration http username key
     OUTPUT_PASSWORD_KEY : str
         A Mimeo Configuration http password key
     VARS_KEY : str
         A Mimeo Configuration vars key
     TEMPLATES_KEY : str
@@ -121,24 +119,18 @@
         The 'stdout' output direction
     OUTPUT_DIRECTION_HTTP : str
         The 'http' output direction
     OUTPUT_DIRECTION_HTTP_REQUEST_POST : str
         The 'POST' http request method
     OUTPUT_DIRECTION_HTTP_REQUEST_PUT : str
         The 'PUT' http request method
-    OUTPUT_DIRECTION_HTTP_AUTH_BASIC : str
-        The 'basic' http auth method
-    OUTPUT_DIRECTION_HTTP_AUTH_DIGEST : str
-        The 'digest' http auth method
     SUPPORTED_OUTPUT_DIRECTIONS : set
         List of supported output directions
     SUPPORTED_REQUEST_METHODS : set
         List of supported http request methods
-    SUPPORTED_AUTH_METHODS : set
-        List of supported auth request methods
     REQUIRED_HTTP_DETAILS : set
         List of required http request output direction details
 
     output : MimeoOutput, default {}
         A Mimeo Output Details settings
     vars : dict, default {}
         A Mimeo Configuration vars setting
@@ -154,15 +146,14 @@
     OUTPUT_DIRECTORY_PATH_KEY = "directory_path"
     OUTPUT_FILE_NAME_KEY = "file_name"
     OUTPUT_METHOD_KEY = "method"
     OUTPUT_PROTOCOL_KEY = "protocol"
     OUTPUT_HOST_KEY = "host"
     OUTPUT_PORT_KEY = "port"
     OUTPUT_ENDPOINT_KEY = "endpoint"
-    OUTPUT_AUTH_KEY = "auth"
     OUTPUT_USERNAME_KEY = "username"
     OUTPUT_PASSWORD_KEY = "password"
     VARS_KEY = "vars"
     TEMPLATES_KEY = "_templates_"
     TEMPLATES_COUNT_KEY = "count"
     TEMPLATES_MODEL_KEY = "model"
     MODEL_CONTEXT_KEY = "context"
@@ -176,26 +167,21 @@
     OUTPUT_DIRECTION_FILE = "file"
     OUTPUT_DIRECTION_STD_OUT = "stdout"
     OUTPUT_DIRECTION_HTTP = "http"
 
     OUTPUT_DIRECTION_HTTP_REQUEST_POST = "POST"
     OUTPUT_DIRECTION_HTTP_REQUEST_PUT = "PUT"
 
-    OUTPUT_DIRECTION_HTTP_AUTH_BASIC = "basic"
-    OUTPUT_DIRECTION_HTTP_AUTH_DIGEST = "digest"
-
     SUPPORTED_OUTPUT_FORMATS = (OUTPUT_FORMAT_XML,)
 
     SUPPORTED_OUTPUT_DIRECTIONS = (OUTPUT_DIRECTION_STD_OUT,
                                    OUTPUT_DIRECTION_FILE,
                                    OUTPUT_DIRECTION_HTTP)
     SUPPORTED_REQUEST_METHODS = (OUTPUT_DIRECTION_HTTP_REQUEST_POST,
                                  OUTPUT_DIRECTION_HTTP_REQUEST_PUT)
-    SUPPORTED_AUTH_METHODS = (OUTPUT_DIRECTION_HTTP_AUTH_BASIC,
-                              OUTPUT_DIRECTION_HTTP_AUTH_DIGEST)
     REQUIRED_HTTP_DETAILS = (OUTPUT_HOST_KEY,
                              OUTPUT_ENDPOINT_KEY,
                              OUTPUT_USERNAME_KEY,
                              OUTPUT_PASSWORD_KEY)
 
     def __init__(
             self,
@@ -371,15 +357,14 @@
         self.directory_path = self._get_directory_path(self.direction, output)
         self.file_name = self._get_file_name(self.direction, output, self.format)
         self.method = self._get_method(self.direction, output)
         self.protocol = self._get_protocol(self.direction, output)
         self.host = self._get_host(self.direction, output)
         self.port = self._get_port(self.direction, output)
         self.endpoint = self._get_endpoint(self.direction, output)
-        self.auth = self._get_auth(self.direction, output)
         self.username = self._get_username(self.direction, output)
         self.password = self._get_password(self.direction, output)
 
     @staticmethod
     def _get_direction(
             output: dict,
     ) -> str:
@@ -661,49 +646,14 @@
             Otherwise, None.
         """
         if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
             return output.get(MimeoConfig.OUTPUT_ENDPOINT_KEY)
         return None
 
     @staticmethod
-    def _get_auth(
-            direction: str,
-            output: dict,
-    ) -> str | None:
-        """Extract an HTTP auth method from the source dictionary.
-
-        It is extracted only when the output direction is 'http'.
-
-        Parameters
-        ----------
-        direction : str
-            The configured output direction
-        output : dict
-            A source config output details dictionary
-
-        Returns
-        -------
-        auth: str | None
-            The configured HTTP auth method when the output direction is 'http'.
-            Otherwise, None. If the 'auth' setting is missing returns
-            'basic' by default.
-        """
-        auth = None
-        if direction == MimeoConfig.OUTPUT_DIRECTION_HTTP:
-            auth = output.get(
-                MimeoConfig.OUTPUT_AUTH_KEY,
-                MimeoConfig.OUTPUT_DIRECTION_HTTP_AUTH_BASIC)
-            if auth not in MimeoConfig.SUPPORTED_AUTH_METHODS:
-                raise UnsupportedPropertyValueError(
-                    MimeoConfig.OUTPUT_AUTH_KEY,
-                    auth,
-                    MimeoConfig.SUPPORTED_AUTH_METHODS)
-        return auth
-
-    @staticmethod
     def _get_username(
             direction: str,
             output: dict,
     ) -> str | None:
         """Extract a username from the source dictionary.
 
         It is extracted only when the output direction is 'http'.
```

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/__init__.py` & `mimeograph-0.5.0/src/mimeo/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/consumer.py` & `mimeograph-0.5.0/src/mimeo/consumers/consumer.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 It exports only one class:
     * Consumer
         An abstract class for data consumers in Mimeo.
 """
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
+from typing import Collection, Generator
 
 
 class Consumer(metaclass=ABCMeta):
     """An abstract class for data consumers in Mimeo.
 
     Its subclasses are meant to be used in the Mimeo processing.
     Every supported output direction has a Consumer representation.
@@ -39,19 +40,19 @@
             True if the subclass includes the consume method
         """
         return "consume" in subclass.__dict__ and callable(subclass.consume)
 
     @abstractmethod
     def consume(
             self,
-            data: str,
+            data: Collection | Generator,
     ):
         """Consume data generated by Mimeo.
 
         It is an abstract method to implement in subclasses
 
         Parameters
         ----------
-        data : str
+        data : Collection | Generator
             Stringified data generated by Mimeo
         """
         raise NotImplementedError
```

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.5.0/src/mimeo/consumers/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.5.0/src/mimeo/consumers/file_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     * FileConsumer
         A Consumer implementation saving data in the filesystem.
 """
 from __future__ import annotations
 
 import logging
 from pathlib import Path
+from typing import Collection, Generator
+
+import aiofiles
 
 from mimeo.config.mimeo_config import MimeoOutput
 from mimeo.consumers import Consumer
 
 logger = logging.getLogger(__name__)
 
 
@@ -44,34 +47,36 @@
         Parameters
         ----------
         output : MimeoOutput
             Configured Mimeo Output Details
         """
         self.directory = output.directory_path
         self.output_path_tmplt = f"{self.directory}/{output.file_name}"
-        self._count = 0
 
-    def consume(
+    async def consume(
             self,
-            data: str,
+            data: Collection | Generator,
     ) -> None:
         """Save data generated by Mimeo into a file.
 
         It is an implementation of Consumer's abstract method.
         If the output directory does not exist it is created.
         Every file name has an index inside its path.
 
         Parameters
         ----------
-        data : str
+        data : Collection | Generator
             Stringified data generated by Mimeo
         """
-        logger.fine("Consuming data [%s]", data)
-        if not Path(self.directory).exists():
-            logger.info("Creating output directory [%s]", self.directory)
-            Path(self.directory).mkdir(parents=True, exist_ok=True)
-
-        self._count += 1
-        file_name = self.output_path_tmplt.format(self._count)
-
-        logger.info("Writing data into file [%s]", file_name)
-        Path(file_name).write_text(data)
+        count = 0
+        for data_unit in data:
+            logger.fine("Consuming data [%s]", data_unit)
+            if not Path(self.directory).exists():
+                logger.info("Creating output directory [%s]", self.directory)
+                Path(self.directory).mkdir(parents=True, exist_ok=True)
+
+            count += 1
+            file_name = self.output_path_tmplt.format(count)
+
+            logger.info("Writing data into file [%s]", file_name)
+            async with aiofiles.open(file_name, mode="w") as file:
+                await file.write(data_unit)
```

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.5.0/src/mimeo/consumers/http_consumer.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 It exports only one class:
     * HttpConsumer
         A Consumer implementation sending data in HTTP requests.
 """
 from __future__ import annotations
 
+import asyncio
 import logging
+import uuid
+from typing import Collection, Generator
 
-from requests import Response, Session
-from requests.auth import HTTPBasicAuth, HTTPDigestAuth
+import aiohttp
+from aiohttp import ClientSession
 
 from mimeo.config.mimeo_config import MimeoOutput
 from mimeo.consumers import Consumer
 
 logger = logging.getLogger(__name__)
 
 
@@ -46,39 +49,42 @@
         Parameters
         ----------
         output : MimeoOutput
             Configured Mimeo Output Details
         """
         self.method = output.method
         self.url = HttpConsumer.__build_url(output)
-        auth_impl = HTTPBasicAuth if output.auth == "basic" else HTTPDigestAuth
-        self.__auth = auth_impl(output.username, output.password)
+        self.__auth = aiohttp.BasicAuth(output.username, output.password, "utf-8")
 
-    def consume(
+    async def consume(
             self,
-            data: str,
-    ) -> Response:
+            data: Collection | Generator,
+    ):
         """Send data generated by Mimeo in an HTTP request.
 
         It is an implementation of Consumer's abstract method.
 
         Parameters
         ----------
-        data : str
+        data : Collection | Generator
             Stringified data generated by Mimeo
         """
-        logger.fine("Consuming data [%s]", data)
-        with Session() as sess:
-            logger.info("Sending request %s %s", self.method, self.url)
-            return sess.request(
+        async def send_request(sess: ClientSession, data_unit: str):
+            req_id = str(uuid.uuid4())
+            logger.info("Sending request %s %s [%s]", self.method, self.url, req_id)
+            resp = await sess.request(
                 self.method,
                 self.url,
                 auth=self.__auth,
-                data=data,
+                data=data_unit,
                 headers={"Content-Type": "application/xml"})
+            logger.info("[%s] Status: %s", req_id, resp.status)
+
+        async with ClientSession() as s:
+            await asyncio.gather(*[send_request(s, d) for d in data])
 
     @staticmethod
     def __build_url(
             output: MimeoOutput,
     ) -> str:
         """Build a URL based on Mimeo Output Details.
```

### Comparing `mimeograph-0.4.3/src/mimeo/consumers/raw_consumer.py` & `mimeograph-0.5.0/src/mimeo/consumers/raw_consumer.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 It exports only one class:
     * RawConsumer
         A Consumer implementation printing data in the standard output.
 """
 from __future__ import annotations
 
+from typing import Collection, Generator
+
 from mimeo.consumers import Consumer
 
 
 class RawConsumer(Consumer):
     """A Consumer implementation printing data in the standard output.
 
     This Consumer is instantiated for the 'stdout' output direction
@@ -17,21 +19,22 @@
 
     Methods
     -------
     consume
         Print data generated in the standard output.
     """
 
-    def consume(
+    async def consume(
             self,
-            data: str,
+            data: Collection | Generator,
     ) -> None:
         """Print data generated in the standard output.
 
         It is an implementation of Consumer's abstract method.
 
         Parameters
         ----------
-        data : str
+        data : Collection | Generator
             Stringified data generated by Mimeo
         """
-        print(data)
+        for data_unit in data:
+            print(data_unit)
```

### Comparing `mimeograph-0.4.3/src/mimeo/context/__init__.py` & `mimeograph-0.5.0/src/mimeo/context/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/context/decorators.py` & `mimeograph-0.5.0/src/mimeo/context/decorators.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/context/exc.py` & `mimeograph-0.5.0/src/mimeo/context/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/context/mimeo_context.py` & `mimeograph-0.5.0/src/mimeo/context/mimeo_context.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.5.0/src/mimeo/context/mimeo_context_manager.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.5.0/src/mimeo/context/mimeo_iteration.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/__init__.py` & `mimeograph-0.5.0/src/mimeo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/cities.py` & `mimeograph-0.5.0/src/mimeo/database/cities.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/countries.py` & `mimeograph-0.5.0/src/mimeo/database/countries.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/exc.py` & `mimeograph-0.5.0/src/mimeo/database/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/first_names.py` & `mimeograph-0.5.0/src/mimeo/database/first_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/last_names.py` & `mimeograph-0.5.0/src/mimeo/database/last_names.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/database/mimeo_db.py` & `mimeograph-0.5.0/src/mimeo/database/mimeo_db.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/generators/__init__.py` & `mimeograph-0.5.0/src/mimeo/generators/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 It contains modules supporting the Mimeo Config output formats:
 * generator
     The Mimeo Generator module.
 * generator_factory
     The Mimeo Generator Factory module.
 * xml_generator
     The Mimeo XML Generator module.
+* exc
+    The Mimeo Generators Exceptions module.
 
 This package exports the following classes:
 * Generator:
     An abstract class for data generators in Mimeo.
 * GeneratorFactory:
     A Factory class instantiating a Generator based on Mimeo Config.
 * XMLGenerator:
     A Generator implementation producing data in the XML format.
     Corresponds to the 'xml' output format
 
 To use this package, simply import the desired class:
     from mimeo.generators import GeneratorFactory
+    from mimeo.generators.exc import UnsupportedStructureError
 """
 from .generator import Generator
 from .xml_generator import XMLGenerator
 from .generator_factory import GeneratorFactory
 
 __all__ = ["Generator", "XMLGenerator", "GeneratorFactory"]
```

### Comparing `mimeograph-0.4.3/src/mimeo/generators/generator.py` & `mimeograph-0.5.0/src/mimeo/generators/generator.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/generators/generator_factory.py` & `mimeograph-0.5.0/src/mimeo/generators/generator_factory.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/generators/xml_generator.py` & `mimeograph-0.5.0/src/mimeo/generators/xml_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
 from mimeo.context import MimeoContext
 from mimeo.context.decorators import (mimeo_clear_iterations, mimeo_context,
                                       mimeo_context_switch,
                                       mimeo_next_iteration)
 from mimeo.generators import Generator
+from mimeo.generators.exc import UnsupportedStructureError
 from mimeo.utils import MimeoRenderer
 
 logger = logging.getLogger(__name__)
 
 
 class XMLGenerator(Generator):
     """A Generator implementation producing data in the XML format.
@@ -218,18 +219,20 @@
         Returns
         -------
         ElemTree.Element
             A single data unit generated within a single template iteration.
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
         """
         logger.fine("Rendering element - parent [%s], element_meta [%s]",
                     parent if parent is None else parent.tag, element_meta)
         element_meta = cls._pre_process_node(element_meta)
 
         if cls._is_complex(element_meta):
             return cls._process_complex_value(parent, element_meta)
@@ -329,18 +332,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
         """
         if isinstance(element_meta["value"], dict):
             func = cls._process_dict_value
         elif (isinstance(element_meta["value"], list) and
               element_meta["tag"] != MimeoConfig.TEMPLATES_KEY):
             func = cls._process_list_value
         else:
@@ -367,18 +372,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
 
         Examples
         --------
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
             value={"SomeChild1": 1, "SomeChild2": 2},
@@ -415,24 +422,36 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If the list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
             If the special field value is dict or list
         SpecialFieldNotFoundError
             If the special field does not exist.
         """
-        has_only_atomic_values = all(not isinstance(child, (list, dict))
-                                     for child in element_meta["value"])
+        has_only_atomic_values = all(
+            not isinstance(child, (list, dict)) or
+            MimeoRenderer.is_parametrized_mimeo_util(child)
+            for child in element_meta["value"])
         if has_only_atomic_values:
             return cls._process_list_value_with_atomic_children(parent, element_meta)
-        return cls._process_list_value_with_complex_children(parent, element_meta)
+
+        has_only_dict_values = all(
+            isinstance(child, dict) and
+            not MimeoRenderer.is_parametrized_mimeo_util(child)
+            for child in element_meta["value"])
+        if has_only_dict_values:
+            return cls._process_list_value_with_complex_children(parent, element_meta)
+
+        raise UnsupportedStructureError(element_meta["tag"], element_meta["value"])
 
     @classmethod
     def _process_list_value_with_atomic_children(
             cls,
             parent: ElemTree.Element,
             element_meta: dict,
     ) -> ElemTree.Element:
@@ -451,18 +470,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
 
         Examples
         --------
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
             value=[],
@@ -499,18 +520,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
 
         Examples
         --------
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
             value=[{"SomeChild": {"SomeGrandChild1": 1, "SomeGrandChild2": 2}},
@@ -557,18 +580,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
 
         Examples
         --------
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
             value={"_templates_": [
@@ -623,18 +648,20 @@
         Returns
         -------
         ElemTree.Element
             A processed node
 
         Raises
         ------
+        UnsupportedStructureError
+            If a list value elements are not atomic-only or dict-only.
         InvalidSpecialFieldValueError
-            If the special field value is dict or list
+            If a special field value is dict or list
         SpecialFieldNotFoundError
-            If the special field does not exist.
+            If a special field does not exist.
 
         Examples
         --------
         context = MimeoContextManager().get_current_context()
         parent = ElemTree.Element("Root")
         element_meta = cls._element_meta(
             tag="SomeField",
```

### Comparing `mimeograph-0.4.3/src/mimeo/logging/__init__.py` & `mimeograph-0.5.0/src/mimeo/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/logging/filters.py` & `mimeograph-0.5.0/src/mimeo/logging/filters.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/meta/__init__.py` & `mimeograph-0.5.0/src/mimeo/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/meta/alive.py` & `mimeograph-0.5.0/src/mimeo/meta/alive.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/meta/exc.py` & `mimeograph-0.5.0/src/mimeo/meta/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/mimeo.py` & `mimeograph-0.5.0/src/mimeo/mimeo.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,17 +33,18 @@
             self,
             mimeo_config: MimeoConfig,
     ):
         self._mimeo_config = mimeo_config
         self._generator = GeneratorFactory.get_generator(self._mimeo_config)
         self._consumer = ConsumerFactory.get_consumer(self._mimeo_config)
 
-    def process(
+    async def process(
             self,
     ):
         """Process the Mimeo Configuration (generate data and consume)."""
         logger.info("Starting data generation")
         with MimeoContextManager(self._mimeo_config):
-            for data in self._generator.generate(self._mimeo_config.templates):
-                data_str = self._generator.stringify(data)
-                self._consumer.consume(data_str)
+            data = self._generator.generate(self._mimeo_config.templates)
+            data_str = (self._generator.stringify(data_unit)
+                        for data_unit in data)
+            await self._consumer.consume(data_str)
         logger.info("Data has been processed")
```

### Comparing `mimeograph-0.4.3/src/mimeo/resources/cities.csv` & `mimeograph-0.5.0/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/resources/countries.csv` & `mimeograph-0.5.0/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/resources/exc.py` & `mimeograph-0.5.0/src/mimeo/resources/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/resources/forenames.csv` & `mimeograph-0.5.0/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/resources/logging.yaml` & `mimeograph-0.5.0/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/resources/surnames.txt` & `mimeograph-0.5.0/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/tools.py` & `mimeograph-0.5.0/src/mimeo/tools.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/utils/__init__.py` & `mimeograph-0.5.0/src/mimeo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/utils/exc.py` & `mimeograph-0.5.0/src/mimeo/utils/exc.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.5.0/src/mimeo/utils/mimeo_utils.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeo/utils/renderers.py` & `mimeograph-0.5.0/src/mimeo/utils/renderers.py`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.3/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.5.0/src/mimeograph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.3
+Version: 0.5.0
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,16 @@
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # Mimeo (Mimeograph)
 
 [![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
-[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)
+[![Python](https://img.shields.io/pypi/pyversions/mimeograph?label=Python&style=plastic)](https://www.python.org/)  
 [![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
 [![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
 
 [Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
@@ -191,15 +192,14 @@
 |     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
 |     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
 |     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
 |     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
 |     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
 |              | `--http-method`     | overwrite the `output/method` property                               |
 |              | `--http-protocol`   | overwrite the `output/protocol` property                             |
-|              | `--http-auth`       | overwrite the `output/auth` property                                 |
 |     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
 |              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
@@ -221,15 +221,14 @@
 | `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
 | `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
 | `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
 | `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
 | `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
 | `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
 | `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
 | `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
 | `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
```

### Comparing `mimeograph-0.4.3/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.5.0/src/mimeograph.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/mimeo/database/cities.py
 src/mimeo/database/countries.py
 src/mimeo/database/exc.py
 src/mimeo/database/first_names.py
 src/mimeo/database/last_names.py
 src/mimeo/database/mimeo_db.py
 src/mimeo/generators/__init__.py
+src/mimeo/generators/exc.py
 src/mimeo/generators/generator.py
 src/mimeo/generators/generator_factory.py
 src/mimeo/generators/xml_generator.py
 src/mimeo/logging/__init__.py
 src/mimeo/logging/filters.py
 src/mimeo/meta/__init__.py
 src/mimeo/meta/alive.py
```

### Comparing `mimeograph-0.4.3/tests/test_mimeograph.py` & `mimeograph-0.5.0/tests/test_mimeograph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import shutil
 from pathlib import Path
 
 import pytest
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
@@ -12,15 +11,16 @@
 @pytest.fixture(autouse=True)
 def _teardown():
     yield
     # Teardown
     shutil.rmtree("test_mimeograph-dir")
 
 
-def test_produce():
+@pytest.mark.asyncio()
+async def test_produce():
     config = {
         "output": {
             "direction": "file",
             "format": "xml",
             "indent": 4,
             "xml_declaration": True,
             "directory_path": "test_mimeograph-dir",
@@ -40,15 +40,15 @@
         ],
     }
     mimeo_config = MimeoConfig(config)
     with MimeoContextManager(mimeo_config):
         mimeo = Mimeograph(mimeo_config)
 
         assert not Path("test_mimeograph-dir").exists()
-        mimeo.process()
+        await mimeo.process()
         assert Path("test_mimeograph-dir").exists()
         for i in range(1, 11):
             file_path = f"test_mimeograph-dir/output-{i}.xml"
             assert Path(file_path).exists()
 
             with Path(file_path).open() as file:
                 assert file.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
```

### Comparing `mimeograph-0.4.3/tests/test_tools.py` & `mimeograph-0.5.0/tests/test_tools.py`

 * *Files identical despite different names*

