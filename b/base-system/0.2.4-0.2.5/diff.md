# Comparing `tmp/base_system-0.2.4.tar.gz` & `tmp/base_system-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base_system-0.2.4.tar", last modified: Sat May  6 02:46:02 2023, max compression
+gzip compressed data, was "base_system-0.2.5.tar", last modified: Fri May 12 08:19:19 2023, max compression
```

## Comparing `base_system-0.2.4.tar` & `base_system-0.2.5.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.705841 base_system-0.2.4/
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.4/.gitignore
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.4/.pypirc
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.585773 base_system-0.2.4/BaseFunctionModule/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.4/BaseFunctionModule/__init__.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/asgi.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.4/BaseFunctionModule/settings.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.4/BaseFunctionModule/wsgi.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.4/Dockerfile
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.4/LICENCE
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.4/MANIFEST.in
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:46:02.705841 base_system-0.2.4/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.4/README.rst
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.653812 base_system-0.2.4/base_system/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.4/base_system/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.681828 base_system-0.2.4/base_system/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.4/base_system/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.4/base_system/__pycache__/admin.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.4/base_system/__pycache__/apps.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.4/base_system/__pycache__/export_viewset.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    19488 2023-05-04 08:07:15.000000 base_system-0.2.4/base_system/__pycache__/models.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.4/base_system/__pycache__/serializers.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.4/base_system/__pycache__/tests.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.4/base_system/__pycache__/urls.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-06 02:13:02.000000 base_system-0.2.4/base_system/__pycache__/views.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.4/base_system/__pycache__/viewsets.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/admin.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/apps.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/auth.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.4/base_system/export_viewset.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.693834 base_system-0.2.4/base_system/migrations/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.4/base_system/migrations/0001_initial.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.4/base_system/migrations/0002_drugdirectory_code_medu_cur.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.4/base_system/migrations/0003_alter_extragroup_hospital.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.4/base_system/migrations/0004_alter_extragroup_role_name.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.4/base_system/migrations/__init__.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.701839 base_system-0.2.4/base_system/migrations/__pycache__/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.4/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.4/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.4/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.4/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.4/base_system/migrations/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    25535 2023-05-04 08:07:06.000000 base_system-0.2.4/base_system/models.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.4/base_system/serializers.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.4/base_system/tests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.4/base_system/urls.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-06 02:12:59.000000 base_system-0.2.4/base_system/views.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.4/base_system/viewsets.py
-drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-06 02:46:02.665819 base_system-0.2.4/base_system.egg-info/
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/PKG-INFO
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     1810 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/SOURCES.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/dependency_links.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.4/base_system.egg-info/not-zip-safe
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/requires.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-06 02:46:02.000000 base_system-0.2.4/base_system.egg-info/top_level.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.4/init_data.json
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.4/manage.py
--rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.4/requirements.txt
--rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.4/runtests.py
--rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-06 02:46:02.705841 base_system-0.2.4/setup.cfg
--rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-06 02:44:49.000000 base_system-0.2.4/setup.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.594728 base_system-0.2.5/
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)     1562 2023-01-04 07:42:57.000000 base_system-0.2.5/.gitignore
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      113 2023-02-07 05:55:05.000000 base_system-0.2.5/.pypirc
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.578716 base_system-0.2.5/BaseFunctionModule/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 05:21:26.000000 base_system-0.2.5/BaseFunctionModule/__init__.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/asgi.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11801 2023-05-06 02:43:22.000000 base_system-0.2.5/BaseFunctionModule/settings.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      917 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      413 2023-04-17 08:52:27.000000 base_system-0.2.5/BaseFunctionModule/wsgi.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      280 2023-01-04 05:21:25.000000 base_system-0.2.5/Dockerfile
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1554 2023-01-04 05:21:26.000000 base_system-0.2.5/LICENCE
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      106 2023-01-04 05:21:25.000000 base_system-0.2.5/MANIFEST.in
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 08:19:19.594728 base_system-0.2.5/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      756 2023-04-25 05:48:42.000000 base_system-0.2.5/README.rst
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.578716 base_system-0.2.5/base_system/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2023-01-04 03:02:16.000000 base_system-0.2.5/base_system/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.586722 base_system-0.2.5/base_system/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      148 2023-04-17 09:28:42.000000 base_system-0.2.5/base_system/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-17 09:28:43.000000 base_system-0.2.5/base_system/__pycache__/admin.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      434 2023-04-17 09:28:42.000000 base_system-0.2.5/base_system/__pycache__/apps.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    10658 2023-05-06 02:06:31.000000 base_system-0.2.5/base_system/__pycache__/export_viewset.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    19908 2023-05-09 07:38:01.000000 base_system-0.2.5/base_system/__pycache__/models.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    27610 2023-05-06 02:44:00.000000 base_system-0.2.5/base_system/__pycache__/serializers.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      189 2023-04-18 01:10:23.000000 base_system-0.2.5/base_system/__pycache__/tests.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3179 2023-05-06 02:06:30.000000 base_system-0.2.5/base_system/__pycache__/urls.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23682 2023-05-09 03:12:52.000000 base_system-0.2.5/base_system/__pycache__/views.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    11946 2023-05-06 01:27:33.000000 base_system-0.2.5/base_system/__pycache__/viewsets.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       63 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/admin.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      153 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/apps.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     3320 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/auth.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15572 2023-04-26 08:23:42.000000 base_system-0.2.5/base_system/export_viewset.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.586722 base_system-0.2.5/base_system/migrations/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    39429 2023-04-27 08:58:52.000000 base_system-0.2.5/base_system/migrations/0001_initial.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      441 2023-05-04 02:32:29.000000 base_system-0.2.5/base_system/migrations/0002_drugdirectory_code_medu_cur.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      557 2023-05-04 07:38:30.000000 base_system-0.2.5/base_system/migrations/0003_alter_extragroup_hospital.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      443 2023-05-04 08:07:17.000000 base_system-0.2.5/base_system/migrations/0004_alter_extragroup_role_name.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1144 2023-05-09 03:12:53.000000 base_system-0.2.5/base_system/migrations/0005_expensetype.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      433 2023-05-09 07:38:03.000000 base_system-0.2.5/base_system/migrations/0006_alter_doctor_photo.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        0 2022-09-27 03:45:06.000000 base_system-0.2.5/base_system/migrations/__init__.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.590725 base_system-0.2.5/base_system/migrations/__pycache__/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    15056 2023-05-04 02:32:29.000000 base_system-0.2.5/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      666 2023-05-04 07:38:30.000000 base_system-0.2.5/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      794 2023-05-04 07:38:38.000000 base_system-0.2.5/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      667 2023-05-06 01:27:34.000000 base_system-0.2.5/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1093 2023-05-09 07:38:03.000000 base_system-0.2.5/base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      159 2023-04-17 09:28:44.000000 base_system-0.2.5/base_system/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    25900 2023-05-09 07:37:51.000000 base_system-0.2.5/base_system/models.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    23752 2023-05-06 02:43:58.000000 base_system-0.2.5/base_system/serializers.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       60 2023-02-13 08:28:28.000000 base_system-0.2.5/base_system/tests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     4071 2023-05-06 02:06:28.000000 base_system-0.2.5/base_system/urls.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    58056 2023-05-09 03:12:22.000000 base_system-0.2.5/base_system/views.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)    14978 2023-05-04 08:34:21.000000 base_system-0.2.5/base_system/viewsets.py
+drwxrwxr-x   0 lyh       (1000) lyh       (1000)        0 2023-05-12 08:19:19.582719 base_system-0.2.5/base_system.egg-info/
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1184 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/PKG-INFO
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     1970 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/SOURCES.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/dependency_links.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)        1 2023-05-04 03:18:55.000000 base_system-0.2.5/base_system.egg-info/not-zip-safe
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      108 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/requires.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       12 2023-05-12 08:19:19.000000 base_system-0.2.5/base_system.egg-info/top_level.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)   262434 2023-01-04 05:21:26.000000 base_system-0.2.5/init_data.json
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      674 2023-04-17 08:52:27.000000 base_system-0.2.5/manage.py
+-rwxrwxr-x   0 lyh       (1000) lyh       (1000)      888 2023-01-04 05:21:25.000000 base_system-0.2.5/requirements.txt
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)      574 2023-04-17 08:52:27.000000 base_system-0.2.5/runtests.py
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)       38 2023-05-12 08:19:19.594728 base_system-0.2.5/setup.cfg
+-rw-rw-r--   0 lyh       (1000) lyh       (1000)     2650 2023-05-12 08:19:16.000000 base_system-0.2.5/setup.py
```

### Comparing `base_system-0.2.4/.gitignore` & `base_system-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/BaseFunctionModule/settings.py` & `base_system-0.2.5/BaseFunctionModule/settings.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/BaseFunctionModule/urls.py` & `base_system-0.2.5/BaseFunctionModule/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/LICENCE` & `base_system-0.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/PKG-INFO` & `base_system-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base_system
-Version: 0.2.4
+Version: 0.2.5
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.4/README.rst` & `base_system-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/__pycache__/export_viewset.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/export_viewset.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/__pycache__/models.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  4 08:07:06 2023 UTC, .py size: 25535 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 aa67 5364 bf63 0000  a........gSd.c..
+00000000: 610d 0d0a 0000 0000 4ff8 5964 2c65 0000  a.......O.Yd,e..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 ce01 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6403 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6406 5a0c 4700  d.l.m.Z...d.Z.G.
 00000080: 6407 6408 8400 6408 6509 6a0d 8303 5a0e  d.d...d.e.j...Z.
 00000090: 4700 6409 640a 8400 640a 650e 8303 5a0f  G.d.d...d.e...Z.
@@ -25,1194 +25,1221 @@
 00000180: 650e 8303 5a1d 4700 6427 6428 8400 6428  e...Z.G.d'd(..d(
 00000190: 650e 8303 5a1e 4700 6429 642a 8400 642a  e...Z.G.d)d*..d*
 000001a0: 650e 8303 5a1f 4700 642b 642c 8400 642c  e...Z.G.d+d,..d,
 000001b0: 650e 8303 5a20 4700 642d 642e 8400 642e  e...Z G.d-d...d.
 000001c0: 650e 8303 5a21 4700 642f 6430 8400 6430  e...Z!G.d/d0..d0
 000001d0: 650e 8303 5a22 4700 6431 6432 8400 6432  e...Z"G.d1d2..d2
 000001e0: 650e 8303 5a23 4700 6433 6434 8400 6434  e...Z#G.d3d4..d4
