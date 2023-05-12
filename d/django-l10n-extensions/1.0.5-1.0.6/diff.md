# Comparing `tmp/django-l10n-extensions-1.0.5.tar.gz` & `tmp/django-l10n-extensions-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-l10n-extensions-1.0.5.tar", last modified: Thu Apr  4 12:54:00 2019, max compression
+gzip compressed data, was "django-l10n-extensions-1.0.6.tar", last modified: Fri May 12 13:38:53 2023, max compression
```

## Comparing `django-l10n-extensions-1.0.5.tar` & `django-l10n-extensions-1.0.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/
--rw-rw-r--   0 cees      (1001) cees      (1001)      249 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/DESCRIPTION
--rw-rw-r--   0 cees      (1001) cees      (1001)      135 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/MANIFEST.in
--rw-rw-r--   0 cees      (1001) cees      (1001)     1531 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/PKG-INFO
--rw-rw-r--   0 cees      (1001) cees      (1001)      577 2019-04-04 12:53:51.000000 django-l10n-extensions-1.0.5/setup.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      902 2019-04-04 09:50:18.000000 django-l10n-extensions-1.0.5/README.md
--rw-rw-r--   0 cees      (1001) cees      (1001)       38 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/setup.cfg
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/
--rw-rw-r--   0 cees      (1001) cees      (1001)        1 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 cees      (1001) cees      (1001)     1531 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 cees      (1001) cees      (1001)       38 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/requires.txt
--rw-rw-r--   0 cees      (1001) cees      (1001)        1 2018-08-06 12:30:27.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/not-zip-safe
--rw-rw-r--   0 cees      (1001) cees      (1001)     1902 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 cees      (1001) cees      (1001)       29 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/top_level.txt
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/
--rw-rw-r--   0 cees      (1001) cees      (1001)     1035 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/utils.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/forms/
--rw-rw-r--   0 cees      (1001) cees      (1001)     1150 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/forms/fields.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/forms/__init__.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/commands/
--rw-rw-r--   0 cees      (1001) cees      (1001)     2898 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/commands/makemessages.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/commands/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      596 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/l10n_threading.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/templatetags/
--rw-rw-r--   0 cees      (1001) cees      (1001)     2290 2018-08-23 15:35:50.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/templatetags/inlinetrans.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/templatetags/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     1102 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/urls.py
--rw-rw-r--   0 cees      (1001) cees      (1001)    10935 2018-08-06 11:43:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/measures.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     2147 2018-09-03 07:25:31.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/settings.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     4785 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/po_utils.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     2438 2018-08-06 11:43:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     4424 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/views.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/
--rw-rw-r--   0 cees      (1001) cees      (1001)     7678 2019-04-04 12:52:57.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/fields.py
--rw-rw-r--   0 cees      (1001) cees      (1001)       24 2018-08-06 11:43:00.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     3899 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/models.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      113 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/exceptions.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     1449 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/django_l10n_extensions/mixins.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/management/
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/management/commands/
--rw-rw-r--   0 cees      (1001) cees      (1001)     1813 2018-08-06 11:43:00.000000 django-l10n-extensions-1.0.5/src/tests/management/commands/test_make_messages.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/management/commands/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/management/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     2594 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/test_measures.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/testapp/
--rw-rw-r--   0 cees      (1001) cees      (1001)      119 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/apps.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     1378 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/urls.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/testapp/scripts/
--rw-rw-r--   0 cees      (1001) cees      (1001)       44 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/scripts/sample_script.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/scripts/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     1620 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/settings.py
--rw-rw-r--   0 cees      (1001) cees      (1001)       80 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      362 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/views.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      726 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/models.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/testapp/migrations/
--rw-rw-r--   0 cees      (1001) cees      (1001)     1558 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/migrations/0001_initial.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/testapp/migrations/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     2172 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/conftest.py
-drwxrwxr-x   0 cees      (1001) cees      (1001)        0 2019-04-04 12:54:00.000000 django-l10n-extensions-1.0.5/src/tests/models/
--rw-rw-r--   0 cees      (1001) cees      (1001)     4273 2019-04-04 12:53:08.000000 django-l10n-extensions-1.0.5/src/tests/models/test_trans_fields.py
--rw-rw-r--   0 cees      (1001) cees      (1001)      734 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/models/test_l10n_units.py
--rw-rw-r--   0 cees      (1001) cees      (1001)        0 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/models/__init__.py
--rw-rw-r--   0 cees      (1001) cees      (1001)     4197 2018-07-14 15:51:36.000000 django-l10n-extensions-1.0.5/src/tests/models/test_measure_fields.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/
+-rw-rw-r--   0 cees      (1000) cees      (1000)      249 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/DESCRIPTION
+-rw-rw-r--   0 cees      (1000) cees      (1000)      135 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/MANIFEST.in
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1405 2022-02-14 13:37:25.000000 django-l10n-extensions-1.0.6/README.md
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/setup.cfg
+-rw-rw-r--   0 cees      (1000) cees      (1000)      577 2023-05-12 13:38:18.000000 django-l10n-extensions-1.0.6/setup.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.288999 django-l10n-extensions-1.0.6/src/
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2438 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      113 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/exceptions.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1150 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      596 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/l10n_threading.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2898 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/makemessages.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)    10899 2023-05-12 13:28:40.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/measures.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1449 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/mixins.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       24 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     7649 2023-05-12 13:36:56.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     3899 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/models.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4785 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/po_utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2147 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/settings.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2290 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/inlinetrans.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1102 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1033 2023-05-12 13:35:39.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/utils.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4424 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions/views.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1635 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1902 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)        1 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/not-zip-safe
+-rw-rw-r--   0 cees      (1000) cees      (1000)       38 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/requires.txt
+-rw-rw-r--   0 cees      (1000) cees      (1000)       29 2023-05-12 13:38:53.000000 django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.292999 django-l10n-extensions-1.0.6/src/tests/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2172 2023-05-12 13:27:15.000000 django-l10n-extensions-1.0.6/src/tests/conftest.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/management/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/__init__.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/management/commands/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/commands/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1813 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/management/commands/test_make_messages.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/models/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      734 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_l10n_units.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4197 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_measure_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     4273 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/models/test_trans_fields.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     2594 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/test_measures.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/
+-rw-rw-r--   0 cees      (1000) cees      (1000)       80 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      119 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/apps.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1558 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/0001_initial.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/migrations/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      726 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/models.py
+drwxrwxr-x   0 cees      (1000) cees      (1000)        0 2023-05-12 13:38:53.296999 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/
+-rw-rw-r--   0 cees      (1000) cees      (1000)        0 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/__init__.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)       44 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/scripts/sample_script.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1595 2023-05-12 13:32:29.000000 django-l10n-extensions-1.0.6/src/tests/testapp/settings.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)     1378 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/urls.py
+-rw-rw-r--   0 cees      (1000) cees      (1000)      362 2022-02-14 13:06:47.000000 django-l10n-extensions-1.0.6/src/tests/testapp/views.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-l10n-extensions-1.0.5/PKG-INFO` & `django-l10n-extensions-1.0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: django-l10n-extensions
-Version: 1.0.5
+Version: 1.0.6
 Summary: Extend Django with L10N features.
