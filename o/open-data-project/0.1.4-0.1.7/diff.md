# Comparing `tmp/open_data_project-0.1.4.tar.gz` & `tmp/open_data_project-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_data_project-0.1.4.tar", last modified: Sat May  6 13:10:43 2023, max compression
+gzip compressed data, was "open_data_project-0.1.7.tar", last modified: Fri May 12 00:08:08 2023, max compression
```

## Comparing `open_data_project-0.1.4.tar` & `open_data_project-0.1.7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.918277 open_data_project-0.1.4/
--rw-rw-rw-   0        0        0     1090 2023-04-18 13:50:00.000000 open_data_project-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      112 2023-05-06 13:01:53.000000 open_data_project-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-05-06 13:10:43.917273 open_data_project-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-04-18 13:31:25.000000 open_data_project-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.752280 open_data_project-0.1.4/open_data_project/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.767278 open_data_project-0.1.4/open_data_project/.github/
--rw-rw-rw-   0        0        0     1075 2023-04-17 15:34:45.000000 open_data_project-0.1.4/open_data_project/.github/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.773282 open_data_project-0.1.4/open_data_project/.github/workflows/
--rw-rw-rw-   0        0        0      589 2023-04-17 15:51:57.000000 open_data_project-0.1.4/open_data_project/.github/workflows/alive.yml
--rw-rw-rw-   0        0        0     4492 2023-04-17 15:53:37.000000 open_data_project-0.1.4/open_data_project/.github/workflows/pipeline.yml
--rw-rw-rw-   0        0        0      422 2023-04-17 15:55:20.000000 open_data_project-0.1.4/open_data_project/.github/workflows/test.yml
--rw-rw-rw-   0        0        0     6293 2023-03-13 11:33:45.000000 open_data_project-0.1.4/open_data_project/.gitignore
--rw-rw-rw-   0        0        0     1070 2023-03-13 11:33:45.000000 open_data_project-0.1.4/open_data_project/LICENSE
--rw-rw-rw-   0        0        0     9396 2023-03-13 11:33:45.000000 open_data_project-0.1.4/open_data_project/ODPCategories.json
--rw-rw-rw-   0        0        0        0 2023-03-13 11:33:45.000000 open_data_project-0.1.4/open_data_project/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-04-17 16:18:12.000000 open_data_project-0.1.4/open_data_project/arcgis.py
--rw-rw-rw-   0        0        0     4412 2023-04-17 16:19:14.000000 open_data_project-0.1.4/open_data_project/ckan.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.784280 open_data_project-0.1.4/open_data_project/data/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.794278 open_data_project-0.1.4/open_data_project/data/USMART/
--rw-rw-rw-   0        0        0    28960 2023-04-03 22:14:04.000000 open_data_project-0.1.4/open_data_project/data/USMART/Dumfries and Galloway Council.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.796297 open_data_project-0.1.4/open_data_project/data/arcgis/
--rw-rw-rw-   0        0        0    20932 2023-03-20 16:34:35.000000 open_data_project-0.1.4/open_data_project/data/arcgis/renfrew.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.801277 open_data_project-0.1.4/open_data_project/data/ckan/
--rw-rw-rw-   0        0        0   138393 2023-03-20 16:34:43.000000 open_data_project-0.1.4/open_data_project/data/ckan/Aberdeen City Council.csv
--rw-rw-rw-   0        0        0  1384817 2023-04-03 22:14:04.000000 open_data_project-0.1.4/open_data_project/data/ckan/Spatial Hub.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.814278 open_data_project-0.1.4/open_data_project/data/dcat/
--rw-rw-rw-   0        0        0   121898 2023-03-20 16:35:39.000000 open_data_project-0.1.4/open_data_project/data/dcat/Coral G.csv
--rw-rw-rw-   0        0        0   215835 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/dcat/edinburgh.csv
--rw-rw-rw-   0        0        0   231148 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/dcat/glasgow.csv
--rw-rw-rw-   0        0        0   135957 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/dcat/highland.csv
--rw-rw-rw-   0        0        0  3452193 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/merged_output.json
--rw-rw-rw-   0        0        0  2982715 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/merged_output_untidy.json
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.817278 open_data_project-0.1.4/open_data_project/data/sparkql/
--rw-rw-rw-   0        0        0   113905 2023-04-03 22:14:05.000000 open_data_project-0.1.4/open_data_project/data/sparkql/scotgov-datasets-sparkql.csv
--rw-rw-rw-   0        0        0     2655 2023-04-17 16:19:39.000000 open_data_project-0.1.4/open_data_project/dcat.py
--rw-rw-rw-   0        0        0      593 2023-03-13 11:33:45.000000 open_data_project-0.1.4/open_data_project/error_log.md
--rw-rw-rw-   0        0        0     5950 2023-04-17 16:24:29.000000 open_data_project-0.1.4/open_data_project/export2jkan.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.820278 open_data_project-0.1.4/open_data_project/health_checks/
--rw-rw-rw-   0        0        0     5212 2023-04-17 15:57:00.000000 open_data_project-0.1.4/open_data_project/health_checks/health_categories.py
--rw-rw-rw-   0        0        0        0 2023-03-20 16:34:31.000000 open_data_project-0.1.4/open_data_project/log.json
--rw-rw-rw-   0        0        0      100 2023-03-20 16:34:31.000000 open_data_project-0.1.4/open_data_project/log.md
--rw-rw-rw-   0        0        0     1032 2023-04-27 00:56:03.000000 open_data_project-0.1.4/open_data_project/main.sh
--rw-rw-rw-   0        0        0    16560 2023-04-28 21:57:27.000000 open_data_project-0.1.4/open_data_project/merge_data.py
--rw-rw-rw-   0        0        0     2100 2023-05-02 22:21:49.000000 open_data_project-0.1.4/open_data_project/odp.py
--rw-rw-rw-   0        0        0     4381 2023-04-17 17:28:49.000000 open_data_project-0.1.4/open_data_project/processor.py
--rw-rw-rw-   0        0        0      220 2023-04-17 16:30:06.000000 open_data_project-0.1.4/open_data_project/requirements.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 13:32:03.000000 open_data_project-0.1.4/open_data_project/sources.csv
--rw-rw-rw-   0        0        0     3361 2023-04-17 16:30:30.000000 open_data_project-0.1.4/open_data_project/sparkql_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.842281 open_data_project-0.1.4/open_data_project/tests/
--rw-rw-rw-   0        0        0        0 2023-03-13 11:34:20.000000 open_data_project-0.1.4/open_data_project/tests/__init__.py
--rw-rw-rw-   0        0        0     1188 2023-04-17 16:00:38.000000 open_data_project-0.1.4/open_data_project/tests/arcgis_test.py
--rw-rw-rw-   0        0        0     1540 2023-04-18 21:46:44.000000 open_data_project-0.1.4/open_data_project/tests/ckan_test.py
--rw-rw-rw-   0        0        0     6938 2023-04-17 18:02:47.000000 open_data_project-0.1.4/open_data_project/tests/conftest.py
--rw-rw-rw-   0        0        0     1174 2023-04-17 16:05:46.000000 open_data_project-0.1.4/open_data_project/tests/dcat_test.py
--rw-rw-rw-   0        0        0      754 2023-04-17 16:07:35.000000 open_data_project-0.1.4/open_data_project/tests/export2jkan_test.py
--rw-rw-rw-   0        0        0     4994 2023-04-28 21:59:58.000000 open_data_project-0.1.4/open_data_project/tests/generate_new_mock_data.py
--rw-rw-rw-   0        0        0      650 2023-03-13 11:34:20.000000 open_data_project-0.1.4/open_data_project/tests/how_to_test.md
--rw-rw-rw-   0        0        0     1624 2023-04-17 16:09:04.000000 open_data_project-0.1.4/open_data_project/tests/merge_data_test.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.847276 open_data_project-0.1.4/open_data_project/tests/mock_data/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.850289 open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.857278 open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/expected/
--rw-rw-rw-   0        0        0    14051 2023-03-15 13:04:33.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/expected/renfrew.csv
--rw-rw-rw-   0        0        0  2160868 2023-03-15 13:04:32.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/renfrew.json
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.859293 open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.862291 open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/expected/
--rw-rw-rw-   0        0        0   230300 2023-03-15 13:04:35.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/expected/glasgow.csv
--rw-rw-rw-   0        0        0   377494 2023-03-15 13:04:34.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/glasgow.json
--rw-rw-rw-   0        0        0     2802 2023-03-13 11:34:21.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/get_json_data.json
--rw-rw-rw-   0        0        0      160 2023-04-15 17:21:54.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/mockcsv.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.864276 open_data_project-0.1.4/open_data_project/tests/mock_data/output/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.866276 open_data_project-0.1.4/open_data_project/tests/mock_data/output/arcgis/
--rw-rw-rw-   0        0        0    14051 2023-03-15 13:16:03.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/output/arcgis/renfrew.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.868276 open_data_project-0.1.4/open_data_project/tests/mock_data/output/dcat/
--rw-rw-rw-   0        0        0   230300 2023-03-15 13:16:03.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/output/dcat/glasgow.csv
--rw-rw-rw-   0        0        0      160 2023-03-15 13:16:03.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/output/mockcsv.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.870278 open_data_project-0.1.4/open_data_project/tests/mock_data/output/usmart/
--rw-rw-rw-   0        0        0    27679 2023-03-15 13:16:03.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/output/usmart/Dumfries and Galloway Council.csv
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.872277 open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/
--rw-rw-rw-   0        0        0    93978 2023-03-15 13:04:35.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/Dumfries and Galloway Council.json
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.875292 open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/expected/
--rw-rw-rw-   0        0        0    27679 2023-03-15 13:04:35.000000 open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/expected/Dumfries and Galloway Council.csv
--rw-rw-rw-   0        0        0     4292 2023-04-17 16:08:09.000000 open_data_project-0.1.4/open_data_project/tests/processor_test.py
--rw-rw-rw-   0        0        0     1188 2023-04-17 16:08:21.000000 open_data_project-0.1.4/open_data_project/tests/usmart_test.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.879278 open_data_project-0.1.4/open_data_project/tools/
--rw-rw-rw-   0        0        0      610 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/tools/README.md
--rw-rw-rw-   0        0        0     2492 2023-04-17 16:12:13.000000 open_data_project-0.1.4/open_data_project/tools/alive.py
--rw-rw-rw-   0        0        0     2951 2023-04-17 16:31:16.000000 open_data_project-0.1.4/open_data_project/usmart.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.881277 open_data_project-0.1.4/open_data_project/web-scrapers/
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.893279 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/
--rw-rw-rw-   0        0        0     4769 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/aberdeenshire_council_scraper.py
--rw-rw-rw-   0        0        0     4333 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/east_ayrshire_scraper.py
--rw-rw-rw-   0        0        0     4504 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/moray_council_scraper.py
--rw-rw-rw-   0        0        0    13989 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/nls_scraper.py
--rw-rw-rw-   0        0        0     7691 2023-03-13 11:34:22.000000 open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/sqa_scraper.py
--rw-rw-rw-   0        0        0      763 2023-04-13 18:20:31.000000 open_data_project-0.1.4/open_data_project/web-scrapers/sample_scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:10:43.765277 open_data_project-0.1.4/open_data_project.egg-info/
--rw-rw-rw-   0        0        0      273 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3342 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      133 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-06 13:10:43.000000 open_data_project-0.1.4/open_data_project.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 13:10:43.919292 open_data_project-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-05-06 12:21:39.000000 open_data_project-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.318362 open_data_project-0.1.7/
+-rw-rw-rw-   0        0        0     1090 2023-04-18 13:50:00.000000 open_data_project-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-05-06 13:01:53.000000 open_data_project-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-05-12 00:08:08.317322 open_data_project-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2015 2023-05-06 18:31:28.000000 open_data_project-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.081087 open_data_project-0.1.7/open_data_project/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.121087 open_data_project-0.1.7/open_data_project/.github/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 15:34:45.000000 open_data_project-0.1.7/open_data_project/.github/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.127084 open_data_project-0.1.7/open_data_project/.github/workflows/
+-rw-rw-rw-   0        0        0      589 2023-04-17 15:51:57.000000 open_data_project-0.1.7/open_data_project/.github/workflows/alive.yml
+-rw-rw-rw-   0        0        0     4492 2023-04-17 15:53:37.000000 open_data_project-0.1.7/open_data_project/.github/workflows/pipeline.yml
+-rw-rw-rw-   0        0        0      422 2023-04-17 15:55:20.000000 open_data_project-0.1.7/open_data_project/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     6293 2023-03-13 11:33:45.000000 open_data_project-0.1.7/open_data_project/.gitignore
+-rw-rw-rw-   0        0        0     1070 2023-03-13 11:33:45.000000 open_data_project-0.1.7/open_data_project/LICENSE
+-rw-rw-rw-   0        0        0     9396 2023-03-13 11:33:45.000000 open_data_project-0.1.7/open_data_project/ODPCategories.json
+-rw-rw-rw-   0        0        0        0 2023-03-13 11:33:45.000000 open_data_project-0.1.7/open_data_project/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-04-17 16:18:12.000000 open_data_project-0.1.7/open_data_project/arcgis.py
+-rw-rw-rw-   0        0        0     4412 2023-04-17 16:19:14.000000 open_data_project-0.1.7/open_data_project/ckan.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.138086 open_data_project-0.1.7/open_data_project/data/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.146088 open_data_project-0.1.7/open_data_project/data/USMART/
+-rw-rw-rw-   0        0        0    28960 2023-04-03 22:14:04.000000 open_data_project-0.1.7/open_data_project/data/USMART/Dumfries and Galloway Council.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.148085 open_data_project-0.1.7/open_data_project/data/arcgis/
+-rw-rw-rw-   0        0        0    20932 2023-03-20 16:34:35.000000 open_data_project-0.1.7/open_data_project/data/arcgis/renfrew.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.152085 open_data_project-0.1.7/open_data_project/data/ckan/
+-rw-rw-rw-   0        0        0   138393 2023-03-20 16:34:43.000000 open_data_project-0.1.7/open_data_project/data/ckan/Aberdeen City Council.csv
+-rw-rw-rw-   0        0        0  1384817 2023-04-03 22:14:04.000000 open_data_project-0.1.7/open_data_project/data/ckan/Spatial Hub.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.163084 open_data_project-0.1.7/open_data_project/data/dcat/
+-rw-rw-rw-   0        0        0   121898 2023-03-20 16:35:39.000000 open_data_project-0.1.7/open_data_project/data/dcat/Coral G.csv
+-rw-rw-rw-   0        0        0   215835 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/dcat/edinburgh.csv
+-rw-rw-rw-   0        0        0   231148 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/dcat/glasgow.csv
+-rw-rw-rw-   0        0        0   135957 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/dcat/highland.csv
+-rw-rw-rw-   0        0        0  3452193 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/merged_output.json
+-rw-rw-rw-   0        0        0  2982715 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/merged_output_untidy.json
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.165102 open_data_project-0.1.7/open_data_project/data/sparkql/
+-rw-rw-rw-   0        0        0   113905 2023-04-03 22:14:05.000000 open_data_project-0.1.7/open_data_project/data/sparkql/scotgov-datasets-sparkql.csv
+-rw-rw-rw-   0        0        0     2675 2023-05-11 23:47:50.000000 open_data_project-0.1.7/open_data_project/dcat.py
+-rw-rw-rw-   0        0        0      593 2023-03-13 11:33:45.000000 open_data_project-0.1.7/open_data_project/error_log.md
+-rw-rw-rw-   0        0        0     5950 2023-04-17 16:24:29.000000 open_data_project-0.1.7/open_data_project/export2jkan.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.167085 open_data_project-0.1.7/open_data_project/health_checks/
+-rw-rw-rw-   0        0        0     5212 2023-04-17 15:57:00.000000 open_data_project-0.1.7/open_data_project/health_checks/health_categories.py
+-rw-rw-rw-   0        0        0        0 2023-03-20 16:34:31.000000 open_data_project-0.1.7/open_data_project/log.json
+-rw-rw-rw-   0        0        0      100 2023-03-20 16:34:31.000000 open_data_project-0.1.7/open_data_project/log.md
+-rw-rw-rw-   0        0        0     1032 2023-04-27 00:56:03.000000 open_data_project-0.1.7/open_data_project/main.sh
+-rw-rw-rw-   0        0        0    16560 2023-04-28 21:57:27.000000 open_data_project-0.1.7/open_data_project/merge_data.py
+-rw-rw-rw-   0        0        0     2100 2023-05-12 00:03:26.000000 open_data_project-0.1.7/open_data_project/odp.py
+-rw-rw-rw-   0        0        0     4381 2023-04-17 17:28:49.000000 open_data_project-0.1.7/open_data_project/processor.py
+-rw-rw-rw-   0        0        0      220 2023-04-17 16:30:06.000000 open_data_project-0.1.7/open_data_project/requirements.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 13:32:03.000000 open_data_project-0.1.7/open_data_project/sources.csv
+-rw-rw-rw-   0        0        0     3361 2023-04-17 16:30:30.000000 open_data_project-0.1.7/open_data_project/sparkql_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.198084 open_data_project-0.1.7/open_data_project/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-13 11:34:20.000000 open_data_project-0.1.7/open_data_project/tests/__init__.py
+-rw-rw-rw-   0        0        0     1188 2023-04-17 16:00:38.000000 open_data_project-0.1.7/open_data_project/tests/arcgis_test.py
+-rw-rw-rw-   0        0        0     1540 2023-04-18 21:46:44.000000 open_data_project-0.1.7/open_data_project/tests/ckan_test.py
+-rw-rw-rw-   0        0        0     6938 2023-04-17 18:02:47.000000 open_data_project-0.1.7/open_data_project/tests/conftest.py
+-rw-rw-rw-   0        0        0     1174 2023-04-17 16:05:46.000000 open_data_project-0.1.7/open_data_project/tests/dcat_test.py
+-rw-rw-rw-   0        0        0      754 2023-04-17 16:07:35.000000 open_data_project-0.1.7/open_data_project/tests/export2jkan_test.py
+-rw-rw-rw-   0        0        0     4994 2023-04-28 21:59:58.000000 open_data_project-0.1.7/open_data_project/tests/generate_new_mock_data.py
+-rw-rw-rw-   0        0        0      650 2023-03-13 11:34:20.000000 open_data_project-0.1.7/open_data_project/tests/how_to_test.md
+-rw-rw-rw-   0        0        0     1624 2023-04-17 16:09:04.000000 open_data_project-0.1.7/open_data_project/tests/merge_data_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.202087 open_data_project-0.1.7/open_data_project/tests/mock_data/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.204087 open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.210091 open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/expected/
+-rw-rw-rw-   0        0        0    14051 2023-03-15 13:04:33.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/expected/renfrew.csv
+-rw-rw-rw-   0        0        0  2160868 2023-03-15 13:04:32.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/renfrew.json
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.212087 open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.215086 open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/expected/
+-rw-rw-rw-   0        0        0   230300 2023-03-15 13:04:35.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/expected/glasgow.csv
+-rw-rw-rw-   0        0        0   377494 2023-03-15 13:04:34.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/glasgow.json
+-rw-rw-rw-   0        0        0     2802 2023-03-13 11:34:21.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/get_json_data.json
+-rw-rw-rw-   0        0        0      160 2023-04-15 17:21:54.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/mockcsv.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.218087 open_data_project-0.1.7/open_data_project/tests/mock_data/output/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.220086 open_data_project-0.1.7/open_data_project/tests/mock_data/output/arcgis/
+-rw-rw-rw-   0        0        0    14051 2023-03-15 13:16:03.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/output/arcgis/renfrew.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.252591 open_data_project-0.1.7/open_data_project/tests/mock_data/output/dcat/
+-rw-rw-rw-   0        0        0   230300 2023-03-15 13:16:03.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/output/dcat/glasgow.csv
+-rw-rw-rw-   0        0        0      160 2023-03-15 13:16:03.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/output/mockcsv.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.255603 open_data_project-0.1.7/open_data_project/tests/mock_data/output/usmart/
+-rw-rw-rw-   0        0        0    27679 2023-03-15 13:16:03.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/output/usmart/Dumfries and Galloway Council.csv
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.257634 open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/
+-rw-rw-rw-   0        0        0    93978 2023-03-15 13:04:35.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/Dumfries and Galloway Council.json
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.259604 open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/expected/
+-rw-rw-rw-   0        0        0    27679 2023-03-15 13:04:35.000000 open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/expected/Dumfries and Galloway Council.csv
+-rw-rw-rw-   0        0        0     4292 2023-04-17 16:08:09.000000 open_data_project-0.1.7/open_data_project/tests/processor_test.py
+-rw-rw-rw-   0        0        0     1188 2023-04-17 16:08:21.000000 open_data_project-0.1.7/open_data_project/tests/usmart_test.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.300362 open_data_project-0.1.7/open_data_project/tools/
+-rw-rw-rw-   0        0        0      610 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/tools/README.md
+-rw-rw-rw-   0        0        0     2492 2023-04-17 16:12:13.000000 open_data_project-0.1.7/open_data_project/tools/alive.py
+-rw-rw-rw-   0        0        0     2951 2023-04-17 16:31:16.000000 open_data_project-0.1.7/open_data_project/usmart.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.303324 open_data_project-0.1.7/open_data_project/web-scrapers/
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.314355 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/
+-rw-rw-rw-   0        0        0     4769 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/aberdeenshire_council_scraper.py
+-rw-rw-rw-   0        0        0     4333 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/east_ayrshire_scraper.py
+-rw-rw-rw-   0        0        0     4504 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/moray_council_scraper.py
+-rw-rw-rw-   0        0        0    13989 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/nls_scraper.py
+-rw-rw-rw-   0        0        0     7691 2023-03-13 11:34:22.000000 open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/sqa_scraper.py
+-rw-rw-rw-   0        0        0      763 2023-04-13 18:20:31.000000 open_data_project-0.1.7/open_data_project/web-scrapers/sample_scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-12 00:08:08.120086 open_data_project-0.1.7/open_data_project.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3342 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      133 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-12 00:08:07.000000 open_data_project-0.1.7/open_data_project.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 00:08:08.318362 open_data_project-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-05-12 00:07:38.000000 open_data_project-0.1.7/setup.py
```

### Comparing `open_data_project-0.1.4/LICENSE` & `open_data_project-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/.github/LICENSE` & `open_data_project-0.1.7/open_data_project/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/.github/workflows/alive.yml` & `open_data_project-0.1.7/open_data_project/.github/workflows/alive.yml`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/.github/workflows/pipeline.yml` & `open_data_project-0.1.7/open_data_project/.github/workflows/pipeline.yml`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/.gitignore` & `open_data_project-0.1.7/open_data_project/.gitignore`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/LICENSE` & `open_data_project-0.1.7/open_data_project/LICENSE`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/ODPCategories.json` & `open_data_project-0.1.7/open_data_project/ODPCategories.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/arcgis.py` & `open_data_project-0.1.7/open_data_project/arcgis.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/ckan.py` & `open_data_project-0.1.7/open_data_project/ckan.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/USMART/Dumfries and Galloway Council.csv` & `open_data_project-0.1.7/open_data_project/data/USMART/Dumfries and Galloway Council.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/arcgis/renfrew.csv` & `open_data_project-0.1.7/open_data_project/data/arcgis/renfrew.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/ckan/Aberdeen City Council.csv` & `open_data_project-0.1.7/open_data_project/data/ckan/Aberdeen City Council.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/ckan/Spatial Hub.csv` & `open_data_project-0.1.7/open_data_project/data/ckan/Spatial Hub.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/dcat/Coral G.csv` & `open_data_project-0.1.7/open_data_project/data/dcat/Coral G.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/dcat/edinburgh.csv` & `open_data_project-0.1.7/open_data_project/data/dcat/edinburgh.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/dcat/glasgow.csv` & `open_data_project-0.1.7/open_data_project/data/dcat/glasgow.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/dcat/highland.csv` & `open_data_project-0.1.7/open_data_project/data/dcat/highland.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/merged_output.json` & `open_data_project-0.1.7/open_data_project/data/merged_output.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/merged_output_untidy.json` & `open_data_project-0.1.7/open_data_project/data/merged_output_untidy.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/data/sparkql/scotgov-datasets-sparkql.csv` & `open_data_project-0.1.7/open_data_project/data/sparkql/scotgov-datasets-sparkql.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/dcat.py` & `open_data_project-0.1.7/open_data_project/dcat.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
                 # If there's only one keyword (e.g. the property returned a string, then stick it in an array)
                 if type(keywords) is str:
                     keywords = [keywords]
             
                 ds = [
                     e.get("dct:title", ""),
-                    e.get("dct:publisher", "").replace(" Mapping", ""),
+                    e.get("dct:publisher", "").get("foaf:name","").replace(" Mapping", ""),
                     "",  # link to page
                     "",  # Link to data
                     "",  #FileName
                     "",  # date created
                     parser.parse(e.get("dct:issued", "")).date(),
                     "",  # size
                     "",  # size unit
```

### Comparing `open_data_project-0.1.4/open_data_project/error_log.md` & `open_data_project-0.1.7/open_data_project/error_log.md`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/export2jkan.py` & `open_data_project-0.1.7/open_data_project/export2jkan.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/health_checks/health_categories.py` & `open_data_project-0.1.7/open_data_project/health_checks/health_categories.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/main.sh` & `open_data_project-0.1.7/open_data_project/main.sh`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/merge_data.py` & `open_data_project-0.1.7/open_data_project/merge_data.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/odp.py` & `open_data_project-0.1.7/open_data_project/odp.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/processor.py` & `open_data_project-0.1.7/open_data_project/processor.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/sparkql_statistics.py` & `open_data_project-0.1.7/open_data_project/sparkql_statistics.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/arcgis_test.py` & `open_data_project-0.1.7/open_data_project/tests/arcgis_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/ckan_test.py` & `open_data_project-0.1.7/open_data_project/tests/ckan_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/conftest.py` & `open_data_project-0.1.7/open_data_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/dcat_test.py` & `open_data_project-0.1.7/open_data_project/tests/dcat_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/export2jkan_test.py` & `open_data_project-0.1.7/open_data_project/tests/export2jkan_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/generate_new_mock_data.py` & `open_data_project-0.1.7/open_data_project/tests/generate_new_mock_data.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/how_to_test.md` & `open_data_project-0.1.7/open_data_project/tests/how_to_test.md`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/merge_data_test.py` & `open_data_project-0.1.7/open_data_project/tests/merge_data_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/expected/renfrew.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/expected/renfrew.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/arcgis/renfrew.json` & `open_data_project-0.1.7/open_data_project/tests/mock_data/arcgis/renfrew.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/expected/glasgow.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/expected/glasgow.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/dcat/glasgow.json` & `open_data_project-0.1.7/open_data_project/tests/mock_data/dcat/glasgow.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/get_json_data.json` & `open_data_project-0.1.7/open_data_project/tests/mock_data/get_json_data.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/output/arcgis/renfrew.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/output/arcgis/renfrew.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/output/dcat/glasgow.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/output/dcat/glasgow.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/output/usmart/Dumfries and Galloway Council.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/output/usmart/Dumfries and Galloway Council.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/Dumfries and Galloway Council.json` & `open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/Dumfries and Galloway Council.json`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/mock_data/usmart/expected/Dumfries and Galloway Council.csv` & `open_data_project-0.1.7/open_data_project/tests/mock_data/usmart/expected/Dumfries and Galloway Council.csv`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/processor_test.py` & `open_data_project-0.1.7/open_data_project/tests/processor_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tests/usmart_test.py` & `open_data_project-0.1.7/open_data_project/tests/usmart_test.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tools/README.md` & `open_data_project-0.1.7/open_data_project/tools/README.md`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/tools/alive.py` & `open_data_project-0.1.7/open_data_project/tools/alive.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/usmart.py` & `open_data_project-0.1.7/open_data_project/usmart.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/aberdeenshire_council_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/aberdeenshire_council_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/east_ayrshire_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/east_ayrshire_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/moray_council_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/moray_council_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/nls_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/nls_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/Open Data Scotland example scrapers/sqa_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/Open Data Scotland example scrapers/sqa_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project/web-scrapers/sample_scraper.py` & `open_data_project-0.1.7/open_data_project/web-scrapers/sample_scraper.py`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/open_data_project.egg-info/SOURCES.txt` & `open_data_project-0.1.7/open_data_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_data_project-0.1.4/setup.py` & `open_data_project-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "open_data_project",
-    version = "0.1.4",
+    version = "0.1.7",
     author = "Danail Dimov",
     author_email = "d.dimov62@gmail.com",
     description = "A Python package to retrieve the data for your open data portal and to launch the front-end structure for its website.",
     packages = find_packages(),
     include_package_data = True,
     install_requires = ["beautifulsoup4",
                         "black",
```