-000001f0: 6509 6a0d 8303 5a24 6401 5300 2935 e900  e.j...Z$d.S.)5..
-00000200: 0000 004e 2902 da0c 4162 7374 7261 6374  ...N)...Abstract
-00000210: 5573 6572 da05 4772 6f75 7029 01da 0b43  User..Group)...C
-00000220: 6f6e 7465 6e74 5479 7065 2901 da06 6d6f  ontentType)...mo
-00000230: 6465 6c73 2901 da08 7365 7474 696e 6773  dels)...settings
-00000240: 2902 2902 da01 3175 0300 0000 e794 b729  ).)...1u.......)
-00000250: 02da 0130 7503 0000 00e5 a5b3 6300 0000  ...0u.......c...
-00000260: 0000 0000 0000 0000 0000 0000 0005 0000  ................
-00000270: 0040 0000 0073 4800 0000 6500 5a01 6400  .@...sH...e.Z.d.
-00000280: 5a02 6503 6a04 6401 6402 6402 6403 8d03  Z.e.j.d.d.d.d...
-00000290: 5a05 6503 6a04 6404 6402 6402 6405 8d03  Z.e.j.d.d.d.d...
-000002a0: 5a06 6503 6a07 6406 6402 6407 8d02 5a08  Z.e.j.d.d.d...Z.
-000002b0: 4700 6408 6409 8400 6409 8302 5a09 640a  G.d.d...d...Z.d.
-000002c0: 5300 290b da10 4d65 6469 6361 6c42 6173  S.)...MedicalBas
-000002d0: 654d 6f64 656c f50c 0000 00e5 889b e5bb  eModel..........
-000002e0: bae6 97b6 e997 b454 a903 da0c 7665 7262  .......T....verb
-000002f0: 6f73 655f 6e61 6d65 da0c 6175 746f 5f6e  ose_name..auto_n
-00000300: 6f77 5f61 6464 da04 6e75 6c6c f50c 0000  ow_add..null....
-00000310: 00e6 9bb4 e696 b0e6 97b6 e997 b4a9 0372  ...............r
-00000320: 0c00 0000 da08 6175 746f 5f6e 6f77 720e  ......auto_nowr.
-00000330: 0000 00f5 0c00 0000 e698 afe5 90a6 e590  ................
-00000340: afe7 94a8 a902 720c 0000 00da 0764 6566  ......r......def
-00000350: 6175 6c74 6300 0000 0000 0000 0000 0000  aultc...........
-00000360: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
-00000370: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000380: 5300 2903 7a15 4d65 6469 6361 6c42 6173  S.).z.MedicalBas
-00000390: 654d 6f64 656c 2e4d 6574 6154 4e29 04da  eModel.MetaTN)..
-000003a0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000003b0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000003c0: 655f 5fda 0861 6273 7472 6163 74a9 0072  e__..abstract..r
-000003d0: 1900 0000 7219 0000 00fa 372f 686f 6d65  ....r.....7/home
-000003e0: 2f6c 7968 2f77 6f72 6b2f 4261 7365 4675  /lyh/work/BaseFu
-000003f0: 6e63 7469 6f6e 4d6f 6475 6c65 2f62 6173  nctionModule/bas
-00000400: 655f 7379 7374 656d 2f6d 6f64 656c 732e  e_system/models.
-00000410: 7079 da04 4d65 7461 1500 0000 7302 0000  py..Meta....s...
-00000420: 0008 0172 1b00 0000 4e29 0a72 1500 0000  ...r....N).r....
-00000430: 7216 0000 0072 1700 0000 7205 0000 00da  r....r....r.....
-00000440: 0d44 6174 6554 696d 6546 6965 6c64 da0c  .DateTimeField..
-00000450: 6372 6561 7465 645f 7469 6d65 da0c 7570  created_time..up
-00000460: 6461 7465 645f 7469 6d65 da0c 426f 6f6c  dated_time..Bool
-00000470: 6561 6e46 6965 6c64 da09 6973 5f61 6374  eanField..is_act
-00000480: 6976 6572 1b00 0000 7219 0000 0072 1900  iver....r....r..
-00000490: 0000 7219 0000 0072 1a00 0000 7209 0000  ..r....r....r...
-000004a0: 0010 0000 0073 0800 0000 0801 1001 1001  .....s..........
-000004b0: 0e02 7209 0000 0063 0000 0000 0000 0000  ..r....c........
-000004c0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-000004d0: 73d8 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
-000004e0: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
-000004f0: 0464 0564 0664 0664 078d 045a 0665 036a  .d.d.d.d...Z.e.j
-00000500: 0764 0864 0664 0664 098d 035a 0865 036a  .d.d.d.d...Z.e.j
-00000510: 0464 0264 0a64 0664 0b8d 035a 0965 036a  .d.d.d.d...Z.e.j
-00000520: 0764 0c64 0d8d 015a 0a65 036a 0b64 0e64  .d.d...Z.e.j.d.d
-00000530: 0d8d 015a 0c65 036a 0b64 0f64 0d8d 015a  ...Z.e.j.d.d...Z
-00000540: 0d65 036a 0e64 1064 1165 036a 0f64 0664  .e.j.d.d.e.j.d.d
-00000550: 128d 045a 1065 036a 0464 1364 0564 1464  ...Z.e.j.d.d.d.d
-00000560: 0664 158d 045a 1165 036a 0464 1664 0564  .d...Z.e.j.d.d.d
-00000570: 1764 188d 035a 1265 036a 0464 1964 0564  .d...Z.e.j.d.d.d
-00000580: 0664 0664 078d 045a 1365 036a 0464 1a64  .d.d...Z.e.j.d.d
-00000590: 0564 0664 0664 078d 045a 1447 0064 1b64  .d.d.d...Z.G.d.d
-000005a0: 1c84 0064 1c83 025a 1564 1d53 0029 1eda  ...d...Z.d.S.)..
-000005b0: 0848 6f73 7069 7461 6cf5 0600 0000 e590  .Hospital.......
-000005c0: 8de7 a7b0 e9ff 0000 00a9 0272 0c00 0000  ...........r....
-000005d0: da0a 6d61 785f 6c65 6e67 7468 f50c 0000  ..max_length....
-000005e0: 00e8 8194 e7b3 bbe6 96b9 e5bc 8fe9 6400  ..............d.
-000005f0: 0000 54a9 0472 0c00 0000 7225 0000 0072  ..T..r....r%...r
-00000600: 0e00 0000 da05 626c 616e 6b75 0c00 0000  ......blanku....
-00000610: e58c bbe9 99a2 e7ae 80e4 bb8b a903 720c  ..............r.
-00000620: 0000 0072 0e00 0000 7229 0000 00f5 0600  ...r....r)......
-00000630: 0000 e7bc 96e7 a081 a903 7225 0000 0072  ..........r%...r
-00000640: 0c00 0000 da06 756e 6971 7565 750c 0000  ......uniqueu...
-00000650: 00e5 8cbb e999 a2e5 9cb0 e59d 8029 0172  .............).r
-00000660: 0c00 0000 7506 0000 00e7 bb8f e5ba a675  ....u..........u
-00000670: 0600 0000 e7bb b4e5 baa6 da04 7365 6c66  ............self
-00000680: f50c 0000 00e6 8980 e5b1 9ee5 8cbb e999  ................
-00000690: a2a9 0372 0c00 0000 da09 6f6e 5f64 656c  ...r......on_del
-000006a0: 6574 6572 0e00 0000 750c 0000 00e5 8cbb  eter....u.......
-000006b0: e999 a2e5 9bbe e789 875a 0f68 6f73 7069  .........Z.hospi
-000006c0: 7461 6c5f 696d 6167 6573 2904 720c 0000  tal_images).r...
-000006d0: 0072 2500 0000 7214 0000 0072 2900 0000  .r%...r....r)...
-000006e0: da04 6c6f 676f 5a0d 686f 7370 6974 616c  ..logoZ.hospital
-000006f0: 5f6c 6f67 6fa9 0372 0c00 0000 7225 0000  _logo..r....r%..
-00000700: 0072 1400 0000 f509 0000 00e5 889b e5bb  .r..............
-00000710: bae4 baba f509 0000 00e6 9bb4 e696 b0e4  ................
-00000720: baba 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000730: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
-00000740: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-00000750: 6504 5a05 6403 5300 2904 7a0d 486f 7370  e.Z.d.S.).z.Hosp
-00000760: 6974 616c 2e4d 6574 615a 0b62 735f 686f  ital.MetaZ.bs_ho
-00000770: 7370 6974 616c 7506 0000 00e5 8cbb e999  spitalu.........
-00000780: a24e a906 7215 0000 0072 1600 0000 7217  .N..r....r....r.
-00000790: 0000 00da 0864 625f 7461 626c 6572 0c00  .....db_tabler..
-000007a0: 0000 da13 7665 7262 6f73 655f 6e61 6d65  ....verbose_name
-000007b0: 5f70 6c75 7261 6c72 1900 0000 7219 0000  _pluralr....r...
-000007c0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000007d0: 2e00 0000 7306 0000 0008 0104 0104 0172  ....s..........r
-000007e0: 1b00 0000 4e29 1672 1500 0000 7216 0000  ....N).r....r...
-000007f0: 0072 1700 0000 7205 0000 00da 0943 6861  .r....r......Cha
-00000800: 7246 6965 6c64 da04 6e61 6d65 da05 7068  rField..name..ph
-00000810: 6f6e 65da 0954 6578 7446 6965 6c64 da09  one..TextField..
-00000820: 696e 7472 6f64 7563 65da 0763 6f64 656e  introduce..coden
-00000830: 756d da07 6164 6472 6573 73da 0a46 6c6f  um..address..Flo
-00000840: 6174 4669 656c 645a 096c 6f6e 6769 7475  atFieldZ.longitu
-00000850: 6465 5a08 6c61 7469 7475 6465 da0a 466f  deZ.latitude..Fo
-00000860: 7265 6967 6e4b 6579 da07 4341 5343 4144  reignKey..CASCAD
-00000870: 45da 0670 6172 656e 745a 0a68 6f73 5f69  E..parentZ.hos_i
-00000880: 6d61 6765 7372 3200 0000 da0a 6372 6561  magesr2.....crea
-00000890: 7465 645f 6279 da0a 7570 6461 7465 645f  ted_by..updated_
-000008a0: 6279 721b 0000 0072 1900 0000 7219 0000  byr....r....r...
-000008b0: 0072 1900 0000 721a 0000 0072 2100 0000  .r....r....r!...
-000008c0: 1900 0000 7324 0000 0008 010e 0112 0110  ....s$..........
-000008d0: 0110 010c 010c 010c 0104 0102 0102 0104  ................
-000008e0: 0102 fc06 0712 0210 0112 0112 0272 2100  .............r!.
-000008f0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000900: 0000 0006 0000 0040 0000 0073 a200 0000  .......@...s....
-00000910: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
-00000920: 6403 8d02 5a05 6503 6a04 6404 6402 6405  d...Z.e.j.d.d.d.
-00000930: 6405 6406 8d04 5a06 6503 6a04 6407 6402  d.d...Z.e.j.d.d.
-00000940: 6405 6405 6406 8d04 5a07 6503 6a04 6408  d.d.d...Z.e.j.d.
-00000950: 6402 6403 8d02 5a08 6503 6a04 6409 640a  d.d...Z.e.j.d.d.
-00000960: 6405 6405 6406 8d04 5a09 6503 6a0a 640b  d.d.d...Z.e.j.d.
-00000970: 6405 6405 640c 8d03 5a0b 6503 6a0c 650d  d.d.d...Z.e.j.e.
-00000980: 640d 6503 6a0e 640e 8d03 5a0f 6503 6a0c  d.e.j.d...Z.e.j.
-00000990: 640f 6410 6503 6a0e 6405 6411 8d04 5a10  d.d.e.j.d.d...Z.
-000009a0: 4700 6412 6413 8400 6413 8302 5a11 6414  G.d.d...d...Z.d.
-000009b0: 5300 2915 da06 4f66 6669 6365 7222 0000  S.)...Officer"..
-000009c0: 0072 2300 0000 7224 0000 0075 0c00 0000  .r#...r$...u....
-000009d0: e7a7 91e5 aea4 e4bd 8de7 bdae 5472 2800  ............Tr(.
-000009e0: 0000 7226 0000 00f5 0c00 0000 e7a7 91e5  ..r&............
-000009f0: aea4 e7bc 96e7 a081 7506 0000 00e7 b1bb  ........u.......
-00000a00: e59e 8b72 2700 0000 750c 0000 00e7 a791  ...r'...u.......
-00000a10: e5ae a4e7 ae80 e4bb 8b72 2a00 0000 722f  .........r*...r/
-00000a20: 0000 00a9 0272 0c00 0000 7231 0000 0072  .....r....r1...r
-00000a30: 2e00 0000 750c 0000 00e4 b88a e7ba a7e7  ....u...........
-00000a40: a791 e5ae a472 3000 0000 6300 0000 0000  .....r0...c.....
-00000a50: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00000a60: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00000a70: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
-00000a80: 6404 5300 2905 7a0b 4f66 6669 6365 2e4d  d.S.).z.Office.M
-00000a90: 6574 615a 0962 735f 6f66 6669 6365 7506  etaZ.bs_officeu.
-00000aa0: 0000 00e7 a791 e5ae a4a9 0129 0272 3e00  ...........).r>.
-00000ab0: 0000 da08 686f 7370 6974 616c 4ea9 0772  ....hospitalN..r
-00000ac0: 1500 0000 7216 0000 0072 1700 0000 7237  ....r....r....r7
-00000ad0: 0000 0072 0c00 0000 7238 0000 00da 0f75  ...r....r8.....u
-00000ae0: 6e69 7175 655f 746f 6765 7468 6572 7219  nique_togetherr.
-00000af0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000b00: 0000 721b 0000 004a 0000 0073 0800 0000  ..r....J...s....
-00000b10: 0801 0401 0401 0401 721b 0000 004e 2912  ........r....N).
-00000b20: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00000b30: 0500 0000 7239 0000 0072 3a00 0000 723f  ....r9...r:...r?
-00000b40: 0000 0072 3b00 0000 723e 0000 005a 0b6f  ...r;...r>...Z.o
-00000b50: 6666 6963 655f 7479 7065 723c 0000 0072  ffice_typer<...r
-00000b60: 3d00 0000 7241 0000 0072 2100 0000 7242  =...rA...r!...rB
-00000b70: 0000 0072 4a00 0000 7243 0000 0072 1b00  ...rJ...rC...r..
-00000b80: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00000b90: 0072 1a00 0000 7246 0000 0037 0000 0073  .r....rF...7...s
-00000ba0: 2400 0000 0801 0e01 1201 1201 0e01 1201  $...............
-00000bb0: 1001 0401 0201 0201 04fd 0605 0401 0201  ................
-00000bc0: 0201 0401 02fc 0607 7246 0000 0063 0000  ........rF...c..
-00000bd0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000be0: 0000 4000 0000 736c 0000 0065 005a 0164  ..@...sl...e.Z.d
-00000bf0: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
-00000c00: 0565 036a 0464 0464 0264 038d 025a 0665  .e.j.d.d.d...Z.e
-00000c10: 036a 0765 0864 0565 036a 0964 068d 035a  .j.e.d.e.j.d...Z
-00000c20: 0a65 036a 0464 0764 0864 0964 0964 0a8d  .e.j.d.d.d.d.d..
-00000c30: 045a 0b65 036a 0464 0b64 0864 0964 0964  .Z.e.j.d.d.d.d.d
-00000c40: 0a8d 045a 0c47 0064 0c64 0d84 0064 0d83  ...Z.G.d.d...d..
-00000c50: 025a 0d64 0e53 0029 0fda 0d50 6f73 6974  .Z.d.S.)...Posit
-00000c60: 696f 6e54 6974 6c65 7222 0000 0072 2300  ionTitler"...r#.
-00000c70: 0000 7224 0000 0075 0c00 0000 e881 8ce7  ..r$...u........
-00000c80: a7b0 e7bc 96e7 a081 722f 0000 0072 4800  ........r/...rH.
-00000c90: 0000 7234 0000 0072 2700 0000 5472 2800  ..r4...r'...Tr(.
-00000ca0: 0000 7235 0000 0063 0000 0000 0000 0000  ..r5...c........
-00000cb0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00000cc0: 731c 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000cd0: 0364 025a 0465 045a 0564 035a 0664 0453  .d.Z.e.Z.d.Z.d.S
-00000ce0: 0029 057a 1250 6f73 6974 696f 6e54 6974  .).z.PositionTit
-00000cf0: 6c65 2e4d 6574 615a 1162 735f 706f 7369  le.MetaZ.bs_posi
-00000d00: 7469 6f6e 5f74 6974 6c65 f506 0000 00e8  tion_title......
-00000d10: 818c e7a7 b072 4900 0000 4e72 4b00 0000  .....rI...NrK...
-00000d20: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00000d30: 1a00 0000 721b 0000 005e 0000 0073 0800  ....r....^...s..
-00000d40: 0000 0801 0401 0401 0401 721b 0000 004e  ..........r....N
-00000d50: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
-00000d60: 0072 0500 0000 7239 0000 0072 3a00 0000  .r....r9...r:...
-00000d70: 723e 0000 0072 4100 0000 7221 0000 0072  r>...rA...r!...r
-00000d80: 4200 0000 724a 0000 0072 4400 0000 7245  B...rJ...rD...rE
-00000d90: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
-00000da0: 0000 7219 0000 0072 1a00 0000 724d 0000  ..r....r....rM..
-00000db0: 0053 0000 0073 1400 0000 0801 0e01 0e01  .S...s..........
-00000dc0: 0401 0201 0201 04fd 0605 1201 1202 724d  ..............rM
-00000dd0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000de0: 0000 0000 0700 0000 4000 0000 734e 0100  ........@...sN..
-00000df0: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
-00000e00: 0264 038d 025a 0565 036a 0464 0464 0264  .d...Z.e.j.d.d.d
-00000e10: 0564 0564 068d 045a 0665 036a 0464 0764  .d.d...Z.e.j.d.d
-00000e20: 0864 0564 0564 068d 045a 0765 036a 0464  .d.d.d...Z.e.j.d
-00000e30: 0964 0a64 0564 0564 068d 045a 0865 036a  .d.d.d.d...Z.e.j
-00000e40: 0464 0b64 0c64 038d 025a 0965 036a 0464  .d.d.d...Z.e.j.d
-00000e50: 0d64 0264 0564 0564 068d 045a 0a65 036a  .d.d.d.d...Z.e.j
-00000e60: 0b65 0c64 0e65 036a 0d64 0f8d 035a 0e65  .e.d.e.j.d...Z.e
-00000e70: 036a 0464 1064 1165 0f64 0564 0564 128d  .j.d.d.e.d.d.d..
-00000e80: 055a 1065 036a 0464 1364 1464 0564 0564  .Z.e.j.d.d.d.d.d
-00000e90: 068d 045a 1165 036a 0464 1564 0864 0564  ...Z.e.j.d.d.d.d
-00000ea0: 0564 068d 045a 1265 036a 0b65 1364 1665  .d...Z.e.j.e.d.e
-00000eb0: 036a 0d64 0f8d 035a 1465 036a 0b65 1564  .j.d...Z.e.j.e.d
-00000ec0: 1765 036a 0d64 0f8d 035a 1665 036a 1764  .e.j.d...Z.e.j.d
-00000ed0: 1864 0564 0564 198d 035a 1865 036a 0464  .d.d.d...Z.e.j.d
-00000ee0: 1a64 1464 1b64 1c8d 035a 1965 036a 1a64  .d.d.d...Z.e.j.d
-00000ef0: 1d64 0564 0564 198d 035a 1b65 036a 0464  .d.d.d...Z.e.j.d
-00000f00: 1e64 0264 0564 0564 068d 045a 1c65 036a  .d.d.d.d...Z.e.j
-00000f10: 0464 1f64 0264 0564 0564 068d 045a 1d65  .d.d.d.d.d...Z.e
-00000f20: 036a 1e64 2064 0564 218d 025a 1f47 0064  .j.d d.d!..Z.G.d
-00000f30: 2264 2384 0064 2383 025a 2064 2453 0029  "d#..d#..Z d$S.)
-00000f40: 25da 0644 6f63 746f 7272 2200 0000 e914  %..Doctorr".....
-00000f50: 0000 0072 2400 0000 7226 0000 0054 7228  ...r$...r&...Tr(
-00000f60: 0000 0075 0600 0000 e982 aee7 aeb1 7227  ...u..........r'
-00000f70: 0000 0075 0600 0000 e59c b0e5 9d80 7223  ...u..........r#
-00000f80: 0000 0075 0600 0000 e5b7 a5e5 8fb7 e940  ...u...........@
-00000f90: 0000 0075 0600 0000 e881 8ce4 bd8d 724e  ...u..........rN
-00000fa0: 0000 0072 4800 0000 f506 0000 00e6 80a7  ...rH...........
-00000fb0: e588 abe9 0200 0000 a905 720c 0000 0072  ..........r....r
-00000fc0: 2500 0000 da07 6368 6f69 6365 7372 0e00  %.....choicesr..
-00000fd0: 0000 7229 0000 0075 0600 0000 e6b0 91e6  ..r)...u........
-00000fe0: 978f e90a 0000 00f5 0c00 0000 e8ba abe4  ................
-00000ff0: bbbd e8af 81e5 8fb7 f50c 0000 00e6 8980  ................
-00001000: e5b1 9ee7 a791 e5ae a472 2f00 0000 f50c  .........r/.....
-00001010: 0000 00e5 87ba e794 9fe6 97a5 e69c 9f72  ...............r
-00001020: 2a00 0000 750c 0000 00e5 8cbb e794 9fe7  *...u...........
-00001030: 85a7 e789 875a 0c64 6f63 746f 725f 7068  .....Z.doctor_ph
-00001040: 6f74 6f72 3300 0000 750c 0000 00e5 8cbb  otor3...u.......
-00001050: e794 9fe6 8f8f e8bf b072 3400 0000 7235  .........r4...r5
-00001060: 0000 0075 1500 0000 e698 afe5 90a6 e4ba  ...u............
-00001070: 92e8 8194 e7bd 91e6 8ea5 e8af 8a72 1300  .............r..
-00001080: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001090: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
-000010a0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
-000010b0: 6504 5a05 6403 5300 2904 7a0b 446f 6374  e.Z.d.S.).z.Doct
-000010c0: 6f72 2e4d 6574 615a 0962 735f 646f 6374  or.MetaZ.bs_doct
-000010d0: 6f72 7509 0000 00e5 8cbb e794 9fe8 a1a8  oru.............
-000010e0: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
-000010f0: 7219 0000 0072 1a00 0000 721b 0000 0089  r....r....r.....
-00001100: 0000 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
-00001110: 0000 004e 2921 7215 0000 0072 1600 0000  ...N)!r....r....
-00001120: 7217 0000 0072 0500 0000 7239 0000 0072  r....r....r9...r
-00001130: 3a00 0000 723b 0000 00da 0565 6d61 696c  :...r;.....email
-00001140: 723f 0000 0072 3e00 0000 da08 706f 7369  r?...r>.....posi
-00001150: 7469 6f6e 7241 0000 0072 4d00 0000 7242  tionrA...rM...rB
-00001160: 0000 005a 0e70 6f73 6974 696f 6e5f 7469  ...Z.position_ti
-00001170: 746c 65da 0d47 454e 4445 525f 4348 4f49  tle..GENDER_CHOI
-00001180: 4345 da06 6765 6e64 6572 5a06 6e61 7469  CE..genderZ.nati
-00001190: 6f6e 5a05 6964 6e75 6d72 4600 0000 da06  onZ.idnumrF.....
-000011a0: 6f66 6669 6365 7221 0000 0072 4a00 0000  officer!...rJ...
-000011b0: da09 4461 7465 4669 656c 64da 0862 6972  ..DateField..bir
-000011c0: 7468 6461 795a 0570 686f 746f 723c 0000  thdayZ.photor<..
-000011d0: 00da 0864 6573 6372 6962 6572 4400 0000  ...describerD...
-000011e0: 7245 0000 0072 1f00 0000 5a11 6973 5f6f  rE...r....Z.is_o
-000011f0: 6e6c 696e 655f 636f 6e73 756c 7472 1b00  nline_consultr..
-00001200: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
-00001210: 0072 1a00 0000 724f 0000 0067 0000 0073  .r....rO...g...s
-00001220: 3e00 0000 0801 0e01 1201 1201 1201 0e01  >...............
-00001230: 1201 0401 0201 0201 04fd 0605 1401 1201  ................
-00001240: 1201 0401 0201 0201 04fd 0605 0401 0201  ................
-00001250: 0201 04fd 0605 1002 1001 1001 1201 1202  ................
-00001260: 0e02 724f 0000 0063 0000 0000 0000 0000  ..rO...c........
-00001270: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
-00001280: 736e 0100 0065 005a 0164 005a 0265 036a  sn...e.Z.d.Z.e.j
-00001290: 0464 0164 0264 0364 0364 048d 045a 0565  .d.d.d.d.d...Z.e
-000012a0: 036a 0464 0564 0664 0364 0364 048d 045a  .j.d.d.d.d.d...Z
-000012b0: 0665 036a 0764 0764 0364 0364 088d 035a  .e.j.d.d.d.d...Z
-000012c0: 0865 036a 0464 0964 0a65 0964 0364 0364  .e.j.d.d.e.d.d.d
-000012d0: 0b8d 055a 0a65 036a 0464 0c64 0664 0364  ...Z.e.j.d.d.d.d
-000012e0: 0364 048d 045a 0b65 036a 0c64 0d64 0e64  .d...Z.e.j.d.d.d
-000012f0: 0364 0364 0f8d 045a 0d65 036a 0e65 0f64  .d.d...Z.e.j.e.d
-00001300: 1065 036a 1064 0364 118d 045a 1165 036a  .e.j.d.d...Z.e.j
-00001310: 0e65 1264 1265 036a 1064 0364 118d 045a  .e.d.e.j.d.d...Z
-00001320: 1365 036a 0e65 1464 1365 036a 1064 0364  .e.j.e.d.e.j.d.d
-00001330: 118d 045a 1565 036a 0464 1464 0664 1564  ...Z.e.j.d.d.d.d
-00001340: 168d 035a 1665 036a 0464 1764 0264 0364  ...Z.e.j.d.d.d.d
-00001350: 0364 048d 045a 1765 036a 0464 1864 0264  .d...Z.e.j.d.d.d
-00001360: 0364 0364 048d 045a 1865 036a 1964 1964  .d.d...Z.e.j.d.d
-00001370: 0364 0364 088d 035a 1a65 036a 0464 1a64  .d.d...Z.e.j.d.d
-00001380: 0664 0364 0364 048d 045a 1b65 036a 0464  .d.d.d...Z.e.j.d
-00001390: 1b64 0664 0364 0364 048d 045a 1c65 036a  .d.d.d.d...Z.e.j
-000013a0: 1d64 1c64 0364 0364 1d8d 035a 1e65 036a  .d.d.d.d...Z.e.j
-000013b0: 1d64 1e64 0364 0364 1f8d 035a 1f47 0064  .d.d.d.d...Z.G.d
-000013c0: 2064 2184 0064 2183 025a 2065 2164 2264   d!..d!..Z e!d"d
-000013d0: 2384 0083 015a 2265 2164 2464 2584 0083  #....Z"e!d$d%...
-000013e0: 015a 2365 2164 2664 2784 0083 015a 2464  .Z#e!d&d'....Z$d
-000013f0: 2853 0029 29da 0455 7365 7272 2200 0000  (S.))..Userr"...
-00001400: 7223 0000 0054 7228 0000 0072 2600 0000  r#...Tr(...r&...
-00001410: 7227 0000 0072 5900 0000 722a 0000 0072  r'...rY...r*...r
-00001420: 5200 0000 7253 0000 0072 5400 0000 7257  R...rS...rT...rW
-00001430: 0000 00f5 0600 0000 e68e 92e5 ba8f e901  ................
-00001440: 0000 00a9 0472 0c00 0000 7214 0000 0072  .....r....r....r
-00001450: 0e00 0000 7229 0000 0072 5800 0000 7230  ....r)...rX...r0
-00001460: 0000 0072 2f00 0000 750c 0000 00e7 bb91  ...r/...u.......
-00001470: e5ae 9ae5 8cbb e794 9f75 0c00 0000 e794  .........u......
-00001480: a8e6 88b7 e5a4 b4e5 838f 5a0b 7573 6572  ..........Z.user
-00001490: 5f61 7661 7461 7272 3300 0000 750c 0000  _avatarr3...u...
-000014a0: 00e9 bb98 e8ae a4e8 a792 e889 b275 0f00  .............u..
-000014b0: 0000 e58f afe6 938d e4bd 9ce7 a791 e5ae  ................
-000014c0: a475 0c00 0000 e6b3 a8e9 878a e8af b4e6  .u..............
-000014d0: 988e 7234 0000 0072 3500 0000 720a 0000  ..r4...r5...r...
-000014e0: 0072 0b00 0000 720f 0000 0072 1000 0000  .r....r....r....
-000014f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00001500: 0001 0000 0040 0000 0073 1000 0000 6500  .....@...s....e.
-00001510: 5a01 6400 5a02 6401 5a03 6402 5300 2903  Z.d.Z.d.Z.d.S.).
-00001520: 7a09 5573 6572 2e4d 6574 6175 0c00 0000  z.User.Metau....
-00001530: e794 a8e6 88b7 e4bf a1e6 81af 4e29 0472  ............N).r
-00001540: 1500 0000 7216 0000 0072 1700 0000 720c  ....r....r....r.
-00001550: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00001560: 0000 721a 0000 0072 1b00 0000 b200 0000  ..r....r........
-00001570: 7302 0000 0008 0272 1b00 0000 6301 0000  s......r....c...
-00001580: 0000 0000 0000 0000 0002 0000 0002 0000  ................
-00001590: 0043 0000 0073 1800 0000 7c00 6a00 7d01  .C...s....|.j.}.
-000015a0: 7c01 7314 7c00 6a01 a002 a100 7d01 7c01  |.s.|.j.....}.|.
-000015b0: 5300 2901 758e 0000 000a 2020 2020 2020  S.).u.....      
-000015c0: 2020 e88e b7e5 8f96 e5bd 93e5 898d e794    ..............
-000015d0: a8e6 88b7 e9bb 98e8 aea4 e794 a8e6 88b7  ................
-000015e0: e7bb 842c 0a20 2020 2020 2020 20e5 a682  ...,.        ...
-000015f0: e69e 9ce6 9caa e8ae bee7 bdae efbc 8ce8  ................
-00001600: bf94 e59b 9ee7 acac e4b8 80e4 b8aa e794  ................
-00001610: a8e6 88b7 e7bb 840a 2020 2020 2020 2020  ........        
-00001620: e590 a6e5 8899 e8bf 94e5 9b9e e8ae bee7  ................
-00001630: bdae e79a 84e7 94a8 e688 b7e7 bb84 0a20  ............... 
-00001640: 2020 2020 2020 2029 035a 0d64 6566 6175         ).Z.defau
-00001650: 6c74 5f67 726f 7570 da06 6772 6f75 7073  lt_group..groups
-00001660: da05 6669 7273 74a9 0272 2e00 0000 5a09  ..first..r....Z.
-00001670: 7265 745f 6772 6f75 7072 1900 0000 7219  ret_groupr....r.
-00001680: 0000 0072 1a00 0000 da11 6765 745f 6465  ...r......get_de
-00001690: 6661 756c 745f 6772 6f75 70ba 0000 0073  fault_group....s
-000016a0: 0800 0000 0007 0601 0401 0a01 7a16 5573  ............z.Us
-000016b0: 6572 2e67 6574 5f64 6566 6175 6c74 5f67  er.get_default_g
-000016c0: 726f 7570 6301 0000 0000 0000 0000 0000  roupc...........
-000016d0: 0002 0000 0002 0000 0043 0000 0073 1c00  .........C...s..
-000016e0: 0000 7c00 6a00 a001 a100 7d01 7c01 7318  ..|.j.....}.|.s.
-000016f0: 7c00 6a00 a002 a100 7d01 7c01 5300 a901  |.j.....}.|.S...
-00001700: 4e29 0372 6600 0000 da03 616c 6cda 046e  N).rf.....all..n
-00001710: 6f6e 6572 6800 0000 7219 0000 0072 1900  onerh...r....r..
-00001720: 0000 721a 0000 00da 0d67 6574 5f61 6c6c  ..r......get_all
-00001730: 6772 6f75 7073 c600 0000 7308 0000 0000  groups....s.....
-00001740: 020a 0104 010a 017a 1255 7365 722e 6765  .......z.User.ge
-00001750: 745f 616c 6c67 726f 7570 7363 0100 0000  t_allgroupsc....
-00001760: 0000 0000 0000 0000 0200 0000 0100 0000  ................
-00001770: 4300 0000 7318 0000 0064 017d 017c 006a  C...s....d.}.|.j
-00001780: 007d 017c 0173 147c 006a 017d 017c 0153  .}.|.s.|.j.}.|.S
-00001790: 0029 0275 3300 0000 0a20 2020 2020 2020  .).u3....       
-000017a0: 20e8 8eb7 e58f 96e7 94a8 e688 b7e9 bb98   ...............
-000017b0: e8ae a4e7 9a84 e7bb 84e7 bb87 e69c bae6  ................
-000017c0: 9e84 0a20 2020 2020 2020 204e 2902 725e  ...        N).r^
-000017d0: 0000 0072 4a00 0000 2902 722e 0000 005a  ...rJ...).r....Z
-000017e0: 0772 6574 5f6f 7267 7219 0000 0072 1900  .ret_orgr....r..
-000017f0: 0000 721a 0000 00da 1867 6574 5f64 6566  ..r......get_def
-00001800: 6175 6c74 5f6f 7267 616e 697a 6174 696f  ault_organizatio
-00001810: 6ecd 0000 0073 0a00 0000 0005 0401 0601  n....s..........
-00001820: 0401 0601 7a1d 5573 6572 2e67 6574 5f64  ....z.User.get_d
-00001830: 6566 6175 6c74 5f6f 7267 616e 697a 6174  efault_organizat
-00001840: 696f 6e4e 2925 7215 0000 0072 1600 0000  ionN)%r....r....
-00001850: 7217 0000 0072 0500 0000 7239 0000 0072  r....r....r9...r
-00001860: 3a00 0000 723b 0000 0072 5f00 0000 7260  :...r;...r_...r`
-00001870: 0000 0072 5c00 0000 725d 0000 005a 0969  ...r\...r]...Z.i
-00001880: 6463 6172 646e 756d da0c 496e 7465 6765  dcardnum..Intege
-00001890: 7246 6965 6c64 da08 6f72 6465 725f 6279  rField..order_by
-000018a0: 7241 0000 0072 4600 0000 7242 0000 0072  rA...rF...rB...r
-000018b0: 5e00 0000 7221 0000 0072 4a00 0000 724f  ^...r!...rJ...rO
-000018c0: 0000 005a 0664 6f63 746f 725a 0a61 7661  ...Z.doctorZ.ava
-000018d0: 7461 725f 7572 6c5a 1064 6566 6175 6c74  tar_urlZ.default
-000018e0: 5f67 726f 7570 5f69 645a 0c61 6c6c 6f77  _group_idZ.allow
-000018f0: 5f6f 6666 6963 6572 3c00 0000 da04 6e6f  _officer<.....no
-00001900: 7465 7244 0000 0072 4500 0000 721c 0000  terD...rE...r...
-00001910: 0072 1d00 0000 721e 0000 0072 1b00 0000  .r....r....r....
-00001920: da08 7072 6f70 6572 7479 7269 0000 0072  ..propertyri...r
-00001930: 6d00 0000 726e 0000 0072 1900 0000 7219  m...rn...r....r.
-00001940: 0000 0072 1900 0000 721a 0000 0072 6200  ...r....r....rb.
-00001950: 0000 8f00 0000 734e 0000 0008 0112 0112  ......sN........
-00001960: 0110 0114 0112 0112 0104 0102 0102 0104  ................
-00001970: 0102 fc06 0604 0102 0102 0104 0102 fc06  ................
-00001980: 0604 0102 0102 0104 0102 fc06 0710 0112  ................
-00001990: 0112 0110 0112 0112 0110 0110 020e 0802  ................
-000019a0: 010a 0b02 010a 0602 0172 6200 0000 6300  .........rb...c.
-000019b0: 0000 0000 0000 0000 0000 0000 0000 0007  ................
-000019c0: 0000 0040 0000 0073 ce00 0000 6500 5a01  ...@...s....e.Z.
-000019d0: 6400 5a02 6401 5a03 6504 6a05 6506 6504  d.Z.d.Z.e.j.e.e.
-000019e0: 6a07 6402 6403 6403 6404 8d05 5a08 6504  j.d.d.d.d...Z.e.
-000019f0: 6a09 6405 6406 6403 6407 8d03 5a0a 6504  j.d.d.d.d...Z.e.
-00001a00: 6a09 6405 6408 6403 6409 8d03 5a0b 6504  j.d.d.d.d...Z.e.
-00001a10: 6a0c 6403 640a 6403 640b 8d03 5a0d 6504  j.d.d.d.d...Z.e.
-00001a20: 6a09 640c 6405 6403 6403 640d 8d04 5a0e  j.d.d.d.d.d...Z.
-00001a30: 6504 6a0f 6510 640e 6504 6a07 640f 6403  e.j.e.d.e.j.d.d.
-00001a40: 6410 8d05 5a11 6504 6a12 6411 6412 6403  d...Z.e.j.d.d.d.
-00001a50: 6413 8d03 5a13 6504 6a09 6405 6414 6403  d...Z.e.j.d.d.d.
-00001a60: 6403 6415 8d04 5a14 6504 6a15 6416 6403  d.d...Z.e.j.d.d.
-00001a70: 6403 6417 8d03 5a16 6504 6a15 6418 6403  d.d...Z.e.j.d.d.
-00001a80: 6403 6419 8d03 5a17 4700 641a 641b 8400  d.d...Z.G.d.d...
-00001a90: 641b 8302 5a18 641c 5300 291d da0a 4578  d...Z.d.S.)...Ex
-00001aa0: 7472 6147 726f 7570 7519 0000 000a 2020  traGroupu.....  
-00001ab0: 2020 e8a7 92e8 89b2 e689 a9e5 8585 e8a1    ..............
-00001ac0: a80a 2020 2020 da0b 6578 7472 615f 6772  ..    ..extra_gr
-00001ad0: 6f75 7054 2904 7231 0000 00da 0c72 656c  oupT).r1.....rel
-00001ae0: 6174 6564 5f6e 616d 6572 0e00 0000 7229  ated_namer....r)
-00001af0: 0000 00e9 3200 0000 750c 0000 00e8 a792  ....2...u.......
-00001b00: e889 b2e4 bba3 e7a0 8172 2c00 0000 750c  .........r,...u.
-00001b10: 0000 00e8 a792 e889 b2e5 908d e7a7 b029  ...............)
-00001b20: 0372 2500 0000 720c 0000 0072 2900 0000  .r%...r....r)...
-00001b30: 7212 0000 0029 0372 1400 0000 720c 0000  r....).r....r...
-00001b40: 0072 0e00 0000 7506 0000 00e6 8f8f e8bf  .r....u.........
-00001b50: b029 0372 2500 0000 720e 0000 0072 2900  .).r%...r....r).
-00001b60: 0000 722f 0000 0072 6600 0000 a904 720c  ..r/...rf.....r.
-00001b70: 0000 0072 3100 0000 7275 0000 0072 0e00  ...r1...ru...r..
-00001b80: 0000 7263 0000 0072 6400 0000 a903 720c  ..rc...rd.....r.
-00001b90: 0000 0072 1400 0000 720e 0000 0072 3400  ...r....r....r4.
-00001ba0: 0000 a904 7225 0000 0072 0c00 0000 720e  ....r%...r....r.
-00001bb0: 0000 0072 2900 0000 720a 0000 0072 0b00  ...r)...r....r..
-00001bc0: 0000 7512 0000 00e6 9c80 e590 8ee6 9bb4  ..u.............
-00001bd0: e696 b0e6 97b6 e997 b472 1000 0000 6300  .........r....c.
-00001be0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001bf0: 0000 0040 0000 0073 1800 0000 6500 5a01  ...@...s....e.Z.
-00001c00: 6400 5a02 6401 5a03 6402 5a04 6504 5a05  d.Z.d.Z.d.Z.e.Z.
-00001c10: 6403 5300 2904 7a0f 4578 7472 6147 726f  d.S.).z.ExtraGro
-00001c20: 7570 2e4d 6574 615a 0e62 735f 6578 7472  up.MetaZ.bs_extr
-00001c30: 615f 6772 6f75 7075 0600 0000 e8a7 92e8  a_groupu........
-00001c40: 89b2 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
-00001c50: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00001c60: 00ee 0000 0073 0600 0000 0801 0401 0401  .....s..........
-00001c70: 721b 0000 004e 2919 7215 0000 0072 1600  r....N).r....r..
-00001c80: 0000 7217 0000 00da 075f 5f64 6f63 5f5f  ..r......__doc__
-00001c90: 7205 0000 00da 0d4f 6e65 546f 4f6e 6546  r......OneToOneF
-00001ca0: 6965 6c64 7203 0000 0072 4200 0000 da05  ieldr....rB.....
-00001cb0: 6772 6f75 7072 3900 0000 5a09 726f 6c65  groupr9...Z.role
-00001cc0: 5f63 6f64 655a 0972 6f6c 655f 6e61 6d65  _codeZ.role_name
-00001cd0: 721f 0000 0072 2000 0000 7271 0000 0072  r....r ...rq...r
-00001ce0: 4100 0000 7221 0000 0072 4a00 0000 726f  A...r!...rJ...ro
-00001cf0: 0000 0072 7000 0000 5a0c 6372 6561 7465  ...rp...Z.create
-00001d00: 645f 7573 6572 721c 0000 005a 0a63 7265  d_userr....Z.cre
-00001d10: 6174 6564 5f61 745a 0a75 7064 6174 6564  ated_atZ.updated
-00001d20: 5f61 7472 1b00 0000 7219 0000 0072 1900  _atr....r....r..
-00001d30: 0000 7219 0000 0072 1a00 0000 7273 0000  ..r....r....rs..
-00001d40: 00d9 0000 0073 2400 0000 0801 0403 1601  .....s$.........
-00001d50: 1001 1001 1001 1201 0401 0201 0201 0401  ................
-00001d60: 0201 02fb 0607 1001 1201 1001 1002 7273  ..............rs
-00001d70: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001d80: 0000 0000 0700 0000 4000 0000 738c 0000  ........@...s...
-00001d90: 0065 005a 0164 005a 0264 015a 0365 046a  .e.Z.d.Z.d.Z.e.j
-00001da0: 0564 0264 0364 048d 025a 0665 046a 0764  .d.d.d...Z.e.j.d
-00001db0: 0564 0664 078d 025a 0865 046a 0964 0864  .d.d...Z.e.j.d.d
-00001dc0: 0964 0664 0a8d 035a 0a65 046a 0964 0b64  .d.d...Z.e.j.d.d
-00001dd0: 0964 0664 0664 0c8d 045a 0b65 046a 0564  .d.d.d...Z.e.j.d
-00001de0: 0d64 0e64 0664 0664 0f8d 045a 0c65 046a  .d.d.d.d...Z.e.j
-00001df0: 0d64 1064 1165 046a 0e64 1264 0664 138d  .d.d.e.j.d.d.d..
-00001e00: 055a 0f47 0064 1464 1584 0064 1583 025a  .Z.G.d.d...d...Z
-00001e10: 1064 1664 1784 005a 1164 1853 0029 19da  .d.d...Z.d.S.)..
-00001e20: 1043 6f6e 7465 6e74 5479 7065 4361 7465  .ContentTypeCate
-00001e30: 7375 1600 0000 0a20 2020 20e8 8f9c e58d  su.....    .....
-00001e40: 95e5 908d e7a7 b00a 2020 2020 7222 0000  ........    r"..
-00001e50: 0072 5000 0000 2901 7225 0000 0072 1200  .rP...).r%...r..
-00001e60: 0000 5429 0172 1400 0000 7263 0000 0072  ..T).r....rc...r
-00001e70: 6400 0000 7278 0000 0075 0600 0000 e7ba  d...rx...u......
-00001e80: a7e5 88ab 7265 0000 00f5 0600 0000 e59b  ....re..........
-00001e90: bee6 a087 e9f4 0100 0072 2800 0000 722e  .........r(...r.
-00001ea0: 0000 0075 0c00 0000 e788 b6e7 baa7 e88f  ...u............
-00001eb0: 9ce5 8d95 da08 6368 696c 6472 656e 7277  ......childrenrw
-00001ec0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001ed0: 0000 0000 0100 0000 4000 0000 731c 0000  ........@...s...
-00001ee0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00001ef0: 0465 045a 0564 035a 0664 0453 0029 057a  .e.Z.d.Z.d.S.).z
-00001f00: 1543 6f6e 7465 6e74 5479 7065 4361 7465  .ContentTypeCate
-00001f10: 732e 4d65 7461 5a14 6273 5f63 6f6e 7465  s.MetaZ.bs_conte
-00001f20: 6e74 5f74 7970 655f 6361 7473 750c 0000  nt_type_catsu...
-00001f30: 00e8 8f9c e58d 95e5 908d e7a7 b0a9 0172  ...............r
-00001f40: 7000 0000 4ea9 0772 1500 0000 7216 0000  p...N..r....r...
-00001f50: 0072 1700 0000 7237 0000 0072 0c00 0000  .r....r7...r....
-00001f60: 7238 0000 00da 086f 7264 6572 696e 6772  r8.....orderingr
-00001f70: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-00001f80: 0000 0072 1b00 0000 0501 0000 7308 0000  ...r........s...
-00001f90: 0008 0104 0104 0104 0172 1b00 0000 6301  .........r....c.
-00001fa0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001fb0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-00001fc0: 5300 726a 0000 00a9 0172 3a00 0000 a901  S.rj.....r:.....
-00001fd0: 722e 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00001fe0: 1a00 0000 da07 5f5f 7374 725f 5f0b 0100  ......__str__...
-00001ff0: 0073 0200 0000 0001 7a18 436f 6e74 656e  .s......z.Conten
-00002000: 7454 7970 6543 6174 6573 2e5f 5f73 7472  tTypeCates.__str
-00002010: 5f5f 4e29 1272 1500 0000 7216 0000 0072  __N).r....r....r
-00002020: 1700 0000 727a 0000 0072 0500 0000 7239  ....rz...r....r9
-00002030: 0000 0072 3a00 0000 721f 0000 0072 2000  ...r:...r....r .
-00002040: 0000 726f 0000 0072 7000 0000 da05 6c65  ..ro...rp.....le
-00002050: 7665 6cda 0a69 636f 6e5f 636c 6173 7372  vel..icon_classr
-00002060: 4100 0000 7242 0000 0072 4300 0000 721b  A...rB...rC...r.
-00002070: 0000 0072 8600 0000 7219 0000 0072 1900  ...r....r....r..
-00002080: 0000 7219 0000 0072 1a00 0000 727d 0000  ..r....r....r}..
-00002090: 00f4 0000 0073 1e00 0000 0801 0403 0e01  .....s..........
-000020a0: 0e01 1001 1201 1201 0401 0201 0201 0401  ................
-000020b0: 0201 02fb 0608 0e06 727d 0000 0063 0000  ........r}...c..
-000020c0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-000020d0: 0000 4000 0000 73ce 0000 0065 005a 0164  ..@...s....e.Z.d
-000020e0: 005a 0264 015a 0365 046a 0564 0264 0364  .Z.d.Z.e.j.d.d.d
-000020f0: 0464 058d 035a 0665 046a 0765 0864 0665  .d...Z.e.j.e.d.e
-00002100: 046a 0964 0764 088d 045a 0a65 046a 0764  .j.d.d...Z.e.j.d
-00002110: 0964 0a65 046a 0964 0b64 088d 045a 0b65  .d.e.j.d.d...Z.e
-00002120: 046a 0564 0c64 0d64 0464 0464 0e8d 045a  .j.d.d.d.d.d...Z
-00002130: 0c65 046a 0d64 0f64 0464 0464 108d 035a  .e.j.d.d.d.d...Z
-00002140: 0e65 046a 0d64 1164 0464 0464 108d 035a  .e.j.d.d.d.d...Z
-00002150: 0f65 046a 0564 1264 1364 0464 148d 035a  .e.j.d.d.d.d...Z
-00002160: 1065 046a 1164 1564 0464 168d 025a 1265  .e.j.d.d.d...Z.e
-00002170: 046a 1364 1764 0464 0464 188d 035a 1465  .j.d.d.d.d...Z.e
-00002180: 046a 1564 1964 1a64 0464 1b8d 035a 1647  .j.d.d.d.d...Z.G
-00002190: 0064 1c64 1d84 0064 1d83 025a 1764 1e64  .d.d...d...Z.d.d
-000021a0: 1f84 005a 1864 2053 0029 21da 0d43 6f6e  ...Z.d S.)!..Con
-000021b0: 7465 6e74 5479 7065 4578 7516 0000 000a  tentTypeExu.....
-000021c0: 2020 2020 e58a 9fe8 83bd e7b1 bbe5 88ab      ............
-000021d0: 0a20 2020 2072 2200 0000 7250 0000 0054  .    r"...rP...T
-000021e0: 2902 7225 0000 0072 0e00 0000 750c 0000  ).r%...r....u...
-000021f0: 00e7 b3bb e7bb 9fe5 ba94 e794 a8da 0965  ...............e
-00002200: 7874 656e 7369 6f6e 2903 720c 0000 0072  xtension).r....r
-00002210: 3100 0000 7275 0000 0072 7d00 0000 7506  1...ru...r}...u.
-00002220: 0000 00e8 8f9c e58d 955a 0d63 6f6e 7465  .........Z.conte
-00002230: 6e74 5f63 6174 6573 727e 0000 0072 7f00  nt_catesr~...r..
-00002240: 0000 7228 0000 00da 0375 726c 722a 0000  ..r(.....urlr*..
-00002250: 0075 0600 0000 e7bb 84e6 8890 7506 0000  .u..........u...
-00002260: 00e5 8f82 e695 b072 7600 0000 a903 720c  .......rv.....r.
-00002270: 0000 0072 2500 0000 720e 0000 0075 0900  ...r%...r....u..
-00002280: 0000 e987 8de5 ae9a e590 91a9 0272 0c00  .............r..
-00002290: 0000 720e 0000 0072 1200 0000 2902 7214  ..r....r....).r.
-000022a0: 0000 0072 0e00 0000 7263 0000 0072 6400  ...r....rc...rd.
-000022b0: 0000 7278 0000 0063 0000 0000 0000 0000  ..rx...c........
-000022c0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-000022d0: 731c 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-000022e0: 0364 025a 0465 045a 0564 035a 0664 0453  .d.Z.e.Z.d.Z.d.S
-000022f0: 0029 057a 1243 6f6e 7465 6e74 5479 7065  .).z.ContentType
-00002300: 4578 2e4d 6574 615a 1262 735f 636f 6e74  Ex.MetaZ.bs_cont
-00002310: 656e 745f 7479 7065 5f65 7875 1200 0000  ent_type_exu....
-00002320: e58a 9fe8 83bd e7b1 bbe5 88ab e8a1 a5e5  ................
-00002330: 8585 7281 0000 004e 7282 0000 0072 1900  ..r....Nr....r..
-00002340: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00002350: 0072 1b00 0000 2801 0000 7308 0000 0008  .r....(...s.....
-00002360: 0104 0104 0104 0172 1b00 0000 6301 0000  .......r....c...
-00002370: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00002380: 0043 0000 0073 0600 0000 7c00 6a00 5300  .C...s....|.j.S.
-00002390: 726a 0000 0072 8400 0000 7285 0000 0072  rj...r....r....r
-000023a0: 1900 0000 7219 0000 0072 1a00 0000 7286  ....r....r....r.
-000023b0: 0000 002e 0100 0073 0200 0000 0001 7a15  .......s......z.
-000023c0: 436f 6e74 656e 7454 7970 6545 782e 5f5f  ContentTypeEx.__
-000023d0: 7374 725f 5f4e 2919 7215 0000 0072 1600  str__N).r....r..
-000023e0: 0000 7217 0000 0072 7a00 0000 7205 0000  ..r....rz...r...
-000023f0: 0072 3900 0000 723a 0000 0072 4100 0000  .r9...r:...rA...
-00002400: 7204 0000 0072 4200 0000 da0c 636f 6e74  r....rB.....cont
-00002410: 656e 745f 7479 7065 5a10 636f 6e74 656e  ent_typeZ.conten
-00002420: 745f 7479 7065 5f63 6174 7288 0000 0072  t_type_catr....r
-00002430: 3c00 0000 da09 6672 6f6e 745f 7572 6c5a  <.....front_urlZ
-00002440: 0f66 726f 6e74 5f63 6f6d 706f 6e65 6e74  .front_component
-00002450: 5a0c 6672 6f6e 745f 7061 7261 6d73 da08  Z.front_params..
-00002460: 5552 4c46 6965 6c64 5a12 6672 6f6e 745f  URLFieldZ.front_
-00002470: 7265 6469 7265 6374 5f75 726c 721f 0000  redirect_urlr...
-00002480: 0072 2000 0000 726f 0000 0072 7000 0000  .r ...ro...rp...
-00002490: 721b 0000 0072 8600 0000 7219 0000 0072  r....r....r....r
-000024a0: 1900 0000 7219 0000 0072 1a00 0000 7289  ....r....r....r.
-000024b0: 0000 000f 0100 0073 2e00 0000 0801 0403  .......s........
-000024c0: 1001 0401 0201 0201 0401 02fc 0606 0401  ................
-000024d0: 0201 0201 0401 02fc 0606 1201 1001 1001  ................
-000024e0: 1001 0e01 1001 1002 0e06 7289 0000 0063  ..........r....c
-000024f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002500: 0600 0000 4000 0000 739c 0000 0065 005a  ....@...s....e.Z
-00002510: 0164 005a 0265 036a 0464 0164 0264 0364  .d.Z.e.j.d.d.d.d
-00002520: 048d 035a 0565 036a 0464 0564 0264 068d  ...Z.e.j.d.d.d..
-00002530: 025a 0665 036a 0464 0764 0864 068d 025a  .Z.e.j.d.d.d...Z
-00002540: 0765 036a 0864 0964 0364 0a8d 025a 0965  .e.j.d.d.d...Z.e
-00002550: 036a 0a65 0b64 0b65 036a 0c64 0364 0c8d  .j.e.d.e.j.d.d..
-00002560: 045a 0d65 036a 0464 0d64 0264 0364 0364  .Z.e.j.d.d.d.d.d
-00002570: 0e8d 045a 0e65 036a 0464 0f64 0264 0364  ...Z.e.j.d.d.d.d
-00002580: 0364 0e8d 045a 0f65 036a 1065 1164 1064  .d...Z.e.j.e.d.d
-00002590: 0364 118d 035a 1247 0064 1264 1384 0064  .d...Z.G.d.d...d
-000025a0: 1383 025a 1364 1453 0029 15da 0f45 7870  ...Z.d.S.)...Exp
-000025b0: 656e 7365 5374 616e 6461 7264 750c 0000  enseStandardu...
-000025c0: 00e8 b4b9 e794 a8e7 b1bb e59e 8b72 2700  .............r'.
-000025d0: 0000 5472 8c00 0000 750c 0000 00e6 a087  ..Tr....u.......
-000025e0: e587 86e5 908d e7a7 b072 2400 0000 750c  .........r$...u.
-000025f0: 0000 00e6 a087 e587 86e7 bc96 e7a0 8172  ...............r
-00002600: 2300 0000 7506 0000 00e8 b4b9 e794 a872  #...u..........r
-00002610: 8d00 0000 722f 0000 0072 3000 0000 7234  ....r/...r0...r4
-00002620: 0000 0072 2800 0000 7235 0000 0075 1200  ...r(...r5...u..
-00002630: 0000 e58c bbe7 949f e8b4 b9e7 94a8 e6a0  ................
-00002640: 87e5 8786 2902 720c 0000 0072 2900 0000  ....).r....r)...
-00002650: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00002660: 0001 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
-00002670: 5a01 6400 5a02 6401 5a03 6402 5a04 6504  Z.d.Z.d.Z.d.Z.e.
-00002680: 5a05 6403 5a06 6404 5300 2905 7a14 4578  Z.d.Z.d.S.).z.Ex
-00002690: 7065 6e73 6553 7461 6e64 6172 642e 4d65  penseStandard.Me
-000026a0: 7461 5a13 6273 5f65 7870 656e 7365 5f73  taZ.bs_expense_s
-000026b0: 7461 6e64 6172 6475 0f00 0000 e8b4 b9e7  tandardu........
-000026c0: 94a8 e6a0 87e5 8786 e8a1 a829 0129 02da  ...........).)..
-000026d0: 0d73 7461 6e64 6172 645f 636f 6465 724a  .standard_coderJ
-000026e0: 0000 004e 724b 0000 0072 1900 0000 7219  ...NrK...r....r.
-000026f0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00002700: 0000 4201 0000 7308 0000 0008 0104 0104  ..B...s.........
-00002710: 0104 0172 1b00 0000 4e29 1472 1500 0000  ...r....N).r....
-00002720: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
-00002730: 3900 0000 5a0c 6578 7065 6e73 655f 7479  9...Z.expense_ty
-00002740: 7065 5a0d 7374 616e 6461 7264 5f6e 616d  peZ.standard_nam
-00002750: 6572 9200 0000 7240 0000 005a 0466 6565  er....r@...Z.fee
-00002760: 7372 4100 0000 7221 0000 0072 4200 0000  srA...r!...rB...
-00002770: 724a 0000 0072 4400 0000 7245 0000 00da  rJ...rD...rE....
-00002780: 0f4d 616e 7954 6f4d 616e 7946 6965 6c64  .ManyToManyField
-00002790: 724f 0000 005a 0764 6f63 746f 7273 721b  rO...Z.doctorsr.
-000027a0: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-000027b0: 0000 721a 0000 0072 9100 0000 3201 0000  ..r....r....2...
-000027c0: 731c 0000 0008 0210 010e 010e 010e 0104  s...............
-000027d0: 0102 0102 0104 0102 fc06 0612 0112 0110  ................
-000027e0: 0272 9100 0000 6300 0000 0000 0000 0000  .r....c.........
-000027f0: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
-00002800: 4c00 0000 6500 5a01 6400 5a02 6503 6a04  L...e.Z.d.Z.e.j.
-00002810: 6401 6402 6403 8d02 5a05 6503 6a04 6404  d.d.d...Z.e.j.d.
-00002820: 6402 6403 8d02 5a06 6503 6a07 6405 6406  d.d...Z.e.j.d.d.
-00002830: 6503 6a08 6407 6408 6409 8d05 5a09 4700  e.j.d.d.d...Z.G.
-00002840: 640a 640b 8400 640b 8302 5a0a 640c 5300  d.d...d...Z.d.S.
-00002850: 290d da0e 496e 7370 6563 7469 6f6e 5479  )...InspectionTy
-00002860: 7065 f512 0000 00e6 a380 e69f a5e7 b1bb  pe..............
-00002870: e59e 8be7 bc96 e7a0 8172 7600 0000 7224  .........rv...r$
-00002880: 0000 00f5 1200 0000 e6a3 80e6 9fa5 e7b1  ................
-00002890: bbe5 9e8b e590 8de7 a7b0 722e 0000 00f5  ..........r.....
-000028a0: 0600 0000 e788 b6e7 baa7 7280 0000 0054  ..........r....T
-000028b0: 7277 0000 0063 0000 0000 0000 0000 0000  rw...c..........
-000028c0: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-000028d0: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-000028e0: 025a 0465 045a 0564 0353 0029 047a 1349  .Z.e.Z.d.S.).z.I
-000028f0: 6e73 7065 6374 696f 6e54 7970 652e 4d65  nspectionType.Me
-00002900: 7461 5a12 6273 5f69 6e73 7065 6374 696f  taZ.bs_inspectio
-00002910: 6e5f 7479 7065 7512 0000 00e6 a380 e69f  n_typeu.........
-00002920: a5e5 ad97 e585 b8e7 b1bb e59e 8b4e 7236  .............Nr6
-00002930: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
-00002940: 0000 721a 0000 0072 1b00 0000 5601 0000  ..r....r....V...
-00002950: 7306 0000 0008 0104 0104 0172 1b00 0000  s..........r....
-00002960: 4ea9 0b72 1500 0000 7216 0000 0072 1700  N..r....r....r..
-00002970: 0000 7205 0000 0072 3900 0000 da0a 636f  ..r....r9.....co
-00002980: 6465 5f73 7276 7470 da0a 6e61 6d65 5f73  de_srvtp..name_s
-00002990: 7276 7470 7241 0000 0072 4200 0000 7243  rvtprA...rB...rC
-000029a0: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
-000029b0: 0000 7219 0000 0072 1a00 0000 7294 0000  ..r....r....r...
-000029c0: 004b 0100 0073 1400 0000 0801 0e01 0e01  .K...s..........
-000029d0: 0401 0201 0201 0401 0201 02fb 0608 7294  ..............r.
-000029e0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000029f0: 0000 0000 0600 0000 4000 0000 73a6 0000  ........@...s...
-00002a00: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
-00002a10: 0264 0364 048d 035a 0565 036a 0464 0564  .d.d...Z.e.j.d.d
-00002a20: 0664 078d 025a 0665 036a 0464 0864 0964  .d...Z.e.j.d.d.d
-00002a30: 078d 025a 0765 036a 0464 0864 0a64 078d  ...Z.e.j.d.d.d..
-00002a40: 025a 0865 036a 0964 0b64 0364 0c8d 025a  .Z.e.j.d.d.d...Z
-00002a50: 0a65 036a 0464 0864 0d64 0364 0364 0e8d  .e.j.d.d.d.d.d..
-00002a60: 045a 0b65 036a 0464 0864 0f64 0364 0364  .Z.e.j.d.d.d.d.d
-00002a70: 0e8d 045a 0c65 036a 0464 1064 1164 0364  ...Z.e.j.d.d.d.d
-00002a80: 128d 035a 0d65 036a 0464 1364 1164 0364  ...Z.e.j.d.d.d.d
-00002a90: 128d 035a 0e47 0064 1464 1584 0064 1583  ...Z.G.d.d...d..
-00002aa0: 025a 0f64 1653 0029 17da 1649 6e73 7065  .Z.d.S.)...Inspe
-00002ab0: 6374 696f 6e44 6963 7469 6f6e 6172 6965  ctionDictionarie
-00002ac0: 7372 2300 0000 f50c 0000 00e9 a1b9 e79b  sr#.............
-00002ad0: aee7 bc96 e7a0 8154 722c 0000 0072 5100  .......Tr,...rQ.
-00002ae0: 0000 f50c 0000 00e9 a1b9 e79b aee5 908d  ................
-00002af0: e7a7 b0a9 0272 2500 0000 720c 0000 00e9  .....r%...r.....
-00002b00: 8000 0000 f50c 0000 00e5 8cbb e999 a2e7  ................
-00002b10: bc96 e7a0 8172 4700 0000 f50c 0000 00e9  .....rG.........
-00002b20: a1b9 e79b aee8 b4b9 e794 a872 8d00 0000  ...........r....
-00002b30: f506 0000 00e5 a487 e6b3 a872 7900 0000  ...........ry...
-00002b40: f50c 0000 00e5 8cba e588 86e5 ad97 e6ae  ................
-00002b50: b572 9500 0000 7276 0000 0072 8c00 0000  .r....rv...r....
-00002b60: 7296 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002b70: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
-00002b80: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00002b90: 025a 0465 045a 0564 0353 0029 047a 1b49  .Z.e.Z.d.S.).z.I
-00002ba0: 6e73 7065 6374 696f 6e44 6963 7469 6f6e  nspectionDiction
-00002bb0: 6172 6965 732e 4d65 7461 5a1a 6273 5f69  aries.MetaZ.bs_i
-00002bc0: 6e73 7065 6374 696f 6e5f 6469 6374 696f  nspection_dictio
-00002bd0: 6e61 7269 6573 750c 0000 00e6 a380 e69f  nariesu.........
-00002be0: a5e5 ad97 e585 b84e 7236 0000 0072 1900  .......Nr6...r..
-00002bf0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00002c00: 0072 1b00 0000 6701 0000 7306 0000 0008  .r....g...s.....
-00002c10: 0104 0104 0172 1b00 0000 4ea9 1072 1500  .....r....N..r..
-00002c20: 0000 7216 0000 0072 1700 0000 7205 0000  ..r....r....r...
-00002c30: 0072 3900 0000 5a0c 7072 6f6a 6563 745f  .r9...Z.project_
-00002c40: 636f 6465 5a0c 7072 6f6a 6563 745f 6e61  codeZ.project_na
-00002c50: 6d65 da0d 686f 7370 6974 616c 5f63 6f64  me..hospital_cod
-00002c60: 655a 0b6f 6666 6963 655f 636f 6465 7240  eZ.office_coder@
-00002c70: 0000 005a 0c70 726f 6a65 6374 5f66 6565  ...Z.project_fee
-00002c80: 735a 0772 656d 6172 6b73 5a0b 6469 7374  sZ.remarksZ.dist
-00002c90: 696e 6775 6973 6872 9900 0000 729a 0000  inguishr....r...
-00002ca0: 0072 1b00 0000 7219 0000 0072 1900 0000  .r....r....r....
-00002cb0: 7219 0000 0072 1a00 0000 729b 0000 005c  r....r....r....\
-00002cc0: 0100 0073 1400 0000 0801 1001 0e01 0e01  ...s............
-00002cd0: 0e01 0e01 1201 1201 1001 1002 729b 0000  ............r...
-00002ce0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00002cf0: 0000 0700 0000 4000 0000 734c 0000 0065  ......@...sL...e
-00002d00: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
-00002d10: 038d 025a 0565 036a 0464 0464 0264 038d  ...Z.e.j.d.d.d..
-00002d20: 025a 0665 036a 0764 0564 0665 036a 0864  .Z.e.j.d.d.e.j.d
-00002d30: 0764 0864 098d 055a 0947 0064 0a64 0b84  .d.d...Z.G.d.d..
-00002d40: 0064 0b83 025a 0a64 0c53 0029 0dda 0f45  .d...Z.d.S.)...E
-00002d50: 7861 6d69 6e61 7469 6f6e 5479 7065 7295  xaminationTyper.
-00002d60: 0000 0072 7600 0000 7224 0000 0072 9600  ...rv...r$...r..
-00002d70: 0000 722e 0000 0072 9700 0000 7280 0000  ..r....r....r...
-00002d80: 0054 7277 0000 0063 0000 0000 0000 0000  .Trw...c........
-00002d90: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00002da0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00002db0: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-00002dc0: 1445 7861 6d69 6e61 7469 6f6e 5479 7065  .ExaminationType
-00002dd0: 2e4d 6574 615a 1362 735f 6578 616d 696e  .MetaZ.bs_examin
-00002de0: 6174 696f 6e5f 7479 7065 7512 0000 00e6  ation_typeu.....
-00002df0: a380 e9aa 8ce5 ad97 e585 b8e7 b1bb e59e  ................
-00002e00: 8b4e 7236 0000 0072 1900 0000 7219 0000  .Nr6...r....r...
-00002e10: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00002e20: 7801 0000 7306 0000 0008 0104 0104 0172  x...s..........r
-00002e30: 1b00 0000 4e72 9800 0000 7219 0000 0072  ....Nr....r....r
-00002e40: 1900 0000 7219 0000 0072 1a00 0000 72a6  ....r....r....r.
-00002e50: 0000 006d 0100 0073 1400 0000 0801 0e01  ...m...s........
-00002e60: 0e01 0401 0201 0201 0401 0201 02fb 0608  ................
-00002e70: 72a6 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002e80: 0000 0000 0000 0600 0000 4000 0000 73a6  ..........@...s.
-00002e90: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-00002ea0: 0164 0264 0364 048d 035a 0565 036a 0464  .d.d.d...Z.e.j.d
-00002eb0: 0564 0664 078d 025a 0665 036a 0464 0864  .d.d...Z.e.j.d.d
-00002ec0: 0964 078d 025a 0765 036a 0464 0864 0a64  .d...Z.e.j.d.d.d
-00002ed0: 078d 025a 0865 036a 0964 0b64 0364 0c8d  ...Z.e.j.d.d.d..
-00002ee0: 025a 0a65 036a 0464 0864 0d64 0364 0364  .Z.e.j.d.d.d.d.d
-00002ef0: 0e8d 045a 0b65 036a 0464 0864 0f64 0364  ...Z.e.j.d.d.d.d
-00002f00: 0364 0e8d 045a 0c65 036a 0464 1064 1164  .d...Z.e.j.d.d.d
-00002f10: 0364 128d 035a 0d65 036a 0464 1364 1164  .d...Z.e.j.d.d.d
-00002f20: 0364 128d 035a 0e47 0064 1464 1584 0064  .d...Z.G.d.d...d
-00002f30: 1583 025a 0f64 1653 0029 17da 1745 7861  ...Z.d.S.)...Exa
-00002f40: 6d69 6e61 7469 6f6e 4469 6374 696f 6e61  minationDictiona
-00002f50: 7269 6573 7223 0000 0072 9c00 0000 5472  riesr#...r....Tr
-00002f60: 2c00 0000 7251 0000 0072 9d00 0000 729e  ,...rQ...r....r.
-00002f70: 0000 0072 9f00 0000 72a0 0000 0072 4700  ...r....r....rG.
-00002f80: 0000 72a1 0000 0072 8d00 0000 72a2 0000  ..r....r....r...
-00002f90: 0072 7900 0000 72a3 0000 0075 1200 0000  .ry...r....u....
-00002fa0: e6a3 80e9 aa8c e7b1 bbe5 9e8b e7bc 96e7  ................
-00002fb0: a081 7276 0000 0072 8c00 0000 7512 0000  ..rv...r....u...
-00002fc0: 00e6 a380 e9aa 8ce7 b1bb e59e 8be5 908d  ................
-00002fd0: e7a7 b063 0000 0000 0000 0000 0000 0000  ...c............
-00002fe0: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-00002ff0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-00003000: 0465 045a 0564 0353 0029 047a 1c45 7861  .e.Z.d.S.).z.Exa
-00003010: 6d69 6e61 7469 6f6e 4469 6374 696f 6e61  minationDictiona
-00003020: 7269 6573 2e4d 6574 615a 1b62 735f 6578  ries.MetaZ.bs_ex
-00003030: 616d 696e 6174 696f 6e5f 6469 6374 696f  amination_dictio
-00003040: 6e61 7269 6573 750c 0000 00e6 a380 e9aa  nariesu.........
-00003050: 8ce5 ad97 e585 b84e 7236 0000 0072 1900  .......Nr6...r..
-00003060: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00003070: 0072 1b00 0000 8901 0000 7306 0000 0008  .r........s.....
-00003080: 0104 0104 0172 1b00 0000 4e72 a400 0000  .....r....Nr....
-00003090: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-000030a0: 1a00 0000 72a7 0000 007e 0100 0073 1400  ....r....~...s..
-000030b0: 0000 0801 1001 0e01 0e01 0e01 0e01 1201  ................
-000030c0: 1201 1001 1002 72a7 0000 0063 0000 0000  ......r....c....
-000030d0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-000030e0: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
-000030f0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-00003100: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
-00003110: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
-00003120: 0764 0a53 0029 0bda 1344 7275 6750 7265  .d.S.)...DrugPre
-00003130: 7061 7261 7469 6f6e 5479 7065 7223 0000  parationTyper#..
-00003140: 0072 2b00 0000 5472 2c00 0000 7251 0000  .r+...Tr,...rQ..
-00003150: 0075 0c00 0000 e7b1 bbe5 9e8b e590 8de7  .u..............
-00003160: a7b0 7279 0000 0063 0000 0000 0000 0000  ..ry...c........
-00003170: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00003180: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00003190: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-000031a0: 1844 7275 6750 7265 7061 7261 7469 6f6e  .DrugPreparation
-000031b0: 5479 7065 2e4d 6574 615a 1862 735f 6472  Type.MetaZ.bs_dr
-000031c0: 7567 5f70 7265 7061 7261 7469 6f6e 5f74  ug_preparation_t
-000031d0: 7970 6575 1200 0000 e88d afe5 9381 e588  ypeu............
-000031e0: b6e5 8982 e7b1 bbe5 9e8b 4e72 3600 0000  ..........Nr6...
-000031f0: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
-00003200: 1a00 0000 721b 0000 0093 0100 0073 0600  ....r........s..
-00003210: 0000 0801 0401 0401 721b 0000 004e 2908  ........r....N).
-00003220: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
-00003230: 0500 0000 7239 0000 0072 3e00 0000 da09  ....r9...r>.....
-00003240: 7479 7065 5f6e 616d 6572 1b00 0000 7219  type_namer....r.
-00003250: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00003260: 0000 72a8 0000 008f 0100 0073 0600 0000  ..r........s....
-00003270: 0801 1001 1202 72a8 0000 0063 0000 0000  ......r....c....
-00003280: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003290: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
-000032a0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-000032b0: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
-000032c0: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
-000032d0: 0764 0a53 0029 0bda 0844 7275 6754 7970  .d.S.)...DrugTyp
-000032e0: 6572 2b00 0000 7223 0000 0054 a903 720c  er+...r#...T..r.
-000032f0: 0000 0072 2500 0000 722d 0000 0072 2200  ...r%...r-...r".
-00003300: 0000 7251 0000 0072 2800 0000 6300 0000  ..rQ...r(...c...
-00003310: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00003320: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
-00003330: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
-00003340: 5300 2904 7a0d 4472 7567 5479 7065 2e4d  S.).z.DrugType.M
-00003350: 6574 615a 0c62 735f 6472 7567 5f74 7970  etaZ.bs_drug_typ
-00003360: 65f5 0c00 0000 e88d afe5 9381 e7b1 bbe5  e...............
-00003370: 9e8b 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
-00003380: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00003390: 009d 0100 0073 0600 0000 0801 0401 0401  .....s..........
-000033a0: 721b 0000 004e a908 7215 0000 0072 1600  r....N..r....r..
-000033b0: 0000 7217 0000 0072 0500 0000 7239 0000  ..r....r....r9..
-000033c0: 00da 0463 6f64 6572 3a00 0000 721b 0000  ...coder:...r...
-000033d0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-000033e0: 721a 0000 0072 aa00 0000 9901 0000 7306  r....r........s.
-000033f0: 0000 0008 0110 0112 0272 aa00 0000 6300  .........r....c.
-00003400: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00003410: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
-00003420: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-00003430: 8d03 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
-00003440: 6407 8d04 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
-00003450: 8302 5a07 640a 5300 290b da0c 4472 7567  ..Z.d.S.)...Drug
-00003460: 4361 7465 676f 7279 7223 0000 0072 2b00  Categoryr#...r+.
-00003470: 0000 5472 2c00 0000 7251 0000 0075 0c00  ..Tr,...rQ...u..
-00003480: 0000 e7b1 bbe5 88ab e590 8de7 a7b0 7279  ..............ry
-00003490: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000034a0: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
-000034b0: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
-000034c0: 0465 045a 0564 0353 0029 047a 1144 7275  .e.Z.d.S.).z.Dru
-000034d0: 6743 6174 6567 6f72 792e 4d65 7461 5a10  gCategory.MetaZ.
-000034e0: 6273 5f64 7275 675f 6361 7465 676f 7279  bs_drug_category
-000034f0: 750c 0000 00e8 8daf e593 81e7 b1bb e588  u...............
-00003500: ab4e 7236 0000 0072 1900 0000 7219 0000  .Nr6...r....r...
-00003510: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00003520: a701 0000 7306 0000 0008 0104 0104 0172  ....s..........r
-00003530: 1b00 0000 4e29 0872 1500 0000 7216 0000  ....N).r....r...
-00003540: 0072 1700 0000 7205 0000 0072 3900 0000  .r....r....r9...
-00003550: 723e 0000 005a 0d63 6174 6567 6f72 795f  r>...Z.category_
-00003560: 6e61 6d65 721b 0000 0072 1900 0000 7219  namer....r....r.
-00003570: 0000 0072 1900 0000 721a 0000 0072 af00  ...r....r....r..
-00003580: 0000 a301 0000 7306 0000 0008 0110 0112  ......s.........
-00003590: 0272 af00 0000 6300 0000 0000 0000 0000  .r....c.........
-000035a0: 0000 0000 0000 0006 0000 0040 0000 0073  ...........@...s
-000035b0: 9e01 0000 6500 5a01 6400 5a02 6503 6a04  ....e.Z.d.Z.e.j.
-000035c0: 6401 6402 6403 6404 8d03 5a05 6503 6a04  d.d.d.d...Z.e.j.
-000035d0: 6405 6406 6403 6403 6407 8d04 5a06 6503  d.d.d.d.d...Z.e.
-000035e0: 6a04 6405 6408 6403 6403 6407 8d04 5a07  j.d.d.d.d.d...Z.
-000035f0: 6503 6a04 6405 6409 6403 6403 6407 8d04  e.j.d.d.d.d.d...
-00003600: 5a08 6503 6a04 640a 640b 6403 6403 640c  Z.e.j.d.d.d.d.d.
-00003610: 8d04 5a09 6503 6a0a 650b 640d 6503 6a0c  ..Z.e.j.e.d.e.j.
-00003620: 640e 8d03 5a0d 6503 6a0a 650e 640f 6503  d...Z.e.j.e.d.e.
-00003630: 6a0c 640e 8d03 5a0f 6503 6a0a 6510 6410  j.d...Z.e.j.e.d.
-00003640: 6503 6a0c 640e 8d03 5a11 6503 6a04 6411  e.j.d...Z.e.j.d.
-00003650: 640b 6403 6403 640c 8d04 5a12 6503 6a04  d.d.d.d...Z.e.j.
-00003660: 6412 640b 6403 6403 640c 8d04 5a13 6503  d.d.d.d.d...Z.e.
-00003670: 6a04 6413 640b 6403 6403 640c 8d04 5a14  j.d.d.d.d.d...Z.
-00003680: 6503 6a04 6414 640b 6403 6403 640c 8d04  e.j.d.d.d.d.d...
-00003690: 5a15 6503 6a04 6415 640b 6403 6403 640c  Z.e.j.d.d.d.d.d.
-000036a0: 8d04 5a16 6503 6a04 6416 640b 6403 6403  ..Z.e.j.d.d.d.d.
-000036b0: 640c 8d04 5a17 6503 6a04 6417 640b 6403  d...Z.e.j.d.d.d.
-000036c0: 6403 640c 8d04 5a18 6503 6a19 6418 6403  d.d...Z.e.j.d.d.
-000036d0: 6419 8d02 5a1a 6503 6a04 641a 6405 6403  d...Z.e.j.d.d.d.
-000036e0: 6403 640c 8d04 5a1b 6503 6a04 641b 6405  d.d...Z.e.j.d.d.
-000036f0: 6403 6403 640c 8d04 5a1c 6503 6a04 641c  d.d.d...Z.e.j.d.
-00003700: 6405 6403 6403 640c 8d04 5a1d 6503 6a04  d.d.d.d...Z.e.j.
-00003710: 6405 641d 6403 6403 6407 8d04 5a1e 6503  d.d.d.d.d...Z.e.
-00003720: 6a04 6405 641e 6403 6403 6407 8d04 5a1f  j.d.d.d.d.d...Z.
-00003730: 6503 6a04 641f 6405 6403 6420 8d03 5a20  e.j.d.d.d.d ..Z 
-00003740: 4700 6421 6422 8400 6422 8302 5a21 6423  G.d!d"..d"..Z!d#
-00003750: 5300 2924 da0d 4472 7567 4469 7265 6374  S.)$..DrugDirect
-00003760: 6f72 79f5 0c00 0000 e88d afe5 9381 e7bc  ory.............
-00003770: 96e7 a081 7223 0000 0054 72ab 0000 0072  ....r#...Tr....r
-00003780: 5100 0000 f50c 0000 00e8 8daf e593 81e5  Q...............
-00003790: 908d e7a7 b072 7900 0000 f506 0000 00e8  .....ry.........
-000037a0: a784 e6a0 bc75 0c00 0000 e59f bae6 9cac  .....u..........
-000037b0: e58d 95e4 bd8d 7512 0000 00e6 80bb e987  ......u.........
-000037c0: 8fe5 8d95 e4bd 8de7 bc96 e7a0 8172 5000  .............rP.
-000037d0: 0000 7228 0000 00f5 0c00 0000 e588 b6e5  ..r(............
-000037e0: 8982 e7b1 bbe5 9e8b 7248 0000 00f5 0600  ........rH......
-000037f0: 0000 e7b1 bbe5 88ab 72ac 0000 0075 0c00  ........r....u..
-00003800: 0000 e58d 95e4 bd8d e589 82e9 878f 7513  ..............u.
-00003810: 0000 00e8 aea1 e987 8f2f e99b b6e5 94ae  ........./......
-00003820: e58d 95e4 bd8d 7512 0000 00e8 aea1 e987  ......u.........
-00003830: 8fe5 8d95 e4bd 8de7 bc96 e7a0 81f5 0c00  ................
-00003840: 0000 e5ba 93e5 ad98 e695 b0e9 878f 750c  ..............u.
-00003850: 0000 00e5 ba93 e5ad 98e5 8d95 e4bd 8d75  ...............u
-00003860: 0c00 0000 e58c bbe4 bf9d e7b1 bbe5 88ab  ................
-00003870: 750c 0000 00e5 869c e590 88e7 b1bb e588  u...............
-00003880: ab75 0f00 0000 e698 afe5 90a6 e698 afe5  .u..............
-00003890: 9fba e88d af72 1300 0000 750c 0000 00e9  .....r....u.....
-000038a0: ab98 e58d b1e7 ad89 e7ba a775 1200 0000  ...........u....
-000038b0: e59b bde5 aeb6 e8b4 afe6 a087 e7bc 96e7  ................
-000038c0: a081 7512 0000 00e5 9bbd e5ae b6e8 b4af  ..u.............
-000038d0: e6a0 87e5 908d e7a7 b0f5 0600 0000 e4ba  ................
-000038e0: a7e5 9cb0 f50c 0000 00e7 949f e4ba a7e5  ................
-000038f0: 8e82 e5ae b675 1800 0000 e58d 95e6 aca1  .....u..........
-00003900: e794 a8e9 878f e58d 95e4 bd8d e7bc 96e7  ................
-00003910: a081 728c 0000 0063 0000 0000 0000 0000  ..r....c........
-00003920: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00003930: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00003940: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-00003950: 1244 7275 6744 6972 6563 746f 7279 2e4d  .DrugDirectory.M
-00003960: 6574 615a 1162 735f 6472 7567 5f64 6972  etaZ.bs_drug_dir
-00003970: 6563 746f 7279 750c 0000 00e8 8daf e593  ectoryu.........
-00003980: 81e7 9bae e5bd 954e 7236 0000 0072 1900  .......Nr6...r..
-00003990: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000039a0: 0072 1b00 0000 d101 0000 7306 0000 0008  .r........s.....
-000039b0: 0104 0104 0172 1b00 0000 4e29 2272 1500  .....r....N)"r..
-000039c0: 0000 7216 0000 0072 1700 0000 7205 0000  ..r....r....r...
-000039d0: 0072 3900 0000 da09 6472 7567 5f63 6f64  .r9.....drug_cod
-000039e0: 65da 0964 7275 675f 6e61 6d65 da09 7374  e..drug_name..st
-000039f0: 616e 6461 7264 735a 0a74 6f74 616c 5f75  andardsZ.total_u
-00003a00: 6e69 745a 0f74 6f74 616c 5f75 6e69 745f  nitZ.total_unit_
-00003a10: 636f 6465 7241 0000 0072 a800 0000 da0a  coderA...r......
-00003a20: 444f 5f4e 4f54 4849 4e47 da10 7072 6570  DO_NOTHING..prep
-00003a30: 6172 6174 696f 6e5f 7479 7065 72af 0000  aration_typer...
-00003a40: 00da 0863 6174 6567 6f72 7972 aa00 0000  ...categoryr....
-00003a50: da09 6472 7567 5f74 7970 655a 0975 6e69  ..drug_typeZ.uni
-00003a60: 745f 646f 7365 5a0c 6d65 6173 7572 655f  t_doseZ.measure_
-00003a70: 756e 6974 5a11 6d65 6173 7572 655f 756e  unitZ.measure_un
-00003a80: 6974 5f63 6f64 655a 0a73 746f 636b 5f6c  it_codeZ.stock_l
-00003a90: 6566 745a 0a73 746f 636b 5f75 6e69 745a  eftZ.stock_unitZ
-00003aa0: 036d 6963 5a0c 7263 635f 6361 7465 676f  .micZ.rcc_catego
-00003ab0: 7279 721f 0000 005a 0c69 735f 6573 7365  ryr....Z.is_esse
-00003ac0: 6e74 6961 6c5a 0868 725f 6c65 7665 6c5a  ntialZ.hr_levelZ
-00003ad0: 0767 625f 636f 6465 5a07 6762 5f6e 616d  .gb_codeZ.gb_nam
-00003ae0: 65da 0c6f 7269 6769 6e5f 706c 6163 65da  e..origin_place.
-00003af0: 0c6d 616e 7566 6163 7475 7265 725a 0d63  .manufacturerZ.c
-00003b00: 6f64 655f 6d65 6475 5f63 7572 721b 0000  ode_medu_curr...
-00003b10: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00003b20: 721a 0000 0072 b000 0000 ad01 0000 7346  r....r........sF
-00003b30: 0000 0008 0110 0112 0112 0112 0112 0104  ................
-00003b40: 0102 0102 0104 fd06 0504 0102 0102 0104  ................
-00003b50: fd06 0504 0102 0102 0104 fd06 0512 0112  ................
-00003b60: 0112 0112 0112 0112 0112 010e 0112 0112  ................
-00003b70: 0112 0112 0112 0110 0272 b000 0000 6300  .........r....c.
-00003b80: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00003b90: 0000 0040 0000 0073 3c00 0000 6500 5a01  ...@...s<...e.Z.
-00003ba0: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-00003bb0: 8d03 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
-00003bc0: 6407 8d04 5a06 4700 6408 6409 8400 6409  d...Z.G.d.d...d.
-00003bd0: 8302 5a07 640a 5300 290b da0c 5068 6172  ..Z.d.S.)...Phar
-00003be0: 6d61 6379 5479 7065 722b 0000 0072 2300  macyTyper+...r#.
-00003bf0: 0000 5472 ab00 0000 7222 0000 0072 5100  ..Tr....r"...rQ.
-00003c00: 0000 7228 0000 0063 0000 0000 0000 0000  ..r(...c........
-00003c10: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
-00003c20: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00003c30: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
-00003c40: 1150 6861 726d 6163 7954 7970 652e 4d65  .PharmacyType.Me
-00003c50: 7461 5a10 6273 5f70 6861 726d 6163 795f  taZ.bs_pharmacy_
-00003c60: 7479 7065 f50c 0000 00e8 8daf e688 bfe7  type............
-00003c70: b1bb e59e 8b4e 7236 0000 0072 1900 0000  .....Nr6...r....
-00003c80: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00003c90: 1b00 0000 db01 0000 7306 0000 0008 0104  ........s.......
-00003ca0: 0104 0172 1b00 0000 4e72 ad00 0000 7219  ...r....Nr....r.
+000001f0: 650e 8303 5a24 4700 6435 6436 8400 6436  e...Z$G.d5d6..d6
+00000200: 6509 6a0d 8303 5a25 6401 5300 2937 e900  e.j...Z%d.S.)7..
+00000210: 0000 004e 2902 da0c 4162 7374 7261 6374  ...N)...Abstract
+00000220: 5573 6572 da05 4772 6f75 7029 01da 0b43  User..Group)...C
+00000230: 6f6e 7465 6e74 5479 7065 2901 da06 6d6f  ontentType)...mo
+00000240: 6465 6c73 2901 da08 7365 7474 696e 6773  dels)...settings
+00000250: 2902 2902 da01 3175 0300 0000 e794 b729  ).)...1u.......)
+00000260: 02da 0130 7503 0000 00e5 a5b3 6300 0000  ...0u.......c...
+00000270: 0000 0000 0000 0000 0000 0000 0005 0000  ................
+00000280: 0040 0000 0073 4800 0000 6500 5a01 6400  .@...sH...e.Z.d.
+00000290: 5a02 6503 6a04 6401 6402 6402 6403 8d03  Z.e.j.d.d.d.d...
+000002a0: 5a05 6503 6a04 6404 6402 6402 6405 8d03  Z.e.j.d.d.d.d...
+000002b0: 5a06 6503 6a07 6406 6402 6407 8d02 5a08  Z.e.j.d.d.d...Z.
+000002c0: 4700 6408 6409 8400 6409 8302 5a09 640a  G.d.d...d...Z.d.
+000002d0: 5300 290b da10 4d65 6469 6361 6c42 6173  S.)...MedicalBas
+000002e0: 654d 6f64 656c f50c 0000 00e5 889b e5bb  eModel..........
+000002f0: bae6 97b6 e997 b454 a903 da0c 7665 7262  .......T....verb
+00000300: 6f73 655f 6e61 6d65 da0c 6175 746f 5f6e  ose_name..auto_n
+00000310: 6f77 5f61 6464 da04 6e75 6c6c f50c 0000  ow_add..null....
+00000320: 00e6 9bb4 e696 b0e6 97b6 e997 b4a9 0372  ...............r
+00000330: 0c00 0000 da08 6175 746f 5f6e 6f77 720e  ......auto_nowr.
+00000340: 0000 00f5 0c00 0000 e698 afe5 90a6 e590  ................
+00000350: afe7 94a8 a902 720c 0000 00da 0764 6566  ......r......def
+00000360: 6175 6c74 6300 0000 0000 0000 0000 0000  aultc...........
+00000370: 0000 0000 0001 0000 0040 0000 0073 1000  .........@...s..
+00000380: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00000390: 5300 2903 7a15 4d65 6469 6361 6c42 6173  S.).z.MedicalBas
+000003a0: 654d 6f64 656c 2e4d 6574 6154 4e29 04da  eModel.MetaTN)..
+000003b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000003c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000003d0: 655f 5fda 0861 6273 7472 6163 74a9 0072  e__..abstract..r
+000003e0: 1900 0000 7219 0000 00fa 372f 686f 6d65  ....r.....7/home
+000003f0: 2f6c 7968 2f77 6f72 6b2f 4261 7365 4675  /lyh/work/BaseFu
+00000400: 6e63 7469 6f6e 4d6f 6475 6c65 2f62 6173  nctionModule/bas
+00000410: 655f 7379 7374 656d 2f6d 6f64 656c 732e  e_system/models.
+00000420: 7079 da04 4d65 7461 1500 0000 7302 0000  py..Meta....s...
+00000430: 0008 0172 1b00 0000 4e29 0a72 1500 0000  ...r....N).r....
+00000440: 7216 0000 0072 1700 0000 7205 0000 00da  r....r....r.....
+00000450: 0d44 6174 6554 696d 6546 6965 6c64 da0c  .DateTimeField..
+00000460: 6372 6561 7465 645f 7469 6d65 da0c 7570  created_time..up
+00000470: 6461 7465 645f 7469 6d65 da0c 426f 6f6c  dated_time..Bool
+00000480: 6561 6e46 6965 6c64 da09 6973 5f61 6374  eanField..is_act
+00000490: 6976 6572 1b00 0000 7219 0000 0072 1900  iver....r....r..
+000004a0: 0000 7219 0000 0072 1a00 0000 7209 0000  ..r....r....r...
+000004b0: 0010 0000 0073 0800 0000 0801 1001 1001  .....s..........
+000004c0: 0e02 7209 0000 0063 0000 0000 0000 0000  ..r....c........
+000004d0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
+000004e0: 73d8 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
+000004f0: 0464 0164 0264 038d 025a 0565 036a 0464  .d.d.d...Z.e.j.d
+00000500: 0464 0564 0664 0664 078d 045a 0665 036a  .d.d.d.d...Z.e.j
+00000510: 0764 0864 0664 0664 098d 035a 0865 036a  .d.d.d.d...Z.e.j
+00000520: 0464 0264 0a64 0664 0b8d 035a 0965 036a  .d.d.d.d...Z.e.j
+00000530: 0764 0c64 0d8d 015a 0a65 036a 0b64 0e64  .d.d...Z.e.j.d.d
+00000540: 0d8d 015a 0c65 036a 0b64 0f64 0d8d 015a  ...Z.e.j.d.d...Z
+00000550: 0d65 036a 0e64 1064 1165 036a 0f64 0664  .e.j.d.d.e.j.d.d
+00000560: 128d 045a 1065 036a 0464 1364 0564 1464  ...Z.e.j.d.d.d.d
+00000570: 0664 158d 045a 1165 036a 0464 1664 0564  .d...Z.e.j.d.d.d
+00000580: 1764 188d 035a 1265 036a 0464 1964 0564  .d...Z.e.j.d.d.d
+00000590: 0664 0664 078d 045a 1365 036a 0464 1a64  .d.d...Z.e.j.d.d
+000005a0: 0564 0664 0664 078d 045a 1447 0064 1b64  .d.d.d...Z.G.d.d
+000005b0: 1c84 0064 1c83 025a 1564 1d53 0029 1eda  ...d...Z.d.S.)..
+000005c0: 0848 6f73 7069 7461 6cf5 0600 0000 e590  .Hospital.......
+000005d0: 8de7 a7b0 e9ff 0000 00a9 0272 0c00 0000  ...........r....
+000005e0: da0a 6d61 785f 6c65 6e67 7468 f50c 0000  ..max_length....
+000005f0: 00e8 8194 e7b3 bbe6 96b9 e5bc 8fe9 6400  ..............d.
+00000600: 0000 54a9 0472 0c00 0000 7225 0000 0072  ..T..r....r%...r
+00000610: 0e00 0000 da05 626c 616e 6b75 0c00 0000  ......blanku....
+00000620: e58c bbe9 99a2 e7ae 80e4 bb8b a903 720c  ..............r.
+00000630: 0000 0072 0e00 0000 7229 0000 00f5 0600  ...r....r)......
+00000640: 0000 e7bc 96e7 a081 a903 7225 0000 0072  ..........r%...r
+00000650: 0c00 0000 da06 756e 6971 7565 750c 0000  ......uniqueu...
+00000660: 00e5 8cbb e999 a2e5 9cb0 e59d 8029 0172  .............).r
+00000670: 0c00 0000 7506 0000 00e7 bb8f e5ba a675  ....u..........u
+00000680: 0600 0000 e7bb b4e5 baa6 da04 7365 6c66  ............self
+00000690: f50c 0000 00e6 8980 e5b1 9ee5 8cbb e999  ................
+000006a0: a2a9 0372 0c00 0000 da09 6f6e 5f64 656c  ...r......on_del
+000006b0: 6574 6572 0e00 0000 750c 0000 00e5 8cbb  eter....u.......
+000006c0: e999 a2e5 9bbe e789 875a 0f68 6f73 7069  .........Z.hospi
+000006d0: 7461 6c5f 696d 6167 6573 2904 720c 0000  tal_images).r...
+000006e0: 0072 2500 0000 7214 0000 0072 2900 0000  .r%...r....r)...
+000006f0: da04 6c6f 676f 5a0d 686f 7370 6974 616c  ..logoZ.hospital
+00000700: 5f6c 6f67 6fa9 0372 0c00 0000 7225 0000  _logo..r....r%..
+00000710: 0072 1400 0000 f509 0000 00e5 889b e5bb  .r..............
+00000720: bae4 baba f509 0000 00e6 9bb4 e696 b0e4  ................
+00000730: baba 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000740: 0000 0001 0000 0040 0000 0073 1800 0000  .......@...s....
+00000750: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+00000760: 6504 5a05 6403 5300 2904 7a0d 486f 7370  e.Z.d.S.).z.Hosp
+00000770: 6974 616c 2e4d 6574 615a 0b62 735f 686f  ital.MetaZ.bs_ho
+00000780: 7370 6974 616c 7506 0000 00e5 8cbb e999  spitalu.........
+00000790: a24e a906 7215 0000 0072 1600 0000 7217  .N..r....r....r.
+000007a0: 0000 00da 0864 625f 7461 626c 6572 0c00  .....db_tabler..
+000007b0: 0000 da13 7665 7262 6f73 655f 6e61 6d65  ....verbose_name
+000007c0: 5f70 6c75 7261 6c72 1900 0000 7219 0000  _pluralr....r...
+000007d0: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000007e0: 2e00 0000 7306 0000 0008 0104 0104 0172  ....s..........r
+000007f0: 1b00 0000 4e29 1672 1500 0000 7216 0000  ....N).r....r...
+00000800: 0072 1700 0000 7205 0000 00da 0943 6861  .r....r......Cha
+00000810: 7246 6965 6c64 da04 6e61 6d65 da05 7068  rField..name..ph
+00000820: 6f6e 65da 0954 6578 7446 6965 6c64 da09  one..TextField..
+00000830: 696e 7472 6f64 7563 65da 0763 6f64 656e  introduce..coden
+00000840: 756d da07 6164 6472 6573 73da 0a46 6c6f  um..address..Flo
+00000850: 6174 4669 656c 645a 096c 6f6e 6769 7475  atFieldZ.longitu
+00000860: 6465 5a08 6c61 7469 7475 6465 da0a 466f  deZ.latitude..Fo
+00000870: 7265 6967 6e4b 6579 da07 4341 5343 4144  reignKey..CASCAD
+00000880: 45da 0670 6172 656e 745a 0a68 6f73 5f69  E..parentZ.hos_i
+00000890: 6d61 6765 7372 3200 0000 da0a 6372 6561  magesr2.....crea
+000008a0: 7465 645f 6279 da0a 7570 6461 7465 645f  ted_by..updated_
+000008b0: 6279 721b 0000 0072 1900 0000 7219 0000  byr....r....r...
+000008c0: 0072 1900 0000 721a 0000 0072 2100 0000  .r....r....r!...
+000008d0: 1900 0000 7324 0000 0008 010e 0112 0110  ....s$..........
+000008e0: 0110 010c 010c 010c 0104 0102 0102 0104  ................
+000008f0: 0102 fc06 0712 0210 0112 0112 0272 2100  .............r!.
+00000900: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000910: 0000 0006 0000 0040 0000 0073 a200 0000  .......@...s....
+00000920: 6500 5a01 6400 5a02 6503 6a04 6401 6402  e.Z.d.Z.e.j.d.d.
+00000930: 6403 8d02 5a05 6503 6a04 6404 6402 6405  d...Z.e.j.d.d.d.
+00000940: 6405 6406 8d04 5a06 6503 6a04 6407 6402  d.d...Z.e.j.d.d.
+00000950: 6405 6405 6406 8d04 5a07 6503 6a04 6408  d.d.d...Z.e.j.d.
+00000960: 6402 6403 8d02 5a08 6503 6a04 6409 640a  d.d...Z.e.j.d.d.
+00000970: 6405 6405 6406 8d04 5a09 6503 6a0a 640b  d.d.d...Z.e.j.d.
+00000980: 6405 6405 640c 8d03 5a0b 6503 6a0c 650d  d.d.d...Z.e.j.e.
+00000990: 640d 6503 6a0e 640e 8d03 5a0f 6503 6a0c  d.e.j.d...Z.e.j.
+000009a0: 640f 6410 6503 6a0e 6405 6411 8d04 5a10  d.d.e.j.d.d...Z.
+000009b0: 4700 6412 6413 8400 6413 8302 5a11 6414  G.d.d...d...Z.d.
+000009c0: 5300 2915 da06 4f66 6669 6365 7222 0000  S.)...Officer"..
+000009d0: 0072 2300 0000 7224 0000 0075 0c00 0000  .r#...r$...u....
+000009e0: e7a7 91e5 aea4 e4bd 8de7 bdae 5472 2800  ............Tr(.
+000009f0: 0000 7226 0000 00f5 0c00 0000 e7a7 91e5  ..r&............
+00000a00: aea4 e7bc 96e7 a081 7506 0000 00e7 b1bb  ........u.......
+00000a10: e59e 8b72 2700 0000 750c 0000 00e7 a791  ...r'...u.......
+00000a20: e5ae a4e7 ae80 e4bb 8b72 2a00 0000 722f  .........r*...r/
+00000a30: 0000 00a9 0272 0c00 0000 7231 0000 0072  .....r....r1...r
+00000a40: 2e00 0000 750c 0000 00e4 b88a e7ba a7e7  ....u...........
+00000a50: a791 e5ae a472 3000 0000 6300 0000 0000  .....r0...c.....
+00000a60: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+00000a70: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000a80: 6401 5a03 6402 5a04 6504 5a05 6403 5a06  d.Z.d.Z.e.Z.d.Z.
+00000a90: 6404 5300 2905 7a0b 4f66 6669 6365 2e4d  d.S.).z.Office.M
+00000aa0: 6574 615a 0962 735f 6f66 6669 6365 7506  etaZ.bs_officeu.
+00000ab0: 0000 00e7 a791 e5ae a4a9 0129 0272 3e00  ...........).r>.
+00000ac0: 0000 da08 686f 7370 6974 616c 4ea9 0772  ....hospitalN..r
+00000ad0: 1500 0000 7216 0000 0072 1700 0000 7237  ....r....r....r7
+00000ae0: 0000 0072 0c00 0000 7238 0000 00da 0f75  ...r....r8.....u
+00000af0: 6e69 7175 655f 746f 6765 7468 6572 7219  nique_togetherr.
+00000b00: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00000b10: 0000 721b 0000 004a 0000 0073 0800 0000  ..r....J...s....
+00000b20: 0801 0401 0401 0401 721b 0000 004e 2912  ........r....N).
+00000b30: 7215 0000 0072 1600 0000 7217 0000 0072  r....r....r....r
+00000b40: 0500 0000 7239 0000 0072 3a00 0000 723f  ....r9...r:...r?
+00000b50: 0000 0072 3b00 0000 723e 0000 005a 0b6f  ...r;...r>...Z.o
+00000b60: 6666 6963 655f 7479 7065 723c 0000 0072  ffice_typer<...r
+00000b70: 3d00 0000 7241 0000 0072 2100 0000 7242  =...rA...r!...rB
+00000b80: 0000 0072 4a00 0000 7243 0000 0072 1b00  ...rJ...rC...r..
+00000b90: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00000ba0: 0072 1a00 0000 7246 0000 0037 0000 0073  .r....rF...7...s
+00000bb0: 2400 0000 0801 0e01 1201 1201 0e01 1201  $...............
+00000bc0: 1001 0401 0201 0201 04fd 0605 0401 0201  ................
+00000bd0: 0201 0401 02fc 0607 7246 0000 0063 0000  ........rF...c..
+00000be0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00000bf0: 0000 4000 0000 736c 0000 0065 005a 0164  ..@...sl...e.Z.d
+00000c00: 005a 0265 036a 0464 0164 0264 038d 025a  .Z.e.j.d.d.d...Z
+00000c10: 0565 036a 0464 0464 0264 038d 025a 0665  .e.j.d.d.d...Z.e
+00000c20: 036a 0765 0864 0565 036a 0964 068d 035a  .j.e.d.e.j.d...Z
+00000c30: 0a65 036a 0464 0764 0864 0964 0964 0a8d  .e.j.d.d.d.d.d..
+00000c40: 045a 0b65 036a 0464 0b64 0864 0964 0964  .Z.e.j.d.d.d.d.d
+00000c50: 0a8d 045a 0c47 0064 0c64 0d84 0064 0d83  ...Z.G.d.d...d..
+00000c60: 025a 0d64 0e53 0029 0fda 0d50 6f73 6974  .Z.d.S.)...Posit
+00000c70: 696f 6e54 6974 6c65 7222 0000 0072 2300  ionTitler"...r#.
+00000c80: 0000 7224 0000 0075 0c00 0000 e881 8ce7  ..r$...u........
+00000c90: a7b0 e7bc 96e7 a081 722f 0000 0072 4800  ........r/...rH.
+00000ca0: 0000 7234 0000 0072 2700 0000 5472 2800  ..r4...r'...Tr(.
+00000cb0: 0000 7235 0000 0063 0000 0000 0000 0000  ..r5...c........
+00000cc0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00000cd0: 731c 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00000ce0: 0364 025a 0465 045a 0564 035a 0664 0453  .d.Z.e.Z.d.Z.d.S
+00000cf0: 0029 057a 1250 6f73 6974 696f 6e54 6974  .).z.PositionTit
+00000d00: 6c65 2e4d 6574 615a 1162 735f 706f 7369  le.MetaZ.bs_posi
+00000d10: 7469 6f6e 5f74 6974 6c65 f506 0000 00e8  tion_title......
+00000d20: 818c e7a7 b072 4900 0000 4e72 4b00 0000  .....rI...NrK...
+00000d30: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000d40: 1a00 0000 721b 0000 005e 0000 0073 0800  ....r....^...s..
+00000d50: 0000 0801 0401 0401 0401 721b 0000 004e  ..........r....N
+00000d60: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
+00000d70: 0072 0500 0000 7239 0000 0072 3a00 0000  .r....r9...r:...
+00000d80: 723e 0000 0072 4100 0000 7221 0000 0072  r>...rA...r!...r
+00000d90: 4200 0000 724a 0000 0072 4400 0000 7245  B...rJ...rD...rE
+00000da0: 0000 0072 1b00 0000 7219 0000 0072 1900  ...r....r....r..
+00000db0: 0000 7219 0000 0072 1a00 0000 724d 0000  ..r....r....rM..
+00000dc0: 0053 0000 0073 1400 0000 0801 0e01 0e01  .S...s..........
+00000dd0: 0401 0201 0201 04fd 0605 1201 1202 724d  ..............rM
+00000de0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000df0: 0000 0000 0700 0000 4000 0000 734e 0100  ........@...sN..
+00000e00: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00000e10: 0264 038d 025a 0565 036a 0464 0464 0264  .d...Z.e.j.d.d.d
+00000e20: 0564 0564 068d 045a 0665 036a 0464 0764  .d.d...Z.e.j.d.d
+00000e30: 0864 0564 0564 068d 045a 0765 036a 0464  .d.d.d...Z.e.j.d
+00000e40: 0964 0a64 0564 0564 068d 045a 0865 036a  .d.d.d.d...Z.e.j
+00000e50: 0464 0b64 0c64 038d 025a 0965 036a 0464  .d.d.d...Z.e.j.d
+00000e60: 0d64 0264 0564 0564 068d 045a 0a65 036a  .d.d.d.d...Z.e.j
+00000e70: 0b65 0c64 0e65 036a 0d64 0f8d 035a 0e65  .e.d.e.j.d...Z.e
+00000e80: 036a 0464 1064 1165 0f64 0564 0564 128d  .j.d.d.e.d.d.d..
+00000e90: 055a 1065 036a 0464 1364 1464 0564 0564  .Z.e.j.d.d.d.d.d
+00000ea0: 068d 045a 1165 036a 0464 1564 0864 0564  ...Z.e.j.d.d.d.d
+00000eb0: 0564 068d 045a 1265 036a 0b65 1364 1665  .d...Z.e.j.e.d.e
+00000ec0: 036a 0d64 0f8d 035a 1465 036a 0b65 1564  .j.d...Z.e.j.e.d
+00000ed0: 1765 036a 0d64 0f8d 035a 1665 036a 1764  .e.j.d...Z.e.j.d
+00000ee0: 1864 0564 0564 198d 035a 1865 036a 0464  .d.d.d...Z.e.j.d
+00000ef0: 1a64 1b64 1c64 1d8d 035a 1965 036a 1a64  .d.d.d...Z.e.j.d
+00000f00: 1e64 0564 0564 198d 035a 1b65 036a 0464  .d.d.d...Z.e.j.d
+00000f10: 1f64 0264 0564 0564 068d 045a 1c65 036a  .d.d.d.d...Z.e.j
+00000f20: 0464 2064 0264 0564 0564 068d 045a 1d65  .d d.d.d.d...Z.e
+00000f30: 036a 1e64 2164 0564 228d 025a 1f47 0064  .j.d!d.d"..Z.G.d
+00000f40: 2364 2484 0064 2483 025a 2064 2553 0029  #d$..d$..Z d%S.)
+00000f50: 26da 0644 6f63 746f 7272 2200 0000 e914  &..Doctorr".....
+00000f60: 0000 0072 2400 0000 7226 0000 0054 7228  ...r$...r&...Tr(
+00000f70: 0000 0075 0600 0000 e982 aee7 aeb1 7227  ...u..........r'
+00000f80: 0000 0075 0600 0000 e59c b0e5 9d80 7223  ...u..........r#
+00000f90: 0000 0075 0600 0000 e5b7 a5e5 8fb7 e940  ...u...........@
+00000fa0: 0000 0075 0600 0000 e881 8ce4 bd8d 724e  ...u..........rN
+00000fb0: 0000 0072 4800 0000 f506 0000 00e6 80a7  ...rH...........
+00000fc0: e588 abe9 0200 0000 a905 720c 0000 0072  ..........r....r
+00000fd0: 2500 0000 da07 6368 6f69 6365 7372 0e00  %.....choicesr..
+00000fe0: 0000 7229 0000 0075 0600 0000 e6b0 91e6  ..r)...u........
+00000ff0: 978f e90a 0000 00f5 0c00 0000 e8ba abe4  ................
+00001000: bbbd e8af 81e5 8fb7 f50c 0000 00e6 8980  ................
+00001010: e5b1 9ee7 a791 e5ae a472 2f00 0000 f50c  .........r/.....
+00001020: 0000 00e5 87ba e794 9fe6 97a5 e69c 9f72  ...............r
+00001030: 2a00 0000 750c 0000 00e5 8cbb e794 9fe7  *...u...........
+00001040: 85a7 e789 87e9 3200 0000 5a0c 646f 6374  ......2...Z.doct
+00001050: 6f72 5f70 686f 746f 7233 0000 0075 0c00  or_photor3...u..
+00001060: 0000 e58c bbe7 949f e68f 8fe8 bfb0 7234  ..............r4
+00001070: 0000 0072 3500 0000 7515 0000 00e6 98af  ...r5...u.......
+00001080: e590 a6e4 ba92 e881 94e7 bd91 e68e a5e8  ................
+00001090: af8a 7213 0000 0063 0000 0000 0000 0000  ..r....c........
+000010a0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+000010b0: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+000010c0: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
+000010d0: 0b44 6f63 746f 722e 4d65 7461 5a09 6273  .Doctor.MetaZ.bs
+000010e0: 5f64 6f63 746f 7275 0900 0000 e58c bbe7  _doctoru........
+000010f0: 949f e8a1 a84e 7236 0000 0072 1900 0000  .....Nr6...r....
+00001100: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00001110: 1b00 0000 8900 0000 7306 0000 0008 0104  ........s.......
+00001120: 0104 0172 1b00 0000 4e29 2172 1500 0000  ...r....N)!r....
+00001130: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
+00001140: 3900 0000 723a 0000 0072 3b00 0000 da05  9...r:...r;.....
+00001150: 656d 6169 6c72 3f00 0000 723e 0000 00da  emailr?...r>....
+00001160: 0870 6f73 6974 696f 6e72 4100 0000 724d  .positionrA...rM
+00001170: 0000 0072 4200 0000 5a0e 706f 7369 7469  ...rB...Z.positi
+00001180: 6f6e 5f74 6974 6c65 da0d 4745 4e44 4552  on_title..GENDER
+00001190: 5f43 484f 4943 45da 0667 656e 6465 725a  _CHOICE..genderZ
+000011a0: 066e 6174 696f 6e5a 0569 646e 756d 7246  .nationZ.idnumrF
+000011b0: 0000 00da 066f 6666 6963 6572 2100 0000  .....officer!...
+000011c0: 724a 0000 00da 0944 6174 6546 6965 6c64  rJ.....DateField
+000011d0: da08 6269 7274 6864 6179 5a05 7068 6f74  ..birthdayZ.phot
+000011e0: 6f72 3c00 0000 da08 6465 7363 7269 6265  or<.....describe
+000011f0: 7244 0000 0072 4500 0000 721f 0000 005a  rD...rE...r....Z
+00001200: 1169 735f 6f6e 6c69 6e65 5f63 6f6e 7375  .is_online_consu
+00001210: 6c74 721b 0000 0072 1900 0000 7219 0000  ltr....r....r...
+00001220: 0072 1900 0000 721a 0000 0072 4f00 0000  .r....r....rO...
+00001230: 6700 0000 733e 0000 0008 010e 0112 0112  g...s>..........
+00001240: 0112 010e 0112 0104 0102 0102 0104 fd06  ................
+00001250: 0514 0112 0112 0104 0102 0102 0104 fd06  ................
+00001260: 0504 0102 0102 0104 fd06 0510 0210 0110  ................
+00001270: 0112 0112 020e 0272 4f00 0000 6300 0000  .......rO...c...
+00001280: 0000 0000 0000 0000 0000 0000 0007 0000  ................
+00001290: 0040 0000 0073 6e01 0000 6500 5a01 6400  .@...sn...e.Z.d.
+000012a0: 5a02 6503 6a04 6401 6402 6403 6403 6404  Z.e.j.d.d.d.d.d.
+000012b0: 8d04 5a05 6503 6a04 6405 6406 6403 6403  ..Z.e.j.d.d.d.d.
+000012c0: 6404 8d04 5a06 6503 6a07 6407 6403 6403  d...Z.e.j.d.d.d.
+000012d0: 6408 8d03 5a08 6503 6a04 6409 640a 6509  d...Z.e.j.d.d.e.
+000012e0: 6403 6403 640b 8d05 5a0a 6503 6a04 640c  d.d.d...Z.e.j.d.
+000012f0: 6406 6403 6403 6404 8d04 5a0b 6503 6a0c  d.d.d.d...Z.e.j.
+00001300: 640d 640e 6403 6403 640f 8d04 5a0d 6503  d.d.d.d.d...Z.e.
+00001310: 6a0e 650f 6410 6503 6a10 6403 6411 8d04  j.e.d.e.j.d.d...
+00001320: 5a11 6503 6a0e 6512 6412 6503 6a10 6403  Z.e.j.e.d.e.j.d.
+00001330: 6411 8d04 5a13 6503 6a0e 6514 6413 6503  d...Z.e.j.e.d.e.
+00001340: 6a10 6403 6411 8d04 5a15 6503 6a04 6414  j.d.d...Z.e.j.d.
+00001350: 6406 6415 6416 8d03 5a16 6503 6a04 6417  d.d.d...Z.e.j.d.
+00001360: 6402 6403 6403 6404 8d04 5a17 6503 6a04  d.d.d.d...Z.e.j.
+00001370: 6418 6402 6403 6403 6404 8d04 5a18 6503  d.d.d.d.d...Z.e.
+00001380: 6a19 6419 6403 6403 6408 8d03 5a1a 6503  j.d.d.d.d...Z.e.
+00001390: 6a04 641a 6406 6403 6403 6404 8d04 5a1b  j.d.d.d.d.d...Z.
+000013a0: 6503 6a04 641b 6406 6403 6403 6404 8d04  e.j.d.d.d.d.d...
+000013b0: 5a1c 6503 6a1d 641c 6403 6403 641d 8d03  Z.e.j.d.d.d.d...
+000013c0: 5a1e 6503 6a1d 641e 6403 6403 641f 8d03  Z.e.j.d.d.d.d...
+000013d0: 5a1f 4700 6420 6421 8400 6421 8302 5a20  Z.G.d d!..d!..Z 
+000013e0: 6521 6422 6423 8400 8301 5a22 6521 6424  e!d"d#....Z"e!d$
+000013f0: 6425 8400 8301 5a23 6521 6426 6427 8400  d%....Z#e!d&d'..
+00001400: 8301 5a24 6428 5300 2929 da04 5573 6572  ..Z$d(S.))..User
+00001410: 7222 0000 0072 2300 0000 5472 2800 0000  r"...r#...Tr(...
+00001420: 7226 0000 0072 2700 0000 7259 0000 0072  r&...r'...rY...r
+00001430: 2a00 0000 7252 0000 0072 5300 0000 7254  *...rR...rS...rT
+00001440: 0000 0072 5700 0000 f506 0000 00e6 8e92  ...rW...........
+00001450: e5ba 8fe9 0100 0000 a904 720c 0000 0072  ..........r....r
+00001460: 1400 0000 720e 0000 0072 2900 0000 7258  ....r....r)...rX
+00001470: 0000 0072 3000 0000 722f 0000 0075 0c00  ...r0...r/...u..
+00001480: 0000 e7bb 91e5 ae9a e58c bbe7 949f 750c  ..............u.
+00001490: 0000 00e7 94a8 e688 b7e5 a4b4 e583 8f5a  ...............Z
+000014a0: 0b75 7365 725f 6176 6174 6172 7233 0000  .user_avatarr3..
+000014b0: 0075 0c00 0000 e9bb 98e8 aea4 e8a7 92e8  .u..............
+000014c0: 89b2 750f 0000 00e5 8faf e693 8de4 bd9c  ..u.............
+000014d0: e7a7 91e5 aea4 750c 0000 00e6 b3a8 e987  ......u.........
+000014e0: 8ae8 afb4 e698 8e72 3400 0000 7235 0000  .......r4...r5..
+000014f0: 0072 0a00 0000 720b 0000 0072 0f00 0000  .r....r....r....
+00001500: 7210 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00001510: 0000 0000 0000 0100 0000 4000 0000 7310  ..........@...s.
+00001520: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00001530: 0253 0029 037a 0955 7365 722e 4d65 7461  .S.).z.User.Meta
+00001540: 750c 0000 00e7 94a8 e688 b7e4 bfa1 e681  u...............
+00001550: af4e 2904 7215 0000 0072 1600 0000 7217  .N).r....r....r.
+00001560: 0000 0072 0c00 0000 7219 0000 0072 1900  ...r....r....r..
+00001570: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00001580: 00b2 0000 0073 0200 0000 0802 721b 0000  .....s......r...
+00001590: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+000015a0: 0000 0200 0000 4300 0000 7318 0000 007c  ......C...s....|
+000015b0: 006a 007d 017c 0173 147c 006a 01a0 02a1  .j.}.|.s.|.j....
+000015c0: 007d 017c 0153 0029 0175 8e00 0000 0a20  .}.|.S.).u..... 
+000015d0: 2020 2020 2020 20e8 8eb7 e58f 96e5 bd93         .........
+000015e0: e589 8de7 94a8 e688 b7e9 bb98 e8ae a4e7  ................
+000015f0: 94a8 e688 b7e7 bb84 2c0a 2020 2020 2020  ........,.      
+00001600: 2020 e5a6 82e6 9e9c e69c aae8 aebe e7bd    ..............
+00001610: aeef bc8c e8bf 94e5 9b9e e7ac ace4 b880  ................
+00001620: e4b8 aae7 94a8 e688 b7e7 bb84 0a20 2020  .............   
+00001630: 2020 2020 20e5 90a6 e588 99e8 bf94 e59b       ...........
+00001640: 9ee8 aebe e7bd aee7 9a84 e794 a8e6 88b7  ................
+00001650: e7bb 840a 2020 2020 2020 2020 2903 5a0d  ....        ).Z.
+00001660: 6465 6661 756c 745f 6772 6f75 70da 0667  default_group..g
+00001670: 726f 7570 73da 0566 6972 7374 a902 722e  roups..first..r.
+00001680: 0000 005a 0972 6574 5f67 726f 7570 7219  ...Z.ret_groupr.
+00001690: 0000 0072 1900 0000 721a 0000 00da 1167  ...r....r......g
+000016a0: 6574 5f64 6566 6175 6c74 5f67 726f 7570  et_default_group
+000016b0: ba00 0000 7308 0000 0000 0706 0104 010a  ....s...........
+000016c0: 017a 1655 7365 722e 6765 745f 6465 6661  .z.User.get_defa
+000016d0: 756c 745f 6772 6f75 7063 0100 0000 0000  ult_groupc......
+000016e0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000016f0: 0000 731c 0000 007c 006a 00a0 01a1 007d  ..s....|.j.....}
+00001700: 017c 0173 187c 006a 00a0 02a1 007d 017c  .|.s.|.j.....}.|
+00001710: 0153 00a9 014e 2903 7267 0000 00da 0361  .S...N).rg.....a
+00001720: 6c6c da04 6e6f 6e65 7269 0000 0072 1900  ll..noneri...r..
+00001730: 0000 7219 0000 0072 1a00 0000 da0d 6765  ..r....r......ge
+00001740: 745f 616c 6c67 726f 7570 73c6 0000 0073  t_allgroups....s
+00001750: 0800 0000 0002 0a01 0401 0a01 7a12 5573  ............z.Us
+00001760: 6572 2e67 6574 5f61 6c6c 6772 6f75 7073  er.get_allgroups
+00001770: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001780: 0001 0000 0043 0000 0073 1800 0000 6401  .....C...s....d.
+00001790: 7d01 7c00 6a00 7d01 7c01 7314 7c00 6a01  }.|.j.}.|.s.|.j.
+000017a0: 7d01 7c01 5300 2902 7533 0000 000a 2020  }.|.S.).u3....  
+000017b0: 2020 2020 2020 e88e b7e5 8f96 e794 a8e6        ..........
+000017c0: 88b7 e9bb 98e8 aea4 e79a 84e7 bb84 e7bb  ................
+000017d0: 87e6 9cba e69e 840a 2020 2020 2020 2020  ........        
+000017e0: 4e29 0272 5f00 0000 724a 0000 0029 0272  N).r_...rJ...).r
+000017f0: 2e00 0000 5a07 7265 745f 6f72 6772 1900  ....Z.ret_orgr..
+00001800: 0000 7219 0000 0072 1a00 0000 da18 6765  ..r....r......ge
+00001810: 745f 6465 6661 756c 745f 6f72 6761 6e69  t_default_organi
+00001820: 7a61 7469 6f6e cd00 0000 730a 0000 0000  zation....s.....
+00001830: 0504 0106 0104 0106 017a 1d55 7365 722e  .........z.User.
+00001840: 6765 745f 6465 6661 756c 745f 6f72 6761  get_default_orga
+00001850: 6e69 7a61 7469 6f6e 4e29 2572 1500 0000  nizationN)%r....
+00001860: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
+00001870: 3900 0000 723a 0000 0072 3b00 0000 7260  9...r:...r;...r`
+00001880: 0000 0072 6100 0000 725d 0000 0072 5e00  ...ra...r]...r^.
+00001890: 0000 5a09 6964 6361 7264 6e75 6dda 0c49  ..Z.idcardnum..I
+000018a0: 6e74 6567 6572 4669 656c 64da 086f 7264  ntegerField..ord
+000018b0: 6572 5f62 7972 4100 0000 7246 0000 0072  er_byrA...rF...r
+000018c0: 4200 0000 725f 0000 0072 2100 0000 724a  B...r_...r!...rJ
+000018d0: 0000 0072 4f00 0000 5a06 646f 6374 6f72  ...rO...Z.doctor
+000018e0: 5a0a 6176 6174 6172 5f75 726c 5a10 6465  Z.avatar_urlZ.de
+000018f0: 6661 756c 745f 6772 6f75 705f 6964 5a0c  fault_group_idZ.
+00001900: 616c 6c6f 775f 6f66 6669 6365 723c 0000  allow_officer<..
+00001910: 00da 046e 6f74 6572 4400 0000 7245 0000  ...noterD...rE..
+00001920: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00001930: 721b 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00001940: 6a00 0000 726e 0000 0072 6f00 0000 7219  j...rn...ro...r.
+00001950: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00001960: 0000 7263 0000 008f 0000 0073 4e00 0000  ..rc.......sN...
+00001970: 0801 1201 1201 1001 1401 1201 1201 0401  ................
+00001980: 0201 0201 0401 02fc 0606 0401 0201 0201  ................
+00001990: 0401 02fc 0606 0401 0201 0201 0401 02fc  ................
+000019a0: 0607 1001 1201 1201 1001 1201 1201 1001  ................
+000019b0: 1002 0e08 0201 0a0b 0201 0a06 0201 7263  ..............rc
+000019c0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000019d0: 0000 0000 0700 0000 4000 0000 73ce 0000  ........@...s...
+000019e0: 0065 005a 0164 005a 0264 015a 0365 046a  .e.Z.d.Z.d.Z.e.j
+000019f0: 0565 0665 046a 0764 0264 0364 0364 048d  .e.e.j.d.d.d.d..
+00001a00: 055a 0865 046a 0964 0564 0664 0364 078d  .Z.e.j.d.d.d.d..
+00001a10: 035a 0a65 046a 0964 0564 0864 0364 098d  .Z.e.j.d.d.d.d..
+00001a20: 035a 0b65 046a 0c64 0364 0a64 0364 0b8d  .Z.e.j.d.d.d.d..
+00001a30: 035a 0d65 046a 0964 0c64 0564 0364 0364  .Z.e.j.d.d.d.d.d
+00001a40: 0d8d 045a 0e65 046a 0f65 1064 0e65 046a  ...Z.e.j.e.d.e.j
+00001a50: 0764 0f64 0364 108d 055a 1165 046a 1264  .d.d.d...Z.e.j.d
+00001a60: 1164 1264 0364 138d 035a 1365 046a 0964  .d.d.d...Z.e.j.d
+00001a70: 0564 1464 0364 0364 158d 045a 1465 046a  .d.d.d.d...Z.e.j
+00001a80: 1564 1664 0364 0364 178d 035a 1665 046a  .d.d.d.d...Z.e.j
+00001a90: 1564 1864 0364 0364 198d 035a 1747 0064  .d.d.d.d...Z.G.d
+00001aa0: 1a64 1b84 0064 1b83 025a 1864 1c53 0029  .d...d...Z.d.S.)
+00001ab0: 1dda 0a45 7874 7261 4772 6f75 7075 1900  ...ExtraGroupu..
+00001ac0: 0000 0a20 2020 20e8 a792 e889 b2e6 89a9  ...    .........
+00001ad0: e585 85e8 a1a8 0a20 2020 20da 0b65 7874  .......    ..ext
+00001ae0: 7261 5f67 726f 7570 5429 0472 3100 0000  ra_groupT).r1...
+00001af0: da0c 7265 6c61 7465 645f 6e61 6d65 720e  ..related_namer.
+00001b00: 0000 0072 2900 0000 725a 0000 0075 0c00  ...r)...rZ...u..
+00001b10: 0000 e8a7 92e8 89b2 e4bb a3e7 a081 722c  ..............r,
+00001b20: 0000 0075 0c00 0000 e8a7 92e8 89b2 e590  ...u............
+00001b30: 8de7 a7b0 2903 7225 0000 0072 0c00 0000  ....).r%...r....
+00001b40: 7229 0000 0072 1200 0000 2903 7214 0000  r)...r....).r...
+00001b50: 0072 0c00 0000 720e 0000 0075 0600 0000  .r....r....u....
+00001b60: e68f 8fe8 bfb0 2903 7225 0000 0072 0e00  ......).r%...r..
+00001b70: 0000 7229 0000 0072 2f00 0000 7267 0000  ..r)...r/...rg..
+00001b80: 00a9 0472 0c00 0000 7231 0000 0072 7600  ...r....r1...rv.
+00001b90: 0000 720e 0000 0072 6400 0000 7265 0000  ..r....rd...re..
+00001ba0: 00a9 0372 0c00 0000 7214 0000 0072 0e00  ...r....r....r..
+00001bb0: 0000 7234 0000 00a9 0472 2500 0000 720c  ..r4.....r%...r.
+00001bc0: 0000 0072 0e00 0000 7229 0000 0072 0a00  ...r....r)...r..
+00001bd0: 0000 720b 0000 0075 1200 0000 e69c 80e5  ..r....u........
+00001be0: 908e e69b b4e6 96b0 e697 b6e9 97b4 7210  ..............r.
+00001bf0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001c00: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
+00001c10: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00001c20: 0465 045a 0564 0353 0029 047a 0f45 7874  .e.Z.d.S.).z.Ext
+00001c30: 7261 4772 6f75 702e 4d65 7461 5a0e 6273  raGroup.MetaZ.bs
+00001c40: 5f65 7874 7261 5f67 726f 7570 7506 0000  _extra_groupu...
+00001c50: 00e8 a792 e889 b24e 7236 0000 0072 1900  .......Nr6...r..
+00001c60: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00001c70: 0072 1b00 0000 ee00 0000 7306 0000 0008  .r........s.....
+00001c80: 0104 0104 0172 1b00 0000 4e29 1972 1500  .....r....N).r..
+00001c90: 0000 7216 0000 0072 1700 0000 da07 5f5f  ..r....r......__
+00001ca0: 646f 635f 5f72 0500 0000 da0d 4f6e 6554  doc__r......OneT
+00001cb0: 6f4f 6e65 4669 656c 6472 0300 0000 7242  oOneFieldr....rB
+00001cc0: 0000 00da 0567 726f 7570 7239 0000 005a  .....groupr9...Z
+00001cd0: 0972 6f6c 655f 636f 6465 5a09 726f 6c65  .role_codeZ.role
+00001ce0: 5f6e 616d 6572 1f00 0000 7220 0000 0072  _namer....r ...r
+00001cf0: 7200 0000 7241 0000 0072 2100 0000 724a  r...rA...r!...rJ
+00001d00: 0000 0072 7000 0000 7271 0000 005a 0c63  ...rp...rq...Z.c
+00001d10: 7265 6174 6564 5f75 7365 7272 1c00 0000  reated_userr....
+00001d20: 5a0a 6372 6561 7465 645f 6174 5a0a 7570  Z.created_atZ.up
+00001d30: 6461 7465 645f 6174 721b 0000 0072 1900  dated_atr....r..
+00001d40: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+00001d50: 0072 7400 0000 d900 0000 7324 0000 0008  .rt.......s$....
+00001d60: 0104 0316 0110 0110 0110 0112 0104 0102  ................
+00001d70: 0102 0104 0102 0102 fb06 0710 0112 0110  ................
+00001d80: 0110 0272 7400 0000 6300 0000 0000 0000  ...rt...c.......
+00001d90: 0000 0000 0000 0000 0007 0000 0040 0000  .............@..
+00001da0: 0073 8c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001db0: 5a03 6504 6a05 6402 6403 6404 8d02 5a06  Z.e.j.d.d.d...Z.
+00001dc0: 6504 6a07 6405 6406 6407 8d02 5a08 6504  e.j.d.d.d...Z.e.
+00001dd0: 6a09 6408 6409 6406 640a 8d03 5a0a 6504  j.d.d.d.d...Z.e.
+00001de0: 6a09 640b 6409 6406 6406 640c 8d04 5a0b  j.d.d.d.d.d...Z.
+00001df0: 6504 6a05 640d 640e 6406 6406 640f 8d04  e.j.d.d.d.d.d...
+00001e00: 5a0c 6504 6a0d 6410 6411 6504 6a0e 6412  Z.e.j.d.d.e.j.d.
+00001e10: 6406 6413 8d05 5a0f 4700 6414 6415 8400  d.d...Z.G.d.d...
+00001e20: 6415 8302 5a10 6416 6417 8400 5a11 6418  d...Z.d.d...Z.d.
+00001e30: 5300 2919 da10 436f 6e74 656e 7454 7970  S.)...ContentTyp
+00001e40: 6543 6174 6573 7516 0000 000a 2020 2020  eCatesu.....    
+00001e50: e88f 9ce5 8d95 e590 8de7 a7b0 0a20 2020  .............   
+00001e60: 2072 2200 0000 7250 0000 0029 0172 2500   r"...rP...).r%.
+00001e70: 0000 7212 0000 0054 2901 7214 0000 0072  ..r....T).r....r
+00001e80: 6400 0000 7265 0000 0072 7800 0000 7506  d...re...rx...u.
+00001e90: 0000 00e7 baa7 e588 ab72 6600 0000 f506  .........rf.....
+00001ea0: 0000 00e5 9bbe e6a0 87e9 f401 0000 7228  ..............r(
+00001eb0: 0000 0072 2e00 0000 750c 0000 00e7 88b6  ...r....u.......
+00001ec0: e7ba a7e8 8f9c e58d 95da 0863 6869 6c64  ...........child
+00001ed0: 7265 6e72 7700 0000 6300 0000 0000 0000  renrw...c.......
+00001ee0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+00001ef0: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00001f00: 5a03 6402 5a04 6504 5a05 6403 5a06 6404  Z.d.Z.e.Z.d.Z.d.
+00001f10: 5300 2905 7a15 436f 6e74 656e 7454 7970  S.).z.ContentTyp
+00001f20: 6543 6174 6573 2e4d 6574 615a 1462 735f  eCates.MetaZ.bs_
+00001f30: 636f 6e74 656e 745f 7479 7065 5f63 6174  content_type_cat
+00001f40: 7375 0c00 0000 e88f 9ce5 8d95 e590 8de7  su..............
+00001f50: a7b0 a901 7271 0000 004e a907 7215 0000  ....rq...N..r...
+00001f60: 0072 1600 0000 7217 0000 0072 3700 0000  .r....r....r7...
+00001f70: 720c 0000 0072 3800 0000 da08 6f72 6465  r....r8.....orde
+00001f80: 7269 6e67 7219 0000 0072 1900 0000 7219  ringr....r....r.
+00001f90: 0000 0072 1a00 0000 721b 0000 0005 0100  ...r....r.......
+00001fa0: 0073 0800 0000 0801 0401 0401 0401 721b  .s............r.
+00001fb0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001fc0: 0100 0000 0100 0000 4300 0000 7306 0000  ........C...s...
+00001fd0: 007c 006a 0053 0072 6b00 0000 a901 723a  .|.j.S.rk.....r:
+00001fe0: 0000 00a9 0172 2e00 0000 7219 0000 0072  .....r....r....r
+00001ff0: 1900 0000 721a 0000 00da 075f 5f73 7472  ....r......__str
+00002000: 5f5f 0b01 0000 7302 0000 0000 017a 1843  __....s......z.C
+00002010: 6f6e 7465 6e74 5479 7065 4361 7465 732e  ontentTypeCates.
+00002020: 5f5f 7374 725f 5f4e 2912 7215 0000 0072  __str__N).r....r
+00002030: 1600 0000 7217 0000 0072 7a00 0000 7205  ....r....rz...r.
+00002040: 0000 0072 3900 0000 723a 0000 0072 1f00  ...r9...r:...r..
+00002050: 0000 7220 0000 0072 7000 0000 7271 0000  ..r ...rp...rq..
+00002060: 00da 056c 6576 656c da0a 6963 6f6e 5f63  ...level..icon_c
+00002070: 6c61 7373 7241 0000 0072 4200 0000 7243  lassrA...rB...rC
+00002080: 0000 0072 1b00 0000 7286 0000 0072 1900  ...r....r....r..
+00002090: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
+000020a0: 0072 7d00 0000 f400 0000 731e 0000 0008  .r}.......s.....
+000020b0: 0104 030e 010e 0110 0112 0112 0104 0102  ................
+000020c0: 0102 0104 0102 0102 fb06 080e 0672 7d00  .............r}.
+000020d0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000020e0: 0000 0006 0000 0040 0000 0073 ce00 0000  .......@...s....
+000020f0: 6500 5a01 6400 5a02 6401 5a03 6504 6a05  e.Z.d.Z.d.Z.e.j.
+00002100: 6402 6403 6404 6405 8d03 5a06 6504 6a07  d.d.d.d...Z.e.j.
+00002110: 6508 6406 6504 6a09 6407 6408 8d04 5a0a  e.d.e.j.d.d...Z.
+00002120: 6504 6a07 6409 640a 6504 6a09 640b 6408  e.j.d.d.e.j.d.d.
+00002130: 8d04 5a0b 6504 6a05 640c 640d 6404 6404  ..Z.e.j.d.d.d.d.
+00002140: 640e 8d04 5a0c 6504 6a0d 640f 6404 6404  d...Z.e.j.d.d.d.
+00002150: 6410 8d03 5a0e 6504 6a0d 6411 6404 6404  d...Z.e.j.d.d.d.
+00002160: 6410 8d03 5a0f 6504 6a05 6412 6413 6404  d...Z.e.j.d.d.d.
+00002170: 6414 8d03 5a10 6504 6a11 6415 6404 6416  d...Z.e.j.d.d.d.
+00002180: 8d02 5a12 6504 6a13 6417 6404 6404 6418  ..Z.e.j.d.d.d.d.
+00002190: 8d03 5a14 6504 6a15 6419 641a 6404 641b  ..Z.e.j.d.d.d.d.
+000021a0: 8d03 5a16 4700 641c 641d 8400 641d 8302  ..Z.G.d.d...d...
+000021b0: 5a17 641e 641f 8400 5a18 6420 5300 2921  Z.d.d...Z.d S.)!
+000021c0: da0d 436f 6e74 656e 7454 7970 6545 7875  ..ContentTypeExu
+000021d0: 1600 0000 0a20 2020 20e5 8a9f e883 bde7  .....    .......
+000021e0: b1bb e588 ab0a 2020 2020 7222 0000 0072  ......    r"...r
+000021f0: 5000 0000 5429 0272 2500 0000 720e 0000  P...T).r%...r...
+00002200: 0075 0c00 0000 e7b3 bbe7 bb9f e5ba 94e7  .u..............
+00002210: 94a8 da09 6578 7465 6e73 696f 6e29 0372  ....extension).r
+00002220: 0c00 0000 7231 0000 0072 7600 0000 727d  ....r1...rv...r}
+00002230: 0000 0075 0600 0000 e88f 9ce5 8d95 5a0d  ...u..........Z.
+00002240: 636f 6e74 656e 745f 6361 7465 7372 7e00  content_catesr~.
+00002250: 0000 727f 0000 0072 2800 0000 da03 7572  ..r....r(.....ur
+00002260: 6c72 2a00 0000 7506 0000 00e7 bb84 e688  lr*...u.........
+00002270: 9075 0600 0000 e58f 82e6 95b0 725a 0000  .u..........rZ..
+00002280: 00a9 0372 0c00 0000 7225 0000 0072 0e00  ...r....r%...r..
+00002290: 0000 7509 0000 00e9 878d e5ae 9ae5 9091  ..u.............
+000022a0: a902 720c 0000 0072 0e00 0000 7212 0000  ..r....r....r...
+000022b0: 0029 0272 1400 0000 720e 0000 0072 6400  .).r....r....rd.
+000022c0: 0000 7265 0000 0072 7800 0000 6300 0000  ..re...rx...c...
+000022d0: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+000022e0: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000022f0: 5a02 6401 5a03 6402 5a04 6504 5a05 6403  Z.d.Z.d.Z.e.Z.d.
+00002300: 5a06 6404 5300 2905 7a12 436f 6e74 656e  Z.d.S.).z.Conten
+00002310: 7454 7970 6545 782e 4d65 7461 5a12 6273  tTypeEx.MetaZ.bs
+00002320: 5f63 6f6e 7465 6e74 5f74 7970 655f 6578  _content_type_ex
+00002330: 7512 0000 00e5 8a9f e883 bde7 b1bb e588  u...............
+00002340: abe8 a1a5 e585 8572 8100 0000 4e72 8200  .......r....Nr..
+00002350: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00002360: 0072 1a00 0000 721b 0000 0028 0100 0073  .r....r....(...s
+00002370: 0800 0000 0801 0401 0401 0401 721b 0000  ............r...
+00002380: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00002390: 0000 0100 0000 4300 0000 7306 0000 007c  ......C...s....|
+000023a0: 006a 0053 0072 6b00 0000 7284 0000 0072  .j.S.rk...r....r
+000023b0: 8500 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+000023c0: 0000 0072 8600 0000 2e01 0000 7302 0000  ...r........s...
+000023d0: 0000 017a 1543 6f6e 7465 6e74 5479 7065  ...z.ContentType
+000023e0: 4578 2e5f 5f73 7472 5f5f 4e29 1972 1500  Ex.__str__N).r..
+000023f0: 0000 7216 0000 0072 1700 0000 727a 0000  ..r....r....rz..
+00002400: 0072 0500 0000 7239 0000 0072 3a00 0000  .r....r9...r:...
+00002410: 7241 0000 0072 0400 0000 7242 0000 00da  rA...r....rB....
+00002420: 0c63 6f6e 7465 6e74 5f74 7970 655a 1063  .content_typeZ.c
+00002430: 6f6e 7465 6e74 5f74 7970 655f 6361 7472  ontent_type_catr
+00002440: 8800 0000 723c 0000 00da 0966 726f 6e74  ....r<.....front
+00002450: 5f75 726c 5a0f 6672 6f6e 745f 636f 6d70  _urlZ.front_comp
+00002460: 6f6e 656e 745a 0c66 726f 6e74 5f70 6172  onentZ.front_par
+00002470: 616d 73da 0855 524c 4669 656c 645a 1266  ams..URLFieldZ.f
+00002480: 726f 6e74 5f72 6564 6972 6563 745f 7572  ront_redirect_ur
+00002490: 6c72 1f00 0000 7220 0000 0072 7000 0000  lr....r ...rp...
+000024a0: 7271 0000 0072 1b00 0000 7286 0000 0072  rq...r....r....r
+000024b0: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+000024c0: 0000 0072 8900 0000 0f01 0000 732e 0000  ...r........s...
+000024d0: 0008 0104 0310 0104 0102 0102 0104 0102  ................
+000024e0: fc06 0604 0102 0102 0104 0102 fc06 0612  ................
+000024f0: 0110 0110 0110 010e 0110 0110 020e 0672  ...............r
+00002500: 8900 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00002510: 0000 0000 0004 0000 0040 0000 0073 3a00  .........@...s:.
+00002520: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00002530: 6a05 6402 6403 6404 8d02 5a06 6504 6a05  j.d.d.d...Z.e.j.
+00002540: 6405 6403 6404 8d02 5a07 4700 6406 6407  d.d.d...Z.G.d.d.
+00002550: 8400 6407 8302 5a08 6408 5300 2909 da0b  ..d...Z.d.S.)...
+00002560: 4578 7065 6e73 6554 7970 6575 1600 0000  ExpenseTypeu....
+00002570: 0a20 2020 20e8 b4b9 e794 a8e7 b1bb e59e  .    ...........
+00002580: 8b0a 2020 2020 7222 0000 0072 5100 0000  ..    r"...rQ...
+00002590: 7224 0000 0072 2b00 0000 6300 0000 0000  r$...r+...c.....
+000025a0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000025b0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000025c0: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
+000025d0: 2904 7a10 4578 7065 6e73 6554 7970 652e  ).z.ExpenseType.
+000025e0: 4d65 7461 5a0f 6273 5f65 7870 656e 7365  MetaZ.bs_expense
+000025f0: 5f74 7970 65f5 0c00 0000 e8b4 b9e7 94a8  _type...........
+00002600: e7b1 bbe5 9e8b 4e72 3600 0000 7219 0000  ......Nr6...r...
+00002610: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00002620: 721b 0000 0039 0100 0073 0600 0000 0801  r....9...s......
+00002630: 0401 0401 721b 0000 004e 2909 7215 0000  ....r....N).r...
+00002640: 0072 1600 0000 7217 0000 0072 7a00 0000  .r....r....rz...
+00002650: 7205 0000 0072 3900 0000 723a 0000 00da  r....r9...r:....
+00002660: 0463 6f64 6572 1b00 0000 7219 0000 0072  .coder....r....r
+00002670: 1900 0000 7219 0000 0072 1a00 0000 7291  ....r....r....r.
+00002680: 0000 0032 0100 0073 0800 0000 0801 0403  ...2...s........
+00002690: 0e01 0e02 7291 0000 0063 0000 0000 0000  ....r....c......
+000026a0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+000026b0: 0000 739c 0000 0065 005a 0164 005a 0265  ..s....e.Z.d.Z.e
+000026c0: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
+000026d0: 036a 0464 0564 0264 068d 025a 0665 036a  .j.d.d.d...Z.e.j
+000026e0: 0464 0764 0864 068d 025a 0765 036a 0864  .d.d.d...Z.e.j.d
+000026f0: 0964 0364 0a8d 025a 0965 036a 0a65 0b64  .d.d...Z.e.j.e.d
+00002700: 0b65 036a 0c64 0364 0c8d 045a 0d65 036a  .e.j.d.d...Z.e.j
+00002710: 0464 0d64 0264 0364 0364 0e8d 045a 0e65  .d.d.d.d.d...Z.e
+00002720: 036a 0464 0f64 0264 0364 0364 0e8d 045a  .j.d.d.d.d.d...Z
+00002730: 0f65 036a 1065 1164 1064 0364 118d 035a  .e.j.e.d.d.d...Z
+00002740: 1247 0064 1264 1384 0064 1383 025a 1364  .G.d.d...d...Z.d
+00002750: 1453 0029 15da 0f45 7870 656e 7365 5374  .S.)...ExpenseSt
+00002760: 616e 6461 7264 7292 0000 0072 2700 0000  andardr....r'...
+00002770: 5472 8c00 0000 750c 0000 00e6 a087 e587  Tr....u.........
+00002780: 86e5 908d e7a7 b072 2400 0000 750c 0000  .......r$...u...
+00002790: 00e6 a087 e587 86e7 bc96 e7a0 8172 2300  .............r#.
+000027a0: 0000 7506 0000 00e8 b4b9 e794 a872 8d00  ..u..........r..
+000027b0: 0000 722f 0000 0072 3000 0000 7234 0000  ..r/...r0...r4..
+000027c0: 0072 2800 0000 7235 0000 0075 1200 0000  .r(...r5...u....
+000027d0: e58c bbe7 949f e8b4 b9e7 94a8 e6a0 87e5  ................
+000027e0: 8786 2902 720c 0000 0072 2900 0000 6300  ..).r....r)...c.
+000027f0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00002800: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
+00002810: 6400 5a02 6401 5a03 6402 5a04 6504 5a05  d.Z.d.Z.d.Z.e.Z.
+00002820: 6403 5a06 6404 5300 2905 7a14 4578 7065  d.Z.d.S.).z.Expe
+00002830: 6e73 6553 7461 6e64 6172 642e 4d65 7461  nseStandard.Meta
+00002840: 5a13 6273 5f65 7870 656e 7365 5f73 7461  Z.bs_expense_sta
+00002850: 6e64 6172 6475 0f00 0000 e8b4 b9e7 94a8  ndardu..........
+00002860: e6a0 87e5 8786 e8a1 a829 0129 02da 0d73  .........).)...s
+00002870: 7461 6e64 6172 645f 636f 6465 724a 0000  tandard_coderJ..
+00002880: 004e 724b 0000 0072 1900 0000 7219 0000  .NrK...r....r...
+00002890: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+000028a0: 4f01 0000 7308 0000 0008 0104 0104 0104  O...s...........
+000028b0: 0172 1b00 0000 4e29 1472 1500 0000 7216  .r....N).r....r.
+000028c0: 0000 0072 1700 0000 7205 0000 0072 3900  ...r....r....r9.
+000028d0: 0000 5a0c 6578 7065 6e73 655f 7479 7065  ..Z.expense_type
+000028e0: 5a0d 7374 616e 6461 7264 5f6e 616d 6572  Z.standard_namer
+000028f0: 9500 0000 7240 0000 005a 0466 6565 7372  ....r@...Z.feesr
+00002900: 4100 0000 7221 0000 0072 4200 0000 724a  A...r!...rB...rJ
+00002910: 0000 0072 4400 0000 7245 0000 00da 0f4d  ...rD...rE.....M
+00002920: 616e 7954 6f4d 616e 7946 6965 6c64 724f  anyToManyFieldrO
+00002930: 0000 005a 0764 6f63 746f 7273 721b 0000  ...Z.doctorsr...
+00002940: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002950: 721a 0000 0072 9400 0000 3f01 0000 731c  r....r....?...s.
+00002960: 0000 0008 0210 010e 010e 010e 0104 0102  ................
+00002970: 0102 0104 0102 fc06 0612 0112 0110 0272  ...............r
+00002980: 9400 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00002990: 0000 0000 0007 0000 0040 0000 0073 4c00  .........@...sL.
+000029a0: 0000 6500 5a01 6400 5a02 6503 6a04 6401  ..e.Z.d.Z.e.j.d.
+000029b0: 6402 6403 8d02 5a05 6503 6a04 6404 6402  d.d...Z.e.j.d.d.
+000029c0: 6403 8d02 5a06 6503 6a07 6405 6406 6503  d...Z.e.j.d.d.e.
+000029d0: 6a08 6407 6408 6409 8d05 5a09 4700 640a  j.d.d.d...Z.G.d.
+000029e0: 640b 8400 640b 8302 5a0a 640c 5300 290d  d...d...Z.d.S.).
+000029f0: da0e 496e 7370 6563 7469 6f6e 5479 7065  ..InspectionType
+00002a00: f512 0000 00e6 a380 e69f a5e7 b1bb e59e  ................
+00002a10: 8be7 bc96 e7a0 8172 5a00 0000 7224 0000  .......rZ...r$..
+00002a20: 00f5 1200 0000 e6a3 80e6 9fa5 e7b1 bbe5  ................
+00002a30: 9e8b e590 8de7 a7b0 722e 0000 00f5 0600  ........r.......
+00002a40: 0000 e788 b6e7 baa7 7280 0000 0054 7277  ........r....Trw
+00002a50: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002a60: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
+00002a70: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00002a80: 0465 045a 0564 0353 0029 047a 1349 6e73  .e.Z.d.S.).z.Ins
+00002a90: 7065 6374 696f 6e54 7970 652e 4d65 7461  pectionType.Meta
+00002aa0: 5a12 6273 5f69 6e73 7065 6374 696f 6e5f  Z.bs_inspection_
+00002ab0: 7479 7065 7512 0000 00e6 a380 e69f a5e5  typeu...........
+00002ac0: ad97 e585 b8e7 b1bb e59e 8b4e 7236 0000  ...........Nr6..
+00002ad0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002ae0: 721a 0000 0072 1b00 0000 6301 0000 7306  r....r....c...s.
+00002af0: 0000 0008 0104 0104 0172 1b00 0000 4ea9  .........r....N.
+00002b00: 0b72 1500 0000 7216 0000 0072 1700 0000  .r....r....r....
+00002b10: 7205 0000 0072 3900 0000 da0a 636f 6465  r....r9.....code
+00002b20: 5f73 7276 7470 da0a 6e61 6d65 5f73 7276  _srvtp..name_srv
+00002b30: 7470 7241 0000 0072 4200 0000 7243 0000  tprA...rB...rC..
+00002b40: 0072 1b00 0000 7219 0000 0072 1900 0000  .r....r....r....
+00002b50: 7219 0000 0072 1a00 0000 7297 0000 0058  r....r....r....X
+00002b60: 0100 0073 1400 0000 0801 0e01 0e01 0401  ...s............
+00002b70: 0201 0201 0401 0201 02fb 0608 7297 0000  ............r...
+00002b80: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00002b90: 0000 0600 0000 4000 0000 73a6 0000 0065  ......@...s....e
+00002ba0: 005a 0164 005a 0265 036a 0464 0164 0264  .Z.d.Z.e.j.d.d.d
+00002bb0: 0364 048d 035a 0565 036a 0464 0564 0664  .d...Z.e.j.d.d.d
+00002bc0: 078d 025a 0665 036a 0464 0864 0964 078d  ...Z.e.j.d.d.d..
+00002bd0: 025a 0765 036a 0464 0864 0a64 078d 025a  .Z.e.j.d.d.d...Z
+00002be0: 0865 036a 0964 0b64 0364 0c8d 025a 0a65  .e.j.d.d.d...Z.e
+00002bf0: 036a 0464 0864 0d64 0364 0364 0e8d 045a  .j.d.d.d.d.d...Z
+00002c00: 0b65 036a 0464 0864 0f64 0364 0364 0e8d  .e.j.d.d.d.d.d..
+00002c10: 045a 0c65 036a 0464 1064 1164 0364 128d  .Z.e.j.d.d.d.d..
+00002c20: 035a 0d65 036a 0464 1364 1164 0364 128d  .Z.e.j.d.d.d.d..
+00002c30: 035a 0e47 0064 1464 1584 0064 1583 025a  .Z.G.d.d...d...Z
+00002c40: 0f64 1653 0029 17da 1649 6e73 7065 6374  .d.S.)...Inspect
+00002c50: 696f 6e44 6963 7469 6f6e 6172 6965 7372  ionDictionariesr
+00002c60: 2300 0000 f50c 0000 00e9 a1b9 e79b aee7  #...............
+00002c70: bc96 e7a0 8154 722c 0000 0072 5100 0000  .....Tr,...rQ...
+00002c80: f50c 0000 00e9 a1b9 e79b aee5 908d e7a7  ................
+00002c90: b0a9 0272 2500 0000 720c 0000 00e9 8000  ...r%...r.......
+00002ca0: 0000 f50c 0000 00e5 8cbb e999 a2e7 bc96  ................
+00002cb0: e7a0 8172 4700 0000 f50c 0000 00e9 a1b9  ...rG...........
+00002cc0: e79b aee8 b4b9 e794 a872 8d00 0000 f506  .........r......
+00002cd0: 0000 00e5 a487 e6b3 a872 7900 0000 f50c  .........ry.....
+00002ce0: 0000 00e5 8cba e588 86e5 ad97 e6ae b572  ...............r
+00002cf0: 9800 0000 725a 0000 0072 8c00 0000 7299  ....rZ...r....r.
+00002d00: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002d10: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
+00002d20: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00002d30: 0465 045a 0564 0353 0029 047a 1b49 6e73  .e.Z.d.S.).z.Ins
+00002d40: 7065 6374 696f 6e44 6963 7469 6f6e 6172  pectionDictionar
+00002d50: 6965 732e 4d65 7461 5a1a 6273 5f69 6e73  ies.MetaZ.bs_ins
+00002d60: 7065 6374 696f 6e5f 6469 6374 696f 6e61  pection_dictiona
+00002d70: 7269 6573 750c 0000 00e6 a380 e69f a5e5  riesu...........
+00002d80: ad97 e585 b84e 7236 0000 0072 1900 0000  .....Nr6...r....
+00002d90: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00002da0: 1b00 0000 7401 0000 7306 0000 0008 0104  ....t...s.......
+00002db0: 0104 0172 1b00 0000 4ea9 1072 1500 0000  ...r....N..r....
+00002dc0: 7216 0000 0072 1700 0000 7205 0000 0072  r....r....r....r
+00002dd0: 3900 0000 5a0c 7072 6f6a 6563 745f 636f  9...Z.project_co
+00002de0: 6465 5a0c 7072 6f6a 6563 745f 6e61 6d65  deZ.project_name
+00002df0: da0d 686f 7370 6974 616c 5f63 6f64 655a  ..hospital_codeZ
+00002e00: 0b6f 6666 6963 655f 636f 6465 7240 0000  .office_coder@..
+00002e10: 005a 0c70 726f 6a65 6374 5f66 6565 735a  .Z.project_feesZ
+00002e20: 0772 656d 6172 6b73 5a0b 6469 7374 696e  .remarksZ.distin
+00002e30: 6775 6973 6872 9c00 0000 729d 0000 0072  guishr....r....r
+00002e40: 1b00 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
+00002e50: 0000 0072 1a00 0000 729e 0000 0069 0100  ...r....r....i..
+00002e60: 0073 1400 0000 0801 1001 0e01 0e01 0e01  .s..............
+00002e70: 0e01 1201 1201 1001 1002 729e 0000 0063  ..........r....c
+00002e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002e90: 0700 0000 4000 0000 734c 0000 0065 005a  ....@...sL...e.Z
+00002ea0: 0164 005a 0265 036a 0464 0164 0264 038d  .d.Z.e.j.d.d.d..
+00002eb0: 025a 0565 036a 0464 0464 0264 038d 025a  .Z.e.j.d.d.d...Z
+00002ec0: 0665 036a 0764 0564 0665 036a 0864 0764  .e.j.d.d.e.j.d.d
+00002ed0: 0864 098d 055a 0947 0064 0a64 0b84 0064  .d...Z.G.d.d...d
+00002ee0: 0b83 025a 0a64 0c53 0029 0dda 0f45 7861  ...Z.d.S.)...Exa
+00002ef0: 6d69 6e61 7469 6f6e 5479 7065 7298 0000  minationTyper...
+00002f00: 0072 5a00 0000 7224 0000 0072 9900 0000  .rZ...r$...r....
+00002f10: 722e 0000 0072 9a00 0000 7280 0000 0054  r....r....r....T
+00002f20: 7277 0000 0063 0000 0000 0000 0000 0000  rw...c..........
+00002f30: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+00002f40: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00002f50: 025a 0465 045a 0564 0353 0029 047a 1445  .Z.e.Z.d.S.).z.E
+00002f60: 7861 6d69 6e61 7469 6f6e 5479 7065 2e4d  xaminationType.M
+00002f70: 6574 615a 1362 735f 6578 616d 696e 6174  etaZ.bs_examinat
+00002f80: 696f 6e5f 7479 7065 7512 0000 00e6 a380  ion_typeu.......
+00002f90: e9aa 8ce5 ad97 e585 b8e7 b1bb e59e 8b4e  ...............N
+00002fa0: 7236 0000 0072 1900 0000 7219 0000 0072  r6...r....r....r
+00002fb0: 1900 0000 721a 0000 0072 1b00 0000 8501  ....r....r......
+00002fc0: 0000 7306 0000 0008 0104 0104 0172 1b00  ..s..........r..
+00002fd0: 0000 4e72 9b00 0000 7219 0000 0072 1900  ..Nr....r....r..
+00002fe0: 0000 7219 0000 0072 1a00 0000 72a9 0000  ..r....r....r...
+00002ff0: 007a 0100 0073 1400 0000 0801 0e01 0e01  .z...s..........
+00003000: 0401 0201 0201 0401 0201 02fb 0608 72a9  ..............r.
+00003010: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003020: 0000 0000 0600 0000 4000 0000 73a6 0000  ........@...s...
+00003030: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00003040: 0264 0364 048d 035a 0565 036a 0464 0564  .d.d...Z.e.j.d.d
+00003050: 0664 078d 025a 0665 036a 0464 0864 0964  .d...Z.e.j.d.d.d
+00003060: 078d 025a 0765 036a 0464 0864 0a64 078d  ...Z.e.j.d.d.d..
+00003070: 025a 0865 036a 0964 0b64 0364 0c8d 025a  .Z.e.j.d.d.d...Z
+00003080: 0a65 036a 0464 0864 0d64 0364 0364 0e8d  .e.j.d.d.d.d.d..
+00003090: 045a 0b65 036a 0464 0864 0f64 0364 0364  .Z.e.j.d.d.d.d.d
+000030a0: 0e8d 045a 0c65 036a 0464 1064 1164 0364  ...Z.e.j.d.d.d.d
+000030b0: 128d 035a 0d65 036a 0464 1364 1164 0364  ...Z.e.j.d.d.d.d
+000030c0: 128d 035a 0e47 0064 1464 1584 0064 1583  ...Z.G.d.d...d..
+000030d0: 025a 0f64 1653 0029 17da 1745 7861 6d69  .Z.d.S.)...Exami
+000030e0: 6e61 7469 6f6e 4469 6374 696f 6e61 7269  nationDictionari
+000030f0: 6573 7223 0000 0072 9f00 0000 5472 2c00  esr#...r....Tr,.
+00003100: 0000 7251 0000 0072 a000 0000 72a1 0000  ..rQ...r....r...
+00003110: 0072 a200 0000 72a3 0000 0072 4700 0000  .r....r....rG...
+00003120: 72a4 0000 0072 8d00 0000 72a5 0000 0072  r....r....r....r
+00003130: 7900 0000 72a6 0000 0075 1200 0000 e6a3  y...r....u......
+00003140: 80e9 aa8c e7b1 bbe5 9e8b e7bc 96e7 a081  ................
+00003150: 725a 0000 0072 8c00 0000 7512 0000 00e6  rZ...r....u.....
+00003160: a380 e9aa 8ce7 b1bb e59e 8be5 908d e7a7  ................
+00003170: b063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00003180: 0000 0100 0000 4000 0000 7318 0000 0065  ......@...s....e
+00003190: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
+000031a0: 045a 0564 0353 0029 047a 1c45 7861 6d69  .Z.d.S.).z.Exami
+000031b0: 6e61 7469 6f6e 4469 6374 696f 6e61 7269  nationDictionari
+000031c0: 6573 2e4d 6574 615a 1b62 735f 6578 616d  es.MetaZ.bs_exam
+000031d0: 696e 6174 696f 6e5f 6469 6374 696f 6e61  ination_dictiona
+000031e0: 7269 6573 750c 0000 00e6 a380 e9aa 8ce5  riesu...........
+000031f0: ad97 e585 b84e 7236 0000 0072 1900 0000  .....Nr6...r....
+00003200: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00003210: 1b00 0000 9601 0000 7306 0000 0008 0104  ........s.......
+00003220: 0104 0172 1b00 0000 4e72 a700 0000 7219  ...r....Nr....r.
+00003230: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00003240: 0000 72aa 0000 008b 0100 0073 1400 0000  ..r........s....
+00003250: 0801 1001 0e01 0e01 0e01 0e01 1201 1201  ................
+00003260: 1001 1002 72aa 0000 0063 0000 0000 0000  ....r....c......
+00003270: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00003280: 0000 733c 0000 0065 005a 0164 005a 0265  ..s<...e.Z.d.Z.e
+00003290: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
+000032a0: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
+000032b0: 0647 0064 0864 0984 0064 0983 025a 0764  .G.d.d...d...Z.d
+000032c0: 0a53 0029 0bda 1344 7275 6750 7265 7061  .S.)...DrugPrepa
+000032d0: 7261 7469 6f6e 5479 7065 7223 0000 0072  rationTyper#...r
+000032e0: 2b00 0000 5472 2c00 0000 7251 0000 0075  +...Tr,...rQ...u
+000032f0: 0c00 0000 e7b1 bbe5 9e8b e590 8de7 a7b0  ................
+00003300: 7279 0000 0063 0000 0000 0000 0000 0000  ry...c..........
+00003310: 0000 0000 0000 0100 0000 4000 0000 7318  ..........@...s.
+00003320: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00003330: 025a 0465 045a 0564 0353 0029 047a 1844  .Z.e.Z.d.S.).z.D
+00003340: 7275 6750 7265 7061 7261 7469 6f6e 5479  rugPreparationTy
+00003350: 7065 2e4d 6574 615a 1862 735f 6472 7567  pe.MetaZ.bs_drug
+00003360: 5f70 7265 7061 7261 7469 6f6e 5f74 7970  _preparation_typ
+00003370: 6575 1200 0000 e88d afe5 9381 e588 b6e5  eu..............
+00003380: 8982 e7b1 bbe5 9e8b 4e72 3600 0000 7219  ........Nr6...r.
+00003390: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000033a0: 0000 721b 0000 00a0 0100 0073 0600 0000  ..r........s....
+000033b0: 0801 0401 0401 721b 0000 004e 2908 7215  ......r....N).r.
+000033c0: 0000 0072 1600 0000 7217 0000 0072 0500  ...r....r....r..
+000033d0: 0000 7239 0000 0072 3e00 0000 da09 7479  ..r9...r>.....ty
+000033e0: 7065 5f6e 616d 6572 1b00 0000 7219 0000  pe_namer....r...
+000033f0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+00003400: 72ab 0000 009c 0100 0073 0600 0000 0801  r........s......
+00003410: 1001 1202 72ab 0000 0063 0000 0000 0000  ....r....c......
+00003420: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00003430: 0000 733c 0000 0065 005a 0164 005a 0265  ..s<...e.Z.d.Z.e
+00003440: 036a 0464 0164 0264 0364 048d 035a 0565  .j.d.d.d.d...Z.e
+00003450: 036a 0464 0564 0664 0364 0364 078d 045a  .j.d.d.d.d.d...Z
+00003460: 0647 0064 0864 0984 0064 0983 025a 0764  .G.d.d...d...Z.d
+00003470: 0a53 0029 0bda 0844 7275 6754 7970 6572  .S.)...DrugTyper
+00003480: 2b00 0000 7223 0000 0054 a903 720c 0000  +...r#...T..r...
+00003490: 0072 2500 0000 722d 0000 0072 2200 0000  .r%...r-...r"...
+000034a0: 7251 0000 0072 2800 0000 6300 0000 0000  rQ...r(...c.....
+000034b0: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
+000034c0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000034d0: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
+000034e0: 2904 7a0d 4472 7567 5479 7065 2e4d 6574  ).z.DrugType.Met
+000034f0: 615a 0c62 735f 6472 7567 5f74 7970 65f5  aZ.bs_drug_type.
+00003500: 0c00 0000 e88d afe5 9381 e7b1 bbe5 9e8b  ................
+00003510: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
+00003520: 7219 0000 0072 1a00 0000 721b 0000 00aa  r....r....r.....
+00003530: 0100 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
+00003540: 0000 004e a908 7215 0000 0072 1600 0000  ...N..r....r....
+00003550: 7217 0000 0072 0500 0000 7239 0000 0072  r....r....r9...r
+00003560: 9300 0000 723a 0000 0072 1b00 0000 7219  ....r:...r....r.
+00003570: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00003580: 0000 72ad 0000 00a6 0100 0073 0600 0000  ..r........s....
+00003590: 0801 1001 1202 72ad 0000 0063 0000 0000  ......r....c....
+000035a0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+000035b0: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
+000035c0: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+000035d0: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
+000035e0: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
+000035f0: 0764 0a53 0029 0bda 0c44 7275 6743 6174  .d.S.)...DrugCat
+00003600: 6567 6f72 7972 2300 0000 722b 0000 0054  egoryr#...r+...T
+00003610: 722c 0000 0072 5100 0000 750c 0000 00e7  r,...rQ...u.....
+00003620: b1bb e588 abe5 908d e7a7 b072 7900 0000  ...........ry...
+00003630: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00003640: 0001 0000 0040 0000 0073 1800 0000 6500  .....@...s....e.
+00003650: 5a01 6400 5a02 6401 5a03 6402 5a04 6504  Z.d.Z.d.Z.d.Z.e.
+00003660: 5a05 6403 5300 2904 7a11 4472 7567 4361  Z.d.S.).z.DrugCa
+00003670: 7465 676f 7279 2e4d 6574 615a 1062 735f  tegory.MetaZ.bs_
+00003680: 6472 7567 5f63 6174 6567 6f72 7975 0c00  drug_categoryu..
+00003690: 0000 e88d afe5 9381 e7b1 bbe5 88ab 4e72  ..............Nr
+000036a0: 3600 0000 7219 0000 0072 1900 0000 7219  6...r....r....r.
+000036b0: 0000 0072 1a00 0000 721b 0000 00b4 0100  ...r....r.......
+000036c0: 0073 0600 0000 0801 0401 0401 721b 0000  .s..........r...
+000036d0: 004e 2908 7215 0000 0072 1600 0000 7217  .N).r....r....r.
+000036e0: 0000 0072 0500 0000 7239 0000 0072 3e00  ...r....r9...r>.
+000036f0: 0000 5a0d 6361 7465 676f 7279 5f6e 616d  ..Z.category_nam
+00003700: 6572 1b00 0000 7219 0000 0072 1900 0000  er....r....r....
+00003710: 7219 0000 0072 1a00 0000 72b1 0000 00b0  r....r....r.....
+00003720: 0100 0073 0600 0000 0801 1001 1202 72b1  ...s..........r.
+00003730: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00003740: 0000 0000 0600 0000 4000 0000 739e 0100  ........@...s...
+00003750: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
+00003760: 0264 0364 048d 035a 0565 036a 0464 0564  .d.d...Z.e.j.d.d
+00003770: 0664 0364 0364 078d 045a 0665 036a 0464  .d.d.d...Z.e.j.d
+00003780: 0564 0864 0364 0364 078d 045a 0765 036a  .d.d.d.d...Z.e.j
+00003790: 0464 0564 0964 0364 0364 078d 045a 0865  .d.d.d.d.d...Z.e
+000037a0: 036a 0464 0a64 0b64 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
+000037b0: 0965 036a 0a65 0b64 0d65 036a 0c64 0e8d  .e.j.e.d.e.j.d..
+000037c0: 035a 0d65 036a 0a65 0e64 0f65 036a 0c64  .Z.e.j.e.d.e.j.d
+000037d0: 0e8d 035a 0f65 036a 0a65 1064 1065 036a  ...Z.e.j.e.d.e.j
+000037e0: 0c64 0e8d 035a 1165 036a 0464 1164 0b64  .d...Z.e.j.d.d.d
+000037f0: 0364 0364 0c8d 045a 1265 036a 0464 1264  .d.d...Z.e.j.d.d
+00003800: 0b64 0364 0364 0c8d 045a 1365 036a 0464  .d.d.d...Z.e.j.d
+00003810: 1364 0b64 0364 0364 0c8d 045a 1465 036a  .d.d.d.d...Z.e.j
+00003820: 0464 1464 0b64 0364 0364 0c8d 045a 1565  .d.d.d.d.d...Z.e
+00003830: 036a 0464 1564 0b64 0364 0364 0c8d 045a  .j.d.d.d.d.d...Z
+00003840: 1665 036a 0464 1664 0b64 0364 0364 0c8d  .e.j.d.d.d.d.d..
+00003850: 045a 1765 036a 0464 1764 0b64 0364 0364  .Z.e.j.d.d.d.d.d
+00003860: 0c8d 045a 1865 036a 1964 1864 0364 198d  ...Z.e.j.d.d.d..
+00003870: 025a 1a65 036a 0464 1a64 0564 0364 0364  .Z.e.j.d.d.d.d.d
+00003880: 0c8d 045a 1b65 036a 0464 1b64 0564 0364  ...Z.e.j.d.d.d.d
+00003890: 0364 0c8d 045a 1c65 036a 0464 1c64 0564  .d...Z.e.j.d.d.d
+000038a0: 0364 0364 0c8d 045a 1d65 036a 0464 0564  .d.d...Z.e.j.d.d
+000038b0: 1d64 0364 0364 078d 045a 1e65 036a 0464  .d.d.d...Z.e.j.d
+000038c0: 0564 1e64 0364 0364 078d 045a 1f65 036a  .d.d.d.d...Z.e.j
+000038d0: 0464 1f64 0564 0364 208d 035a 2047 0064  .d.d.d.d ..Z G.d
+000038e0: 2164 2284 0064 2283 025a 2164 2353 0029  !d"..d"..Z!d#S.)
+000038f0: 24da 0d44 7275 6744 6972 6563 746f 7279  $..DrugDirectory
+00003900: f50c 0000 00e8 8daf e593 81e7 bc96 e7a0  ................
+00003910: 8172 2300 0000 5472 ae00 0000 7251 0000  .r#...Tr....rQ..
+00003920: 00f5 0c00 0000 e88d afe5 9381 e590 8de7  ................
+00003930: a7b0 7279 0000 00f5 0600 0000 e8a7 84e6  ..ry............
+00003940: a0bc 750c 0000 00e5 9fba e69c ace5 8d95  ..u.............
+00003950: e4bd 8d75 1200 0000 e680 bbe9 878f e58d  ...u............
+00003960: 95e4 bd8d e7bc 96e7 a081 7250 0000 0072  ..........rP...r
+00003970: 2800 0000 f50c 0000 00e5 88b6 e589 82e7  (...............
+00003980: b1bb e59e 8b72 4800 0000 f506 0000 00e7  .....rH.........
+00003990: b1bb e588 ab72 af00 0000 750c 0000 00e5  .....r....u.....
+000039a0: 8d95 e4bd 8de5 8982 e987 8f75 1300 0000  ...........u....
+000039b0: e8ae a1e9 878f 2fe9 9bb6 e594 aee5 8d95  ....../.........
+000039c0: e4bd 8d75 1200 0000 e8ae a1e9 878f e58d  ...u............
+000039d0: 95e4 bd8d e7bc 96e7 a081 f50c 0000 00e5  ................
+000039e0: ba93 e5ad 98e6 95b0 e987 8f75 0c00 0000  ...........u....
+000039f0: e5ba 93e5 ad98 e58d 95e4 bd8d 750c 0000  ............u...
+00003a00: 00e5 8cbb e4bf 9de7 b1bb e588 ab75 0c00  .............u..
+00003a10: 0000 e586 9ce5 9088 e7b1 bbe5 88ab 750f  ..............u.
+00003a20: 0000 00e6 98af e590 a6e6 98af e59f bae8  ................
+00003a30: 8daf 7213 0000 0075 0c00 0000 e9ab 98e5  ..r....u........
+00003a40: 8db1 e7ad 89e7 baa7 7512 0000 00e5 9bbd  ........u.......
+00003a50: e5ae b6e8 b4af e6a0 87e7 bc96 e7a0 8175  ...............u
+00003a60: 1200 0000 e59b bde5 aeb6 e8b4 afe6 a087  ................
+00003a70: e590 8de7 a7b0 f506 0000 00e4 baa7 e59c  ................
+00003a80: b0f5 0c00 0000 e794 9fe4 baa7 e58e 82e5  ................
+00003a90: aeb6 7518 0000 00e5 8d95 e6ac a1e7 94a8  ..u.............
+00003aa0: e987 8fe5 8d95 e4bd 8de7 bc96 e7a0 8172  ...............r
+00003ab0: 8c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00003ac0: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
+00003ad0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00003ae0: 5a04 6504 5a05 6403 5300 2904 7a12 4472  Z.e.Z.d.S.).z.Dr
+00003af0: 7567 4469 7265 6374 6f72 792e 4d65 7461  ugDirectory.Meta
+00003b00: 5a11 6273 5f64 7275 675f 6469 7265 6374  Z.bs_drug_direct
+00003b10: 6f72 7975 0c00 0000 e88d afe5 9381 e79b  oryu............
+00003b20: aee5 bd95 4e72 3600 0000 7219 0000 0072  ....Nr6...r....r
+00003b30: 1900 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
+00003b40: 0000 00de 0100 0073 0600 0000 0801 0401  .......s........
+00003b50: 0401 721b 0000 004e 2922 7215 0000 0072  ..r....N)"r....r
+00003b60: 1600 0000 7217 0000 0072 0500 0000 7239  ....r....r....r9
+00003b70: 0000 00da 0964 7275 675f 636f 6465 da09  .....drug_code..
+00003b80: 6472 7567 5f6e 616d 65da 0973 7461 6e64  drug_name..stand
+00003b90: 6172 6473 5a0a 746f 7461 6c5f 756e 6974  ardsZ.total_unit
+00003ba0: 5a0f 746f 7461 6c5f 756e 6974 5f63 6f64  Z.total_unit_cod
+00003bb0: 6572 4100 0000 72ab 0000 00da 0a44 4f5f  erA...r......DO_
+00003bc0: 4e4f 5448 494e 47da 1070 7265 7061 7261  NOTHING..prepara
+00003bd0: 7469 6f6e 5f74 7970 6572 b100 0000 da08  tion_typer......
+00003be0: 6361 7465 676f 7279 72ad 0000 00da 0964  categoryr......d
+00003bf0: 7275 675f 7479 7065 5a09 756e 6974 5f64  rug_typeZ.unit_d
+00003c00: 6f73 655a 0c6d 6561 7375 7265 5f75 6e69  oseZ.measure_uni
+00003c10: 745a 116d 6561 7375 7265 5f75 6e69 745f  tZ.measure_unit_
+00003c20: 636f 6465 5a0a 7374 6f63 6b5f 6c65 6674  codeZ.stock_left
+00003c30: 5a0a 7374 6f63 6b5f 756e 6974 5a03 6d69  Z.stock_unitZ.mi
+00003c40: 635a 0c72 6363 5f63 6174 6567 6f72 7972  cZ.rcc_categoryr
+00003c50: 1f00 0000 5a0c 6973 5f65 7373 656e 7469  ....Z.is_essenti
+00003c60: 616c 5a08 6872 5f6c 6576 656c 5a07 6762  alZ.hr_levelZ.gb
+00003c70: 5f63 6f64 655a 0767 625f 6e61 6d65 da0c  _codeZ.gb_name..
+00003c80: 6f72 6967 696e 5f70 6c61 6365 da0c 6d61  origin_place..ma
+00003c90: 6e75 6661 6374 7572 6572 5a0d 636f 6465  nufacturerZ.code
+00003ca0: 5f6d 6564 755f 6375 7272 1b00 0000 7219  _medu_curr....r.
 00003cb0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00003cc0: 0000 72c2 0000 00d7 0100 0073 0600 0000  ..r........s....
