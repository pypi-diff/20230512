# Comparing `tmp/Keg-Auth-0.7.0.tar.gz` & `tmp/Keg-Auth-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Keg-Auth-0.7.0.tar", last modified: Fri Mar  3 21:09:21 2023, max compression
+gzip compressed data, was "Keg-Auth-0.7.1.tar", last modified: Fri May 12 19:13:23 2023, max compression
```

## Comparing `Keg-Auth-0.7.0.tar` & `Keg-Auth-0.7.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/.circleci/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1049 2021-11-29 16:34:48.000000 Keg-Auth-0.7.0/.circleci/config.yml
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.0/.circleci/pytest.ini
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/Keg_Auth.egg-info/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19513 2023-03-03 21:09:21.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2754 2023-03-03 21:09:21.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/SOURCES.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-03-03 21:09:21.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/dependency_links.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-06-26 19:41:44.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/not-zip-safe
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2023-03-03 21:09:21.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/requires.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       21 2023-03-03 21:09:21.000000 Keg-Auth-0.7.0/Keg_Auth.egg-info/top_level.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      664 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/MANIFEST.in
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19513 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/PKG-INFO
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    16801 2023-03-03 21:09:01.000000 Keg-Auth-0.7.0/changelog.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2021-11-29 16:34:48.000000 Keg-Auth-0.7.0/docker-compose.yml
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/docs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      638 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/Makefile
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      799 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/make.bat
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       71 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/docs/requirements.txt
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/docs/source/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2579 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/conf.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/core.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/forms.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25041 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/docs/source/getting-started.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/grids.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      286 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/docs/source/index.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/docs/source/libs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       90 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/libs/authenticators.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/libs/decorators.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      141 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/libs/index.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/libs/navigation.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/mail.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/docs/source/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/model/entity_registry.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      129 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/model/index.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/model/utils.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/testing.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      866 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/docs/source/upgrade.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/docs/source/views.rst
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      932 2022-02-24 20:26:39.000000 Keg-Auth-0.7.0/keg_auth/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4355 2021-07-06 19:42:05.000000 Keg-Auth-0.7.0/keg_auth/cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19831 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1064 2020-04-02 13:20:21.000000 Keg-Auth-0.7.0/keg_auth/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10715 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/forms.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11025 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/keg_auth/grids.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/i18n/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      113 2018-11-14 17:28:05.000000 Keg-Auth-0.7.0/keg_auth/i18n/babel.cfg
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7041 2020-12-08 20:35:04.000000 Keg-Auth-0.7.0/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11072 2020-12-08 20:35:04.000000 Keg-Auth-0.7.0/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7561 2020-12-08 20:35:04.000000 Keg-Auth-0.7.0/keg_auth/i18n/keg_auth.pot
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/libs/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1013 2022-02-24 20:26:39.000000 Keg-Auth-0.7.0/keg_auth/libs/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    45971 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/libs/authenticators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9474 2021-11-29 16:35:52.000000 Keg-Auth-0.7.0/keg_auth/libs/decorators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9648 2022-02-22 19:50:15.000000 Keg-Auth-0.7.0/keg_auth/libs/navigation.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      404 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/keg_auth/libs/templates.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2527 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/mail.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    28459 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3901 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/keg_auth/model/entity_registry.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      226 2020-04-16 20:22:57.000000 Keg-Auth-0.7.0/keg_auth/model/types.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2474 2021-01-29 21:02:21.000000 Keg-Auth-0.7.0/keg_auth/model/utils.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/static/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/static/i18n/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/static/i18n/es/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/static/i18n/es/LC_MESSAGES/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6521 2020-12-08 20:35:04.000000 Keg-Auth-0.7.0/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.854292 Keg-Auth-0.7.0/keg_auth/templates/
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      488 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/crud-addedit.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1084 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/crud-list.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      149 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/flash-messages-only.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      369 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/forgot-password.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/i18n.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/login.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      254 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/multi-part-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1842 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/navigation.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      576 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/new-user-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      624 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/reset-password-mail.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      270 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/templates/keg-auth/set-password.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    58303 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/testing.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/keg_auth/tests/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.0/keg_auth/tests/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      639 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/tests/conftest.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4718 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/tests/test_auth_manager.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    22575 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/tests/test_authenticators.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7666 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/tests/test_cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1259 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/tests/test_core.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12787 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/tests/test_forms.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2055 2019-06-07 16:29:38.000000 Keg-Auth-0.7.0/keg_auth/tests/test_grids.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2768 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/tests/test_mail.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    30106 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/tests/test_model.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18022 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth/tests/test_navigation.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      187 2022-02-24 20:26:39.000000 Keg-Auth-0.7.0/keg_auth/tests/test_utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    58990 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/tests/test_views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2201 2022-02-24 20:26:39.000000 Keg-Auth-0.7.0/keg_auth/tests/utils.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-03-03 21:08:11.000000 Keg-Auth-0.7.0/keg_auth/version.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26051 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/keg_auth/views.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/keg_auth_ta/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.0/keg_auth_ta/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      950 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth_ta/app.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1119 2020-05-14 15:15:43.000000 Keg-Auth-0.7.0/keg_auth_ta/cli.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      987 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth_ta/config.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      986 2022-02-22 19:50:15.000000 Keg-Auth-0.7.0/keg_auth_ta/events.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      802 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth_ta/extensions.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      174 2018-08-17 20:04:26.000000 Keg-Auth-0.7.0/keg_auth_ta/grids.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/keg_auth_ta/model/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.0/keg_auth_ta/model/__init__.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1526 2020-12-08 18:33:59.000000 Keg-Auth-0.7.0/keg_auth_ta/model/entities.py
-drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/keg_auth_ta/templates/
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      813 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth_ta/templates/base-page.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      508 2021-02-02 19:57:35.000000 Keg-Auth-0.7.0/keg_auth_ta/templates/base.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      158 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/keg_auth_ta/templates/email.j2
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      442 2018-08-17 20:04:26.000000 Keg-Auth-0.7.0/keg_auth_ta/templates/home.html
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6434 2021-11-29 16:35:52.000000 Keg-Auth-0.7.0/keg_auth_ta/views.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      316 2021-11-29 16:34:48.000000 Keg-Auth-0.7.0/keg_auth_ta-config-example.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2141 2023-03-03 20:33:36.000000 Keg-Auth-0.7.0/readme.rst
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      655 2023-03-03 21:09:21.858292 Keg-Auth-0.7.0/setup.cfg
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2306 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/setup.py
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2974 2018-06-22 16:02:06.000000 Keg-Auth-0.7.0/todo.txt
--rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2036 2023-03-03 21:07:57.000000 Keg-Auth-0.7.0/tox.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.698738 Keg-Auth-0.7.1/.circleci/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1003 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/.circleci/config.yml
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/.circleci/pytest.ini
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.698738 Keg-Auth-0.7.1/Keg_Auth.egg-info/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19716 2023-05-12 19:13:22.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2754 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2023-05-12 19:13:22.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2018-06-26 19:41:44.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      439 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       21 2023-05-12 19:13:23.000000 Keg-Auth-0.7.1/Keg_Auth.egg-info/top_level.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      664 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19716 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    17004 2023-05-12 19:13:02.000000 Keg-Auth-0.7.1/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2021-11-29 16:34:48.000000 Keg-Auth-0.7.1/docker-compose.yml
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.702738 Keg-Auth-0.7.1/docs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      638 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/Makefile
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      799 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/make.bat
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       71 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/docs/requirements.txt
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.714738 Keg-Auth-0.7.1/docs/source/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2579 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/conf.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/core.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/forms.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    25041 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/getting-started.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/grids.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      286 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/index.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.722739 Keg-Auth-0.7.1/docs/source/libs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       90 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/authenticators.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/decorators.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      141 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/index.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       78 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/libs/navigation.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       55 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/mail.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.722739 Keg-Auth-0.7.1/docs/source/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       94 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/entity_registry.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      129 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/index.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/model/utils.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       64 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/testing.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      866 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/docs/source/upgrade.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/docs/source/views.rst
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.738739 Keg-Auth-0.7.1/keg_auth/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      932 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4355 2021-07-06 19:42:05.000000 Keg-Auth-0.7.1/keg_auth/cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    19831 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1064 2020-04-02 13:20:21.000000 Keg-Auth-0.7.1/keg_auth/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    10715 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/forms.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11025 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/grids.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.738739 Keg-Auth-0.7.1/keg_auth/i18n/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      113 2018-11-14 17:28:05.000000 Keg-Auth-0.7.1/keg_auth/i18n/babel.cfg
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.742739 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7041 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11072 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7561 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/i18n/keg_auth.pot
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.750739 Keg-Auth-0.7.1/keg_auth/libs/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1013 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/libs/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    45971 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/libs/authenticators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9900 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth/libs/decorators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     9648 2022-02-22 19:50:15.000000 Keg-Auth-0.7.1/keg_auth/libs/navigation.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      404 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/libs/templates.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2527 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/mail.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.754739 Keg-Auth-0.7.1/keg_auth/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    28459 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3901 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/model/entity_registry.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      226 2020-04-16 20:22:57.000000 Keg-Auth-0.7.1/keg_auth/model/types.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2474 2021-01-29 21:02:21.000000 Keg-Auth-0.7.1/keg_auth/model/utils.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/i18n/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/static/i18n/es/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.758739 Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6521 2020-12-08 20:35:04.000000 Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.686738 Keg-Auth-0.7.1/keg_auth/templates/
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.770739 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      488 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-addedit.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1084 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-list.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      149 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/flash-messages-only.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      369 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/forgot-password.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       58 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/i18n.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      453 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/login.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      254 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/multi-part-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1842 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/navigation.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      576 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/new-user-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      624 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/reset-password-mail.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      270 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/templates/keg-auth/set-password.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    58303 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/testing.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.782739 Keg-Auth-0.7.1/keg_auth/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      639 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/conftest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4718 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_auth_manager.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    22575 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_authenticators.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     7666 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1259 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_core.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12787 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/tests/test_forms.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2055 2019-06-07 16:29:38.000000 Keg-Auth-0.7.1/keg_auth/tests/test_grids.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2768 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_mail.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    30106 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_model.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    18022 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth/tests/test_navigation.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      187 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/tests/test_utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    59313 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth/tests/test_views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2201 2022-02-24 20:26:39.000000 Keg-Auth-0.7.1/keg_auth/tests/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2023-05-12 19:12:32.000000 Keg-Auth-0.7.1/keg_auth/version.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    26051 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/keg_auth/views.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.790739 Keg-Auth-0.7.1/keg_auth_ta/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth_ta/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      950 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/app.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1119 2020-05-14 15:15:43.000000 Keg-Auth-0.7.1/keg_auth_ta/cli.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      987 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/config.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      986 2022-02-22 19:50:15.000000 Keg-Auth-0.7.1/keg_auth_ta/events.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      802 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/extensions.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      174 2018-08-17 20:04:26.000000 Keg-Auth-0.7.1/keg_auth_ta/grids.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.790739 Keg-Auth-0.7.1/keg_auth_ta/model/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/keg_auth_ta/model/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1526 2020-12-08 18:33:59.000000 Keg-Auth-0.7.1/keg_auth_ta/model/entities.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2023-05-12 19:13:23.794739 Keg-Auth-0.7.1/keg_auth_ta/templates/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      813 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/base-page.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      508 2021-02-02 19:57:35.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/base.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      158 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/email.j2
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      442 2018-08-17 20:04:26.000000 Keg-Auth-0.7.1/keg_auth_ta/templates/home.html
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6999 2023-05-12 19:12:13.000000 Keg-Auth-0.7.1/keg_auth_ta/views.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      316 2021-11-29 16:34:48.000000 Keg-Auth-0.7.1/keg_auth_ta-config-example.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2141 2023-03-03 20:33:36.000000 Keg-Auth-0.7.1/readme.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      655 2023-05-12 19:13:23.798739 Keg-Auth-0.7.1/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2306 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/setup.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2974 2018-06-22 16:02:06.000000 Keg-Auth-0.7.1/todo.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2036 2023-03-03 21:07:57.000000 Keg-Auth-0.7.1/tox.ini
```

### Comparing `Keg-Auth-0.7.0/.circleci/config.yml` & `Keg-Auth-0.7.1/.circleci/config.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 version: 2
 jobs:
     build:
         docker:
