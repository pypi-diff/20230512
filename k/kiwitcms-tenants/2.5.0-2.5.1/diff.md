# Comparing `tmp/kiwitcms-tenants-2.5.0.tar.gz` & `tmp/kiwitcms-tenants-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-tenants-2.5.0.tar", last modified: Thu Feb  9 23:27:35 2023, max compression
+gzip compressed data, was "kiwitcms-tenants-2.5.1.tar", last modified: Fri May 12 10:02:53 2023, max compression
```

## Comparing `kiwitcms-tenants-2.5.0.tar` & `kiwitcms-tenants-2.5.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.0/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.0/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    15652 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    14915 2023-02-09 23:26:33.000000 kiwitcms-tenants-2.5.0/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.355552 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    15652 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     1899 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       52 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       22 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       45 2023-02-09 23:27:35.000000 kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       22 2023-02-09 22:42:12.000000 kiwitcms-tenants-2.5.0/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)       70 2023-02-09 23:27:35.361552 kiwitcms-tenants-2.5.0/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1639 2023-02-09 23:26:33.000000 kiwitcms-tenants-2.5.0/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.355552 kiwitcms-tenants-2.5.0/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.0/tcms_settings_dir/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2455 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.0/tcms_settings_dir/multi_tenant.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.357551 kiwitcms-tenants-2.5.0/tcms_tenants/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.5.0/tcms_tenants/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     7410 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.0/tcms_tenants/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.5.0/tcms_tenants/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      713 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.0/tcms_tenants/backends.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      628 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/checks.py
--rw-r--r--   0 senko     (1001) senko     (1001)      821 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.0/tcms_tenants/context_processors.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     3133 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/forms.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.353551 kiwitcms-tenants-2.5.0/tcms_tenants/locale/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.353551 kiwitcms-tenants-2.5.0/tcms_tenants/locale/en/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.357551 kiwitcms-tenants-2.5.0/tcms_tenants/locale/en/LC_MESSAGES/
--rw-r--r--   0 senko     (1001) senko     (1001)     4016 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.0/tcms_tenants/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 senko     (1001) senko     (1001)      711 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/menu.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2323 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/middleware.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.358552 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/
--rw-rw-r--   0 senko     (1001) senko     (1001)     2394 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      617 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0002_tenant_owner.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      596 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0003_use_datetime_fields.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      434 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0004_tenant_organization.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.0/tcms_tenants/migrations/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1350 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/models.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1181 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/oss_utils.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1439 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/storage.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.353551 kiwitcms-tenants-2.5.0/tcms_tenants/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.358552 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.359552 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/email/new.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      904 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/invite_users.html
--rw-r--r--   0 senko     (1001) senko     (1001)     3614 2023-02-09 21:48:12.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/new.html
--rw-r--r--   0 senko     (1001) senko     (1001)      295 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/tenant_name.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.359552 kiwitcms-tenants-2.5.0/tcms_tenants/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.0/tcms_tenants/templatetags/tcms_tenants.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.359552 kiwitcms-tenants-2.5.0/tcms_tenants/tests/
--rw-rw-r--   0 senko     (1001) senko     (1001)     3990 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/tests/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.359552 kiwitcms-tenants-2.5.0/tcms_tenants/tests/__pycache__/
--rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.5.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 senko     (1001) senko     (1001)      599 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/urls.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     7972 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.0/tcms_tenants/utils.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     5408 2022-11-14 20:30:28.000000 kiwitcms-tenants-2.5.0/tcms_tenants/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/tenant_groups/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.0/tenant_groups/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.5.0/tenant_groups/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.0/tenant_groups/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1414 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.0/tenant_groups/backends.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      722 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.0/tenant_groups/checks.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/tenant_groups/management/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.5.0/tenant_groups/management/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/tenant_groups/management/commands/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.5.0/tenant_groups/management/commands/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1396 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.0/tenant_groups/management/commands/refresh_tenant_permissions.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-02-09 23:27:35.360551 kiwitcms-tenants-2.5.0/tenant_groups/migrations/
--rw-rw-r--   0 senko     (1001) senko     (1001)     4132 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.0/tenant_groups/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.0/tenant_groups/migrations/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     1333 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.0/tenant_groups/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.226815 kiwitcms-tenants-2.5.1/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.1/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.1/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    15804 2023-05-12 10:02:53.227815 kiwitcms-tenants-2.5.1/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    15067 2023-05-12 10:02:16.000000 kiwitcms-tenants-2.5.1/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.222815 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    15804 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     1899 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       52 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       22 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       45 2023-05-12 10:02:53.000000 kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       22 2023-05-12 09:05:15.000000 kiwitcms-tenants-2.5.1/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)       70 2023-05-12 10:02:53.227815 kiwitcms-tenants-2.5.1/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1639 2023-05-12 10:02:16.000000 kiwitcms-tenants-2.5.1/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.223815 kiwitcms-tenants-2.5.1/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.1/tcms_settings_dir/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2455 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.1/tcms_settings_dir/multi_tenant.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.224815 kiwitcms-tenants-2.5.1/tcms_tenants/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.5.1/tcms_tenants/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     7410 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.1/tcms_tenants/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.5.1/tcms_tenants/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      713 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.1/tcms_tenants/backends.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      628 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/checks.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      821 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.1/tcms_tenants/context_processors.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     3133 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/forms.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.218814 kiwitcms-tenants-2.5.1/tcms_tenants/locale/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.218814 kiwitcms-tenants-2.5.1/tcms_tenants/locale/en/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.224815 kiwitcms-tenants-2.5.1/tcms_tenants/locale/en/LC_MESSAGES/
+-rw-r--r--   0 senko     (1001) senko     (1001)     4016 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.1/tcms_tenants/locale/en/LC_MESSAGES/django.po
+-rw-rw-r--   0 senko     (1001) senko     (1001)      711 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/menu.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2323 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/middleware.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2394 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      617 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0002_tenant_owner.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      596 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0003_use_datetime_fields.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      434 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0004_tenant_organization.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.1/tcms_tenants/migrations/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1350 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/models.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1133 2023-05-12 09:05:15.000000 kiwitcms-tenants-2.5.1/tcms_tenants/oss_utils.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1439 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/storage.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.219814 kiwitcms-tenants-2.5.1/tcms_tenants/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/email/new.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      904 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/invite_users.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     3614 2023-02-09 21:48:12.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/new.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      295 2023-02-09 20:21:54.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/tenant_name.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.5.1/tcms_tenants/templatetags/tcms_tenants.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/tests/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     3990 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/tests/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.225815 kiwitcms-tenants-2.5.1/tcms_tenants/tests/__pycache__/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.5.1/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 senko     (1001) senko     (1001)      599 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/urls.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     7972 2022-11-14 20:17:08.000000 kiwitcms-tenants-2.5.1/tcms_tenants/utils.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     5408 2022-11-14 20:30:28.000000 kiwitcms-tenants-2.5.1/tcms_tenants/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.226815 kiwitcms-tenants-2.5.1/tenant_groups/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.1/tenant_groups/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.5.1/tenant_groups/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.1/tenant_groups/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1414 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.1/tenant_groups/backends.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      722 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.1/tenant_groups/checks.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.226815 kiwitcms-tenants-2.5.1/tenant_groups/management/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.5.1/tenant_groups/management/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.226815 kiwitcms-tenants-2.5.1/tenant_groups/management/commands/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.5.1/tenant_groups/management/commands/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1396 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.1/tenant_groups/management/commands/refresh_tenant_permissions.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2023-05-12 10:02:53.226815 kiwitcms-tenants-2.5.1/tenant_groups/migrations/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     4132 2022-10-25 12:32:42.000000 kiwitcms-tenants-2.5.1/tenant_groups/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.5.1/tenant_groups/migrations/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     1333 2022-09-10 17:52:07.000000 kiwitcms-tenants-2.5.1/tenant_groups/models.py
```

### Comparing `kiwitcms-tenants-2.5.0/LICENSE` & `kiwitcms-tenants-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/PKG-INFO` & `kiwitcms-tenants-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-tenants
-Version: 2.5.0
+Version: 2.5.1
 Summary: Multi-tenant support for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/tenants/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -139,14 +139,21 @@
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
 Changelog
 ---------
 