-00003cd0: 0801 1001 1202 72c2 0000 0063 0000 0000  ......r....c....
-00003ce0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-00003cf0: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
-00003d00: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
-00003d10: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
-00003d20: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
-00003d30: 0764 0a53 0029 0bda 1250 6861 726d 6163  .d.S.)...Pharmac
-00003d40: 7945 6e74 6572 7072 6973 6572 2b00 0000  yEnterpriser+...
-00003d50: 7223 0000 0054 72ab 0000 0072 2200 0000  r#...Tr....r"...
-00003d60: 7251 0000 0072 2800 0000 6300 0000 0000  rQ...r(...c.....
-00003d70: 0000 0000 0000 0000 0000 0001 0000 0040  ...............@
-00003d80: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00003d90: 6401 5a03 6402 5a04 6504 5a05 6403 5300  d.Z.d.Z.e.Z.d.S.
-00003da0: 2904 7a17 5068 6172 6d61 6379 456e 7465  ).z.PharmacyEnte
-00003db0: 7270 7269 7365 2e4d 6574 615a 1662 735f  rprise.MetaZ.bs_
-00003dc0: 7068 6172 6d61 6379 5f65 6e74 6572 7072  pharmacy_enterpr
-00003dd0: 6973 6575 0c00 0000 e88d afe4 bc81 e7ae  iseu............
-00003de0: a1e7 9086 4e72 3600 0000 7219 0000 0072  ....Nr6...r....r
-00003df0: 1900 0000 7219 0000 0072 1a00 0000 721b  ....r....r....r.
-00003e00: 0000 00e5 0100 0073 0600 0000 0801 0401  .......s........
-00003e10: 0401 721b 0000 004e 72ad 0000 0072 1900  ..r....Nr....r..
-00003e20: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00003e30: 0072 c400 0000 e101 0000 7306 0000 0008  .r........s.....
-00003e40: 0110 0112 0272 c400 0000 6300 0000 0000  .....r....c.....
-00003e50: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
-00003e60: 0000 0073 8600 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00003e70: 6503 6a04 6401 6402 6403 6404 8d03 5a05  e.j.d.d.d.d...Z.
-00003e80: 6503 6a04 6405 6406 6403 6403 6407 8d04  e.j.d.d.d.d.d...
-00003e90: 5a06 6503 6a07 6508 6408 6503 6a09 6409  Z.e.j.e.d.e.j.d.
-00003ea0: 8d03 5a0a 6503 6a0b 640a 6403 6403 640b  ..Z.e.j.d.d.d.d.
-00003eb0: 8d03 5a0c 6503 6a07 650d 640c 6503 6a0e  ..Z.e.j.e.d.e.j.
-00003ec0: 6403 640d 8d04 5a0f 6503 6a07 6510 640e  d.d...Z.e.j.e.d.
-00003ed0: 6503 6a0e 6403 640d 8d04 5a11 4700 640f  e.j.d.d...Z.G.d.
-00003ee0: 6410 8400 6410 8302 5a12 6411 5300 2912  d...d...Z.d.S.).
-00003ef0: da12 5068 6172 6d61 6379 4d61 6e61 6765  ..PharmacyManage
-00003f00: 6d65 6e74 750c 0000 00e8 8daf e688 bfe7  mentu...........
-00003f10: bc96 e7a0 8172 2300 0000 5472 ab00 0000  .....r#...Tr....
-00003f20: 750c 0000 00e8 8daf e688 bfe5 908d e7a7  u...............
-00003f30: b072 5100 0000 7228 0000 0072 c300 0000  .rQ...r(...r....
-00003f40: 7248 0000 0075 0c00 0000 e88d afe6 88bf  rH...u..........
-00003f50: e59c b0e5 9d80 722a 0000 0072 2f00 0000  ......r*...r/...
-00003f60: 7230 0000 0075 0c00 0000 e689 80e5 b19e  r0...u..........
-00003f70: e88d afe4 bc81 6300 0000 0000 0000 0000  ......c.........
-00003f80: 0000 0000 0000 0001 0000 0040 0000 0073  ...........@...s
-00003f90: 1800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00003fa0: 6402 5a04 6504 5a05 6403 5300 2904 7a17  d.Z.e.Z.d.S.).z.
-00003fb0: 5068 6172 6d61 6379 4d61 6e61 6765 6d65  PharmacyManageme
-00003fc0: 6e74 2e4d 6574 615a 1662 735f 7068 6172  nt.MetaZ.bs_phar
-00003fd0: 6d61 6379 5f6d 616e 6167 656d 656e 7475  macy_managementu
-00003fe0: 0c00 0000 e88d afe6 88bf e7ae a1e7 9086  ................
-00003ff0: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
-00004000: 7219 0000 0072 1a00 0000 721b 0000 00f7  r....r....r.....
-00004010: 0100 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
-00004020: 0000 004e 2913 7215 0000 0072 1600 0000  ...N).r....r....
-00004030: 7217 0000 0072 0500 0000 7239 0000 005a  r....r....r9...Z
-00004040: 0d70 6861 726d 6163 795f 636f 6465 5a0d  .pharmacy_codeZ.
-00004050: 7068 6172 6d61 6379 5f6e 616d 6572 4100  pharmacy_namerA.
-00004060: 0000 72c2 0000 0072 bc00 0000 5a0d 7068  ..r....r....Z.ph
-00004070: 6172 6d61 6379 5f74 7970 6572 3c00 0000  armacy_typer<...
-00004080: 723f 0000 0072 2100 0000 7242 0000 0072  r?...r!...rB...r
-00004090: 4a00 0000 72c4 0000 005a 0a65 6e74 6572  J...r....Z.enter
-000040a0: 7072 6973 6572 1b00 0000 7219 0000 0072  priser....r....r
-000040b0: 1900 0000 7219 0000 0072 1a00 0000 72c5  ....r....r....r.
-000040c0: 0000 00eb 0100 0073 1600 0000 0801 1001  .......s........
-000040d0: 1201 0401 0201 0201 04fd 0605 1001 1401  ................
-000040e0: 1402 72c5 0000 0063 0000 0000 0000 0000  ..r....c........
-000040f0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
-00004100: 734e 0100 0065 005a 0164 005a 0265 036a  sN...e.Z.d.Z.e.j
-00004110: 0465 0564 0165 036a 0664 0264 038d 045a  .e.d.e.j.d.d...Z
-00004120: 0765 036a 0864 0464 0564 0264 0264 068d  .e.j.d.d.d.d.d..
-00004130: 045a 0965 036a 0864 0764 0864 0264 0264  .Z.e.j.d.d.d.d.d
-00004140: 098d 045a 0a65 036a 0864 0764 0a64 0264  ...Z.e.j.d.d.d.d
-00004150: 0264 098d 045a 0b65 036a 0864 0764 0b64  .d...Z.e.j.d.d.d
-00004160: 0264 0264 098d 045a 0c65 036a 0465 0d64  .d.d...Z.e.j.e.d
-00004170: 0c65 036a 0e64 0d8d 035a 0f65 036a 0465  .e.j.d...Z.e.j.e
-00004180: 1064 0e65 036a 0e64 0d8d 035a 1165 036a  .d.e.j.d...Z.e.j
-00004190: 0465 1264 0f65 036a 0e64 0d8d 035a 1365  .e.d.e.j.d...Z.e
-000041a0: 036a 0864 1064 1164 0264 0264 098d 045a  .j.d.d.d.d.d...Z
-000041b0: 1465 036a 0864 1264 1364 0264 0264 098d  .e.j.d.d.d.d.d..
-000041c0: 045a 1565 036a 0465 1664 1465 036a 0664  .Z.e.j.e.d.e.j.d
-000041d0: 0264 038d 045a 1765 036a 1864 1564 0264  .d...Z.e.j.d.d.d
-000041e0: 0264 168d 035a 1965 036a 1a64 1764 1864  .d...Z.e.j.d.d.d
-000041f0: 0264 198d 035a 1b65 036a 0864 0764 1a64  .d...Z.e.j.d.d.d
-00004200: 0264 0264 098d 045a 1c65 036a 1d64 1b64  .d.d...Z.e.j.d.d
-00004210: 0264 1c8d 025a 1e65 036a 1d64 1d64 0264  .d...Z.e.j.d.d.d
-00004220: 1c8d 025a 1f65 036a 1d64 1e64 0264 1c8d  ...Z.e.j.d.d.d..
-00004230: 025a 2065 036a 1d64 1f64 0264 1c8d 025a  .Z e.j.d.d.d...Z
-00004240: 2147 0064 2064 2184 0064 2183 025a 2264  !G.d d!..d!..Z"d
-00004250: 2253 0029 23da 0c50 6861 726d 6163 7944  "S.)#..PharmacyD
-00004260: 7275 6775 0c00 0000 e689 80e5 b19e e88d  rugu............
-00004270: afe6 88bf 5472 3000 0000 72b1 0000 0072  ....Tr0...r....r
-00004280: 2300 0000 7228 0000 0072 5100 0000 72b2  #...r(...rQ...r.
-00004290: 0000 0072 7900 0000 72b3 0000 0075 0600  ...ry...r....u..
-000042a0: 0000 e58d 95e4 bd8d 72b4 0000 0072 4800  ........r....rH.
-000042b0: 0000 72ac 0000 0072 b500 0000 727f 0000  ..r....r....r...
-000042c0: 0072 b700 0000 e9c8 0000 0072 b800 0000  .r.........r....
-000042d0: 722f 0000 0075 0c00 0000 e69c 89e6 9588  r/...u..........
-000042e0: e697 a5e6 9c9f 7210 0000 0072 b600 0000  ......r....r....
-000042f0: 7201 0000 0072 7800 0000 750c 0000 00e8  r....rx...u.....
-00004300: aea1 e987 8fe5 8d95 e4bd 8d75 0c00 0000  ...........u....
-00004310: e688 90e6 9cac e58d 95e4 bbb7 728d 0000  ............r...
-00004320: 0075 0c00 0000 e688 90e6 9cac e987 91e9  .u..............
-00004330: a29d 750c 0000 00e9 9bb6 e594 aee5 8d95  ..u.............
-00004340: e4bb b775 0c00 0000 e99b b6e5 94ae e987  ...u............
-00004350: 91e9 a29d 6300 0000 0000 0000 0000 0000  ....c...........
-00004360: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
-00004370: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00004380: 5a04 6504 5a05 6403 5300 2904 7a11 5068  Z.e.Z.d.S.).z.Ph
-00004390: 6172 6d61 6379 4472 7567 2e4d 6574 615a  armacyDrug.MetaZ
-000043a0: 1062 735f 7068 6172 6d61 6379 5f64 7275  .bs_pharmacy_dru
-000043b0: 6775 0d00 0000 e88d afe6 88bf 2de8 8daf  gu..........-...
-000043c0: e593 814e 7236 0000 0072 1900 0000 7219  ...Nr6...r....r.
-000043d0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-000043e0: 0000 1d02 0000 7306 0000 0008 0104 0104  ......s.........
-000043f0: 0172 1b00 0000 4e29 2372 1500 0000 7216  .r....N)#r....r.
-00004400: 0000 0072 1700 0000 7205 0000 0072 4100  ...r....r....rA.
-00004410: 0000 72c5 0000 0072 4200 0000 5a08 7068  ..r....rB...Z.ph
-00004420: 6172 6d61 6379 7239 0000 0072 b900 0000  armacyr9...r....
-00004430: 72ba 0000 0072 bb00 0000 da05 756e 6974  r....r......unit
-00004440: 7372 a800 0000 72bc 0000 0072 bd00 0000  sr....r....r....
-00004450: 72aa 0000 0072 bf00 0000 72af 0000 0072  r....r....r....r
-00004460: be00 0000 72c0 0000 0072 c100 0000 7221  ....r....r....r!
-00004470: 0000 0072 4a00 0000 725f 0000 005a 0a76  ...rJ...r_...Z.v
-00004480: 616c 6964 5f64 6174 6572 6f00 0000 5a12  alid_datero...Z.
-00004490: 696e 7665 6e74 6f72 795f 7175 616e 7469  inventory_quanti
-000044a0: 7479 5a10 6d65 6173 7572 656d 656e 745f  tyZ.measurement_
-000044b0: 756e 6974 7240 0000 005a 0f63 6f73 745f  unitr@...Z.cost_
-000044c0: 756e 6974 5f70 7269 6365 5a0b 636f 7374  unit_priceZ.cost
-000044d0: 5f61 6d6f 756e 745a 1172 6574 6169 6c5f  _amountZ.retail_
-000044e0: 756e 6974 5f70 7269 6365 5a0d 7265 7461  unit_priceZ.reta
-000044f0: 696c 5f61 6d6f 756e 7472 1b00 0000 7219  il_amountr....r.
-00004500: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00004510: 0000 72c6 0000 00fd 0100 0073 3e00 0000  ..r........s>...
-00004520: 0801 1401 1201 1201 1201 1201 0401 0201  ................
-00004530: 0201 04fd 0605 0401 0201 0201 04fd 0605  ................
-00004540: 0401 0201 0201 04fd 0605 1201 1201 1401  ................
-00004550: 1001 1001 1201 0e01 0e01 0e01 0e02 72c6  ..............r.
-00004560: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00004570: 0000 0000 0600 0000 4000 0000 73b6 0000  ........@...s...
-00004580: 0065 005a 0164 005a 0265 036a 0464 0164  .e.Z.d.Z.e.j.d.d
-00004590: 0264 038d 025a 0565 036a 0464 0164 0464  .d...Z.e.j.d.d.d
-000045a0: 038d 025a 0665 036a 0464 0164 0564 0664  ...Z.e.j.d.d.d.d
-000045b0: 0664 078d 045a 0765 036a 0464 0164 0864  .d...Z.e.j.d.d.d
-000045c0: 038d 025a 0865 036a 0464 0164 0964 038d  ...Z.e.j.d.d.d..
-000045d0: 025a 0965 036a 0464 0a64 0b64 038d 025a  .Z.e.j.d.d.d...Z
-000045e0: 0a65 036a 0464 0a64 0c64 038d 025a 0b65  .e.j.d.d.d...Z.e
-000045f0: 036a 0c64 0d64 0664 0664 0e8d 035a 0d65  .j.d.d.d.d...Z.e
-00004600: 036a 0c64 0f64 0664 0664 108d 035a 0e65  .j.d.d.d.d...Z.e
-00004610: 036a 0f64 1164 0664 128d 025a 1047 0064  .j.d.d.d...Z.G.d
-00004620: 1364 1484 0064 1483 025a 1164 1564 1684  .d...d...Z.d.d..
-00004630: 005a 1264 1753 0029 18da 0741 7069 496e  .Z.d.S.)...ApiIn
-00004640: 666f 7276 0000 0072 a000 0000 729e 0000  forv...r....r...
-00004650: 0075 0c00 0000 e8af b7e6 b182 e7bc 96e7  .u..............
-00004660: a081 750c 0000 00e8 afb7 e6b1 82e5 908d  ..u.............
-00004670: e7a7 b054 7279 0000 0075 0c00 0000 e8af  ...Try...u......
-00004680: b7e6 b182 e696 b9e5 bc8f 7512 0000 00e8  ..........u.....
-00004690: afb7 e6b1 82e6 95b0 e68d aee7 b1bb e59e  ................
-000046a0: 8b72 c700 0000 7511 0000 0069 70e5 9cb0  .r....u....ip...
-000046b0: e59d 80e6 8896 e59f 9fe5 908d 750c 0000  ............u...
-000046c0: 00e8 afb7 e6b1 82e8 b7af e794 b172 0a00  .............r..
-000046d0: 0000 720b 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-000046e0: 0072 1200 0000 7213 0000 0063 0000 0000  .r....r....c....
-000046f0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00004700: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
-00004710: 0264 015a 0364 025a 0465 045a 0564 035a  .d.Z.d.Z.e.Z.d.Z
-00004720: 0664 0453 0029 057a 0c41 7069 496e 666f  .d.S.).z.ApiInfo
-00004730: 2e4d 6574 615a 0b62 735f 6170 695f 696e  .MetaZ.bs_api_in
-00004740: 666f 750c 0000 00e6 8ea5 e58f a3e4 bfa1  fou.............
-00004750: e681 af29 01a9 02da 086f 7267 5f63 6f64  ...).....org_cod
-00004760: 65da 0872 6571 5f63 6f64 654e 724b 0000  e..req_codeNrK..
-00004770: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00004780: 721a 0000 0072 1b00 0000 2f02 0000 7308  r....r..../...s.
-00004790: 0000 0008 0104 0104 0104 0172 1b00 0000  ...........r....
-000047a0: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
-000047b0: 0005 0000 0043 0000 0073 ba00 0000 7400  .....C...s....t.
-000047c0: 6a01 6a02 7c01 6401 1900 7c02 6402 8d02  j.j.|.d...|.d...
-000047d0: a003 a100 7d03 7c03 72a8 7c03 6a04 7c03  ....}.|.r.|.j.|.
-000047e0: 6a05 1700 7d04 7c03 6a06 6403 6b02 7242  j...}.|.j.d.k.rB
-000047f0: 7407 6a08 7c04 7c01 6404 8d02 7d05 6e58  t.j.|.|.d...}.nX
-00004800: 7c03 6a06 6405 6b02 725c 7407 6a09 7c04  |.j.d.k.r\t.j.|.
-00004810: 7c01 6406 8d02 7d05 6e3e 7c03 6a06 6407  |.d...}.n>|.j.d.
-00004820: 6b02 7276 7407 6a0a 7c04 7c01 6408 8d02  k.rvt.j.|.|.d...
-00004830: 7d05 6e24 7c03 6a06 6409 6b02 728e 7407  }.n$|.j.d.k.r.t.
-00004840: 6a0b 7c04 640a 8d01 7d05 6e0c 7407 6a0c  j.|.d...}.n.t.j.
-00004850: 7c04 640a 8d01 7d05 740d a00e 7c05 6a0f  |.d...}.t...|.j.
-00004860: a101 7d06 6e0e 640b 640c 640d 6900 640e  ..}.n.d.d.d.i.d.
-00004870: 9c04 7d06 7c06 5300 290f 4e72 a500 0000  ..}.|.S.).Nr....
-00004880: 72ca 0000 00da 0450 4f53 5429 0272 8b00  r......POST).r..
-00004890: 0000 da04 6a73 6f6e da03 4745 5429 0272  ....json..GET).r
-000048a0: 8b00 0000 da06 7061 7261 6d73 da03 5055  ......params..PU
-000048b0: 5429 0272 8b00 0000 da04 6461 7461 da06  T).r......data..
-000048c0: 4445 4c45 5445 2901 728b 0000 0046 69d1  DELETE).r....Fi.
-000048d0: 0700 0075 1e00 0000 e4b8 8de5 ad98 e59c  ...u............
-000048e0: a8e5 afb9 e68e a5e5 8cbb e999 a2e4 bfa1  ................
-000048f0: e681 afef bc81 2904 da07 7375 6363 6573  ......)...succes
-00004900: 7372 ae00 0000 da07 6d65 7373 6167 6572  sr......messager
-00004910: d200 0000 2910 72c9 0000 00da 076f 626a  ....).r......obj
-00004920: 6563 7473 da06 6669 6c74 6572 7267 0000  ects..filterrg..
-00004930: 00da 0969 705f 646f 6d61 696e 728f 0000  ...ip_domainr...
-00004940: 00da 0a72 6571 5f6d 6574 686f 64da 0872  ...req_method..r
-00004950: 6571 7565 7374 73da 0470 6f73 74da 0367  equests..post..g
-00004960: 6574 da03 7075 74da 0664 656c 6574 65da  et..put..delete.
-00004970: 0570 6174 6368 72ce 0000 00da 056c 6f61  .patchr......loa
-00004980: 6473 da04 7465 7874 2907 722e 0000 005a  ds..text).r....Z
-00004990: 0769 6e5f 6461 7461 72cc 0000 005a 0c61  .in_datar....Z.a
-000049a0: 7069 5f69 6e66 6f5f 6f62 6a5a 0763 6d73  pi_info_objZ.cms
-000049b0: 5f75 726c da03 7265 735a 0872 6573 5f6a  _url..resZ.res_j
-000049c0: 736f 6e72 1900 0000 7219 0000 0072 1a00  sonr....r....r..
-000049d0: 0000 da09 7772 6974 6562 6163 6b37 0200  ....writeback7..
-000049e0: 0073 1e00 0000 0001 1801 0401 0c01 0a01  .s..............
-000049f0: 1001 0a01 1001 0a01 1001 0a01 0e02 0c01  ................
-00004a00: 0e02 0e01 7a11 4170 6949 6e66 6f2e 7772  ....z.ApiInfo.wr
-00004a10: 6974 6562 6163 6b4e 2913 7215 0000 0072  itebackN).r....r
-00004a20: 1600 0000 7217 0000 0072 0500 0000 7239  ....r....r....r9
-00004a30: 0000 0072 cb00 0000 72cc 0000 005a 0872  ...r....r....Z.r
-00004a40: 6571 5f6e 616d 6572 d900 0000 728e 0000  eq_namer....r...
-00004a50: 0072 d800 0000 728f 0000 0072 1c00 0000  .r....r....r....
-00004a60: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00004a70: 2000 0000 721b 0000 0072 e300 0000 7219   ...r....r....r.
-00004a80: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00004a90: 0000 72c9 0000 0023 0200 0073 1800 0000  ..r....#...s....
-00004aa0: 0801 0e01 0e01 1201 0e01 0e01 0e01 0e01  ................
-00004ab0: 1001 1001 0e02 0e08 72c9 0000 0029 2572  ........r....)%r
-00004ac0: ce00 0000 da02 6f73 72da 0000 00da 1a64  ......osr......d
-00004ad0: 6a61 6e67 6f2e 636f 6e74 7269 622e 6175  jango.contrib.au
-00004ae0: 7468 2e6d 6f64 656c 7372 0200 0000 7203  th.modelsr....r.
-00004af0: 0000 00da 2264 6a61 6e67 6f2e 636f 6e74  ...."django.cont
-00004b00: 7269 622e 636f 6e74 656e 7474 7970 6573  rib.contenttypes
-00004b10: 2e6d 6f64 656c 7372 0400 0000 da09 646a  .modelsr......dj
-00004b20: 616e 676f 2e64 6272 0500 0000 da0b 646a  ango.dbr......dj
-00004b30: 616e 676f 2e63 6f6e 6672 0600 0000 725c  ango.confr....r\
-00004b40: 0000 00da 054d 6f64 656c 7209 0000 0072  .....Modelr....r
-00004b50: 2100 0000 7246 0000 0072 4d00 0000 724f  !...rF...rM...rO
-00004b60: 0000 0072 6200 0000 7273 0000 0072 7d00  ...rb...rs...r}.
-00004b70: 0000 7289 0000 0072 9100 0000 7294 0000  ..r....r....r...
-00004b80: 0072 9b00 0000 72a6 0000 0072 a700 0000  .r....r....r....
-00004b90: 72a8 0000 0072 aa00 0000 72af 0000 0072  r....r....r....r
-00004ba0: b000 0000 72c2 0000 0072 c400 0000 72c5  ....r....r....r.
-00004bb0: 0000 0072 c600 0000 72c9 0000 0072 1900  ...r....r....r..
-00004bc0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00004bd0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00004be0: 3c00 0000 0801 0802 0801 1001 0c01 0c01  <...............
-00004bf0: 0c02 0406 1209 101e 101c 1014 1028 104a  .............(.J
-00004c00: 121b 121b 1223 1019 1011 1011 1011 1011  .....#..........
-00004c10: 100a 100a 100a 102a 100a 100a 1012 1026  .......*.......&
+00003cc0: 0000 72b2 0000 00ba 0100 0073 4600 0000  ..r........sF...
+00003cd0: 0801 1001 1201 1201 1201 1201 0401 0201  ................
+00003ce0: 0201 04fd 0605 0401 0201 0201 04fd 0605  ................
+00003cf0: 0401 0201 0201 04fd 0605 1201 1201 1201  ................
+00003d00: 1201 1201 1201 1201 0e01 1201 1201 1201  ................
+00003d10: 1201 1201 1002 72b2 0000 0063 0000 0000  ......r....c....
+00003d20: 0000 0000 0000 0000 0000 0000 0600 0000  ................
+00003d30: 4000 0000 733c 0000 0065 005a 0164 005a  @...s<...e.Z.d.Z
+00003d40: 0265 036a 0464 0164 0264 0364 048d 035a  .e.j.d.d.d.d...Z
+00003d50: 0565 036a 0464 0564 0664 0364 0364 078d  .e.j.d.d.d.d.d..
+00003d60: 045a 0647 0064 0864 0984 0064 0983 025a  .Z.G.d.d...d...Z
+00003d70: 0764 0a53 0029 0bda 0c50 6861 726d 6163  .d.S.)...Pharmac
+00003d80: 7954 7970 6572 2b00 0000 7223 0000 0054  yTyper+...r#...T
+00003d90: 72ae 0000 0072 2200 0000 7251 0000 0072  r....r"...rQ...r
+00003da0: 2800 0000 6300 0000 0000 0000 0000 0000  (...c...........
+00003db0: 0000 0000 0001 0000 0040 0000 0073 1800  .........@...s..
+00003dc0: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00003dd0: 5a04 6504 5a05 6403 5300 2904 7a11 5068  Z.e.Z.d.S.).z.Ph
+00003de0: 6172 6d61 6379 5479 7065 2e4d 6574 615a  armacyType.MetaZ
+00003df0: 1062 735f 7068 6172 6d61 6379 5f74 7970  .bs_pharmacy_typ
+00003e00: 65f5 0c00 0000 e88d afe6 88bf e7b1 bbe5  e...............
+00003e10: 9e8b 4e72 3600 0000 7219 0000 0072 1900  ..Nr6...r....r..
+00003e20: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00003e30: 00e8 0100 0073 0600 0000 0801 0401 0401  .....s..........
+00003e40: 721b 0000 004e 72b0 0000 0072 1900 0000  r....Nr....r....
+00003e50: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00003e60: c400 0000 e401 0000 7306 0000 0008 0110  ........s.......
+00003e70: 0112 0272 c400 0000 6300 0000 0000 0000  ...r....c.......
+00003e80: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
+00003e90: 0073 3c00 0000 6500 5a01 6400 5a02 6503  .s<...e.Z.d.Z.e.
+00003ea0: 6a04 6401 6402 6403 6404 8d03 5a05 6503  j.d.d.d.d...Z.e.
+00003eb0: 6a04 6405 6406 6403 6403 6407 8d04 5a06  j.d.d.d.d.d...Z.
+00003ec0: 4700 6408 6409 8400 6409 8302 5a07 640a  G.d.d...d...Z.d.
+00003ed0: 5300 290b da12 5068 6172 6d61 6379 456e  S.)...PharmacyEn
+00003ee0: 7465 7270 7269 7365 722b 0000 0072 2300  terpriser+...r#.
+00003ef0: 0000 5472 ae00 0000 7222 0000 0072 5100  ..Tr....r"...rQ.
+00003f00: 0000 7228 0000 0063 0000 0000 0000 0000  ..r(...c........
+00003f10: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
+00003f20: 7318 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
+00003f30: 0364 025a 0465 045a 0564 0353 0029 047a  .d.Z.e.Z.d.S.).z
+00003f40: 1750 6861 726d 6163 7945 6e74 6572 7072  .PharmacyEnterpr
+00003f50: 6973 652e 4d65 7461 5a16 6273 5f70 6861  ise.MetaZ.bs_pha
+00003f60: 726d 6163 795f 656e 7465 7270 7269 7365  rmacy_enterprise
+00003f70: 750c 0000 00e8 8daf e4bc 81e7 aea1 e790  u...............
+00003f80: 864e 7236 0000 0072 1900 0000 7219 0000  .Nr6...r....r...
+00003f90: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
+00003fa0: f201 0000 7306 0000 0008 0104 0104 0172  ....s..........r
+00003fb0: 1b00 0000 4e72 b000 0000 7219 0000 0072  ....Nr....r....r
+00003fc0: 1900 0000 7219 0000 0072 1a00 0000 72c6  ....r....r....r.
+00003fd0: 0000 00ee 0100 0073 0600 0000 0801 1001  .......s........
+00003fe0: 1202 72c6 0000 0063 0000 0000 0000 0000  ..r....c........
+00003ff0: 0000 0000 0000 0000 0600 0000 4000 0000  ............@...
+00004000: 7386 0000 0065 005a 0164 005a 0265 036a  s....e.Z.d.Z.e.j
+00004010: 0464 0164 0264 0364 048d 035a 0565 036a  .d.d.d.d...Z.e.j
+00004020: 0464 0564 0664 0364 0364 078d 045a 0665  .d.d.d.d.d...Z.e
+00004030: 036a 0765 0864 0865 036a 0964 098d 035a  .j.e.d.e.j.d...Z
+00004040: 0a65 036a 0b64 0a64 0364 0364 0b8d 035a  .e.j.d.d.d.d...Z
+00004050: 0c65 036a 0765 0d64 0c65 036a 0e64 0364  .e.j.e.d.e.j.d.d
+00004060: 0d8d 045a 0f65 036a 0765 1064 0e65 036a  ...Z.e.j.e.d.e.j
+00004070: 0e64 0364 0d8d 045a 1147 0064 0f64 1084  .d.d...Z.G.d.d..
+00004080: 0064 1083 025a 1264 1153 0029 12da 1250  .d...Z.d.S.)...P
+00004090: 6861 726d 6163 794d 616e 6167 656d 656e  harmacyManagemen
+000040a0: 7475 0c00 0000 e88d afe6 88bf e7bc 96e7  tu..............
+000040b0: a081 7223 0000 0054 72ae 0000 0075 0c00  ..r#...Tr....u..
+000040c0: 0000 e88d afe6 88bf e590 8de7 a7b0 7251  ..............rQ
+000040d0: 0000 0072 2800 0000 72c5 0000 0072 4800  ...r(...r....rH.
+000040e0: 0000 750c 0000 00e8 8daf e688 bfe5 9cb0  ..u.............
+000040f0: e59d 8072 2a00 0000 722f 0000 0072 3000  ...r*...r/...r0.
+00004100: 0000 750c 0000 00e6 8980 e5b1 9ee8 8daf  ..u.............
+00004110: e4bc 8163 0000 0000 0000 0000 0000 0000  ...c............
+00004120: 0000 0000 0100 0000 4000 0000 7318 0000  ........@...s...
+00004130: 0065 005a 0164 005a 0264 015a 0364 025a  .e.Z.d.Z.d.Z.d.Z
+00004140: 0465 045a 0564 0353 0029 047a 1750 6861  .e.Z.d.S.).z.Pha
+00004150: 726d 6163 794d 616e 6167 656d 656e 742e  rmacyManagement.
+00004160: 4d65 7461 5a16 6273 5f70 6861 726d 6163  MetaZ.bs_pharmac
+00004170: 795f 6d61 6e61 6765 6d65 6e74 750c 0000  y_managementu...
+00004180: 00e8 8daf e688 bfe7 aea1 e790 864e 7236  .............Nr6
+00004190: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
+000041a0: 0000 721a 0000 0072 1b00 0000 0402 0000  ..r....r........
+000041b0: 7306 0000 0008 0104 0104 0172 1b00 0000  s..........r....
+000041c0: 4e29 1372 1500 0000 7216 0000 0072 1700  N).r....r....r..
+000041d0: 0000 7205 0000 0072 3900 0000 5a0d 7068  ..r....r9...Z.ph
+000041e0: 6172 6d61 6379 5f63 6f64 655a 0d70 6861  armacy_codeZ.pha
+000041f0: 726d 6163 795f 6e61 6d65 7241 0000 0072  rmacy_namerA...r
+00004200: c400 0000 72be 0000 005a 0d70 6861 726d  ....r....Z.pharm
+00004210: 6163 795f 7479 7065 723c 0000 0072 3f00  acy_typer<...r?.
+00004220: 0000 7221 0000 0072 4200 0000 724a 0000  ..r!...rB...rJ..
+00004230: 0072 c600 0000 5a0a 656e 7465 7270 7269  .r....Z.enterpri
+00004240: 7365 721b 0000 0072 1900 0000 7219 0000  ser....r....r...
+00004250: 0072 1900 0000 721a 0000 0072 c700 0000  .r....r....r....
+00004260: f801 0000 7316 0000 0008 0110 0112 0104  ....s...........
+00004270: 0102 0102 0104 fd06 0510 0114 0114 0272  ...............r
+00004280: c700 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00004290: 0000 0000 0006 0000 0040 0000 0073 4e01  .........@...sN.
+000042a0: 0000 6500 5a01 6400 5a02 6503 6a04 6505  ..e.Z.d.Z.e.j.e.
+000042b0: 6401 6503 6a06 6402 6403 8d04 5a07 6503  d.e.j.d.d...Z.e.
+000042c0: 6a08 6404 6405 6402 6402 6406 8d04 5a09  j.d.d.d.d.d...Z.
+000042d0: 6503 6a08 6407 6408 6402 6402 6409 8d04  e.j.d.d.d.d.d...
+000042e0: 5a0a 6503 6a08 6407 640a 6402 6402 6409  Z.e.j.d.d.d.d.d.
+000042f0: 8d04 5a0b 6503 6a08 6407 640b 6402 6402  ..Z.e.j.d.d.d.d.
+00004300: 6409 8d04 5a0c 6503 6a04 650d 640c 6503  d...Z.e.j.e.d.e.
+00004310: 6a0e 640d 8d03 5a0f 6503 6a04 6510 640e  j.d...Z.e.j.e.d.
+00004320: 6503 6a0e 640d 8d03 5a11 6503 6a04 6512  e.j.d...Z.e.j.e.
+00004330: 640f 6503 6a0e 640d 8d03 5a13 6503 6a08  d.e.j.d...Z.e.j.
+00004340: 6410 6411 6402 6402 6409 8d04 5a14 6503  d.d.d.d.d...Z.e.
+00004350: 6a08 6412 6413 6402 6402 6409 8d04 5a15  j.d.d.d.d.d...Z.
+00004360: 6503 6a04 6516 6414 6503 6a06 6402 6403  e.j.e.d.e.j.d.d.
+00004370: 8d04 5a17 6503 6a18 6415 6402 6402 6416  ..Z.e.j.d.d.d.d.
+00004380: 8d03 5a19 6503 6a1a 6417 6418 6402 6419  ..Z.e.j.d.d.d.d.
+00004390: 8d03 5a1b 6503 6a08 6407 641a 6402 6402  ..Z.e.j.d.d.d.d.
+000043a0: 6409 8d04 5a1c 6503 6a1d 641b 6402 641c  d...Z.e.j.d.d.d.
+000043b0: 8d02 5a1e 6503 6a1d 641d 6402 641c 8d02  ..Z.e.j.d.d.d...
+000043c0: 5a1f 6503 6a1d 641e 6402 641c 8d02 5a20  Z.e.j.d.d.d...Z 
+000043d0: 6503 6a1d 641f 6402 641c 8d02 5a21 4700  e.j.d.d.d...Z!G.
+000043e0: 6420 6421 8400 6421 8302 5a22 6422 5300  d d!..d!..Z"d"S.
+000043f0: 2923 da0c 5068 6172 6d61 6379 4472 7567  )#..PharmacyDrug
+00004400: 750c 0000 00e6 8980 e5b1 9ee8 8daf e688  u...............
+00004410: bf54 7230 0000 0072 b300 0000 7223 0000  .Tr0...r....r#..
+00004420: 0072 2800 0000 7251 0000 0072 b400 0000  .r(...rQ...r....
+00004430: 7279 0000 0072 b500 0000 7506 0000 00e5  ry...r....u.....
+00004440: 8d95 e4bd 8d72 b600 0000 7248 0000 0072  .....r....rH...r
+00004450: af00 0000 72b7 0000 0072 7f00 0000 72b9  ....r....r....r.
+00004460: 0000 00e9 c800 0000 72ba 0000 0072 2f00  ........r....r/.
+00004470: 0000 750c 0000 00e6 9c89 e695 88e6 97a5  ..u.............
+00004480: e69c 9f72 1000 0000 72b8 0000 0072 0100  ...r....r....r..
+00004490: 0000 7278 0000 0075 0c00 0000 e8ae a1e9  ..rx...u........
+000044a0: 878f e58d 95e4 bd8d 750c 0000 00e6 8890  ........u.......
+000044b0: e69c ace5 8d95 e4bb b772 8d00 0000 750c  .........r....u.
+000044c0: 0000 00e6 8890 e69c ace9 8791 e9a2 9d75  ...............u
+000044d0: 0c00 0000 e99b b6e5 94ae e58d 95e4 bbb7  ................
+000044e0: 750c 0000 00e9 9bb6 e594 aee9 8791 e9a2  u...............
+000044f0: 9d63 0000 0000 0000 0000 0000 0000 0000  .c..............
+00004500: 0000 0100 0000 4000 0000 7318 0000 0065  ......@...s....e
+00004510: 005a 0164 005a 0264 015a 0364 025a 0465  .Z.d.Z.d.Z.d.Z.e
+00004520: 045a 0564 0353 0029 047a 1150 6861 726d  .Z.d.S.).z.Pharm
+00004530: 6163 7944 7275 672e 4d65 7461 5a10 6273  acyDrug.MetaZ.bs
+00004540: 5f70 6861 726d 6163 795f 6472 7567 750d  _pharmacy_drugu.
+00004550: 0000 00e8 8daf e688 bf2d e88d afe5 9381  .........-......
+00004560: 4e72 3600 0000 7219 0000 0072 1900 0000  Nr6...r....r....
+00004570: 7219 0000 0072 1a00 0000 721b 0000 002a  r....r....r....*
+00004580: 0200 0073 0600 0000 0801 0401 0401 721b  ...s..........r.
+00004590: 0000 004e 2923 7215 0000 0072 1600 0000  ...N)#r....r....
+000045a0: 7217 0000 0072 0500 0000 7241 0000 0072  r....r....rA...r
+000045b0: c700 0000 7242 0000 005a 0870 6861 726d  ....rB...Z.pharm
+000045c0: 6163 7972 3900 0000 72bb 0000 0072 bc00  acyr9...r....r..
+000045d0: 0000 72bd 0000 00da 0575 6e69 7473 72ab  ..r......unitsr.
+000045e0: 0000 0072 be00 0000 72bf 0000 0072 ad00  ...r....r....r..
+000045f0: 0000 72c1 0000 0072 b100 0000 72c0 0000  ..r....r....r...
+00004600: 0072 c200 0000 72c3 0000 0072 2100 0000  .r....r....r!...
+00004610: 724a 0000 0072 6000 0000 5a0a 7661 6c69  rJ...r`...Z.vali
+00004620: 645f 6461 7465 7270 0000 005a 1269 6e76  d_daterp...Z.inv
+00004630: 656e 746f 7279 5f71 7561 6e74 6974 795a  entory_quantityZ
+00004640: 106d 6561 7375 7265 6d65 6e74 5f75 6e69  .measurement_uni
+00004650: 7472 4000 0000 5a0f 636f 7374 5f75 6e69  tr@...Z.cost_uni
+00004660: 745f 7072 6963 655a 0b63 6f73 745f 616d  t_priceZ.cost_am
+00004670: 6f75 6e74 5a11 7265 7461 696c 5f75 6e69  ountZ.retail_uni
+00004680: 745f 7072 6963 655a 0d72 6574 6169 6c5f  t_priceZ.retail_
+00004690: 616d 6f75 6e74 721b 0000 0072 1900 0000  amountr....r....
+000046a0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+000046b0: c800 0000 0a02 0000 733e 0000 0008 0114  ........s>......
+000046c0: 0112 0112 0112 0112 0104 0102 0102 0104  ................
+000046d0: fd06 0504 0102 0102 0104 fd06 0504 0102  ................
+000046e0: 0102 0104 fd06 0512 0112 0114 0110 0110  ................
+000046f0: 0112 010e 010e 010e 010e 0272 c800 0000  ...........r....
+00004700: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004710: 0006 0000 0040 0000 0073 b600 0000 6500  .....@...s....e.
+00004720: 5a01 6400 5a02 6503 6a04 6401 6402 6403  Z.d.Z.e.j.d.d.d.
+00004730: 8d02 5a05 6503 6a04 6401 6404 6403 8d02  ..Z.e.j.d.d.d...
+00004740: 5a06 6503 6a04 6401 6405 6406 6406 6407  Z.e.j.d.d.d.d.d.
+00004750: 8d04 5a07 6503 6a04 6401 6408 6403 8d02  ..Z.e.j.d.d.d...
+00004760: 5a08 6503 6a04 6401 6409 6403 8d02 5a09  Z.e.j.d.d.d...Z.
+00004770: 6503 6a04 640a 640b 6403 8d02 5a0a 6503  e.j.d.d.d...Z.e.
+00004780: 6a04 640a 640c 6403 8d02 5a0b 6503 6a0c  j.d.d.d...Z.e.j.
+00004790: 640d 6406 6406 640e 8d03 5a0d 6503 6a0c  d.d.d.d...Z.e.j.
+000047a0: 640f 6406 6406 6410 8d03 5a0e 6503 6a0f  d.d.d.d...Z.e.j.
+000047b0: 6411 6406 6412 8d02 5a10 4700 6413 6414  d.d.d...Z.G.d.d.
+000047c0: 8400 6414 8302 5a11 6415 6416 8400 5a12  ..d...Z.d.d...Z.
+000047d0: 6417 5300 2918 da07 4170 6949 6e66 6f72  d.S.)...ApiInfor
+000047e0: 5a00 0000 72a3 0000 0072 a100 0000 750c  Z...r....r....u.
+000047f0: 0000 00e8 afb7 e6b1 82e7 bc96 e7a0 8175  ...............u
+00004800: 0c00 0000 e8af b7e6 b182 e590 8de7 a7b0  ................
+00004810: 5472 7900 0000 750c 0000 00e8 afb7 e6b1  Try...u.........
+00004820: 82e6 96b9 e5bc 8f75 1200 0000 e8af b7e6  .......u........
+00004830: b182 e695 b0e6 8dae e7b1 bbe5 9e8b 72c9  ..............r.
+00004840: 0000 0075 1100 0000 6970 e59c b0e5 9d80  ...u....ip......
+00004850: e688 96e5 9f9f e590 8d75 0c00 0000 e8af  .........u......
+00004860: b7e6 b182 e8b7 afe7 94b1 720a 0000 0072  ..........r....r
+00004870: 0b00 0000 720f 0000 0072 1000 0000 7212  ....r....r....r.
+00004880: 0000 0072 1300 0000 6300 0000 0000 0000  ...r....c.......
+00004890: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
+000048a0: 0073 1c00 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000048b0: 5a03 6402 5a04 6504 5a05 6403 5a06 6404  Z.d.Z.e.Z.d.Z.d.
+000048c0: 5300 2905 7a0c 4170 6949 6e66 6f2e 4d65  S.).z.ApiInfo.Me
+000048d0: 7461 5a0b 6273 5f61 7069 5f69 6e66 6f75  taZ.bs_api_infou
+000048e0: 0c00 0000 e68e a5e5 8fa3 e4bf a1e6 81af  ................
+000048f0: 2901 a902 da08 6f72 675f 636f 6465 da08  ).....org_code..
+00004900: 7265 715f 636f 6465 4e72 4b00 0000 7219  req_codeNrK...r.
+00004910: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00004920: 0000 721b 0000 003c 0200 0073 0800 0000  ..r....<...s....
+00004930: 0801 0401 0401 0401 721b 0000 0063 0300  ........r....c..
+00004940: 0000 0000 0000 0000 0000 0700 0000 0500  ................
+00004950: 0000 4300 0000 73ba 0000 0074 006a 016a  ..C...s....t.j.j
+00004960: 027c 0164 0119 007c 0264 028d 02a0 03a1  .|.d...|.d......
+00004970: 007d 037c 0372 a87c 036a 047c 036a 0517  .}.|.r.|.j.|.j..
+00004980: 007d 047c 036a 0664 036b 0272 4274 076a  .}.|.j.d.k.rBt.j
+00004990: 087c 047c 0164 048d 027d 056e 587c 036a  .|.|.d...}.nX|.j
+000049a0: 0664 056b 0272 5c74 076a 097c 047c 0164  .d.k.r\t.j.|.|.d
+000049b0: 068d 027d 056e 3e7c 036a 0664 076b 0272  ...}.n>|.j.d.k.r
+000049c0: 7674 076a 0a7c 047c 0164 088d 027d 056e  vt.j.|.|.d...}.n
+000049d0: 247c 036a 0664 096b 0272 8e74 076a 0b7c  $|.j.d.k.r.t.j.|
+000049e0: 0464 0a8d 017d 056e 0c74 076a 0c7c 0464  .d...}.n.t.j.|.d
+000049f0: 0a8d 017d 0574 0da0 0e7c 056a 0fa1 017d  ...}.t...|.j...}
+00004a00: 066e 0e64 0b64 0c64 0d69 0064 0e9c 047d  .n.d.d.d.i.d...}
+00004a10: 067c 0653 0029 0f4e 72a8 0000 0072 cc00  .|.S.).Nr....r..
+00004a20: 0000 da04 504f 5354 2902 728b 0000 00da  ....POST).r.....
+00004a30: 046a 736f 6eda 0347 4554 2902 728b 0000  .json..GET).r...
+00004a40: 00da 0670 6172 616d 73da 0350 5554 2902  ...params..PUT).
+00004a50: 728b 0000 00da 0464 6174 61da 0644 454c  r......data..DEL
+00004a60: 4554 4529 0172 8b00 0000 4669 d107 0000  ETE).r....Fi....
+00004a70: 751e 0000 00e4 b88d e5ad 98e5 9ca8 e5af  u...............
+00004a80: b9e6 8ea5 e58c bbe9 99a2 e4bf a1e6 81af  ................
+00004a90: efbc 8129 04da 0773 7563 6365 7373 7293  ...)...successr.
+00004aa0: 0000 00da 076d 6573 7361 6765 72d4 0000  .....messager...
+00004ab0: 0029 1072 cb00 0000 da07 6f62 6a65 6374  .).r......object
+00004ac0: 73da 0666 696c 7465 7272 6800 0000 da09  s..filterrh.....
+00004ad0: 6970 5f64 6f6d 6169 6e72 8f00 0000 da0a  ip_domainr......
+00004ae0: 7265 715f 6d65 7468 6f64 da08 7265 7175  req_method..requ
+00004af0: 6573 7473 da04 706f 7374 da03 6765 74da  ests..post..get.
+00004b00: 0370 7574 da06 6465 6c65 7465 da05 7061  .put..delete..pa
+00004b10: 7463 6872 d000 0000 da05 6c6f 6164 73da  tchr......loads.
+00004b20: 0474 6578 7429 0772 2e00 0000 5a07 696e  .text).r....Z.in
+00004b30: 5f64 6174 6172 ce00 0000 5a0c 6170 695f  _datar....Z.api_
+00004b40: 696e 666f 5f6f 626a 5a07 636d 735f 7572  info_objZ.cms_ur
+00004b50: 6cda 0372 6573 5a08 7265 735f 6a73 6f6e  l..resZ.res_json
+00004b60: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
+00004b70: 0977 7269 7465 6261 636b 4402 0000 731e  .writebackD...s.
+00004b80: 0000 0000 0118 0104 010c 010a 0110 010a  ................
+00004b90: 0110 010a 0110 010a 010e 020c 010e 020e  ................
+00004ba0: 017a 1141 7069 496e 666f 2e77 7269 7465  .z.ApiInfo.write
+00004bb0: 6261 636b 4e29 1372 1500 0000 7216 0000  backN).r....r...
+00004bc0: 0072 1700 0000 7205 0000 0072 3900 0000  .r....r....r9...
+00004bd0: 72cd 0000 0072 ce00 0000 5a08 7265 715f  r....r....Z.req_
+00004be0: 6e61 6d65 72db 0000 0072 8e00 0000 72da  namer....r....r.
+00004bf0: 0000 0072 8f00 0000 721c 0000 0072 1d00  ...r....r....r..
+00004c00: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00004c10: 0072 1b00 0000 72e5 0000 0072 1900 0000  .r....r....r....
+00004c20: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00004c30: cb00 0000 3002 0000 7318 0000 0008 010e  ....0...s.......
+00004c40: 010e 0112 010e 010e 010e 010e 0110 0110  ................
+00004c50: 010e 020e 0872 cb00 0000 2926 72d0 0000  .....r....)&r...
+00004c60: 00da 026f 7372 dc00 0000 da1a 646a 616e  ...osr......djan
+00004c70: 676f 2e63 6f6e 7472 6962 2e61 7574 682e  go.contrib.auth.
+00004c80: 6d6f 6465 6c73 7202 0000 0072 0300 0000  modelsr....r....
+00004c90: da22 646a 616e 676f 2e63 6f6e 7472 6962  ."django.contrib
+00004ca0: 2e63 6f6e 7465 6e74 7479 7065 732e 6d6f  .contenttypes.mo
+00004cb0: 6465 6c73 7204 0000 00da 0964 6a61 6e67  delsr......djang
+00004cc0: 6f2e 6462 7205 0000 00da 0b64 6a61 6e67  o.dbr......djang
+00004cd0: 6f2e 636f 6e66 7206 0000 0072 5d00 0000  o.confr....r]...
+00004ce0: da05 4d6f 6465 6c72 0900 0000 7221 0000  ..Modelr....r!..
+00004cf0: 0072 4600 0000 724d 0000 0072 4f00 0000  .rF...rM...rO...
+00004d00: 7263 0000 0072 7400 0000 727d 0000 0072  rc...rt...r}...r
+00004d10: 8900 0000 7291 0000 0072 9400 0000 7297  ....r....r....r.
+00004d20: 0000 0072 9e00 0000 72a9 0000 0072 aa00  ...r....r....r..
+00004d30: 0000 72ab 0000 0072 ad00 0000 72b1 0000  ..r....r....r...
+00004d40: 0072 b200 0000 72c4 0000 0072 c600 0000  .r....r....r....
+00004d50: 72c7 0000 0072 c800 0000 72cb 0000 0072  r....r....r....r
+00004d60: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
+00004d70: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00004d80: 0073 3e00 0000 0801 0802 0801 1001 0c01  .s>.............
+00004d90: 0c01 0c02 0406 1209 101e 101c 1014 1028  ...............(
+00004da0: 104a 121b 121b 1223 100d 1019 1011 1011  .J.....#........
+00004db0: 1011 1011 100a 100a 100a 102a 100a 100a  ...........*....
+00004dc0: 1012 1026                                ...&
```