-            - image: level12/python-test-multi
+            - image: level12/python-test-multi:ubuntu2004
             - image: postgres:12
               environment:
                 POSTGRES_DB: kegauth_tests
                 POSTGRES_HOST_AUTH_METHOD: trust
         steps:
             - checkout
 
             - run:
                 name: folder listing for debugging
                 command: ls -al
 
             - run:
                 name: install tox
-                command: pip install tox
+                command: python3.10 -m pip install tox
 
             - run:
                 name: version checks
                 command: |
-                    python --version
-                    pip --version
-                    virtualenv --version
+                    python3.10 --version
                     tox --version
 
             - run:
                 name: run tox
                 command: tox
 
             - store_test_results:
```

### Comparing `Keg-Auth-0.7.0/Keg_Auth.egg-info/PKG-INFO` & `Keg-Auth-0.7.1/Keg_Auth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Keg-Auth
-Version: 0.7.0
+Version: 0.7.1
 Summary: Authentication plugin for Keg
 Home-page: https://github.com/level12/keg-auth
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 - `cd keg_auth_ta`
 - `python app.py ...`
 
 
 Changelog
 =========
 
+0.7.1 released 2023-05-12
+-------------------------
+
+- allow request loaders to be specified directly to requires decorators (cd42358_)
+
+.. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
+
+
 0.7.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (88a6173_)
 - support keg testing app context changes (d0ec64f_)
 
 .. _88a6173: https://github.com/level12/keg-auth/commit/88a6173
