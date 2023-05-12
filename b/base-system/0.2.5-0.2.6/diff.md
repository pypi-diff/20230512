# Comparing `tmp/base_system-0.2.5.tar.gz` & `tmp/base_system-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.5.tar", last modified: Fri May 12 08:19:19 2023, max compression
+gzip compressed data, was "base_system-0.2.6.tar", last modified: Fri May 12 09:20:38 2023, max compression
```

## Comparing `base_system-0.2.5.tar` & `base_system-0.2.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.594728 base_system-0.2.5/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.5/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.5/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.578716 base_system-0.2.5/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.5/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.5/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.5/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.5/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.5/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 08:19:19.594728 base_system-0.2.5/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.5/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.578716 base_system-0.2.5/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.5/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.586722 base_system-0.2.5/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.5/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.5/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.5/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.5/base_system/__pycache__/export_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19908 2023-05-09 07:38:01.000000 base_system-0.2.5/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.5/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.5/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.5/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-09 03:12:52.000000 base_system-0.2.5/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.5/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/auth.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.5/base_system/export_viewset.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.586722 base_system-0.2.5/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.5/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.5/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.5/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.5/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1144 2023-05-09 03:12:53.000000 base_system-0.2.5/base_system/migrations/0005_expensetype.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      433 2023-05-09 07:38:03.000000 base_system-0.2.5/base_system/migrations/0006_alter_doctor_photo.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.590725 base_system-0.2.5/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.5/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.5/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.5/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.5/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1093 2023-05-09 07:38:03.000000 base_system-0.2.5/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.5/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25900 2023-05-09 07:37:51.000000 base_system-0.2.5/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.5/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.5/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.5/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-09 03:12:22.000000 base_system-0.2.5/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.5/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.582719 base_system-0.2.5/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1970 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.5/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.5/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.5/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.5/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.5/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-12 08:19:19.594728 base_system-0.2.5/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-12 08:19:16.000000 base_system-0.2.5/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.547817 base_system-0.2.6/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.6/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.6/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.455763 base_system-0.2.6/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.6/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.6/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.6/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.6/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.6/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.6/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.6/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.6/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 09:20:38.547817 base_system-0.2.6/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.6/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.467770 base_system-0.2.6/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.6/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.499789 base_system-0.2.6/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.6/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.6/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.6/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.6/base_system/__pycache__/export_viewset.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19908 2023-05-09 07:38:01.000000 base_system-0.2.6/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.6/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.6/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.6/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-09 03:12:52.000000 base_system-0.2.6/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.6/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.6/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.6/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.6/base_system/auth.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.6/base_system/export_viewset.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.531808 base_system-0.2.6/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.6/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.6/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.6/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.6/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1144 2023-05-09 03:12:53.000000 base_system-0.2.6/base_system/migrations/0005_expensetype.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      433 2023-05-09 07:38:03.000000 base_system-0.2.6/base_system/migrations/0006_alter_doctor_photo.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.6/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.543815 base_system-0.2.6/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.6/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.6/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.6/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.6/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1093 2023-05-09 07:38:03.000000 base_system-0.2.6/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.6/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25900 2023-05-09 07:37:51.000000 base_system-0.2.6/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.6/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.6/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.6/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-09 03:12:22.000000 base_system-0.2.6/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15097 2023-05-12 09:18:57.000000 base_system-0.2.6/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 09:20:38.475775 base_system-0.2.6/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 09:20:38.000000 base_system-0.2.6/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1970 2023-05-12 09:20:38.000000 base_system-0.2.6/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-12 09:20:38.000000 base_system-0.2.6/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.6/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-12 09:20:38.000000 base_system-0.2.6/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-12 09:20:38.000000 base_system-0.2.6/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.6/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.6/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.6/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.6/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-12 09:20:38.547817 base_system-0.2.6/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-12 09:20:29.000000 base_system-0.2.6/setup.py
```

### Comparing `base_system-0.2.5/.gitignore` & `base_system-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/BaseFunctionModule/settings.py` & `base_system-0.2.6/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/BaseFunctionModule/urls.py` & `base_system-0.2.6/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/LICENCE` & `base_system-0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/PKG-INFO` & `base_system-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.5
+Version: 0.2.6
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.5/README.rst` & `base_system-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/export_viewset.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/export_viewset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/views.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.6/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/auth.py` & `base_system-0.2.6/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/export_viewset.py` & `base_system-0.2.6/base_system/export_viewset.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/0001_initial.py` & `base_system-0.2.6/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.6/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/0005_expensetype.py` & `base_system-0.2.6/base_system/migrations/0005_expensetype.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.6/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.6/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.6/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc` & `base_system-0.2.6/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc` & `base_system-0.2.6/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/models.py` & `base_system-0.2.6/base_system/models.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/serializers.py` & `base_system-0.2.6/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/urls.py` & `base_system-0.2.6/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/views.py` & `base_system-0.2.6/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/base_system/viewsets.py` & `base_system-0.2.6/base_system/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         extra['group']=group.pk
 
         serializer = ExtraGroupSerializer(data=extra)
         serializer.is_valid(raise_exception=True)
         serializer.save()
         return Response(data=GroupSerializer(group).data, status=status.HTTP_201_CREATED)
 