+v2.5.1 (12 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Update to django-tenants==3.5.0
+- Replace ``form_errors_to_list()`` which was removed in Kiwi TCMS v12.2
+
+
 v2.5.0 (10 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update to django-tenants==3.4.8
 - Bug fix on Create Tenant page for Kiwi TCMS v11.7 or later
```

### Comparing `kiwitcms-tenants-2.5.0/README.rst` & `kiwitcms-tenants-2.5.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,21 @@
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
 Changelog
 ---------
 
+v2.5.1 (12 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Update to django-tenants==3.5.0
+- Replace ``form_errors_to_list()`` which was removed in Kiwi TCMS v12.2
+
+
 v2.5.0 (10 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update to django-tenants==3.4.8
 - Bug fix on Create Tenant page for Kiwi TCMS v11.7 or later
```

### Comparing `kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/PKG-INFO` & `kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-tenants
-Version: 2.5.0
+Version: 2.5.1
 Summary: Multi-tenant support for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/tenants/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Framework :: Django
@@ -139,14 +139,21 @@
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
 Changelog
 ---------
 
+v2.5.1 (12 May 2023)
+~~~~~~~~~~~~~~~~~~~~
+
+- Update to django-tenants==3.5.0
+- Replace ``form_errors_to_list()`` which was removed in Kiwi TCMS v12.2
+
+
 v2.5.0 (10 Feb 2023)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Update to django-tenants==3.4.8
 - Bug fix on Create Tenant page for Kiwi TCMS v11.7 or later
```

### Comparing `kiwitcms-tenants-2.5.0/kiwitcms_tenants.egg-info/SOURCES.txt` & `kiwitcms-tenants-2.5.1/kiwitcms_tenants.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/setup.py` & `kiwitcms-tenants-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name='kiwitcms-tenants',
-    version='2.5.0',
+    version='2.5.1',
     description='Multi-tenant support for Kiwi TCMS',
     long_description=get_long_description(),
     author='Kiwi TCMS',
     author_email='info@kiwitcms.org',
     url='https://github.com/kiwitcms/tenants/',
     license='GPLv3+',
     install_requires=get_install_requires('requirements.txt'),
```

### Comparing `kiwitcms-tenants-2.5.0/tcms_settings_dir/multi_tenant.py` & `kiwitcms-tenants-2.5.1/tcms_settings_dir/multi_tenant.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/admin.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/backends.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/backends.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/checks.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/context_processors.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/context_processors.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/forms.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/forms.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/locale/en/LC_MESSAGES/django.po` & `kiwitcms-tenants-2.5.1/tcms_tenants/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/menu.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/menu.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/middleware.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/middleware.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0001_initial.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0002_tenant_owner.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0002_tenant_owner.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0003_use_datetime_fields.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0003_use_datetime_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/models.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/models.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/oss_utils.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/oss_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# Copyright (c) 2019-2022 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 import datetime
 
 from django.contrib.auth import get_user_model
-from tcms.core.utils import form_errors_to_list
 
 from tcms_tenants.forms import NewTenantForm
 from tcms_tenants.utils import create_tenant
 
 
 def create_oss_tenant(owner, name, schema_name, organization):
     """
@@ -32,8 +31,8 @@
         'organization': organization,
         'publicly_readable': False,
         'paid_until': datetime.datetime(2999, 12, 31),
     })
     if form.is_valid():
         return create_tenant(form, request)
 
-    raise RuntimeError(form_errors_to_list(form))
+    raise RuntimeError(list(form.errors.items()))
```

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/storage.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/storage.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/invite_users.html` & `kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/invite_users.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/templates/tcms_tenants/new.html` & `kiwitcms-tenants-2.5.1/tcms_tenants/templates/tcms_tenants/new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/tests/__init__.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc` & `kiwitcms-tenants-2.5.1/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/urls.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/utils.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tcms_tenants/views.py` & `kiwitcms-tenants-2.5.1/tcms_tenants/views.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/admin.py` & `kiwitcms-tenants-2.5.1/tenant_groups/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/backends.py` & `kiwitcms-tenants-2.5.1/tenant_groups/backends.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/checks.py` & `kiwitcms-tenants-2.5.1/tenant_groups/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/management/commands/refresh_tenant_permissions.py` & `kiwitcms-tenants-2.5.1/tenant_groups/management/commands/refresh_tenant_permissions.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/migrations/0001_initial.py` & `kiwitcms-tenants-2.5.1/tenant_groups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.5.0/tenant_groups/models.py` & `kiwitcms-tenants-2.5.1/tenant_groups/models.py`

 * *Files identical despite different names*

