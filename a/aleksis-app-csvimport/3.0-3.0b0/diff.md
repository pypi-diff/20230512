# Comparing `tmp/aleksis_app_csvimport-3.0.tar.gz` & `tmp/aleksis_app_csvimport-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_csvimport-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_csvimport-3.0b0.tar", max compression
```

## Comparing `aleksis_app_csvimport-3.0.tar` & `aleksis_app_csvimport-3.0b0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0     6113 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1594 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/README.rst
--rw-r--r--   0        0        0      155 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__init__.py
--rw-r--r--   0        0        0      454 2023-05-12 16:57:44.873428 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      421 2023-05-12 16:57:47.069533 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     1977 2023-05-12 16:57:45.545460 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     1525 2023-05-12 16:57:47.329545 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/default_templates.cpython-311.pyc
--rw-r--r--   0        0        0    30602 2023-05-12 16:57:46.465504 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc
--rw-r--r--   0        0        0      704 2023-05-12 16:57:47.129536 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0    11426 2023-05-12 16:57:46.457504 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     2891 2023-05-12 16:57:47.169538 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1134 2023-05-12 16:57:47.089534 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      435 2023-05-12 16:57:44.873428 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0      129 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/admin.py
--rw-r--r--   0        0        0     1258 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/apps.py
--rw-r--r--   0        0        0      603 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/default_templates.py
--rw-r--r--   0        0        0     4758 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/default_templates.yaml
--rw-r--r--   0        0        0    15561 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/field_types.py
--rw-r--r--   0        0        0     1946 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/forms.py
--rw-r--r--   0        0        0     1469 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/index.js
--rw-r--r--   0        0        0      187 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/messages/de.json
--rw-r--r--   0        0        0      182 2023-05-12 16:55:09.814056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/messages/en.json
--rw-r--r--   0        0        0      225 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/messages/ru.json
--rw-r--r--   0        0        0      221 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/messages/uk.json
--rw-r--r--   0        0        0      463 2023-05-12 16:57:47.381548 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9782 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8154 2023-05-12 16:57:47.385548 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15409 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-12 16:57:47.385548 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9698 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-12 16:57:47.369547 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-12 16:57:47.373547 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10397 2023-05-12 16:57:47.373547 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15137 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-12 16:57:47.389548 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9652 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10206 2023-05-12 16:57:47.385548 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14949 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/management/commands/__init__.py
--rw-r--r--   0        0        0     1875 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/management/commands/csv_import.py
--rw-r--r--   0        0        0      718 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/menus.py
--rw-r--r--   0        0        0     7500 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0001_initial.py
--rw-r--r--   0        0        0     1549 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0002_importjob.py
--rw-r--r--   0        0        0      510 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0003_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      540 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0004_args.py
--rw-r--r--   0        0        0      479 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0005_optional_index_col.py
--rw-r--r--   0        0        0      438 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0006_from_default_field.py
--rw-r--r--   0        0        0      709 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py
--rw-r--r--   0        0        0      486 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0008_configurable_quotechar.py
--rw-r--r--   0        0        0        0 2023-05-12 16:55:09.818056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/__init__.py
--rw-r--r--   0        0        0      274 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/model_extensions.py
--rw-r--r--   0        0        0     7521 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/models.py
--rw-r--r--   0        0        0     1573 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/preferences.py
--rw-r--r--   0        0        0      851 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/rules.py
--rw-r--r--   0        0        0      239 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/settings.py
--rw-r--r--   0        0        0      340 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tables.py
--rw-r--r--   0        0        0      373 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tasks.py
--rw-r--r--   0        0        0      934 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/csv_import.html
--rw-r--r--   0        0        0      709 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html
--rw-r--r--   0        0        0      518 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html
--rw-r--r--   0        0        0     1067 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/models/test_template.py
--rw-r--r--   0        0        0     3217 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/models/test_template_load.py
--rw-r--r--   0        0        0     2954 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/test_field_types.py
--rw-r--r--   0        0        0     3358 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py
--rw-r--r--   0        0        0     2876 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/util/test_converters.py
--rw-r--r--   0        0        0      365 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/util/test_import_helpers.py
--rw-r--r--   0        0        0      334 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/urls.py
--rw-r--r--   0        0        0     5561 2023-05-12 16:57:46.465504 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     4538 2023-05-12 16:57:46.465504 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc
--rw-r--r--   0        0        0      732 2023-05-12 16:57:47.017530 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     3824 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/class_range_helpers.py
--rw-r--r--   0        0        0     2274 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/converters.py
--rw-r--r--   0        0        0      359 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/import_helpers.py
--rw-r--r--   0        0        0    12255 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/process.py
--rw-r--r--   0        0        0     2867 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/aleksis/apps/csv_import/views.py
--rw-r--r--   0        0        0      581 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/docs/Makefile
--rw-r--r--   0        0        0      104 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1355 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/docs/admin/01_concept.rst
--rw-r--r--   0        0        0      836 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/docs/admin/05_configuration.rst
--rw-r--r--   0        0        0      619 2023-05-12 16:55:09.822056 aleksis_app_csvimport-3.0/docs/admin/10_exporting_data.rst
--rw-r--r--   0        0        0     1076 2023-05-12 16:55:09.826056 aleksis_app_csvimport-3.0/docs/admin/20_import_data.rst
--rw-r--r--   0        0        0     6400 2023-05-12 16:55:09.826056 aleksis_app_csvimport-3.0/docs/conf.py
--rw-r--r--   0        0        0      532 2023-05-12 16:55:09.826056 aleksis_app_csvimport-3.0/docs/index.rst
--rw-r--r--   0        0        0      787 2023-05-12 16:55:09.826056 aleksis_app_csvimport-3.0/docs/make.bat
--rw-r--r--   0        0        0     1572 2023-05-12 16:55:39.711478 aleksis_app_csvimport-3.0/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-05-12 16:55:09.826056 aleksis_app_csvimport-3.0/tox.ini
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0/setup.py
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0/PKG-INFO
+-rw-r--r--   0        0        0     5835 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1594 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/README.rst
+-rw-r--r--   0        0        0      155 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__init__.py
+-rw-r--r--   0        0        0      454 2023-02-27 16:45:50.770732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      421 2023-02-27 16:45:52.554729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     1977 2023-02-27 16:45:51.310732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     1525 2023-02-27 16:45:52.766729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/default_templates.cpython-311.pyc
+-rw-r--r--   0        0        0    30602 2023-02-27 16:45:52.098730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc
+-rw-r--r--   0        0        0      704 2023-02-27 16:45:52.594729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0    11426 2023-02-27 16:45:52.090730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     2891 2023-02-27 16:45:52.626729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1134 2023-02-27 16:45:52.570729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      435 2023-02-27 16:45:50.778732 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/admin.py
+-rw-r--r--   0        0        0     1258 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/apps.py
+-rw-r--r--   0        0        0      603 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.py
+-rw-r--r--   0        0        0     4758 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.yaml
+-rw-r--r--   0        0        0    15561 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/field_types.py
+-rw-r--r--   0        0        0     1946 2023-02-27 16:28:05.444782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/forms.py
+-rw-r--r--   0        0        0     1469 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/index.js
+-rw-r--r--   0        0        0      187 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/de.json
+-rw-r--r--   0        0        0      182 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/en.json
+-rw-r--r--   0        0        0      225 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/ru.json
+-rw-r--r--   0        0        0      221 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2023-02-27 16:45:52.858729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9782 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8154 2023-02-27 16:45:52.850729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15409 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-02-27 16:45:52.846729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9698 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.858729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.838729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10397 2023-02-27 16:45:52.846729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15137 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-02-27 16:45:52.854729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9652 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10206 2023-02-27 16:45:52.842728 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14949 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/__init__.py
+-rw-r--r--   0        0        0     1875 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/csv_import.py
+-rw-r--r--   0        0        0      718 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/menus.py
+-rw-r--r--   0        0        0     7500 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1549 2023-02-27 16:28:05.448782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0002_importjob.py
+-rw-r--r--   0        0        0      510 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0003_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      540 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0004_args.py
+-rw-r--r--   0        0        0      479 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0005_optional_index_col.py
+-rw-r--r--   0        0        0      438 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0006_from_default_field.py
+-rw-r--r--   0        0        0      709 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py
+-rw-r--r--   0        0        0      486 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0008_configurable_quotechar.py
+-rw-r--r--   0        0        0        0 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/__init__.py
+-rw-r--r--   0        0        0      274 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/model_extensions.py
+-rw-r--r--   0        0        0     7521 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/models.py
+-rw-r--r--   0        0        0     1573 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/preferences.py
+-rw-r--r--   0        0        0      851 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/rules.py
+-rw-r--r--   0        0        0      239 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/settings.py
+-rw-r--r--   0        0        0      340 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tables.py
+-rw-r--r--   0        0        0      373 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tasks.py
+-rw-r--r--   0        0        0      934 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/csv_import.html
+-rw-r--r--   0        0        0      709 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html
+-rw-r--r--   0        0        0      518 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html
+-rw-r--r--   0        0        0     1067 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template.py
+-rw-r--r--   0        0        0     3217 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template_load.py
+-rw-r--r--   0        0        0     2954 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/test_field_types.py
+-rw-r--r--   0        0        0     3358 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py
+-rw-r--r--   0        0        0     2934 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_converters.py
+-rw-r--r--   0        0        0      365 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_import_helpers.py
+-rw-r--r--   0        0        0      334 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/urls.py
+-rw-r--r--   0        0        0     5561 2023-02-27 16:45:52.102730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     4528 2023-02-27 16:45:52.102730 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc
+-rw-r--r--   0        0        0      732 2023-02-27 16:45:52.518729 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     3824 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/class_range_helpers.py
+-rw-r--r--   0        0        0     2295 2023-02-27 16:28:05.452782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/converters.py
+-rw-r--r--   0        0        0      359 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/import_helpers.py
+-rw-r--r--   0        0        0    12255 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/process.py
+-rw-r--r--   0        0        0     2867 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/views.py
+-rw-r--r--   0        0        0      581 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/Makefile
+-rw-r--r--   0        0        0      104 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1355 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/01_concept.rst
+-rw-r--r--   0        0        0      836 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/05_configuration.rst
+-rw-r--r--   0        0        0      619 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/10_exporting_data.rst
+-rw-r--r--   0        0        0     1076 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/admin/20_import_data.rst
+-rw-r--r--   0        0        0     6402 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/conf.py
+-rw-r--r--   0        0        0      532 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/docs/make.bat
+-rw-r--r--   0        0        0     1576 2023-02-27 16:43:10.143036 aleksis_app_csvimport-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-02-27 16:28:05.456782 aleksis_app_csvimport-3.0b0/tox.ini
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0b0/setup.py
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 aleksis_app_csvimport-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_csvimport-3.0/CHANGELOG.rst` & `aleksis_app_csvimport-3.0b0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2023-05-12
--------------------
-
-Changed
-~~~~~~~
-
-* Ukrainian translations were updated.
-* Phonenumber country is now configured using the `PHONENUMBER_DEFAULT_REGION` setting.
-
-`3.0b0`_ - 2023-02-22
----------------------
+`3.0b0` - 2023-02-22
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -203,20 +194,19 @@
 ~~~~~
 
 * Use bootstrap buttons everywhere.
 
 .. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
