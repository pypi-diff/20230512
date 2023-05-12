# Comparing `tmp/aleksis_app_resint-3.0b1.tar.gz` & `tmp/aleksis_app_resint-3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_resint-3.0b1.tar", max compression
+gzip compressed data, was "aleksis_app_resint-3.0b2.tar", max compression
```

## Comparing `aleksis_app_resint-3.0b1.tar` & `aleksis_app_resint-3.0b2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     2446 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/LICENCE.rst
--rw-r--r--   0        0        0     1596 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/README.rst
--rw-r--r--   0        0        0      214 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/aleksis/apps/resint/__init__.py
--rw-r--r--   0        0        0      517 2023-03-09 21:43:13.323108 aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      489 2023-03-09 21:43:14.591106 aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     2624 2023-03-09 21:43:13.807107 aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    16275 2023-03-09 21:43:14.523106 aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     5730 2023-03-09 21:43:14.607106 aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      136 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/aleksis/apps/resint/admin.py
--rw-r--r--   0        0        0     1508 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/aleksis/apps/resint/apps.py
--rw-r--r--   0        0        0     1226 2023-03-09 21:40:48.895355 aleksis_app_resint-3.0b1/aleksis/apps/resint/forms.py
--rw-r--r--   0        0        0     5040 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/frontend/index.js
--rw-r--r--   0        0        0      263 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/frontend/messages/de.json
--rw-r--r--   0        0        0      254 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/frontend/messages/en.json
--rw-r--r--   0        0        0      463 2023-03-09 21:43:14.859105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7819 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4985 2023-03-09 21:43:14.859105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9987 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-09 21:43:14.843105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7735 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:43:14.843105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:43:14.851105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6180 2023-03-09 21:43:14.851105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10692 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:43:14.851105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7689 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6291 2023-03-09 21:43:14.851105 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10806 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4747 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0002_permissions.py
--rw-r--r--   0        0        0      549 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py
--rw-r--r--   0        0        0      692 2023-03-09 21:40:48.899355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0004_edit_permission.py
--rw-r--r--   0        0        0      681 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0005_fix_permissions.py
--rw-r--r--   0        0        0     1847 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0006_livedocument.py
--rw-r--r--   0        0        0      510 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0007_current_file_not_null.py
--rw-r--r--   0        0        0        0 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/__init__.py
--rw-r--r--   0        0        0     9460 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/models.py
--rw-r--r--   0        0        0     4772 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/rules.py
--rw-r--r--   0        0        0     1187 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/tables.py
--rw-r--r--   0        0        0      464 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/group/create.html
--rw-r--r--   0        0        0      418 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/group/edit.html
--rw-r--r--   0        0        0     2675 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/group/list.html
--rw-r--r--   0        0        0      642 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/create.html
--rw-r--r--   0        0        0      640 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/edit.html
--rw-r--r--   0        0        0     1214 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/list.html
--rw-r--r--   0        0        0      406 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/poster/edit.html
--rw-r--r--   0        0        0     3361 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/poster/list.html
--rw-r--r--   0        0        0      537 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/poster/upload.html
--rw-r--r--   0        0        0     1929 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/urls.py
--rw-r--r--   0        0        0     9180 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/aleksis/apps/resint/views.py
--rw-r--r--   0        0        0      581 2023-03-09 21:40:48.903355 aleksis_app_resint-3.0b1/docs/Makefile
--rw-r--r--   0        0        0   154961 2023-03-09 21:40:48.907355 aleksis_app_resint-3.0b1/docs/_static/create_live_document.png
--rw-r--r--   0        0        0   164973 2023-03-09 21:40:48.911355 aleksis_app_resint-3.0b1/docs/_static/create_poster_group.png
--rw-r--r--   0        0        0   180288 2023-03-09 21:40:48.911355 aleksis_app_resint-3.0b1/docs/_static/manage_posters_list.png
--rw-r--r--   0        0        0   137796 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/_static/upload_poster.png
--rw-r--r--   0        0        0      116 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/admin/00_index.rst
--rw-r--r--   0        0        0     1868 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/admin/01_poster_groups.rst
--rw-r--r--   0        0        0      972 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/admin/02_live_documents.rst
--rw-r--r--   0        0        0     6399 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/conf.py
--rw-r--r--   0        0        0      120 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/dev/00_index.rst
--rw-r--r--   0        0        0     1753 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/dev/01_live_document_types.rst
--rw-r--r--   0        0        0      526 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/index.rst
--rw-r--r--   0        0        0      787 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/make.bat
--rw-r--r--   0        0        0       96 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/user/00_index.rst
--rw-r--r--   0        0        0     1007 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/docs/user/01_posters.rst
--rw-r--r--   0        0        0     1552 2023-03-09 21:41:20.575301 aleksis_app_resint-3.0b1/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-03-09 21:40:48.915355 aleksis_app_resint-3.0b1/tox.ini
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b1/setup.py
--rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b1/PKG-INFO
+-rw-r--r--   0        0        0     2652 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/LICENCE.rst
+-rw-r--r--   0        0        0     1596 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/README.rst
+-rw-r--r--   0        0        0      214 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/__init__.py
+-rw-r--r--   0        0        0      517 2023-03-20 17:25:05.537333 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      489 2023-03-20 17:25:06.629331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0     2624 2023-03-20 17:25:05.949332 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    16275 2023-03-20 17:25:06.569331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     5858 2023-03-20 17:25:06.641331 aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      136 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/admin.py
+-rw-r--r--   0        0        0     1508 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/apps.py
+-rw-r--r--   0        0        0     1226 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/forms.py
+-rw-r--r--   0        0        0     4975 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/index.js
+-rw-r--r--   0        0        0      263 2023-03-20 17:18:45.873957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/messages/de.json
+-rw-r--r--   0        0        0      254 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/messages/en.json
+-rw-r--r--   0        0        0      463 2023-03-20 17:25:06.833330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7819 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4985 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9987 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7735 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6180 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10692 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-20 17:25:06.841330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7689 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6291 2023-03-20 17:25:06.845330 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10806 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4747 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0002_permissions.py
+-rw-r--r--   0        0        0      549 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py
+-rw-r--r--   0        0        0      692 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0004_edit_permission.py
+-rw-r--r--   0        0        0      681 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0005_fix_permissions.py
+-rw-r--r--   0        0        0     1847 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0006_livedocument.py
+-rw-r--r--   0        0        0      510 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0007_current_file_not_null.py
+-rw-r--r--   0        0        0        0 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/__init__.py
+-rw-r--r--   0        0        0     9460 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/models.py
+-rw-r--r--   0        0        0     4957 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/rules.py
+-rw-r--r--   0        0        0     1187 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/tables.py
+-rw-r--r--   0        0        0      464 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/create.html
+-rw-r--r--   0        0        0      418 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/edit.html
+-rw-r--r--   0        0        0     2675 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/list.html
+-rw-r--r--   0        0        0      642 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/create.html
+-rw-r--r--   0        0        0      640 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/edit.html
+-rw-r--r--   0        0        0     1214 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/list.html
+-rw-r--r--   0        0        0      406 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/edit.html
+-rw-r--r--   0        0        0     3361 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/list.html
+-rw-r--r--   0        0        0      537 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/upload.html
+-rw-r--r--   0        0        0     1929 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/urls.py
+-rw-r--r--   0        0        0     9180 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/aleksis/apps/resint/views.py
+-rw-r--r--   0        0        0      581 2023-03-20 17:18:45.877957 aleksis_app_resint-3.0b2/docs/Makefile
+-rw-r--r--   0        0        0   154961 2023-03-20 17:18:45.881957 aleksis_app_resint-3.0b2/docs/_static/create_live_document.png
+-rw-r--r--   0        0        0   164973 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/create_poster_group.png
+-rw-r--r--   0        0        0   180288 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/manage_posters_list.png
+-rw-r--r--   0        0        0   137796 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/_static/upload_poster.png
+-rw-r--r--   0        0        0      116 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     1868 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/01_poster_groups.rst
+-rw-r--r--   0        0        0      972 2023-03-20 17:18:45.885957 aleksis_app_resint-3.0b2/docs/admin/02_live_documents.rst
+-rw-r--r--   0        0        0     6399 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/conf.py
+-rw-r--r--   0        0        0      120 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     1753 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/dev/01_live_document_types.rst
+-rw-r--r--   0        0        0      526 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/make.bat
+-rw-r--r--   0        0        0       96 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1007 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/docs/user/01_posters.rst
+-rw-r--r--   0        0        0     1552 2023-03-20 17:23:24.865499 aleksis_app_resint-3.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-03-20 17:18:45.889957 aleksis_app_resint-3.0b2/tox.ini
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b2/setup.py
+-rw-r--r--   0        0        0     2534 1970-01-01 00:00:00.000000 aleksis_app_resint-3.0b2/PKG-INFO
```

### Comparing `aleksis_app_resint-3.0b1/CHANGELOG.rst` & `aleksis_app_resint-3.0b2/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,32 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0b1` - 2023-03-09
---------------------
+`3.0b2`_ - 2023-03-20
+---------------------
+
+Fixed
+~~~~~
+
+* Menu item was shown for all users independent of permissions.
+
+`3.0b1`_ - 2023-03-09
+---------------------
 
 Fixed
 ~~~~~
 
 * Provide PDF documents outside django/ URL namespace again
 
-`3.0b0` - 2023-02-16
---------------------
+`3.0b0`_ - 2023-02-16
+---------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -91,8 +99,9 @@
 
 .. _2.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.0b0
 .. _2.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.0b1
 .. _2.0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.0
 .. _2.1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.1
 .. _2.2: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/2.2
 .. _3.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b0
-.. _3.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b2
+.. _3.0b1: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b1
+.. _3.0b2: https://edugit.org/AlekSIS/official/AlekSIS-App-Resint/-/tags/3.0b2
```

