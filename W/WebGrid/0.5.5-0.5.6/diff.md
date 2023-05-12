# Comparing `tmp/WebGrid-0.5.5.tar.gz` & `tmp/WebGrid-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebGrid-0.5.5.tar", last modified: Fri May 12 12:21:32 2023, max compression
+gzip compressed data, was "WebGrid-0.5.6.tar", last modified: Fri May 12 19:51:46 2023, max compression
```

## Comparing `WebGrid-0.5.5.tar` & `WebGrid-0.5.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2018-11-14 14:19:49.000000 WebGrid-0.5.5/MANIFEST.in
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26652 2023-05-12 12:21:32.096712 WebGrid-0.5.5/PKG-INFO
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/WebGrid.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26652 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2385 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       62 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/entry_points.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2017-06-09 12:44:59.000000 WebGrid-0.5.5/WebGrid.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      341 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        8 2023-05-12 12:21:31.000000 WebGrid-0.5.5/WebGrid.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    23795 2023-05-12 12:18:54.000000 WebGrid-0.5.5/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2191 2021-02-01 15:18:26.000000 WebGrid-0.5.5/readme.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      504 2023-05-12 12:21:32.096712 WebGrid-0.5.5/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2166 2023-05-12 12:18:10.000000 WebGrid-0.5.5/setup.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    69073 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2404 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid/blazeweb.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19193 2022-11-07 21:26:35.000000 WebGrid-0.5.5/webgrid/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    66363 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/filters.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11174 2022-07-25 15:25:24.000000 WebGrid-0.5.5/webgrid/flask.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5320 2023-01-21 00:19:49.000000 WebGrid-0.5.5/webgrid/i18n/es/LC_MESSAGES/webgrid.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9220 2023-01-21 00:19:49.000000 WebGrid-0.5.5/webgrid/i18n/es/LC_MESSAGES/webgrid.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7103 2023-01-21 00:19:49.000000 WebGrid-0.5.5/webgrid/i18n/webgrid.pot
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    62175 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/renderers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/static/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      714 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/application_form_edit.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/b_firstpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/b_lastpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/b_nextpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/b_prevpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/bd_firstpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/bd_lastpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/bd_nextpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/bd_prevpage.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      715 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/delete.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3430 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid/static/gettext.min.js
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/static/i18n/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/static/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/static/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4694 2023-01-21 00:19:49.000000 WebGrid-0.5.5/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    14611 2019-11-26 15:27:36.000000 WebGrid-0.5.5/webgrid/static/jquery.multiple.select.js
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4149 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/multiple-select.css
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3342 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/multiple-select.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      528 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/th_arrow_down.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      514 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/static/th_arrow_up.png
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6503 2020-12-09 21:12:41.000000 WebGrid-0.5.5/webgrid/static/webgrid.css
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    16355 2022-12-12 16:06:22.000000 WebGrid-0.5.5/webgrid/static/webgrid.js
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      570 2020-05-15 19:26:27.000000 WebGrid-0.5.5/webgrid/templates/grid.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2101 2023-01-20 13:59:08.000000 WebGrid-0.5.5/webgrid/templates/grid_footer.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1180 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid/templates/grid_header.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2020-05-15 19:26:27.000000 WebGrid-0.5.5/webgrid/templates/grid_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      351 2020-11-04 20:29:48.000000 WebGrid-0.5.5/webgrid/templates/header_filtering.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      517 2020-10-09 20:16:24.000000 WebGrid-0.5.5/webgrid/templates/header_paging.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      331 2020-10-09 20:16:24.000000 WebGrid-0.5.5/webgrid/templates/header_sorting.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19686 2023-01-20 13:59:08.000000 WebGrid-0.5.5/webgrid/testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      271 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid/tests/conftest.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid/tests/data/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1483 2020-10-09 20:16:24.000000 WebGrid-0.5.5/webgrid/tests/data/basic_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1788 2019-09-04 13:29:02.000000 WebGrid-0.5.5/webgrid/tests/data/people_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4262 2020-04-09 13:05:21.000000 WebGrid-0.5.5/webgrid/tests/data/stopwatch_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1532 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid/tests/helpers.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8796 2022-10-18 13:32:21.000000 WebGrid-0.5.5/webgrid/tests/test_api.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13006 2023-03-02 19:26:02.000000 WebGrid-0.5.5/webgrid/tests/test_columns.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    76322 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/tests/test_filters.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    50216 2023-02-24 14:00:14.000000 WebGrid-0.5.5/webgrid/tests/test_rendering.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7880 2023-01-20 13:59:08.000000 WebGrid-0.5.5/webgrid/tests/test_testing.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3123 2023-02-24 14:00:14.000000 WebGrid-0.5.5/webgrid/tests/test_types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    48966 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/tests/test_unit.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3882 2022-10-18 13:32:21.000000 WebGrid-0.5.5/webgrid/types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1845 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid/utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3184 2023-05-12 12:18:10.000000 WebGrid-0.5.5/webgrid/validators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-12 12:18:31.000000 WebGrid-0.5.5/webgrid/version.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid_ta/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1644 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid_ta/app.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/data/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1479 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid_ta/data/basic_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1634 2017-06-09 12:44:51.000000 WebGrid-0.5.5/webgrid_ta/data/people_table.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      980 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5073 2023-01-20 13:59:08.000000 WebGrid-0.5.5/webgrid_ta/grids.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2030 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid_ta/helpers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1336 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2255 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1897 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/i18n/webgrid_ta.pot
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1382 2021-09-10 16:32:05.000000 WebGrid-0.5.5/webgrid_ta/manage.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1704 2020-04-09 13:05:21.000000 WebGrid-0.5.5/webgrid_ta/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4307 2023-02-24 14:00:14.000000 WebGrid-0.5.5/webgrid_ta/model/entities.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17708 2020-01-10 14:33:11.000000 WebGrid-0.5.5/webgrid_ta/model/helpers.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 12:21:32.096712 WebGrid-0.5.5/webgrid_ta/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      829 2020-04-09 13:05:21.000000 WebGrid-0.5.5/webgrid_ta/templates/groups.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1772 2018-11-14 14:19:49.000000 WebGrid-0.5.5/webgrid_ta/templates/index.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1080 2020-10-09 20:16:24.000000 WebGrid-0.5.5/webgrid_ta/views.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2018-11-14 14:19:49.000000 WebGrid-0.5.6/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26815 2023-05-12 19:51:46.489994 WebGrid-0.5.6/PKG-INFO
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.477994 WebGrid-0.5.6/WebGrid.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26815 2023-05-12 19:51:45.000000 WebGrid-0.5.6/WebGrid.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2385 2023-05-12 19:51:46.000000 WebGrid-0.5.6/WebGrid.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 19:51:45.000000 WebGrid-0.5.6/WebGrid.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       62 2023-05-12 19:51:45.000000 WebGrid-0.5.6/WebGrid.egg-info/entry_points.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2017-06-09 12:44:59.000000 WebGrid-0.5.6/WebGrid.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      341 2023-05-12 19:51:46.000000 WebGrid-0.5.6/WebGrid.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        8 2023-05-12 19:51:46.000000 WebGrid-0.5.6/WebGrid.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    23958 2023-05-12 19:51:26.000000 WebGrid-0.5.6/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2191 2021-02-01 15:18:26.000000 WebGrid-0.5.6/readme.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      504 2023-05-12 19:51:46.489994 WebGrid-0.5.6/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2166 2023-05-12 12:18:10.000000 WebGrid-0.5.6/setup.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    69073 2023-05-12 12:18:10.000000 WebGrid-0.5.6/webgrid/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2404 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid/blazeweb.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19193 2022-11-07 21:26:35.000000 WebGrid-0.5.6/webgrid/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    66490 2023-05-12 19:50:51.000000 WebGrid-0.5.6/webgrid/filters.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11174 2022-07-25 15:25:24.000000 WebGrid-0.5.6/webgrid/flask.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.477994 WebGrid-0.5.6/webgrid/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5320 2023-01-21 00:19:49.000000 WebGrid-0.5.6/webgrid/i18n/es/LC_MESSAGES/webgrid.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9220 2023-01-21 00:19:49.000000 WebGrid-0.5.6/webgrid/i18n/es/LC_MESSAGES/webgrid.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7103 2023-01-21 00:19:49.000000 WebGrid-0.5.6/webgrid/i18n/webgrid.pot
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    62283 2023-05-12 19:50:51.000000 WebGrid-0.5.6/webgrid/renderers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/static/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      714 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/application_form_edit.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/b_firstpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/b_lastpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/b_nextpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/b_prevpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      238 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/bd_firstpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      236 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/bd_lastpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      221 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/bd_nextpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      225 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/bd_prevpage.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      715 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/delete.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3430 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid/static/gettext.min.js
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.477994 WebGrid-0.5.6/webgrid/static/i18n/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.477994 WebGrid-0.5.6/webgrid/static/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/static/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4694 2023-01-21 00:19:49.000000 WebGrid-0.5.6/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    14611 2019-11-26 15:27:36.000000 WebGrid-0.5.6/webgrid/static/jquery.multiple.select.js
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4149 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/multiple-select.css
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3342 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/multiple-select.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      528 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/th_arrow_down.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      514 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/static/th_arrow_up.png
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6503 2020-12-09 21:12:41.000000 WebGrid-0.5.6/webgrid/static/webgrid.css
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    16355 2022-12-12 16:06:22.000000 WebGrid-0.5.6/webgrid/static/webgrid.js
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.481994 WebGrid-0.5.6/webgrid/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      570 2020-05-15 19:26:27.000000 WebGrid-0.5.6/webgrid/templates/grid.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2101 2023-01-20 13:59:08.000000 WebGrid-0.5.6/webgrid/templates/grid_footer.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1180 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid/templates/grid_header.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      388 2020-05-15 19:26:27.000000 WebGrid-0.5.6/webgrid/templates/grid_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      351 2020-11-04 20:29:48.000000 WebGrid-0.5.6/webgrid/templates/header_filtering.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      517 2020-10-09 20:16:24.000000 WebGrid-0.5.6/webgrid/templates/header_paging.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      331 2020-10-09 20:16:24.000000 WebGrid-0.5.6/webgrid/templates/header_sorting.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19686 2023-01-20 13:59:08.000000 WebGrid-0.5.6/webgrid/testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      271 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid/tests/conftest.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid/tests/data/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1483 2020-10-09 20:16:24.000000 WebGrid-0.5.6/webgrid/tests/data/basic_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1788 2019-09-04 13:29:02.000000 WebGrid-0.5.6/webgrid/tests/data/people_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4262 2020-04-09 13:05:21.000000 WebGrid-0.5.6/webgrid/tests/data/stopwatch_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1532 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid/tests/helpers.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8796 2022-10-18 13:32:21.000000 WebGrid-0.5.6/webgrid/tests/test_api.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    13006 2023-03-02 19:26:02.000000 WebGrid-0.5.6/webgrid/tests/test_columns.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    76322 2023-05-12 12:18:10.000000 WebGrid-0.5.6/webgrid/tests/test_filters.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    50216 2023-02-24 14:00:14.000000 WebGrid-0.5.6/webgrid/tests/test_rendering.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7880 2023-01-20 13:59:08.000000 WebGrid-0.5.6/webgrid/tests/test_testing.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3123 2023-02-24 14:00:14.000000 WebGrid-0.5.6/webgrid/tests/test_types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    48966 2023-05-12 12:18:10.000000 WebGrid-0.5.6/webgrid/tests/test_unit.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3882 2022-10-18 13:32:21.000000 WebGrid-0.5.6/webgrid/types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1845 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3184 2023-05-12 12:18:10.000000 WebGrid-0.5.6/webgrid/validators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-12 19:51:06.000000 WebGrid-0.5.6/webgrid/version.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid_ta/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1644 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid_ta/app.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/data/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1479 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid_ta/data/basic_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1634 2017-06-09 12:44:51.000000 WebGrid-0.5.6/webgrid_ta/data/people_table.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      980 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     5073 2023-01-20 13:59:08.000000 WebGrid-0.5.6/webgrid_ta/grids.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2030 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid_ta/helpers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      114 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.477994 WebGrid-0.5.6/webgrid_ta/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1336 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2255 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1897 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/i18n/webgrid_ta.pot
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1382 2021-09-10 16:32:05.000000 WebGrid-0.5.6/webgrid_ta/manage.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1704 2020-04-09 13:05:21.000000 WebGrid-0.5.6/webgrid_ta/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4307 2023-02-24 14:00:14.000000 WebGrid-0.5.6/webgrid_ta/model/entities.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17708 2020-01-10 14:33:11.000000 WebGrid-0.5.6/webgrid_ta/model/helpers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:51:46.485994 WebGrid-0.5.6/webgrid_ta/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      829 2020-04-09 13:05:21.000000 WebGrid-0.5.6/webgrid_ta/templates/groups.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1772 2018-11-14 14:19:49.000000 WebGrid-0.5.6/webgrid_ta/templates/index.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1080 2020-10-09 20:16:24.000000 WebGrid-0.5.6/webgrid_ta/views.py
```

### Comparing `WebGrid-0.5.5/PKG-INFO` & `WebGrid-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebGrid
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library for rendering HTML tables and Excel files from SQLAlchemy models.
 Home-page: https://github.com/level12/webgrid
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 * Issue tracker: https://github.com/level12/webgrid/issues
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.5.6 released 2023-05-12
+-------------------------
+
+- fix options validator instance (400288b_)
+
+.. _400288b: https://github.com/level12/webgrid/commit/400288b
+
+
 0.5.5 released 2023-05-12
 -------------------------
 
 - drop formencode dependency in favor of internal validation (9575f12_)
 
 .. _9575f12: https://github.com/level12/webgrid/commit/9575f12