-.. _1.0a1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/1.0a1
-.. _1.0a2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/1.0a2
-.. _2.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0b0
-.. _2.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0b1
-.. _2.0rc1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0rc1
-.. _2.0rc2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0rc2
-.. _2.0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.0
-.. _2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.1
-.. _2.2: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.2
-.. _2.2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.2.1
-.. _2.3: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/2.3
-.. _3.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/3.0b0
-.. _3.0: https://edugit.org/AlekSIS/official/AlekSIS-App-CSVImport/-/tags/3.0
+.. _1.0a1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/1.0a1
+.. _1.0a2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/1.0a2
+.. _2.0b0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0b0
+.. _2.0b1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0b1
+.. _2.0rc1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0rc1
+.. _2.0rc2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0rc2
+.. _2.0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.0
+.. _2.1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.1
+.. _2.2: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.2
+.. _2.2.1: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.2.1
+.. _2.3: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/2.3
+.. _3.0b0: https://edugit.org/Teckids/AlekSIS/AlekSIS-App-CSVImport/-/tags/3.0b0
```

### Comparing `aleksis_app_csvimport-3.0/LICENCE.rst` & `aleksis_app_csvimport-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/README.rst` & `aleksis_app_csvimport-3.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/apps.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 1258
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/default_templates.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/default_templates.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 603
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/field_types.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 15561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 274
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 7521
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/preferences.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 1573
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/__pycache__/rules.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 851
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/apps.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/default_templates.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/default_templates.yaml` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/default_templates.yaml`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/field_types.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/field_types.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/forms.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/frontend/index.js` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/management/commands/csv_import.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/management/commands/csv_import.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/menus.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/menus.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0001_initial.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0002_importjob.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0002_importjob.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0004_args.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0004_args.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/migrations/0007_virtual_template_field.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/models.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/preferences.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/rules.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/csv_import.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/csv_import.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/templates/csv_import/import_template/upload.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/models/test_template.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/models/test_template_load.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/models/test_template_load.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/test_field_types.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/test_field_types.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_class_range_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/tests/util/test_converters.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/tests/util/test_converters.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     parse_sex,
 )
 from aleksis.core.util.core_helpers import get_site_preferences
 
 pytestmark = pytest.mark.django_db
 
 
-def test_parse_phone_number(settings):
-    settings.PHONENUMBER_DEFAULT_REGION = "DE"
+def test_parse_phone_number():
+    get_site_preferences()["internationalisation__phone_number_country"] = "DE"
     fake_number = PhoneNumber(country_code=49, national_number=1635550217)
     assert parse_phone_number("+49-163-555-0217") == fake_number
     assert parse_phone_number("+491635550217") == fake_number
     assert parse_phone_number("0163-555-0217") == fake_number
     assert parse_phone_number("01635550217") == fake_number
-    settings.PHONENUMBER_DEFAULT_REGION = "GB"
+    get_site_preferences()["internationalisation__phone_number_country"] = "GB"
     assert parse_phone_number("0163-555-0217") != fake_number
     assert parse_phone_number("01635550217") != fake_number
 
 
 def test_parse_phone_number_none():
     assert parse_phone_number("") == ""
     assert parse_phone_number("foo") == ""
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/class_range_helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 3824
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/converters.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
-files sz: 2274
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
+files sz: 2295
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
       055a056d065a060100640064036c075a07640064046c086d095a09010064
       0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
-      0f5a0f0100640064086c106d115a1101000200470064098400640aa60200
-      00ab0200000000000000005a1202006512a6000000ab0000000000000000
-      005a1365136a140000000000000000640b6515640c650665096515660219
-      0000000000000000006604640d8404a6000000ab0000000000000000005a
-      1665136a140000000000000000640b6515640c65156604640e8404a60000
-      00ab0000000000000000005a1765136a140000000000000000640b651564
-      0c6506650164036602190000000000000000006604640f8404a6000000ab
-      0000000000000000005a1865136a140000000000000000640b6515640c65
-      05651519000000000000000000660464108404a6000000ab000000000000
-      0000005a19641144005d215a1a6513a01400000000000000000000000000
-      000000000000000200651b6515651aa6020000ab020000000000000000a6
-      010000ab01000000000000000001008c2264035300
+      0f5a0f010002004700640884006409a6020000ab0200000000000000005a
+      1002006510a6000000ab0000000000000000005a1165116a120000000000
+      000000640a6513640b650665096513660219000000000000000000660464
+      0c8404a6000000ab0000000000000000005a1465116a1200000000000000
+      00640a6513640b65136604640d8404a6000000ab0000000000000000005a
+      1565116a120000000000000000640a6513640b6506650164036602190000
+      000000000000006604640e8404a6000000ab0000000000000000005a1665
+      116a120000000000000000640a6513640b65056513190000000000000000
+      006604640f8404a6000000ab0000000000000000005a17641044005d215a
+      186511a01200000000000000000000000000000000000000000200651965
+      136518a6020000ab020000000000000000a6010000ab0100000000000000
+      0001008c2264035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('date',))
                  6 IMPORT_NAME              0 (datetime)
                  8 IMPORT_FROM              1 (date)
                 10 STORE_NAME               1 (date)
@@ -67,424 +67,423 @@
                 72 LOAD_CONST               6 (('SEXES',))
                 74 IMPORT_NAME             12 (aleksis.apps.csv_import.settings)
                 76 IMPORT_FROM             13 (SEXES)
                 78 STORE_NAME              13 (SEXES)
                 80 POP_TOP
    
      9          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               7 (('settings',))
-                86 IMPORT_NAME             14 (aleksis.core)
-                88 IMPORT_FROM             15 (settings)
-                90 STORE_NAME              15 (settings)
+                84 LOAD_CONST               7 (('get_site_preferences',))
+                86 IMPORT_NAME             14 (aleksis.core.util.core_helpers)
+                88 IMPORT_FROM             15 (get_site_preferences)
+                90 STORE_NAME              15 (get_site_preferences)
                 92 POP_TOP
    
-    10          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               8 (('get_site_preferences',))
-                98 IMPORT_NAME             16 (aleksis.core.util.core_helpers)
-               100 IMPORT_FROM             17 (get_site_preferences)
-               102 STORE_NAME              17 (get_site_preferences)
-               104 POP_TOP
-   
-    13         106 PUSH_NULL
-               108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               9 (<code object ConverterRegistry, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 13>)
-               112 MAKE_FUNCTION            0
-               114 LOAD_CONST              10 ('ConverterRegistry')
-               116 PRECALL                  2
-               120 CALL                     2
-               130 STORE_NAME              18 (ConverterRegistry)
-   
-    32         132 PUSH_NULL
-               134 LOAD_NAME               18 (ConverterRegistry)
-               136 PRECALL                  0
-               140 CALL                     0
-               150 STORE_NAME              19 (converter_registry)
-   
-    35         152 LOAD_NAME               19 (converter_registry)
-               154 LOAD_ATTR               20 (register)
-   
-    36         164 LOAD_CONST              11 ('value')
-               166 LOAD_NAME               21 (str)
-               168 LOAD_CONST              12 ('return')
-               170 LOAD_NAME                6 (Union)
-               172 LOAD_NAME                9 (PhoneNumber)
-               174 LOAD_NAME               21 (str)
-               176 BUILD_TUPLE              2
-               178 BINARY_SUBSCR
-               188 BUILD_TUPLE              4
-               190 LOAD_CONST              13 (<code object parse_phone_number, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 35>)
-               192 MAKE_FUNCTION            4 (annotations)
-   
-    35         194 PRECALL                  0
-               198 CALL                     0
-   
-    36         208 STORE_NAME              22 (parse_phone_number)
-   
-    47         210 LOAD_NAME               19 (converter_registry)
-               212 LOAD_ATTR               20 (register)
-   
-    48         222 LOAD_CONST              11 ('value')
-               224 LOAD_NAME               21 (str)
-               226 LOAD_CONST              12 ('return')
-               228 LOAD_NAME               21 (str)
-               230 BUILD_TUPLE              4
-               232 LOAD_CONST              14 (<code object parse_sex, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 47>)
-               234 MAKE_FUNCTION            4 (annotations)
-   
-    47         236 PRECALL                  0
-               240 CALL                     0
-   
-    48         250 STORE_NAME              23 (parse_sex)
-   
-    57         252 LOAD_NAME               19 (converter_registry)
-               254 LOAD_ATTR               20 (register)
-   
-    58         264 LOAD_CONST              11 ('value')
-               266 LOAD_NAME               21 (str)
-               268 LOAD_CONST              12 ('return')
-               270 LOAD_NAME                6 (Union)
-               272 LOAD_NAME                1 (date)
-               274 LOAD_CONST               3 (None)
-               276 BUILD_TUPLE              2
-               278 BINARY_SUBSCR
-               288 BUILD_TUPLE              4
-               290 LOAD_CONST              15 (<code object parse_date, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 57>)
-               292 MAKE_FUNCTION            4 (annotations)
-   
-    57         294 PRECALL                  0
-               298 CALL                     0
-   
-    58         308 STORE_NAME              24 (parse_date)
-   
-    68         310 LOAD_NAME               19 (converter_registry)
-               312 LOAD_ATTR               20 (register)
-   
-    69         322 LOAD_CONST              11 ('value')
-               324 LOAD_NAME               21 (str)
-               326 LOAD_CONST              12 ('return')
-               328 LOAD_NAME                5 (Sequence)
-               330 LOAD_NAME               21 (str)
-               332 BINARY_SUBSCR
-               342 BUILD_TUPLE              4
-               344 LOAD_CONST              16 (<code object parse_comma_separated_data, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 68>)
-               346 MAKE_FUNCTION            4 (annotations)
-   
-    68         348 PRECALL                  0
-               352 CALL                     0
-   
-    69         362 STORE_NAME              25 (parse_comma_separated_data)
-   
-    74         364 LOAD_CONST              17 (('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title'))
-               366 GET_ITER
-           >>  368 FOR_ITER                33 (to 436)
-               370 STORE_NAME              26 (str_converter)
-   
-    75         372 LOAD_NAME               19 (converter_registry)
-               374 LOAD_METHOD             20 (register)
-               396 PUSH_NULL
-               398 LOAD_NAME               27 (getattr)
-               400 LOAD_NAME               21 (str)
-               402 LOAD_NAME               26 (str_converter)
-               404 PRECALL                  2
-               408 CALL                     2
-               418 PRECALL                  1
-               422 CALL                     1
-               432 POP_TOP
-               434 JUMP_BACKWARD           34 (to 368)
+    12          94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST               8 (<code object ConverterRegistry, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 12>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST               9 ('ConverterRegistry')
+               104 PRECALL                  2
+               108 CALL                     2
+               118 STORE_NAME              16 (ConverterRegistry)
+   
+    31         120 PUSH_NULL
+               122 LOAD_NAME               16 (ConverterRegistry)
+               124 PRECALL                  0
+               128 CALL                     0
+               138 STORE_NAME              17 (converter_registry)
+   
+    34         140 LOAD_NAME               17 (converter_registry)
+               142 LOAD_ATTR               18 (register)
+   
+    35         152 LOAD_CONST              10 ('value')
+               154 LOAD_NAME               19 (str)
+               156 LOAD_CONST              11 ('return')
+               158 LOAD_NAME                6 (Union)
+               160 LOAD_NAME                9 (PhoneNumber)
+               162 LOAD_NAME               19 (str)
+               164 BUILD_TUPLE              2
+               166 BINARY_SUBSCR
+               176 BUILD_TUPLE              4
+               178 LOAD_CONST              12 (<code object parse_phone_number, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 34>)
+               180 MAKE_FUNCTION            4 (annotations)
+   
+    34         182 PRECALL                  0
+               186 CALL                     0
+   
+    35         196 STORE_NAME              20 (parse_phone_number)
+   
+    48         198 LOAD_NAME               17 (converter_registry)
+               200 LOAD_ATTR               18 (register)
+   
+    49         210 LOAD_CONST              10 ('value')
+               212 LOAD_NAME               19 (str)
+               214 LOAD_CONST              11 ('return')
+               216 LOAD_NAME               19 (str)
+               218 BUILD_TUPLE              4
+               220 LOAD_CONST              13 (<code object parse_sex, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 48>)
+               222 MAKE_FUNCTION            4 (annotations)
+   
+    48         224 PRECALL                  0
+               228 CALL                     0
+   
+    49         238 STORE_NAME              21 (parse_sex)
+   
+    58         240 LOAD_NAME               17 (converter_registry)
+               242 LOAD_ATTR               18 (register)
+   
+    59         252 LOAD_CONST              10 ('value')
+               254 LOAD_NAME               19 (str)
+               256 LOAD_CONST              11 ('return')
+               258 LOAD_NAME                6 (Union)
+               260 LOAD_NAME                1 (date)
+               262 LOAD_CONST               3 (None)
+               264 BUILD_TUPLE              2
+               266 BINARY_SUBSCR
+               276 BUILD_TUPLE              4
+               278 LOAD_CONST              14 (<code object parse_date, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 58>)
+               280 MAKE_FUNCTION            4 (annotations)
+   
+    58         282 PRECALL                  0
+               286 CALL                     0
+   
+    59         296 STORE_NAME              22 (parse_date)
+   
+    69         298 LOAD_NAME               17 (converter_registry)
+               300 LOAD_ATTR               18 (register)
+   
+    70         310 LOAD_CONST              10 ('value')
+               312 LOAD_NAME               19 (str)
+               314 LOAD_CONST              11 ('return')
+               316 LOAD_NAME                5 (Sequence)
+               318 LOAD_NAME               19 (str)
+               320 BINARY_SUBSCR
+               330 BUILD_TUPLE              4
+               332 LOAD_CONST              15 (<code object parse_comma_separated_data, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 69>)
+               334 MAKE_FUNCTION            4 (annotations)
+   
+    69         336 PRECALL                  0
+               340 CALL                     0
+   
+    70         350 STORE_NAME              23 (parse_comma_separated_data)
+   
+    75         352 LOAD_CONST              16 (('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title'))
+               354 GET_ITER
+           >>  356 FOR_ITER                33 (to 424)
+               358 STORE_NAME              24 (str_converter)
+   
+    76         360 LOAD_NAME               17 (converter_registry)
+               362 LOAD_METHOD             18 (register)
+               384 PUSH_NULL
+               386 LOAD_NAME               25 (getattr)
+               388 LOAD_NAME               19 (str)
+               390 LOAD_NAME               24 (str_converter)
+               392 PRECALL                  2
+               396 CALL                     2
+               406 PRECALL                  1
+               410 CALL                     1
+               420 POP_TOP
+               422 JUMP_BACKWARD           34 (to 356)
    
-    74     >>  436 LOAD_CONST               3 (None)
-               438 RETURN_VALUE
+    75     >>  424 LOAD_CONST               3 (None)
+               426 RETURN_VALUE
    consts
       0
       ('date',)
       ('Any', 'Callable', 'Sequence', 'Union')
       None
       ('PhoneNumber',)
       ('NumberParseException',)
       ('SEXES',)
-      ('settings',)
       ('get_site_preferences',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a03640284005a04640365056506670165
             066602190000000000000000006404650565066701650666021900000000
             00000000006604640584045a076406650864046505650667016506660219
             0000000000000000006604640784045a0964085300
-          13           0 RESUME                   0
+          12           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ConverterRegistry')
                        8 STORE_NAME               2 (__qualname__)
          
-          14          10 LOAD_CONST               1 ('Registry of known conversion functions.')
+          13          10 LOAD_CONST               1 ('Registry of known conversion functions.')
                       12 STORE_NAME               3 (__doc__)
          
-          16          14 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 16>)
+          15          14 LOAD_CONST               2 (<code object __init__, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 15>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__init__)
          
-          19          20 LOAD_CONST               3 ('func')
+          18          20 LOAD_CONST               3 ('func')
                       22 LOAD_NAME                5 (Callable)
                       24 LOAD_NAME                6 (Any)
                       26 BUILD_LIST               1
                       28 LOAD_NAME                6 (Any)
                       30 BUILD_TUPLE              2
                       32 BINARY_SUBSCR
                       42 LOAD_CONST               4 ('return')
                       44 LOAD_NAME                5 (Callable)
                       46 LOAD_NAME                6 (Any)
                       48 BUILD_LIST               1
                       50 LOAD_NAME                6 (Any)
                       52 BUILD_TUPLE              2
                       54 BINARY_SUBSCR
                       64 BUILD_TUPLE              4
-                      66 LOAD_CONST               5 (<code object register, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 19>)
+                      66 LOAD_CONST               5 (<code object register, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 18>)
                       68 MAKE_FUNCTION            4 (annotations)
                       70 STORE_NAME               7 (register)
          
-          27          72 LOAD_CONST               6 ('name')
+          26          72 LOAD_CONST               6 ('name')
                       74 LOAD_NAME                8 (str)
                       76 LOAD_CONST               4 ('return')
                       78 LOAD_NAME                5 (Callable)
                       80 LOAD_NAME                6 (Any)
                       82 BUILD_LIST               1
                       84 LOAD_NAME                6 (Any)
                       86 BUILD_TUPLE              2
                       88 BINARY_SUBSCR
                       98 BUILD_TUPLE              4
-                     100 LOAD_CONST               7 (<code object get_from_name, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 27>)
+                     100 LOAD_CONST               7 (<code object get_from_name, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 26>)
                      102 MAKE_FUNCTION            4 (annotations)
                      104 STORE_NAME               9 (get_from_name)
                      106 LOAD_CONST               8 (None)
                      108 RETURN_VALUE
          consts
             'ConverterRegistry'
             'Registry of known conversion functions.'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code 0x970069007c005f00000000000000000064005300
-                16           0 RESUME                   0
+                15           0 RESUME                   0
                
-                17           2 BUILD_MAP                0
+                16           2 BUILD_MAP                0
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (_converters)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                names      ('_converters',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
                name       '__init__'
-               firstlineno 16
+               firstlineno 15
                lnotab 0x0201
             'func'
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c016a0000000000000000007c006a010000000000000000760072
                   1874050000000000000000000064017c016a0000000000000000009b0064
                   029d03a6010000ab01000000000000000082017c017c006a010000000000
                   0000007c016a0000000000000000003c0000007c015300
-                19           0 RESUME                   0
+                18           0 RESUME                   0
                
-                21           2 LOAD_FAST                1 (func)
+                20           2 LOAD_FAST                1 (func)
                              4 LOAD_ATTR                0 (__name__)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (_converters)
                             26 CONTAINS_OP              0
                             28 POP_JUMP_FORWARD_IF_FALSE    24 (to 78)
                
-                22          30 LOAD_GLOBAL              5 (NULL + ValueError)
+                21          30 LOAD_GLOBAL              5 (NULL + ValueError)
                             42 LOAD_CONST               1 ('The converter ')
                             44 LOAD_FAST                1 (func)
                             46 LOAD_ATTR                0 (__name__)
                             56 FORMAT_VALUE             0
                             58 LOAD_CONST               2 (' is already registered.')
                             60 BUILD_STRING             3
                             62 PRECALL                  1
                             66 CALL                     1
                             76 RAISE_VARARGS            1
                
-                23     >>   78 LOAD_FAST                1 (func)
+                22     >>   78 LOAD_FAST                1 (func)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                1 (_converters)
                             92 LOAD_FAST                1 (func)
                             94 LOAD_ATTR                0 (__name__)
                            104 STORE_SUBSCR
                
-                25         108 LOAD_FAST                1 (func)
+                24         108 LOAD_FAST                1 (func)
                            110 RETURN_VALUE
                consts
                   'Register a conversion function.'
                   'The converter '
                   ' is already registered.'
                names      ('__name__', '_converters', 'ValueError')
                varnames   ('self', 'func')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
                name       'register'
-               firstlineno 19
+               firstlineno 18
                lnotab 0x02021c0130011e02
             'name'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x97007c006a0000000000000000007c01190000000000000000005300
-                27           0 RESUME                   0
+                26           0 RESUME                   0
                
-                29           2 LOAD_FAST                0 (self)
+                28           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (_converters)
                             14 LOAD_FAST                1 (name)
                             16 BINARY_SUBSCR
                             26 RETURN_VALUE
                consts
                   'Get a conversion function by its name.'
                names      ('_converters',)
                varnames   ('self', 'name')
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
                name       'get_from_name'
-               firstlineno 27
+               firstlineno 26
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'Callable', 'Any', 'register', 'str', 'get_from_name')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'ConverterRegistry'
-         firstlineno 13
+         firstlineno 12
          lnotab 0x0a01040206033408
       'ConverterRegistry'
       'value'
       'return'
       code
          argcount  : 1
          nlocals   : 2
-         stacksize : 4
+         stacksize : 5
          flags     : 3
          code
             0x970009007401000000000000000000006a0100000000000000007c0074
-            04000000000000000000006a030000000000000000a6020000ab02000000
-            00000000007d017c01a00400000000000000000000000000000000000000
-            00a6000000ab00000000000000000072027c0153006e102300740a000000
-            0000000000000024007203010059006e04770078035900770164015300
-          35           0 RESUME                   0
+            0500000000000000000000a6000000ab0000000000000000006401190000
+            00000000000000a6020000ab0200000000000000007d017c01a003000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0072027c0153006e10230074080000000000000000000024007203010059
+            006e04770078035900770164025300
+          34           0 RESUME                   0
          
-          38           2 NOP
+          37           2 NOP
          
-          39           4 LOAD_GLOBAL              1 (NULL + PhoneNumber)
+          38           4 LOAD_GLOBAL              1 (NULL + PhoneNumber)
                       16 LOAD_ATTR                1 (from_string)
-                      26 LOAD_FAST                0 (value)
-                      28 LOAD_GLOBAL              4 (settings)
-                      40 LOAD_ATTR                3 (PHONENUMBER_DEFAULT_REGION)
-                      50 PRECALL                  2
-                      54 CALL                     2
-                      64 STORE_FAST               1 (number)
-         
-          40          66 LOAD_FAST                1 (number)
-                      68 LOAD_METHOD              4 (is_valid)
-                      90 PRECALL                  0
-                      94 CALL                     0
-                     104 POP_JUMP_FORWARD_IF_FALSE     2 (to 110)
-         
-          41         106 LOAD_FAST                1 (number)
-                     108 RETURN_VALUE
-         
-          40     >>  110 JUMP_FORWARD            16 (to 144)
-                 >>  112 PUSH_EXC_INFO
          
-          42         114 LOAD_GLOBAL             10 (NumberParseException)
-                     126 CHECK_EXC_MATCH
-                     128 POP_JUMP_FORWARD_IF_FALSE     3 (to 136)
-                     130 POP_TOP
-         
-          43         132 POP_EXCEPT
-                     134 JUMP_FORWARD             4 (to 144)
-         
-          42     >>  136 RERAISE                  0
-                 >>  138 COPY                     3
-                     140 POP_EXCEPT
-                     142 RERAISE                  1
+          39          26 LOAD_FAST                0 (value)
+                      28 LOAD_GLOBAL              5 (NULL + get_site_preferences)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 LOAD_CONST               1 ('internationalisation__phone_number_country')
+                      56 BINARY_SUBSCR
+         
+          38          66 PRECALL                  2
+                      70 CALL                     2
+                      80 STORE_FAST               1 (number)
+         
+          41          82 LOAD_FAST                1 (number)
+                      84 LOAD_METHOD              3 (is_valid)
+                     106 PRECALL                  0
+                     110 CALL                     0
+                     120 POP_JUMP_FORWARD_IF_FALSE     2 (to 126)
+         
+          42         122 LOAD_FAST                1 (number)
+                     124 RETURN_VALUE
+         
+          41     >>  126 JUMP_FORWARD            16 (to 160)
+                 >>  128 PUSH_EXC_INFO
+         
+          43         130 LOAD_GLOBAL              8 (NumberParseException)
+                     142 CHECK_EXC_MATCH
+                     144 POP_JUMP_FORWARD_IF_FALSE     3 (to 152)
+                     146 POP_TOP
+         
+          44         148 POP_EXCEPT
+                     150 JUMP_FORWARD             4 (to 160)
+         
+          43     >>  152 RERAISE                  0
+                 >>  154 COPY                     3
+                     156 POP_EXCEPT
+                     158 RERAISE                  1
          
-          44     >>  144 LOAD_CONST               1 ('')
-                     146 RETURN_VALUE
+          45     >>  160 LOAD_CONST               2 ('')
+                     162 RETURN_VALUE
          ExceptionTable:
-           4 to 106 -> 112 [0]
-           112 to 130 -> 138 [1] lasti
-           136 to 136 -> 138 [1] lasti
+           4 to 122 -> 128 [0]
+           128 to 146 -> 154 [1] lasti
+           152 to 152 -> 154 [1] lasti
          consts
             'Parse a phone number.'
+            'internationalisation__phone_number_country'
             ''
-         names      ('PhoneNumber', 'from_string', 'settings', 'PHONENUMBER_DEFAULT_REGION', 'is_valid', 'NumberParseException')
+         names      ('PhoneNumber', 'from_string', 'get_site_preferences', 'is_valid', 'NumberParseException')
          varnames   ('value', 'number')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_phone_number'
-         firstlineno 35
-         lnotab 0x020302013e01280104ff0402120104ff0802
+         firstlineno 34
+         lnotab 0x02030201160128ff1003280104ff0402120104ff0802
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 2
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000007d007c00740200000000000000000000760072
             0d7402000000000000000000007c00190000000000000000005300640153
             00
-          47           0 RESUME                   0
+          48           0 RESUME                   0
          
-          50           2 LOAD_FAST                0 (value)
+          51           2 LOAD_FAST                0 (value)
                        4 LOAD_METHOD              0 (lower)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               0 (value)
          
-          51          42 LOAD_FAST                0 (value)
+          52          42 LOAD_FAST                0 (value)
                       44 LOAD_GLOBAL              2 (SEXES)
                       56 CONTAINS_OP              0
                       58 POP_JUMP_FORWARD_IF_FALSE    13 (to 86)
          
-          52          60 LOAD_GLOBAL              2 (SEXES)
+          53          60 LOAD_GLOBAL              2 (SEXES)
                       72 LOAD_FAST                0 (value)
                       74 BINARY_SUBSCR
                       84 RETURN_VALUE
          
-          54     >>   86 LOAD_CONST               1 ('')
+          55     >>   86 LOAD_CONST               1 ('')
                       88 RETURN_VALUE
          consts
             'Parse sex via SEXES dictionary.'
             ''
          names      ('lower', 'SEXES')
          varnames   ('value',)
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_sex'
-         firstlineno 47
+         firstlineno 48
          lnotab 0x0203280112011a02
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
@@ -492,61 +491,61 @@
             01190000000000000000007d017c0172157c01a001000000000000000000
             00000000000000000000006402a6010000ab0100000000000000006e0167
             007d0209007405000000000000000000006a0300000000000000007c007c
             02ac03a6020000ab020000000000000000a0040000000000000000000000
             000000000000000000a6000000ab00000000000000000053002300740a00
             000000000000000000740c00000000000000000000660224007204010059
             00640453007700780359007701
-          57           0 RESUME                   0
+          58           0 RESUME                   0
          
-          60           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
+          61           2 LOAD_GLOBAL              1 (NULL + get_site_preferences)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 LOAD_CONST               1 ('csv_import__date_languages')
                       30 BINARY_SUBSCR
                       40 STORE_FAST               1 (languages_raw)
          
-          61          42 LOAD_FAST                1 (languages_raw)
+          62          42 LOAD_FAST                1 (languages_raw)
                       44 POP_JUMP_FORWARD_IF_FALSE    21 (to 88)
                       46 LOAD_FAST                1 (languages_raw)
                       48 LOAD_METHOD              1 (split)
                       70 LOAD_CONST               2 (',')
                       72 PRECALL                  1
                       76 CALL                     1
                       86 JUMP_FORWARD             1 (to 90)
                  >>   88 BUILD_LIST               0
                  >>   90 STORE_FAST               2 (languages)
          
-          62          92 NOP
+          63          92 NOP
          
-          63          94 LOAD_GLOBAL              5 (NULL + dateparser)
+          64          94 LOAD_GLOBAL              5 (NULL + dateparser)
                      106 LOAD_ATTR                3 (parse)
                      116 LOAD_FAST                0 (value)
                      118 LOAD_FAST                2 (languages)
                      120 KW_NAMES                 3
                      122 PRECALL                  2
                      126 CALL                     2
                      136 LOAD_METHOD              4 (date)
                      158 PRECALL                  0
                      162 CALL                     0
                      172 RETURN_VALUE
                  >>  174 PUSH_EXC_INFO
          
-          64         176 LOAD_GLOBAL             10 (ValueError)
+          65         176 LOAD_GLOBAL             10 (ValueError)
                      188 LOAD_GLOBAL             12 (AttributeError)
                      200 BUILD_TUPLE              2
                      202 CHECK_EXC_MATCH
                      204 POP_JUMP_FORWARD_IF_FALSE     4 (to 214)
                      206 POP_TOP
          
-          65         208 POP_EXCEPT
+          66         208 POP_EXCEPT
                      210 LOAD_CONST               4 (None)
                      212 RETURN_VALUE
          
-          64     >>  214 RERAISE                  0
+          65     >>  214 RERAISE                  0
                  >>  216 COPY                     3
                      218 POP_EXCEPT
                      220 RERAISE                  1
          ExceptionTable:
            94 to 170 -> 174 [0]
            174 to 206 -> 216 [1] lasti
            214 to 214 -> 216 [1] lasti
@@ -558,31 +557,31 @@
             None
          names      ('get_site_preferences', 'split', 'dateparser', 'parse', 'date', 'ValueError', 'AttributeError')
          varnames   ('value', 'languages_raw', 'languages')
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_date'
-         firstlineno 57
+         firstlineno 58
          lnotab 0x02032801320102015201200106ff
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 8
          flags     : 3
          code
             0x9700740100000000000000000000740300000000000000000000640184
             007c00a00200000000000000000000000000000000000000006402a60100
             00ab010000000000000000a6020000ab020000000000000000a6010000ab
             0100000000000000005300
-          68           0 RESUME                   0
+          69           0 RESUME                   0
          
-          71           2 LOAD_GLOBAL              1 (NULL + list)
+          72           2 LOAD_GLOBAL              1 (NULL + list)
                       14 LOAD_GLOBAL              3 (NULL + filter)
-                      26 LOAD_CONST               1 (<code object <lambda>, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 71>)
+                      26 LOAD_CONST               1 (<code object <lambda>, file "/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py", line 72>)
                       28 MAKE_FUNCTION            0
                       30 LOAD_FAST                0 (value)
                       32 LOAD_METHOD              2 (split)
                       54 LOAD_CONST               2 (',')
                       56 PRECALL                  1
                       60 CALL                     1
                       70 PRECALL                  2
@@ -594,41 +593,40 @@
             'Parse a string with comma-separated data.'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 19
                code 0x97007c005300
-                71           0 RESUME                   0
+                72           0 RESUME                   0
                              2 LOAD_FAST                0 (v)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('v',)
                freevars   ()
                cellvars   ()
                filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
                name       '<lambda>'
-               firstlineno 71
+               firstlineno 72
                lnotab 0x
             ','
          names      ('list', 'filter', 'split')
          varnames   ('value',)
          freevars   ()
          cellvars   ()
          filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
          name       'parse_comma_separated_data'
-         firstlineno 68
+         firstlineno 69
          lnotab 0x0203
       ('capitalize', 'lstrip', 'strip', 'rstrip', 'lower', 'upper', 'title')
-   names      ('datetime', 'date', 'typing', 'Any', 'Callable', 'Sequence', 'Union', 'dateparser', 'phonenumber_field.phonenumber', 'PhoneNumber', 'phonenumbers', 'NumberParseException', 'aleksis.apps.csv_import.settings', 'SEXES', 'aleksis.core', 'settings', 'aleksis.core.util.core_helpers', 'get_site_preferences', 'ConverterRegistry', 'converter_registry', 'register', 'str', 'parse_phone_number', 'parse_sex', 'parse_date', 'parse_comma_separated_data', 'str_converter', 'getattr')
+   names      ('datetime', 'date', 'typing', 'Any', 'Callable', 'Sequence', 'Union', 'dateparser', 'phonenumber_field.phonenumber', 'PhoneNumber', 'phonenumbers', 'NumberParseException', 'aleksis.apps.csv_import.settings', 'SEXES', 'aleksis.core.util.core_helpers', 'get_site_preferences', 'ConverterRegistry', 'converter_registry', 'register', 'str', 'parse_phone_number', 'parse_sex', 'parse_date', 'parse_comma_separated_data', 'str_converter', 'getattr')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-CSVImport/aleksis/apps/csv_import/util/converters.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c01180208010c010c020c010c010c031a1314030c011eff0e
-      01020b0c010eff0e0102090c011eff0e01020a0c011aff0e010205080140
-      ff
+      0x00ff02010c01180208010c010c020c010c031a1314030c011eff0e0102
+      0d0c010eff0e0102090c011eff0e01020a0c011aff0e010205080140ff
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/__pycache__/import_helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6d6f5e64 (Fri May 12 16:55:09 2023 UTC)
+moddate:  0x15dafc63 (Mon Feb 27 16:28:05 2023 UTC)
 files sz: 359
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/class_range_helpers.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/class_range_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/converters.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/converters.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Callable, Sequence, Union
 
 import dateparser
 from phonenumber_field.phonenumber import PhoneNumber
 from phonenumbers import NumberParseException
 
 from aleksis.apps.csv_import.settings import SEXES
-from aleksis.core import settings
 from aleksis.core.util.core_helpers import get_site_preferences
 
 
 class ConverterRegistry:
     """Registry of known conversion functions."""
 
     def __init__(self):
@@ -32,15 +31,17 @@
 converter_registry = ConverterRegistry()
 
 
 @converter_registry.register
 def parse_phone_number(value: str) -> Union[PhoneNumber, str]:
     """Parse a phone number."""
     try:
-        number = PhoneNumber.from_string(value, settings.PHONENUMBER_DEFAULT_REGION)
+        number = PhoneNumber.from_string(
+            value, get_site_preferences()["internationalisation__phone_number_country"]
+        )
         if number.is_valid():
             return number
     except NumberParseException:
         pass
     return ""
```

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/util/process.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/util/process.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/aleksis/apps/csv_import/views.py` & `aleksis_app_csvimport-3.0b0/aleksis/apps/csv_import/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/Makefile` & `aleksis_app_csvimport-3.0b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/admin/01_concept.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/01_concept.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/admin/05_configuration.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/05_configuration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/admin/10_exporting_data.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/10_exporting_data.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/admin/20_import_data.rst` & `aleksis_app_csvimport-3.0b0/docs/admin/20_import_data.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/conf.py` & `aleksis_app_csvimport-3.0b0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-CSVImport"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0"
+release = "3.0b0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_csvimport-3.0/docs/index.rst` & `aleksis_app_csvimport-3.0b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/docs/make.bat` & `aleksis_app_csvimport-3.0b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/pyproject.toml` & `aleksis_app_csvimport-3.0b0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-CSVImport"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -33,15 +33,15 @@
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.0.0"
 phonenumbers = "^8.10"
 dateparser = "^1.0.0"