```

### Comparing `Keg-Auth-0.7.0/Keg_Auth.egg-info/SOURCES.txt` & `Keg-Auth-0.7.1/Keg_Auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/MANIFEST.in` & `Keg-Auth-0.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/PKG-INFO` & `Keg-Auth-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Keg-Auth
-Version: 0.7.0
+Version: 0.7.1
 Summary: Authentication plugin for Keg
 Home-page: https://github.com/level12/keg-auth
 Author: Randy Syring
 Author-email: randy.syring@level12.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -84,14 +84,22 @@
 - `cd keg_auth_ta`
 - `python app.py ...`
 
 
 Changelog
 =========
 
+0.7.1 released 2023-05-12
+-------------------------
+
+- allow request loaders to be specified directly to requires decorators (cd42358_)
+
+.. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
+
+
 0.7.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (88a6173_)
 - support keg testing app context changes (d0ec64f_)
 
 .. _88a6173: https://github.com/level12/keg-auth/commit/88a6173
```

### Comparing `Keg-Auth-0.7.0/changelog.rst` & `Keg-Auth-0.7.1/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+0.7.1 released 2023-05-12
+-------------------------
+
+- allow request loaders to be specified directly to requires decorators (cd42358_)
+
+.. _cd42358: https://github.com/level12/keg-auth/commit/cd42358
+
+
 0.7.0 released 2023-03-03
 -------------------------
 
 - support SQLAlchemy 2.0 (88a6173_)
 - support keg testing app context changes (d0ec64f_)
 
 .. _88a6173: https://github.com/level12/keg-auth/commit/88a6173