```

### Comparing `WebGrid-0.5.5/WebGrid.egg-info/PKG-INFO` & `WebGrid-0.5.6/WebGrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebGrid
-Version: 0.5.5
+Version: 0.5.6
 Summary: A library for rendering HTML tables and Excel files from SQLAlchemy models.
 Home-page: https://github.com/level12/webgrid
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 * Issue tracker: https://github.com/level12/webgrid/issues
 * Questions & comments: http://groups.google.com/group/blazelibs
 
 
 Changelog
 =========
 
+0.5.6 released 2023-05-12
+-------------------------
+
+- fix options validator instance (400288b_)
+
+.. _400288b: https://github.com/level12/webgrid/commit/400288b
+
+
 0.5.5 released 2023-05-12
 -------------------------
 
 - drop formencode dependency in favor of internal validation (9575f12_)
 
 .. _9575f12: https://github.com/level12/webgrid/commit/9575f12
```

### Comparing `WebGrid-0.5.5/WebGrid.egg-info/SOURCES.txt` & `WebGrid-0.5.6/WebGrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/changelog.rst` & `WebGrid-0.5.6/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.5.6 released 2023-05-12
+-------------------------
+
+- fix options validator instance (400288b_)
+
+.. _400288b: https://github.com/level12/webgrid/commit/400288b
+
+
 0.5.5 released 2023-05-12
 -------------------------
 
 - drop formencode dependency in favor of internal validation (9575f12_)
 
 .. _9575f12: https://github.com/level12/webgrid/commit/9575f12