-aleksis-core = "^3.0"
+aleksis-core = "^3.0b0"
 "ruamel.yaml" = "^0.17.19"
 tqdm = "^4.62.3"
 chardet = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
```

### Comparing `aleksis_app_csvimport-3.0/tox.ini` & `aleksis_app_csvimport-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_csvimport-3.0/setup.py` & `aleksis_app_csvimport-3.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,28 +23,28 @@
                              'locale/ru/LC_MESSAGES/*',
                              'locale/tr_TR/LC_MESSAGES/*',
                              'locale/uk/LC_MESSAGES/*',
                              'templates/csv_import/*',
                              'templates/csv_import/import_template/*']}
 
 install_requires = \
-['aleksis-core>=3.0,<4.0',
+['aleksis-core>=3.0b0,<4.0',
  'chardet>=5.0.0,<6.0.0',
  'dateparser>=1.0.0,<2.0.0',
  'pandas>=1.0.0,<2.0.0',
  'phonenumbers>=8.10,<9.0',
  'ruamel.yaml>=0.17.19,<0.18.0',
  'tqdm>=4.62.3,<5.0.0']
 
 entry_points = \
 {'aleksis.app': ['csv_import = aleksis.apps.csv_import.apps:CSVImportConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-csvimport',
-    'version': '3.0',
+    'version': '3.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp for CSV import',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp for CSV imports\n====================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThis app provides general CSV imports functions to interact with school administration software.\n\n* Generic and customisable importer based on templates\n* Register import templates in the frontend\n\nSupported systems:\n\n* Schild-NRW (North Rhine-Westphalia, Germany)\n* Pedasos (Schleswig-Holstein, Germany\n\nLicence\n-------\n\n::\n\n  Copyright © 2019, 2020, 2022 Dominik George <dominik.george@teckids.org>\n  Copyright © 2020, 2021, 2022 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>\n  Copyright © 2019 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2022 magicfelix <felix@felix-zauberer.de>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_csvimport-3.0/PKG-INFO` & `aleksis_app_csvimport-3.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-csvimport
-Version: 3.0
+Version: 3.0b0
 Summary: AlekSIS (School Information System) — App for CSV import
 Home-page: https://aleksis.org/
 License: EUPL-1.2
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
 Requires-Dist: dateparser (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: phonenumbers (>=8.10,<9.0)
 Requires-Dist: ruamel.yaml (>=0.17.19,<0.18.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Documentation, https://aleksis.edugit.io/AlekSIS/docs/html/
```