-
-- inline translation of your Django web application in the browser
-- L10N model field to enable translation of database content
-- L10N unit models e.g. Area  (m2, acres, hectares, etc.) or Temperature(°C, °F, K)
-
 Home-page: https://github.com/ceasaro/django-l10n-extensions
 Author: Cees van Wieringen
 Author-email: ceesvw@gmail.com
-License: UNKNOWN
-Description: # Django L10N extensions
-        Django L10N extensions adds some useful L10N extensions to the Django framework
-        
-        The project in maintained on [github](https://github.com/ceasaro/django-l10n-extensions)
-        
-        [Read the docs](http://django-l10n-extensions.readthedocs.io)
-        
-        
-         ## Create new distribution
-         To create a new distribution from this package follow these steps:
-         1) create new virualenv met python 3 `mkvirtualenv -p /usr/bin/python3 django-l10n-extensions`
-         2) install requirements `pip install -r setup/requirements.txt`
-         3) update the version in `./setup.py`, otherwise you will overwrite an already existing version. 
-         4) Make a new distribution run: `python setup.py sdist bdist_wheel`
-         5) Optional upload to pypi TEST: `twine upload --repository-url https://test.pypi.org/legacy/ dist/*` 
-         
-         to upload to PRODUCTION remove the `--repository-url` argument (make sure your local `~/.pypirc` is correct)
-         
-Platform: UNKNOWN
+
+# Django L10N extensions
+Django L10N extensions adds some useful L10N extensions to the Django framework
+
+The project in maintained on [github](https://github.com/ceasaro/django-l10n-extensions)
+
+[Read the docs](http://django-l10n-extensions.readthedocs.io)
+
+
+ ## Create new distribution
+ To create a new distribution from this package follow these steps:
+ 1) create new virualenv met python 3 `mkvirtualenv -p /usr/bin/python3 django-l10n-extensions`
+ 2) install requirements `pip install -r setup/requirements.txt`
+ 3) update the version in `./setup.py`, otherwise you will overwrite an already existing version. 
+ 4) Make a new distribution run: `python setup.py sdist bdist_wheel`
+ 5) Optional upload to pypi TEST: `twine upload --repository-url https://test.pypi.org/legacy/ dist/*` 
+ 
+ to upload to PRODUCTION remove the `--repository-url` argument (make sure your local `~/.pypirc` is correct)
+ 
+
+# Date and time in python
+**CONCEPT version**
+
+Always work in UTC and use date / datetime aware instances
+
+e.g. python 3
+datetime.utcfromtimestamp(0).timestamp() --> -3600  # datetime instance has no timezone and python fallback on OS timezone
+
+datetime.utcnow() is also timezone unaware
+use 
+datetime.utc(tz=timezone.utc)
+
+datetime.strptime("1970-0101T00:00:00", "%Y-%m-%dT%H:%M:%S) is also timezone unaware
+use
+datetime.strptime("1970-0101T00:00:00", "%Y-%m-%dT%H:%M:%S).replace(tzinfo=timezone.utc)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-l10n-extensions-1.0.5/setup.py` & `django-l10n-extensions-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django-l10n-extensions',
-    version='1.0.5',
+    version='1.0.6',
     author=u'Cees van Wieringen',
     author_email='ceesvw@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='./src'),
     include_package_data=True,
     install_requires=['GitPython==1.0.1', 'Django>=2', 'polib>=1.0'],
     url='https://github.com/ceasaro/django-l10n-extensions',
```

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/PKG-INFO` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: django-l10n-extensions
-Version: 1.0.5
+Version: 1.0.6
 Summary: Extend Django with L10N features.
-
-- inline translation of your Django web application in the browser
-- L10N model field to enable translation of database content
-- L10N unit models e.g. Area  (m2, acres, hectares, etc.) or Temperature(°C, °F, K)
-
 Home-page: https://github.com/ceasaro/django-l10n-extensions
 Author: Cees van Wieringen
 Author-email: ceesvw@gmail.com
-License: UNKNOWN
-Description: # Django L10N extensions
-        Django L10N extensions adds some useful L10N extensions to the Django framework
-        
-        The project in maintained on [github](https://github.com/ceasaro/django-l10n-extensions)
-        
-        [Read the docs](http://django-l10n-extensions.readthedocs.io)
-        
-        
-         ## Create new distribution
-         To create a new distribution from this package follow these steps:
-         1) create new virualenv met python 3 `mkvirtualenv -p /usr/bin/python3 django-l10n-extensions`
-         2) install requirements `pip install -r setup/requirements.txt`
-         3) update the version in `./setup.py`, otherwise you will overwrite an already existing version. 
-         4) Make a new distribution run: `python setup.py sdist bdist_wheel`
-         5) Optional upload to pypi TEST: `twine upload --repository-url https://test.pypi.org/legacy/ dist/*` 
-         
-         to upload to PRODUCTION remove the `--repository-url` argument (make sure your local `~/.pypirc` is correct)
-         
-Platform: UNKNOWN
+
+# Django L10N extensions
+Django L10N extensions adds some useful L10N extensions to the Django framework
+
+The project in maintained on [github](https://github.com/ceasaro/django-l10n-extensions)
+
+[Read the docs](http://django-l10n-extensions.readthedocs.io)
+
+
+ ## Create new distribution
+ To create a new distribution from this package follow these steps:
+ 1) create new virualenv met python 3 `mkvirtualenv -p /usr/bin/python3 django-l10n-extensions`
+ 2) install requirements `pip install -r setup/requirements.txt`
+ 3) update the version in `./setup.py`, otherwise you will overwrite an already existing version. 
+ 4) Make a new distribution run: `python setup.py sdist bdist_wheel`
+ 5) Optional upload to pypi TEST: `twine upload --repository-url https://test.pypi.org/legacy/ dist/*` 
+ 
+ to upload to PRODUCTION remove the `--repository-url` argument (make sure your local `~/.pypirc` is correct)
+ 
+
+# Date and time in python
+**CONCEPT version**
+
+Always work in UTC and use date / datetime aware instances
+
+e.g. python 3
+datetime.utcfromtimestamp(0).timestamp() --> -3600  # datetime instance has no timezone and python fallback on OS timezone
+
+datetime.utcnow() is also timezone unaware
+use 
+datetime.utc(tz=timezone.utc)
+
+datetime.strptime("1970-0101T00:00:00", "%Y-%m-%dT%H:%M:%S) is also timezone unaware
+use
+datetime.strptime("1970-0101T00:00:00", "%Y-%m-%dT%H:%M:%S).replace(tzinfo=timezone.utc)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions.egg-info/SOURCES.txt` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/utils.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this programe.  If not, see <http://www.gnu.org/licenses/>.
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 html_escape_table = {
     "&": "&amp;",
     '"': "&quot;",
     "'": "&apos;",
     ">": "&gt;",
     "<": "&lt;",
 }
 
 
 def html_escape(text):
     if not text:
         return
-    return "".join(html_escape_table.get(c, c) for c in force_text(text))
+    return "".join(html_escape_table.get(c, c) for c in force_str(text))
```

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/forms/fields.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/management/commands/makemessages.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/l10n_threading.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/l10n_threading.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/templatetags/inlinetrans.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/templatetags/inlinetrans.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/urls.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/urls.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/measures.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/measures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding=utf-8
 from copy import deepcopy
 
 from django.contrib.gis.measure import MeasureBase, NUMERIC_TYPES, Distance as GisDistance, Area as GisArea, \
     AREA_PREFIX, pretty_name
-from django.utils import six
 from django.utils.formats import number_format
 
 from django_l10n_extensions.l10n_threading import get_l10n
 
 VOLUME_PREFIX = 'cu_'
 
 
@@ -296,15 +295,15 @@
     def default_units(self, kwargs):
         """
         Return the unit value and the default units specified
         from the given keyword arguments dictionary.
         """
         val = 0.0
         default_unit = self.STANDARD_UNIT
-        for unit, value in six.iteritems(kwargs):
+        for unit, value in kwargs.items():
             if not isinstance(value, float):
                 value = float(value)
             if unit in self.UNITS:
                 val = self.UNITS_REVERSE[unit](value)
             elif unit in self.ALIAS:
                 u = self.ALIAS[unit]
                 val = self.UNITS_REVERSE[u](value)
```

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/settings.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/settings.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/po_utils.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/po_utils.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/__init__.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/views.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/views.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/fields.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
 from django.db import models
-from django.utils.translation import ugettext, pgettext, npgettext, ngettext
+from django.utils.translation import gettext, pgettext, npgettext, ngettext
 
 from django_l10n_extensions.forms import fields
 from django_l10n_extensions.exceptions import L10NException
 from django_l10n_extensions import measures
 
 
 class T9N(object):
@@ -15,15 +15,15 @@
         self.plural = msgid_plural or kwargs.get('p')
         if not self.msgid:
             raise ValueError("Invalid arguments passed, need at least a msgid")
 
     def __str__(self):
         if self.msgctxt:
             return pgettext(self.msgctxt, self.msgid)
-        return ugettext(self.msgid)
+        return gettext(self.msgid)
 
     def trans(self, count):
         if self.msgctxt:
             return npgettext(self.msgctxt, self.msgid, self.plural, count)
         return ngettext(self.msgid, self.plural, count)
 
     def __eq__(self, other):
@@ -41,15 +41,15 @@
 
     def __len__(self):
         return len(self.__str__())
 
 
 class TransField(models.CharField):
 
-    def from_db_value(self, value, expression, connection, context):
+    def from_db_value(self, value, expression, connection):
         return self.to_python(value)
 
     def to_python(self, value):
         if isinstance(value, T9N) or not value  :
             return value
         try:
             return T9N(**json.loads(value))
@@ -90,15 +90,15 @@
     def construct_measure(self, value, unit=None):
         if not self.measure_class:
             raise L10NException('A measure class is required for {0}'.format(self.__class__))
         if not self.DEFAULT_UNIT:
             raise L10NException('A DEFAULT_UNIT is required for {0}'.format(self.__class__))
         return self.measure_class(**{unit if unit else self.DEFAULT_UNIT: value})
 
-    def from_db_value(self, value, expression, connection, context):
+    def from_db_value(self, value, expression, connection):
         if type(value) in [float, int]:
             return self.construct_measure(value)
 
     def to_python(self, value):
         if isinstance(value, self.measure_class):
             return value
         if value is not None:
@@ -125,15 +125,15 @@
     def construct_measure(self, value, unit=None):
         if not self.measure_class:
             raise L10NException('A measure class is required for {0}'.format(self.__class__))
         if not self.DEFAULT_UNIT:
             raise L10NException('A DEFAULT_UNIT is required for {0}'.format(self.__class__))
         return self.measure_class(**{unit if unit else self.DEFAULT_UNIT: value})
 
-    def from_db_value(self, value, expression, connection, context):
+    def from_db_value(self, value, expression, connection):
         if type(value) in [float, int]:
             return self.construct_measure(value)
 
     def to_python(self, value):
         if isinstance(value, self.measure_class):
             return value
         if value is not None:
```

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/models/models.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/models/models.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/django_l10n_extensions/mixins.py` & `django-l10n-extensions-1.0.6/src/django_l10n_extensions/mixins.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/management/commands/test_make_messages.py` & `django-l10n-extensions-1.0.6/src/tests/management/commands/test_make_messages.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/test_measures.py` & `django-l10n-extensions-1.0.6/src/tests/test_measures.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/testapp/urls.py` & `django-l10n-extensions-1.0.6/src/tests/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/testapp/settings.py` & `django-l10n-extensions-1.0.6/src/tests/testapp/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 SECRET_KEY = 'dummy'
 
 INSTALLED_APPS = [
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.admin',
     'django.contrib.sessions',
-    'django_extensions',
     'django_l10n_extensions',
     'tests.testapp',
 ]
 
 MIDDLEWARE_CLASSES = (
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.locale.LocaleMiddleware',
```

### Comparing `django-l10n-extensions-1.0.5/src/tests/testapp/models.py` & `django-l10n-extensions-1.0.6/src/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/testapp/migrations/0001_initial.py` & `django-l10n-extensions-1.0.6/src/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/conftest.py` & `django-l10n-extensions-1.0.6/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/models/test_trans_fields.py` & `django-l10n-extensions-1.0.6/src/tests/models/test_trans_fields.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/models/test_l10n_units.py` & `django-l10n-extensions-1.0.6/src/tests/models/test_l10n_units.py`

 * *Files identical despite different names*

### Comparing `django-l10n-extensions-1.0.5/src/tests/models/test_measure_fields.py` & `django-l10n-extensions-1.0.6/src/tests/models/test_measure_fields.py`

 * *Files identical despite different names*