### Comparing `base_system-0.2.4/base_system/__pycache__/serializers.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/serializers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/__pycache__/urls.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/urls.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/__pycache__/views.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/views.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May  6 02:12:59 2023 UTC, .py size: 58056 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 abb7 5564 c8e2 0000  a.........Ud....
+00000000: 610d 0d0a 0000 0000 16ba 5964 c8e2 0000  a.........Yd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1003 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6400 6404 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

### Comparing `base_system-0.2.4/base_system/__pycache__/viewsets.cpython-39.pyc` & `base_system-0.2.5/base_system/__pycache__/viewsets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/auth.py` & `base_system-0.2.5/base_system/auth.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/export_viewset.py` & `base_system-0.2.5/base_system/export_viewset.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/0001_initial.py` & `base_system-0.2.5/base_system/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/0003_alter_extragroup_hospital.py` & `base_system-0.2.5/base_system/migrations/0003_alter_extragroup_hospital.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc` & `base_system-0.2.5/base_system/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc` & `base_system-0.2.5/base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc` & `base_system-0.2.5/base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc` & `base_system-0.2.5/base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/models.py` & `base_system-0.2.5/base_system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     hospital = models.ForeignKey(
         Hospital,
         verbose_name="所属医院",
         on_delete=models.CASCADE,
     )
     birthday = models.DateField(verbose_name='出生日期', null=True, blank=True)
     # photo = models.ImageField(verbose_name="医生照片", upload_to="images/doctor", null=True, blank=True)