```

### Comparing `Keg-Auth-0.7.0/docs/Makefile` & `Keg-Auth-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/docs/make.bat` & `Keg-Auth-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/docs/source/conf.py` & `Keg-Auth-0.7.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/docs/source/getting-started.rst` & `Keg-Auth-0.7.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/docs/source/upgrade.rst` & `Keg-Auth-0.7.1/docs/source/upgrade.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/__init__.py` & `Keg-Auth-0.7.1/keg_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/cli.py` & `Keg-Auth-0.7.1/keg_auth/cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/core.py` & `Keg-Auth-0.7.1/keg_auth/core.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/extensions.py` & `Keg-Auth-0.7.1/keg_auth/extensions.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/forms.py` & `Keg-Auth-0.7.1/keg_auth/forms.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/grids.py` & `Keg-Auth-0.7.1/keg_auth/grids.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo` & `Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.mo`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po` & `Keg-Auth-0.7.1/keg_auth/i18n/es/LC_MESSAGES/keg_auth.po`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/i18n/keg_auth.pot` & `Keg-Auth-0.7.1/keg_auth/i18n/keg_auth.pot`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/libs/__init__.py` & `Keg-Auth-0.7.1/keg_auth/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/libs/authenticators.py` & `Keg-Auth-0.7.1/keg_auth/libs/authenticators.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/libs/decorators.py` & `Keg-Auth-0.7.1/keg_auth/libs/decorators.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,22 @@
             should be the closest decorator to the method
 
         Examples:
         - @requires_user
         - @requires_user()
         - @requires_user(on_authentication_failure=lambda: flask.abort(400))
         - @requires_user(http_methods_excluded=['OPTIONS'])
+        - @requires_user(request_loaders=[JwtRequestLoader])
     """
-    def __init__(self, on_authentication_failure=None, http_methods_excluded=None):
+    def __init__(self, on_authentication_failure=None, http_methods_excluded=None,
+                 request_loaders=None):
         # defaults for these handlers are provided, but may be overridden here
         self._on_authentication_failure = on_authentication_failure
         self.http_methods_excluded = http_methods_excluded
+        self.request_loaders = request_loaders
 
     def __call__(self, class_or_function):
         # decorator may be applied to a class or a function, but the effect is different
         if inspect.isclass(class_or_function):
             if issubclass(class_or_function, flask.Blueprint):
                 return self.decorate_blueprint(class_or_function)
             return self.decorate_class(class_or_function)
@@ -123,15 +126,23 @@
 
         # if flask_login has an authenticated user in session, that's who we want
         if flask_login.current_user.is_authenticated:
             return
 
         # no user in session right now, so we need to run request loaders to see if any match
         user = None
-        for loader in flask.current_app.auth_manager.request_loaders.values():
+        all_loaders = (
+            (self.request_loaders or [])
+            + list(flask.current_app.auth_manager.request_loaders.values())
+        )
+
+        for loader in all_loaders:
+            if inspect.isclass(loader):
+                loader = loader(flask.current_app)
+
             user = loader.get_authenticated_user()
             if user:
                 break
 
         if not user or not user.is_authenticated:
             if instance and callable(getattr(instance, 'on_authentication_failure', None)):
                 instance.on_authentication_failure()
@@ -152,18 +163,19 @@
         - @requires_permissions(has_any('token1', 'token2'))
         - @requires_permissions(has_all('token1', 'token2'))
         - @requires_permissions(has_all(has_any('token1', 'token2'), 'token3'))
         - @requires_permissions(custom_authorization_callable that takes user arg)
         - @requires_permissions('token1', on_authorization_failure=lambda: flask.abort(404))
     """
     def __init__(self, condition, on_authentication_failure=None, on_authorization_failure=None,
-                 http_methods_excluded=None):
+                 http_methods_excluded=None, request_loaders=None):
         super(RequiresPermissions, self).__init__(
             on_authentication_failure=on_authentication_failure,
             http_methods_excluded=http_methods_excluded,
+            request_loaders=request_loaders,
         )
         self.condition = condition
         self._on_authorization_failure = on_authorization_failure
 
     def store_auth_info(self, obj):
         super(RequiresPermissions, self).store_auth_info(obj)
         condition = self.condition
```