```

### Comparing `WebGrid-0.5.5/readme.rst` & `WebGrid-0.5.6/readme.rst`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/setup.py` & `WebGrid-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/__init__.py` & `WebGrid-0.5.6/webgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/blazeweb.py` & `WebGrid-0.5.6/webgrid/blazeweb.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/extensions.py` & `WebGrid-0.5.6/webgrid/extensions.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/filters.py` & `WebGrid-0.5.6/webgrid/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,18 @@
             self.op = None
 
         self.value1_set_with = values
 
     def process(self, value):
         """Apply the `value_modifier` to a value."""
         if self.value_modifier is not None:
-            value = self.value_modifier.process(value)
+            validator = self.value_modifier
+            if inspect.isclass(self.value_modifier):
+                validator = validator()
+            value = validator.process(value)
             if value not in self.option_keys:
                 return _NoValue
             if self.default_op and value == -1:
                 return _NoValue
         return value
 
     def match_keys_for_value(self, value):
```

### Comparing `WebGrid-0.5.5/webgrid/flask.py` & `WebGrid-0.5.6/webgrid/flask.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/i18n/es/LC_MESSAGES/webgrid.mo` & `WebGrid-0.5.6/webgrid/i18n/es/LC_MESSAGES/webgrid.mo`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/i18n/es/LC_MESSAGES/webgrid.po` & `WebGrid-0.5.6/webgrid/i18n/es/LC_MESSAGES/webgrid.po`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/i18n/webgrid.pot` & `WebGrid-0.5.6/webgrid/i18n/webgrid.pot`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/renderers.py` & `WebGrid-0.5.6/webgrid/renderers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import absolute_import
 
 import re
 from abc import ABC, abstractmethod
 from dataclasses import asdict