### Comparing `aleksis_app_resint-3.0b1/LICENCE.rst` & `aleksis_app_resint-3.0b2/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/README.rst` & `aleksis_app_resint-3.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x60520a64 (Thu Mar  9 21:40:48 2023 UTC)
+moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
 files sz: 214
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/apps.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x60520a64 (Thu Mar  9 21:40:48 2023 UTC)
+moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
 files sz: 1508
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/models.cpython-311.pyc` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x60520a64 (Thu Mar  9 21:40:48 2023 UTC)
+moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
 files sz: 9460
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/__pycache__/rules.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x60520a64 (Thu Mar  9 21:40:48 2023 UTC)
-files sz: 4772
+moddate:  0x75951864 (Mon Mar 20 17:18:45 2023 UTC)
+files sz: 4957
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -47,15 +47,16 @@
       0000000200650e6426a6010000ab0100000000000000007a0700007a0100
       005a220200650564286522a6020000ab0200000000000000000100652102
       00650d6429a6010000ab0100000000000000007a0100005a230200650564
       2a6523a6020000ab020000000000000000010065210200650d642ba60100
       00ab0100000000000000007a0100005a2402006505642c6524a6020000ab
       020000000000000000010065210200650d642da6010000ab010000000000
       0000007a0100005a2502006505642e6525a6020000ab0200000000000000
-      000100642f5300
+      000100651a65167a07000065217a0700005a2602006505642f6526a60200
+      00ab020000000000000000010064305300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('User',))
                  6 IMPORT_NAME              0 (django.contrib.auth.models)
                  8 IMPORT_FROM              1 (User)
                 10 STORE_NAME               1 (User)
@@ -542,16 +543,32 @@
    142        1298 PUSH_NULL
               1300 LOAD_NAME                5 (add_perm)
               1302 LOAD_CONST              46 ('resint.delete_livedocument_rule')
               1304 LOAD_NAME               37 (delete_live_document_predicate)
               1306 PRECALL                  2
               1310 CALL                     2
               1320 POP_TOP
-              1322 LOAD_CONST              47 (None)
-              1324 RETURN_VALUE
+   
+   147        1322 LOAD_NAME               26 (view_posters_predicate)
+              1324 LOAD_NAME               22 (view_poster_groups_predicate)
+              1326 BINARY_OP                7 (|)
+              1330 LOAD_NAME               33 (view_live_documents_predicate)
+              1332 BINARY_OP                7 (|)
+   
+   146        1336 STORE_NAME              38 (view_menu_predicate)
+   
+   149        1338 PUSH_NULL
+              1340 LOAD_NAME                5 (add_perm)
+              1342 LOAD_CONST              47 ('resint.view_menu_rule')
+              1344 LOAD_NAME               38 (view_menu_predicate)
+              1346 PRECALL                  2
+              1350 CALL                     2
+              1360 POP_TOP
+              1362 LOAD_CONST              48 (None)
+              1364 RETURN_VALUE
    consts
       0
       ('User',)
       ('HttpRequest',)
       ('add_perm', 'predicate')
       ('Poster', 'PosterGroup')
       ('check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person')
@@ -758,23 +775,24 @@
       'resint.view_livedocument_rule'
       'resint.add_livedocument'
       'resint.add_livedocument_rule'
       'resint.change_livedocument'
       'resint.edit_livedocument_rule'
       'resint.delete_livedocument'
       'resint.delete_livedocument_rule'
+      'resint.view_menu_rule'
       None
-   names      ('django.contrib.auth.models', 'User', 'django.http', 'HttpRequest', 'rules', 'add_perm', 'predicate', 'aleksis.apps.resint.models', 'Poster', 'PosterGroup', 'aleksis.core.util.predicates', 'check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'str', 'has_poster_group_object_perm', 'bool', 'permission_validator', 'is_public_poster_group', 'show_poster_group_in_menu', 'view_poster_groups_predicate', 'add_poster_group_predicate', 'edit_poster_group_predicate', 'delete_poster_group_predicate', 'view_posters_predicate', 'upload_poster_predicate', 'edit_poster_predicate', 'delete_poster_predicate', 'view_poster_pdf_predicate', 'view_poster_pdf_menu_predicate', 'view_poster_menu_predicate', 'view_live_documents_predicate', 'view_live_document_predicate', 'add_live_document_predicate', 'edit_live_document_predicate', 'delete_live_document_predicate')
+   names      ('django.contrib.auth.models', 'User', 'django.http', 'HttpRequest', 'rules', 'add_perm', 'predicate', 'aleksis.apps.resint.models', 'Poster', 'PosterGroup', 'aleksis.core.util.predicates', 'check_object_permission', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'str', 'has_poster_group_object_perm', 'bool', 'permission_validator', 'is_public_poster_group', 'show_poster_group_in_menu', 'view_poster_groups_predicate', 'add_poster_group_predicate', 'edit_poster_group_predicate', 'delete_poster_group_predicate', 'view_posters_predicate', 'upload_poster_predicate', 'edit_poster_predicate', 'delete_poster_predicate', 'view_poster_pdf_predicate', 'view_poster_pdf_menu_predicate', 'view_poster_menu_predicate', 'view_live_documents_predicate', 'view_live_document_predicate', 'add_live_document_predicate', 'edit_live_document_predicate', 'delete_live_document_predicate', 'view_menu_predicate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-App-Resint/aleksis/apps/resint/rules.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c02100210011c090c0a140702010eff0e01020402010e
       ff0e0102050201140116ff04ff06041803060102ff1403180302012cff06
       03180302012cff060318020201140116ff040216fe04ff06051803020114
       0116ff04ff060418030201140114ff040214fe04ff060518030201140114
       ff040214fe04ff06051803020102012cff04ff0604180302012cff060318
       030a0118041c01180302012cff06031803060102ff14031803060102ff14
-      031803060102ff1403
+      031803060102ff140318050eff0203
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/apps.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/forms.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/frontend/index.js` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/frontend/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,13 @@
-import {
-    hasPersonValidator
-} from "aleksis.core/routeValidators";
-
 export default {
     meta: {
         inMenu: true,
         titleKey: "resint.menu_title",
         icon: "mdi-open-in-app",
-        validators: [hasPersonValidator],
+        permission: "resint.view_menu_rule",
     },
     children: [{
         path: "",
         component: () => import("aleksis.core/components/LegacyBaseTemplate.vue"),
         name: "resint.posterIndex",
         meta: {
             inMenu: true,
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0001_initial.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0002_permissions.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0002_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0003_group_in_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0004_edit_permission.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0004_edit_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0005_fix_permissions.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0005_fix_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/migrations/0006_livedocument.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/migrations/0006_livedocument.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/models.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/rules.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,7 +136,14 @@
 add_perm("resint.edit_livedocument_rule", edit_live_document_predicate)
 
 # Delete live document
 delete_live_document_predicate = view_live_documents_predicate & has_global_perm(
     "resint.delete_livedocument"
 )
 add_perm("resint.delete_livedocument_rule", delete_live_document_predicate)
+
+
+# View menu
+view_menu_predicate = (
+    view_posters_predicate | view_poster_groups_predicate | view_live_documents_predicate
+)
+add_perm("resint.view_menu_rule", view_menu_predicate)
```

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/tables.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/group/list.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/create.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/edit.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/live_document/list.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/live_document/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/poster/list.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/templates/resint/poster/upload.html` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/templates/resint/poster/upload.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/urls.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/aleksis/apps/resint/views.py` & `aleksis_app_resint-3.0b2/aleksis/apps/resint/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/Makefile` & `aleksis_app_resint-3.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/_static/create_live_document.png` & `aleksis_app_resint-3.0b2/docs/_static/create_live_document.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/_static/create_poster_group.png` & `aleksis_app_resint-3.0b2/docs/_static/create_poster_group.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/_static/manage_posters_list.png` & `aleksis_app_resint-3.0b2/docs/_static/manage_posters_list.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/_static/upload_poster.png` & `aleksis_app_resint-3.0b2/docs/_static/upload_poster.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/admin/01_poster_groups.rst` & `aleksis_app_resint-3.0b2/docs/admin/01_poster_groups.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/admin/02_live_documents.rst` & `aleksis_app_resint-3.0b2/docs/admin/02_live_documents.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/conf.py` & `aleksis_app_resint-3.0b2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-App-Resint"
 copyright = "2018-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0b1"
+release = "3.0b2"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_app_resint-3.0b1/docs/dev/01_live_document_types.rst` & `aleksis_app_resint-3.0b2/docs/dev/01_live_document_types.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/index.rst` & `aleksis_app_resint-3.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/make.bat` & `aleksis_app_resint-3.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/docs/user/01_posters.rst` & `aleksis_app_resint-3.0b2/docs/user/01_posters.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/pyproject.toml` & `aleksis_app_resint-3.0b2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Resint"
-version = "3.0b1"
+version = "3.0b2"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_app_resint-3.0b1/tox.ini` & `aleksis_app_resint-3.0b2/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_resint-3.0b1/setup.py` & `aleksis_app_resint-3.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ['AlekSIS-Core>=3.0b0,<4.0']
 
 entry_points = \
 {'aleksis.app': ['resint = aleksis.apps.resint.apps:ResintConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-resint',
-    'version': '3.0b1',
+    'version': '3.0b2',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Resint (Public poster)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Resint (Public poster)\n================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nThe Resint app provides an interface for uploading PDF posters attached by a calendar week in which this poster is valid.\nThe app provides a public URL `current.pdf` which always returns the current poster PDF and adds a poster item linked to\nthe same URL.\n\nAdditionally, it provides data models and update logic for so-called live documents which are periodically updated PDF files.\n\nLicence\n-------\n\n::\n\n  Copyright © 2018, 2019, 2020, 2021 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2019 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2020, 2021 Frank Poetzsch-Heffter <p-h@katharineum.de>\n  Copyright © 2022 Dominik George <dominik.george@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/official/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Julian Leucker',
     'author_email': 'leuckeju@katharineum.de',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'dev@jonathanweth.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_app_resint-3.0b1/PKG-INFO` & `aleksis_app_resint-3.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-resint
-Version: 3.0b1
+Version: 3.0b2
 Summary: AlekSIS (School Information System) — App Resint (Public poster)
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Author: Julian Leucker
 Author-email: leuckeju@katharineum.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
```