-    photo = models.CharField(verbose_name="医生照片", max_length=10, default='doctor_photo')
+    photo = models.CharField(verbose_name="医生照片", max_length=50, default='doctor_photo')
     describe = models.TextField(verbose_name="医生描述", null=True, blank=True)
     created_by = models.CharField(verbose_name="创建人", max_length=20, null=True, blank=True)
     updated_by = models.CharField(verbose_name="更新人", max_length=20, null=True, blank=True)
 
     is_online_consult = models.BooleanField(verbose_name="是否互联网接诊", default=True)
 
     class Meta:
@@ -299,16 +299,29 @@
         verbose_name_plural = verbose_name
         ordering = ('order_by',)
 
     def __str__(self):
         return self.name
 
 
+class ExpenseType(MedicalBaseModel):
+    """
+    费用类型
+    """
+    name = models.CharField(verbose_name="名称", max_length=64)
+    code = models.CharField(verbose_name="编码", max_length=64)
+
+    class Meta:
+        db_table = "bs_expense_type"
+        verbose_name = "费用类型"
+        verbose_name_plural = verbose_name
+
+
 class ExpenseStandard(MedicalBaseModel):
-    # 挂号费用：1、电话问诊：2、在线问诊：3
+    # 挂号费用类型1:预约挂号, 2:电话问诊, 3:在线问诊, 4:在线复诊
     expense_type = models.CharField(verbose_name="费用类型", max_length=100, null=True)
     standard_name = models.CharField(verbose_name="标准名称", max_length=100)
     standard_code = models.CharField(verbose_name="标准编码", max_length=255)
     fees = models.FloatField(verbose_name="费用", null=True)
     hospital = models.ForeignKey(
         Hospital,
         verbose_name='所属医院',
```

### Comparing `base_system-0.2.4/base_system/serializers.py` & `base_system-0.2.5/base_system/serializers.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/urls.py` & `base_system-0.2.5/base_system/urls.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/views.py` & `base_system-0.2.5/base_system/views.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system/viewsets.py` & `base_system-0.2.5/base_system/viewsets.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/base_system.egg-info/PKG-INFO` & `base_system-0.2.5/base_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: base-system
-Version: 0.2.4
+Version: 0.2.5
 Summary: Basic feature component
 Home-page: https://github.com/zcjwin
 Author: zcjwin
 Author-email: win_zcj@163.com
 License: UNKNOWN
 Keywords: base_system
 Platform: UNKNOWN
```

### Comparing `base_system-0.2.4/base_system.egg-info/SOURCES.txt` & `base_system-0.2.5/base_system.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,13 +41,16 @@
 base_system/__pycache__/urls.cpython-39.pyc
 base_system/__pycache__/views.cpython-39.pyc
 base_system/__pycache__/viewsets.cpython-39.pyc
 base_system/migrations/0001_initial.py
 base_system/migrations/0002_drugdirectory_code_medu_cur.py
 base_system/migrations/0003_alter_extragroup_hospital.py
 base_system/migrations/0004_alter_extragroup_role_name.py
+base_system/migrations/0005_expensetype.py
+base_system/migrations/0006_alter_doctor_photo.py
 base_system/migrations/__init__.py
 base_system/migrations/__pycache__/0001_initial.cpython-39.pyc
 base_system/migrations/__pycache__/0002_drugdirectory_code_medu_cur.cpython-39.pyc
 base_system/migrations/__pycache__/0003_alter_extragroup_hospital.cpython-39.pyc
 base_system/migrations/__pycache__/0004_alter_extragroup_role_name.cpython-39.pyc
+base_system/migrations/__pycache__/0005_expensetype.cpython-39.pyc
 base_system/migrations/__pycache__/__init__.cpython-39.pyc
```

### Comparing `base_system-0.2.4/init_data.json` & `base_system-0.2.5/init_data.json`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/manage.py` & `base_system-0.2.5/manage.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/requirements.txt` & `base_system-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/runtests.py` & `base_system-0.2.5/runtests.py`

 * *Files identical despite different names*

### Comparing `base_system-0.2.4/setup.py` & `base_system-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="base_system",
-    version='0.2.4',
+    version='0.2.5',
     description="Basic feature component",
     keywords='base_system',
     # long_description=README,
     long_description_content_type="text/markdown",
     author='zcjwin',
     author_email='win_zcj@163.com',
     url="https://github.com/zcjwin",
```

