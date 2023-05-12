# Comparing `tmp/django-admob-ssv-1.0.4.tar.gz` & `tmp/django_admob_ssv-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admob-ssv-1.0.4.tar", last modified: Sun Feb  2 17:41:51 2020, max compression
+gzip compressed data, was "django_admob_ssv-2.0.0.tar", max compression
```

## Comparing `django-admob-ssv-1.0.4.tar` & `django_admob_ssv-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,9 @@
-drwxr-xr-x   0 john      (1000) users      (100)        0 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/
--rw-r--r--   0 john      (1000) users      (100)     3706 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)     2183 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/README.md
-drwxr-xr-x   0 john      (1000) users      (100)        0 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/django_admob_ssv/
--rw-r--r--   0 john      (1000) users      (100)       89 2020-02-02 17:36:04.000000 django-admob-ssv-1.0.4/django_admob_ssv/__init__.py
--rw-r--r--   0 john      (1000) users      (100)      104 2020-02-02 17:34:36.000000 django-admob-ssv-1.0.4/django_admob_ssv/apps.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/django_admob_ssv/conf/
--rw-r--r--   0 john      (1000) users      (100)        2 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/django_admob_ssv/conf/__init__.py
--rw-r--r--   0 john      (1000) users      (100)      437 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/django_admob_ssv/conf/settings.py
--rw-r--r--   0 john      (1000) users      (100)       92 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/django_admob_ssv/signals.py
--rw-r--r--   0 john      (1000) users      (100)     1404 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/django_admob_ssv/utils.py
--rw-r--r--   0 john      (1000) users      (100)     1524 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/django_admob_ssv/views.py
-drwxr-xr-x   0 john      (1000) users      (100)        0 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/
--rw-r--r--   0 john      (1000) users      (100)     3706 2020-02-02 17:41:51.000000 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) users      (100)      419 2020-02-02 17:41:51.000000 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) users      (100)        1 2020-02-02 17:41:51.000000 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) users      (100)       27 2020-02-02 17:41:51.000000 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/requires.txt
--rw-r--r--   0 john      (1000) users      (100)       17 2020-02-02 17:41:51.000000 django-admob-ssv-1.0.4/django_admob_ssv.egg-info/top_level.txt
--rw-r--r--   0 john      (1000) users      (100)       38 2020-02-02 17:41:51.623024 django-admob-ssv-1.0.4/setup.cfg
--rw-r--r--   0 john      (1000) users      (100)     1387 2020-02-02 17:21:08.000000 django-admob-ssv-1.0.4/setup.py
+-rw-r--r--   0        0        0     1054 2020-02-02 17:21:08.157959 django_admob_ssv-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4692 2023-05-11 23:28:08.625387 django_admob_ssv-2.0.0/README.md
+-rw-r--r--   0        0        0       53 2023-05-10 00:50:56.437043 django_admob_ssv-2.0.0/admob_ssv/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-10 00:50:56.437043 django_admob_ssv-2.0.0/admob_ssv/apps.py
+-rw-r--r--   0        0        0      744 2023-05-12 14:01:57.966517 django_admob_ssv-2.0.0/admob_ssv/conf.py
+-rw-r--r--   0        0        0       68 2023-05-10 01:06:06.824655 django_admob_ssv-2.0.0/admob_ssv/signals.py
+-rw-r--r--   0        0        0     3665 2023-05-12 14:01:57.966517 django_admob_ssv-2.0.0/admob_ssv/views.py
+-rw-r--r--   0        0        0     1661 2023-05-12 14:02:15.096857 django_admob_ssv-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6304 1970-01-01 00:00:00.000000 django_admob_ssv-2.0.0/PKG-INFO
```