### Comparing `Keg-Auth-0.7.0/keg_auth/libs/navigation.py` & `Keg-Auth-0.7.1/keg_auth/libs/navigation.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/mail.py` & `Keg-Auth-0.7.1/keg_auth/mail.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/model/__init__.py` & `Keg-Auth-0.7.1/keg_auth/model/__init__.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/model/entity_registry.py` & `Keg-Auth-0.7.1/keg_auth/model/entity_registry.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/model/utils.py` & `Keg-Auth-0.7.1/keg_auth/model/utils.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json` & `Keg-Auth-0.7.1/keg_auth/static/i18n/es/LC_MESSAGES/keg_auth.json`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/templates/keg-auth/crud-list.html` & `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/crud-list.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/templates/keg-auth/navigation.html` & `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/navigation.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/templates/keg-auth/new-user-mail.j2` & `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/new-user-mail.j2`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/templates/keg-auth/reset-password-mail.j2` & `Keg-Auth-0.7.1/keg_auth/templates/keg-auth/reset-password-mail.j2`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/testing.py` & `Keg-Auth-0.7.1/keg_auth/testing.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/conftest.py` & `Keg-Auth-0.7.1/keg_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_auth_manager.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_auth_manager.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_authenticators.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_cli.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_core.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_forms.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_grids.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_mail.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_model.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_navigation.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_navigation.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/test_views.py` & `Keg-Auth-0.7.1/keg_auth/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -570,14 +570,23 @@
         token = jwt_auth.create_access_token(user)
 
         client = flask_webtest.TestApp(flask.current_app)
         client.set_authorization(('Bearer', token))
         resp = client.get('/jwt-required', status=200)
         assert resp.text == 'jwt-required'
 