-    def check_data(self, data):
+    def check_data(self, data, flag=1):
         # 校验角色额外信息数据
         extra = dict()
         # data = dict(data)
         extra["note"] = data.get("note")
         extra["is_active"] = data.get("is_active", 1)
         extra["hospital"] = data.get("hospital_id")
         extra["order_by"] = data.get("order_by")
@@ -146,38 +146,39 @@
         extra = serializer.data
 
         # 校验角色数据
         group_data = dict()
         permissions = data.get("permission_ids")
         # group_data["permission_ids"] = eval(permissions) if permissions else None
         group_data["permission_ids"] = permissions if permissions else []
-        if data.get("name"):
-            group_data["name"] = data.get("name")
-            serializer = GroupSerializer(data=group_data)
-            serializer.is_valid(raise_exception=True)
-            # group_data = serializer.data
+        if flag == 1:  # 如果flag==1时验证group数据，否则不验证
+            if data.get("name"):
+                group_data["name"] = data.get("name")
+                serializer = GroupSerializer(data=group_data)
+                serializer.is_valid(raise_exception=True)
+                # group_data = serializer.data
 
         return extra, group_data
 
     @transaction.atomic
     def update(self, request, *args, **kwargs):
         group = self.get_object()
         extra_group = group.extra_group
-        if request.data.get("name") == group.name:
-            del request.data["name"]
-        extra, group_data = self.check_data(request.data)
+        # if request.data.get("name") == group.name:
+        #     del request.data["name"]
+        extra, group_data = self.check_data(request.data, flag=2)
         extra_group.note = extra["note"]
         extra_group.is_active = extra["is_active"]
         extra_group.index = extra["order_by"]
         extra_group.hospital_id = extra["hospital"]
         extra_group.created_user = extra["created_user"]
         extra_group.role_code = extra["role_code"]
         extra_group.role_name = extra["role_name"]
         extra_group.save()
-        group.name = group_data.get('name', group.name)
+        # group.name = group_data.get('name', group.name)
         # if group_data.get("permission_ids"):
         group.permissions.set(group_data["permission_ids"])
         group.save()
         return Response(data=GroupSerializer(group).data, status=status.HTTP_205_RESET_CONTENT)
 
     # def destroy(self, request, *args, **kwargs):
     #     group = self.get_object()
```

### Comparing `base_system-0.2.5/base_system.egg-info/PKG-INFO` & `base_system-0.2.6/base_system.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.5
+Version: 0.2.6
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.5/base_system.egg-info/SOURCES.txt` & `base_system-0.2.6/base_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/init_data.json` & `base_system-0.2.6/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/manage.py` & `base_system-0.2.6/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/requirements.txt` & `base_system-0.2.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/runtests.py` & `base_system-0.2.6/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.5/setup.py` & `base_system-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.5',
+    version='0.2.6',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