+import inspect
 import io
 from operator import itemgetter
 from collections import defaultdict
 import json
 from typing import Dict, Union
 
 import six
@@ -547,14 +548,17 @@
             options=options,
         )
 
     def filtering_filter_options_multi(self, filter, field_name):
         """Render the multiselect options."""
         # Assume the multiselect filter has been set up with OptionsFilterBase.setup_validator
         selected = filter.value1 or []
+        validator = filter.value_modifier
+        if inspect.isclass(validator):
+            validator = validator()
         return self._render_jinja(
             '''
             {% for value, label in filter.options_seq %}
                 <li>
                     <label>
                         <input
                             {% if transform(value) in selected %}checked{% endif %}
@@ -566,15 +570,15 @@
                     </label>
                 </li>
             {% endfor %}
             ''',
             filter=filter,
             field_name=field_name,
             selected=selected,
-            transform=filter.value_modifier.process if filter.value_modifier else lambda x: x,
+            transform=validator.process if validator else lambda x: x,
         )
 
     def filtering_col_inputs2(self, col):
         """Render the second filter input, currently only a freeform."""
         filter = col.filter
         field_name = 'v2({0})'.format(col.key)
         field_name = self.grid.prefix_qs_arg_key(field_name)
```

### Comparing `WebGrid-0.5.5/webgrid/static/application_form_edit.png` & `WebGrid-0.5.6/webgrid/static/application_form_edit.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/delete.png` & `WebGrid-0.5.6/webgrid/static/delete.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/gettext.min.js` & `WebGrid-0.5.6/webgrid/static/gettext.min.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json` & `WebGrid-0.5.6/webgrid/static/i18n/es/LC_MESSAGES/webgrid.json`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/jquery.multiple.select.js` & `WebGrid-0.5.6/webgrid/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/multiple-select.css` & `WebGrid-0.5.6/webgrid/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/multiple-select.png` & `WebGrid-0.5.6/webgrid/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/th_arrow_down.png` & `WebGrid-0.5.6/webgrid/static/th_arrow_down.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/th_arrow_up.png` & `WebGrid-0.5.6/webgrid/static/th_arrow_up.png`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/webgrid.css` & `WebGrid-0.5.6/webgrid/static/webgrid.css`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/static/webgrid.js` & `WebGrid-0.5.6/webgrid/static/webgrid.js`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/templates/grid.html` & `WebGrid-0.5.6/webgrid/templates/grid.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/templates/grid_footer.html` & `WebGrid-0.5.6/webgrid/templates/grid_footer.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/templates/grid_header.html` & `WebGrid-0.5.6/webgrid/templates/grid_header.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/templates/header_paging.html` & `WebGrid-0.5.6/webgrid/templates/header_paging.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/testing.py` & `WebGrid-0.5.6/webgrid/testing.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/data/basic_table.html` & `WebGrid-0.5.6/webgrid/tests/data/basic_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/data/people_table.html` & `WebGrid-0.5.6/webgrid/tests/data/people_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/data/stopwatch_table.html` & `WebGrid-0.5.6/webgrid/tests/data/stopwatch_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/helpers.py` & `WebGrid-0.5.6/webgrid/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_api.py` & `WebGrid-0.5.6/webgrid/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_columns.py` & `WebGrid-0.5.6/webgrid/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_filters.py` & `WebGrid-0.5.6/webgrid/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_rendering.py` & `WebGrid-0.5.6/webgrid/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_testing.py` & `WebGrid-0.5.6/webgrid/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_types.py` & `WebGrid-0.5.6/webgrid/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/tests/test_unit.py` & `WebGrid-0.5.6/webgrid/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/types.py` & `WebGrid-0.5.6/webgrid/types.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/utils.py` & `WebGrid-0.5.6/webgrid/utils.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid/validators.py` & `WebGrid-0.5.6/webgrid/validators.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/app.py` & `WebGrid-0.5.6/webgrid_ta/app.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/data/basic_table.html` & `WebGrid-0.5.6/webgrid_ta/data/basic_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/data/people_table.html` & `WebGrid-0.5.6/webgrid_ta/data/people_table.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/extensions.py` & `WebGrid-0.5.6/webgrid_ta/extensions.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/grids.py` & `WebGrid-0.5.6/webgrid_ta/grids.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/helpers.py` & `WebGrid-0.5.6/webgrid_ta/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo` & `WebGrid-0.5.6/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.mo`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po` & `WebGrid-0.5.6/webgrid_ta/i18n/es/LC_MESSAGES/webgrid_ta.po`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/i18n/webgrid_ta.pot` & `WebGrid-0.5.6/webgrid_ta/i18n/webgrid_ta.pot`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/manage.py` & `WebGrid-0.5.6/webgrid_ta/manage.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/model/__init__.py` & `WebGrid-0.5.6/webgrid_ta/model/__init__.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/model/entities.py` & `WebGrid-0.5.6/webgrid_ta/model/entities.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/model/helpers.py` & `WebGrid-0.5.6/webgrid_ta/model/helpers.py`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/templates/groups.html` & `WebGrid-0.5.6/webgrid_ta/templates/groups.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/templates/index.html` & `WebGrid-0.5.6/webgrid_ta/templates/index.html`

 * *Files identical despite different names*

### Comparing `WebGrid-0.5.5/webgrid_ta/views.py` & `WebGrid-0.5.6/webgrid_ta/views.py`

 * *Files identical despite different names*