+    def test_per_endpoint_loader(self):
+        ents.User.fake()
+
+        client = flask_webtest.TestApp(flask.current_app)
+        resp = client.get('/custom-loader-denied', status=302)
+        assert resp.location.startswith('/login')
+        resp = client.get('/custom-loader-letmein')
+        assert resp.text == 'ok'
+
 
 class TestUserCrud(ViewTestBase):
     permissions = 'auth-manage'
 
     def test_add(self):
         perm_approve = ents.Permission.fake()
         ents.Permission.fake()
```

### Comparing `Keg-Auth-0.7.0/keg_auth/tests/utils.py` & `Keg-Auth-0.7.1/keg_auth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth/views.py` & `Keg-Auth-0.7.1/keg_auth/views.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/app.py` & `Keg-Auth-0.7.1/keg_auth_ta/app.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/cli.py` & `Keg-Auth-0.7.1/keg_auth_ta/cli.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/config.py` & `Keg-Auth-0.7.1/keg_auth_ta/config.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/events.py` & `Keg-Auth-0.7.1/keg_auth_ta/events.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/extensions.py` & `Keg-Auth-0.7.1/keg_auth_ta/extensions.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/model/entities.py` & `Keg-Auth-0.7.1/keg_auth_ta/model/entities.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/templates/base-page.html` & `Keg-Auth-0.7.1/keg_auth_ta/templates/base-page.html`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/keg_auth_ta/views.py` & `Keg-Auth-0.7.1/keg_auth_ta/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 import flask
 import flask_login
 import keg.web
 
 from keg_auth import make_blueprint, requires_permissions, requires_user, has_any, has_all
 from keg_auth.forms import user_form
+from keg_auth.libs.authenticators import RequestLoader
 from keg_auth.views import User as UserBase
 from keg_auth_ta.extensions import csrf, auth_manager
+from keg_auth_ta.model import entities as ents
 
 log = logging.getLogger(__name__)
 
 
 @requires_permissions('permission1')
 class ProtectedBlueprint(flask.Blueprint):
     def on_authentication_failure(self):
@@ -253,7 +255,25 @@
     return 'custom-auth-failure'
 
 
 @private_bp.route('/custom-perm-failure')
 @requires_permissions('permission1', on_authorization_failure=lambda: flask.abort(400))
 def custom_perm_failure():
     return 'custom-perm-failure'
+
+
+class CustomRequestLoader(RequestLoader):
+    def get_authenticated_user(self):
+        if 'letmein' in flask.request.endpoint:
+            return ents.User.query.first()
+
+
+@private_bp.route('/custom-loader-denied')
+@requires_user(request_loaders=[CustomRequestLoader])
+def custom_loader_denied():
+    return 'fail'
+
+
+@private_bp.route('/custom-loader-letmein')
+@requires_user(request_loaders=[CustomRequestLoader])
+def custom_loader_letmein():
+    return 'ok'
```

### Comparing `Keg-Auth-0.7.0/readme.rst` & `Keg-Auth-0.7.1/readme.rst`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/setup.cfg` & `Keg-Auth-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/setup.py` & `Keg-Auth-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/todo.txt` & `Keg-Auth-0.7.1/todo.txt`

 * *Files identical despite different names*

### Comparing `Keg-Auth-0.7.0/tox.ini` & `Keg-Auth-0.7.1/tox.ini`

 * *Files identical despite different names*

