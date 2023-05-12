# Comparing `tmp/sloth-framework-0.1.3.tar.gz` & `tmp/sloth-framework-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.3.tar", last modified: Mon Apr 24 10:11:30 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.4.tar", last modified: Fri May 12 09:17:15 2023, max compression
```

## Comparing `sloth-framework-0.1.3.tar` & `sloth-framework-0.1.4.tar`

### file list

```diff
@@ -1,295 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    37193 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18644 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.965579 sloth-framework-0.1.3/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.969580 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.973580 sloth-framework-0.1.3/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/bootstrap.bundle.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/actions/show_icons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.977580 sloth-framework-0.1.3/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/queryset/timeline.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.961579 sloth-framework-0.1.3/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.981580 sloth-framework-0.1.3/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/documents/document.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.985580 sloth-framework-0.1.3/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21329 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38221 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/valueset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-24 10:11:26.000000 sloth-framework-0.1.3/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:11:30.989580 sloth-framework-0.1.3/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 10:11:30.000000 sloth-framework-0.1.3/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16195 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.262873 sloth-framework-0.1.4/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.266873 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/bootstrap.bundle.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.270872 sloth-framework-0.1.4/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/actions/show_icons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.258872 sloth-framework-0.1.4/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.274872 sloth-framework-0.1.4/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/documents/document.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21661 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41705 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20156 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.278873 sloth-framework-0.1.4/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-12 09:17:10.000000 sloth-framework-0.1.4/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:17:15.282873 sloth-framework-0.1.4/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 09:17:15.000000 sloth-framework-0.1.4/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.3/PKG-INFO` & `sloth-framework-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.3
+Version: 0.1.4
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.3/setup.py` & `sloth-framework-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.3/sloth/Dockerfile` & `sloth-framework-0.1.4/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/__init__.py` & `sloth-framework-0.1.4/sloth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,9 +122,9 @@
 
 
 ModelBase.__new__ = __new__
 models.QuerySet = QuerySet
 models.Manager = Manager
 
 setattr(options, 'DEFAULT_NAMES', options.DEFAULT_NAMES + (
-    'icon', 'fieldsets', 'select_template', 'select_fields', 'search_fields', 'autouser'
+    'icon', 'fieldsets', 'edit_fieldsets', 'select_template', 'select_fields', 'search_fields', 'autouser'
 ))
```

### Comparing `sloth-framework-0.1.3/sloth/__main__.py` & `sloth-framework-0.1.4/sloth/__main__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/actions/__init__.py` & `sloth-framework-0.1.4/sloth/actions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import traceback
 from copy import deepcopy
 from decimal import Decimal
 from functools import lru_cache
 
 from django.apps import apps
 from django.contrib import messages
+from django.db import transaction
 from django.forms.models import ModelFormMetaclass
 from django.forms import *
 from .fields import *
 from django.http import HttpResponse, HttpResponseRedirect
 from django.template.loader import render_to_string
 from django.utils.safestring import mark_safe
 from django.utils.text import slugify
@@ -74,14 +75,22 @@
         ACTIONS[name] = cls
         ACTIONS[to_snake_case(name)] = cls
         if 'ActionView' in [k.__name__ for k in bases]:
             EXPOSE.append(to_snake_case(name))
         return cls
 
 
+class DecimalField(forms.DecimalField):
+    def clean(self, value):
+        if value:
+            value = value.replace('.', '').replace(',', '.')
+        value = super().clean(value)
+        return value
+
+
 class RegionalDateWidget(DateInput):
     input_type = 'date'
 
     def render(self, name, value, attrs=None, renderer=None):
         if isinstance(value, datetime.date):
             value = value.isoformat()
         attrs = attrs or {}
@@ -119,14 +128,17 @@
         self.on_change_data = dict(show=[], hide=[], set=[], show_fieldset=[], hide_fieldset=[])
 
         if forms.ModelForm in self.__class__.__bases__:
             self.instance = kwargs.get('instance', None)
         else:
             self.instance = kwargs.pop('instance', None)
 
+        if self.instance is None and self.instances is not None and self.instances.exists():
+            self.instance = self.instances.first()
+
         if self.has_url_posted_data():
             for k in self.request.GET:
                 if k.startswith('post__'):
                     if 'data' not in kwargs:
                         kwargs['data'] = {}
                     kwargs['data'][k.split('__')[-1]] = self.request.GET[k]
 
@@ -169,34 +181,31 @@
                     pks = list(field.queryset.filter(**{field.username_lookup: self.request.user}).values_list('pk', flat=True)[0:2])
                     if len(pks) == 1:
                         field.queryset = field.queryset.model.objects.filter(pk=pks[0])
                         field.initial = pks[0]
                         field.widget = forms.HiddenInput()
                 else:
                     field.queryset = field.queryset.contextualize(self.request).apply_role_lookups(self.request.user)
-            if hasattr(field, 'picker'):
-                grouper = field.picker if isinstance(field.picker, str) else None
-                if isinstance(field, forms.ModelMultipleChoiceField):
-                    field.widget = inputs.MultiplePickInput(field.queryset, grouper=grouper)
-                else:
-                    field.widget = inputs.PickInput(field.queryset, grouper=grouper)
 
         self.response = {}
         self.fieldsets = {}
         self.one_to_one = {}
         self.one_to_many = {}
 
         confirmation = self.requires_confirmation()
         if confirmation:
             help_text = confirmation if isinstance(confirmation, str) else ''
             self.fields['confirmation'] = forms.BooleanField(
                 label='', initial='on', required=False, help_text=help_text,
                 widget=forms.HiddenInput()
             )
 
+    def render(self, template_name, **context):
+        return HttpResponse(render_to_string([template_name], context, request=self.request))
+
     def get_verbose_name(self):
         return self.get_metadata().get('name')
 
     def get_image(self):
         return self.get_metadata().get('image')
 
     def has_url_posted_data(self):
@@ -401,14 +410,21 @@
             if field_list:
                 self.fieldsets[title] = field_list
 
     def get_api_params(self):
         return to_api_params(self.fields.items())
 
     def save(self, *args, **kwargs):
+        if hasattr(self.instance, '__roles__'):
+            with transaction.atomic():
+                self._save()
+        else:
+            self._save()
+
+    def _save(self, *args, **kwargs):
 
         if hasattr(self.instance, 'pre_save'):
             self.instance.pre_save()
 
         # save one-to-one fields
         for name in self.one_to_one:
             instance = getattr(self.instance, name)
@@ -526,15 +542,15 @@
         return metadata
 
     def get_method(self):
         return getattr(self.metaclass, 'method', 'post') if hasattr(self, 'Meta') else 'post'
 
     def get_instances(self):
         if self.instance:
-            return [self.instance]
+            return type(self.instance).objects.filter(pk=self.instance.pk)
         elif self.instances is not None:
             return self.instances
         elif self.queryset is not None:
             return self.queryset
         return []
 
     def is_modal(self):
@@ -613,14 +629,32 @@
             if getattr(field.widget, 'rmask', None):
                 classes.append('masked-input')
                 field.widget.attrs['data-reverse'] = 'true'
                 field.widget.attrs['data-mask'] = getattr(field.widget, 'rmask')
             if getattr(field.widget, 'formatted', False):
                 classes.append('html-input')
 
+            if hasattr(field, 'picker'):
+                grouper = field.picker if isinstance(field.picker, str) else None
+                if isinstance(field, forms.ModelMultipleChoiceField):
+                    field.widget = inputs.MultiplePickInput(field.queryset, grouper=grouper)
+                else:
+                    field.widget = inputs.PickInput(field.queryset, grouper=grouper)
+
+            if getattr(field, 'addable', False):
+                has_permission = field.queryset.model().has_add_permission(self.request.user)
+                has_permission = has_permission or field.queryset.model().has_permission(self.request.user)
+                help_text = '<div>{}</div>'.format(field.help_text) if field.help_text else ''
+                link = '<a style="text-decoration:none" class="popup" href="/app/{}/{}/add/">Adicionar</a>'.format(
+                    field.queryset.model.metaclass().app_label, field.queryset.model.metaclass().model_name
+                )
+                help_text = '<div style="float:right">{}</div>'.format(link) + help_text
+                if has_permission:
+                    field.help_text = help_text
+
             field.widget.attrs['class'] = ' '.join(classes)
         return mark_safe(
             render_to_string(
                 ['dashboard/form.html'], dict(
                     self=self, fieldsets=self.fieldsets
                 ),
                 request=self.request
@@ -715,31 +749,30 @@
 
         return output
 
     def is_valid(self):
         if self.asynchronous:
             return False
         self.check_ouput(self.view())
-        for field in self.fields.values():
-            if isinstance(field, forms.DecimalField):
-                field.clean = lambda v: v.replace('.', '').replace(',', '.')
         self.load_fieldsets()
         if 'action_choices' in self.request.GET:
             raise JsonReadyResponseException(
                 self.choices(self.request.GET['action_choices'], q=self.request.GET.get('term'))
             )
         if 'on_change_field' in self.request.POST:
             for data in self.on_change_data.values():
                 data.clear()
             field_name = self.request.POST['on_change_field']
             value = self.request.POST.get('on_change_value')
             if value == 'true':
                 value = True
             if value == 'false':
                 value = False
+            if value == 'unknown':
+                value = None
             getattr(self, 'on_{}_change'.format(field_name))(value)
             raise JsonReadyResponseException(self.on_change_data)
         return super().is_valid()
 
     def choices(self, field_name, q=None):
         field = self.fields[field_name]
         attr = getattr(self, 'get_{}_queryset'.format(field_name), None)
@@ -781,16 +814,17 @@
         else:
             self.redirect('/app/api/task/{}/'.format(task.task_id))
 
     def submit(self):
         if self.instances:
             for instance in self.instances:
                 self.instance = instance
-                self._post_clean()
-                self.save()
+                if self.has_permission(self.request.user):
+                    self._post_clean()
+                    self.save()
         else:
             self.save()
         self.message()
         self.redirect()
 
     def process(self):
         try:
```

### Comparing `sloth-framework-0.1.3/sloth/actions/fields.py` & `sloth-framework-0.1.4/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/actions/inputs.py` & `sloth-framework-0.1.4/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/__init__.py` & `sloth-framework-0.1.4/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/actions.py` & `sloth-framework-0.1.4/sloth/api/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
     def view(self):
         self.request.session.clear()
         auth.logout(self.request)
         self.redirect('/')
 
     def has_permission(self, user):
-        return user.is_authenticated
+        return True
 
 
 class Activate2fAuthentication(actions.Action):
     code = actions.CharField(label='Código')
 
     class Meta:
         modal = True
```

### Comparing `sloth-framework-0.1.3/sloth/api/backends/__init__.py` & `sloth-framework-0.1.4/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/dashboard.py` & `sloth-framework-0.1.4/sloth/api/dashboard.py`

 * *Files 21% similar despite different names*

```diff
@@ -130,22 +130,22 @@
                                 label = '{} {}'.format(label, qs.get_attr_metadata(subset)[0])
                             url = cls.get_list_url('/app', subset)
                             if key == 'plus':
                                 url = '{}{}/'.format(url, 'add')
                             for item in self.data[key]:
                                 add_item = add_item and not item['url'] == url
                             if add_item:
-                                self.data[key].append(
-                                    dict(
-                                        url=url, label=label, modal=modal or key == 'plus',
-                                        count=cls.objects.all().apply_role_lookups(self.request.user).count() if count else None,
-                                        icon=getattr(cls.metaclass(), 'icon', None),
-                                        app=app
-                                    )
+                                new_item = dict(
+                                    url=url, label=label, modal=modal or key == 'plus',
+                                    count=cls.objects.all().apply_role_lookups(self.request.user).count() if count else None,
+                                    icon=getattr(cls.metaclass(), 'icon', None),
+                                    app=app
                                 )
+                                self.data[key].append(new_item)
+                                return new_item
 
     def _item(self, key, url, label, icon, count=None, app=None):
         self.data[key].append(
             dict(url=url, label=label, count=count, icon=icon, app=app)
         )
 
     def info(self, *items, app=None):
@@ -153,19 +153,18 @@
 
     def warning(self, *items, app=None):
         self._load('warning', items, app=app)
 
     def search_menu(self, *items, app=None):
         self._load('search', items, app=app)
 
-    def menu(self, *items, app=None):
-        if mobile(self.request):
-            self._load('search', items, app=app)
-        else:
-            self._load('menu', items, app=app)
+    def menu(self, *items, app=None, hierarchy=None, icon=None):
+        item = self._load('menu', items, app=app)
+        if item:
+            item.update(hierarchy=hierarchy, menu_icon=icon)
 
     def top_menu(self, *items, modal=False, app=None):
         self._load('links', items, modal=modal, app=app)
 
     def add_link(self, url, label, app=None):
         self._item('links', url, label, app=app)
 
@@ -340,7 +339,56 @@
                 url = '/app/{}/{}/'.format(app_label, model_name)
                 add_item = True
                 for item in self.data['search']:
                     add_item = add_item and not item['url'] == url
                 if add_item:
                     item = dict(label=pretty(str(model_verbose_name_plural)), description=None, url=url, icon=icon, subitems=[], app=None)
                     self.data['search'].append(item)
+
+    def render_menu(self):
+        icons = {}
+        default_icon = 'record2'
+        def create_submenu(hierarchy, item, level=0):
+            tokens = item['hierarchy'].split('::')
+            if len(tokens) == 1:
+                if level == 0:
+                    icons[tokens[0]] = item['menu_icon'] or item['icon'] or default_icon
+                if tokens[0] not in hierarchy:
+                    hierarchy[tokens[0]] = {}
+                hierarchy[tokens[0]][item['label']] = item
+            else:
+                if level == 0:
+                    icons[tokens[0]] = item['menu_icon'] or default_icon
+                if tokens[0] in hierarchy:
+                    submenu = hierarchy[tokens[0]]
+                else:
+                    submenu = {}
+                    hierarchy[tokens[0]] = submenu
+                item['hierarchy'] = '::'.join(tokens[1:])
+                create_submenu(submenu, item, level+1)
+
+        menu = {}
+        for item in self.data['menu']:
+            if item['hierarchy']:
+                create_submenu(menu, item)
+            else:
+                menu[item['label']] = item
+                icons[item['label']] = item['icon'] or 'record-circle'
+
+        html = []
+        def append_html(label, item, level=0):
+            ident = '\t' * level
+            nbsp = '&nbsp;' * level * 3
+            html.append('{}<li>'.format(ident))
+            icon = '<i class="bi bi-{} menu-item-icon"></i> '.format(icons[label]) if level == 0 else ''
+            if 'url' in item:
+                html.append('{}\t<a href="{}">{}{}{}</a>'.format(ident, item['url'], icon, nbsp, item['label']))
+            else:
+                html.append('{}\t<a href="javascript:">{}{}{}<i class="bi bi-chevron-down chevron"></i></a>'.format(ident, icon, nbsp, label))
+                html.append('{}<ul>'.format(ident))
+                for sublabel, subitem in item.items():
+                    append_html(sublabel, subitem, level+1)
+                html.append('{}</ul>'.format(ident))
+            html.append('{}</li>'.format(ident))
+        for label, item in menu.items():
+            append_html(label, item, 0)
+        return mark_safe('\n'.join(html))
```

### Comparing `sloth-framework-0.1.3/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.4/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/management/commands/query.py` & `sloth-framework-0.1.4/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.4/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.4/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.4/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.4/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.4/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.4/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.4/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.4/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.4/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.4/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.4/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.4/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.4/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.4/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.4/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.4/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.4/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/models.py` & `sloth-framework-0.1.4/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.4/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.4/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.4/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.4/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.4/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.4/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.4/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.4/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.4/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.4/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.4/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.4/sloth/api/static/css/sloth.css`

 * *Files 2% similar despite different names*

```diff
@@ -200,20 +200,26 @@
 .search-and-filters input[type="text"] {
     max-width: 100%;
     width: 100%;
 }
 .search-and-filters .submit-panel{
     padding-top: 24px;
 }
-.queryset .nav-item.selected{
-   border-bottom-color: #1351b4;
+.queryset .nav-item.mobile{
+   width: 100%;
 }
-.queryset .nav-item{
+.queryset .nav-item:not(.mobile){
     border-bottom: solid 3px #EEE;
 }
+.queryset .nav-item.mobile.selected{
+   border: solid 1px #1351b4;
+}
+.queryset .nav-item.selected{
+   border-bottom-color: #1351b4;
+}
 .queryset .search-and-filters form{
     width: 100%;
 }
 .queryset .search-and-filters-controls a{
     text-decoration: none;
 }
 .queryset .search-and-filters-controls{
@@ -243,18 +249,18 @@
     min-height: 70vh;
 }
 
 main > .row > .col{
     padding:0px;
 }
 
-.select2-container--default .select2-selection--single{
+.select2-container--default .select2-selection--single,
+.select2-container--default .select2-selection--multiple{
     height: 38px;
     padding-top: 3px;
-
     border-color: #ced4da !important;
 }
 .select2-container--open {
     z-index: 9999999;
 }
 .select2-selection__arrow{
     margin: 5px;
@@ -300,14 +306,17 @@
     display: inline-block;
     margin-bottom: 10px;
     vertical-align: top;
 }
 .form-field label.required{
     font-weight: bold;
 }
+.form-field help{
+    font-
+}
 .form-submit{
     float: right;
     width: 100%;
     text-align: right;
 }
 .responsive-container > div{
     display: inline-block;
```

### Comparing `sloth-framework-0.1.3/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.4/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.4/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/click.png` & `sloth-framework-0.1.4/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/hand.png` & `sloth-framework-0.1.4/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/icon.png` & `sloth-framework-0.1.4/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.4/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.4/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.4/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.4/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/logo.png` & `sloth-framework-0.1.4/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.4/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.4/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.4/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/images/user.png` & `sloth-framework-0.1.4/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/api.js` & `sloth-framework-0.1.4/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.4/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.4/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.4/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.4/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.4/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.4/sloth/api/static/js/sloth.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -60,35 +60,51 @@
             $('main').html(html).initialize();
         });
     },
     popup: function(url, method, data) {
         $('.alert-dismissible').hide();
         if (url.indexOf('?') > 0) url = url += '&modal=1'
         else url += '?modal=1'
+
+        if (window['POPUP_STACK'] == null) {
+            window['POPUP_STACK'] = [];
+            $('#modal').on('hidden.bs.modal', function(e) {
+                if (window['POPUP_STACK'].length > 0) {
+                    $('#modal .modal-body').replaceWith(window['POPUP_STACK'].pop().initialize());
+                    $('#modal').modal('show');
+                    $('#modal').find('.modal-body').css('visibility', 'visible');
+                } else $('#modal').find('.modal-body').html('');
+            });
+            $('#modal').on('shown.bs.modal', function(e) {
+                $('#modal').responsive();
+            });
+        }
+        if ($('#modal').find('.modal-body').html().trim()) {
+            $('#modal').find('.modal-body').css('visibility', 'hidden');
+            $('#modal .modal-body .select2-hidden-accessible').select2("destroy");
+            window['POPUP_STACK'].push($('#modal').find('.modal-body').clone());
+        }
         $(this).request(url, method || 'GET', data || {}, function(html) {
             $('#modal').find('.modal-body').html(html).initialize();
             if ($('.modal-body input[type=text]:first').length > 0) {
                 window.setTimeout(function() {
                     //$('.modal-body').find('input[type=text], input[type=number]').first().focus();
                 }, 200);
             }
-            $('#modal').on('shown.bs.modal', function(e) {
-                $('#modal').responsive()
-            });
             $('#modal').modal('show');
+            $('#modal').find('.modal-body').css('visibility', 'visible');
         });
     },
     reloadAreas(areas) {
         if (areas != null) {
             $('.reloadable-fieldset').map(function(i, item) {
                 if (areas.indexOf(item.id) >= 0 || areas.length == 0) {
                     $.get($(item).data('path'), function(html) {
                         if ($(item).find('.bi-chevron-right').length) {
                             html = html.replace('bi-chevron-down', 'bi-chevron-right');
-                            console.log(html);
                         }
                         $(item).html(html).initialize();
                     })
                 }
             });
             $('.reloadable-queryset').map(function(i, item) {
                 window['reload' + this.id]();
```

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/sw.js` & `sloth-framework-0.1.4/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/tests.js` & `sloth-framework-0.1.4/sloth/api/static/js/tests.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.4/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.4/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.4/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.4/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.4/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/api/index.html` & `sloth-framework-0.1.4/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.4/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.4/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.4/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,16 @@
     {% for url in dashboard.data.scripts %}
       <script src="{{ url }}?version={{ dashboard.data.footer.version }}"></script>
     {% endfor %}
     {% block extrahead %} {% endblock %}
 
   </head>
   <body id="{{ request.path|url_slug }}">
-
+    {% include "dashboard/menu.html" with menu=dashboard.render_menu %}
     {% block header %}{% include "dashboard/header.html" %}{% endblock %}
-    {% include "dashboard/menu.html" with data=dashboard.data %}
     {% include "dashboard/links.html" with data=dashboard.data %}
 
       <main>
 {% endif %}
 
 {% block content %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -16,15 +16,15 @@
  {% endif %} {% if dashboard.data.navbar.favicon %}
  {% endif %}
  {% if 0 %} {% include "themes/dark.html" %} {% endif %} {% for url in
 dashboard.data.styles %}
  {% endfor %}
  {% for url in dashboard.data.scripts %}
  {% endfor %} {% block extrahead %} {% endblock %}
-{% block header %}{% include "dashboard/header.html" %}{% endblock %} {%
-include "dashboard/menu.html" with data=dashboard.data %} {% include
+{% include "dashboard/menu.html" with menu=dashboard.render_menu %} {% block
+header %}{% include "dashboard/header.html" %}{% endblock %} {% include
 "dashboard/links.html" with data=dashboard.data %}  {% endif %} {% block
 content %} {% endblock %} {% include "dashboard/messages.html" %} {% if not
 request|is_ajax %}
   {% block footer %} {% include "dashboard/footer.html" %} {% endblock %} {%
 include "dashboard/modal.html" %} {% include "dashboard/bottom.html" %}
 {% endif %}
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                             {% if field.field.label  %}
                                 <label>
                                     {{ field.field.label }}{% if field.field.required %}*{% endif %}
                                 </label>
                             {% endif %}
                             {{ field }}
                             {% if field.help_text %}
-                        <span class="help"><i>{{ field.help_text|safe }}</i></span>
+                        <div class="help">{{ field.help_text|safe }}</div>
                             {% endif %}
                             {% if field.errors %}
                                 <div class="errors" role="alert">
                                   {{ field.errors }}
                                 </div>
                             {% endif %}
                         {% endif %}
```

#### html2text {}

```diff
@@ -29,16 +29,17 @@
 endfor %} {{ title }} **
 {% endif %}
 {% for item in itens %} {% if not item.name|is_one_to_one_field_controller %}
 {% with field=self|formfield:item.name %}
 {% if item.name|is_one_to_many_field_controller %} {{ field }} {
 { field.field.label }} {% else %} {% if field.field.label %}  {
 { field.field.label }}{% if field.field.required %}*{% endif %}  {% endif %} {
-{ field }} {% if field.help_text %} {{ field.help_text|safe }} {% endif %} {%
-if field.errors %}
+{ field }} {% if field.help_text %}
+{{ field.help_text|safe }}
+{% endif %} {% if field.errors %}
 {{ field.errors }}
 {% endif %} {% endif %}
 {% endwith %} {% endif %} {% endfor %}
 {% endfor %} {% if self.should_display_buttons %}
  Cancelar
 Loading...
 {{ self.get_metadata.submit }}
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/header.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
     {% if dashboard.data.header.shadow %}
       <style>
         .navbar {box-shadow: 0 .125rem .25rem rgba(0,0,0,.075);}
       </style>
     {% endif %}
     <nav class="navbar navbar-expand">
       <div class="container-fluid">
+        {% if dashboard.data.menu %}
+          <i class="bi bi-list"></i>
+        {% endif %}
         <a class="navbar-brand" href="/app/dashboard/">
           {% if dashboard.data.header.logo %}
             <img height="30" src="{{ dashboard.data.header.logo }}" style="border-radius:3px;">
           {% endif %}
           {% if dashboard.data.header.title %}
             <span>{{ dashboard.data.header.title }}</span>
           {% endif %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% load tags %} {% if request.user.is_authenticated and not request.GET.modal
 %} {% if dashboard.data.header.shadow %}
  {% endif %}
-{%_if_dashboard.data.header.logo_%}_[{{_dashboard.data.header.logo_}}]_{%_endif
-%}_{%_if_dashboard.data.header.title_%}_{{_dashboard.data.header.title_}}_{%
-endif_%} {% if dashboard.data.header.text and not request|mobile %} {
+{% if dashboard.data.menu %}  {% endif %} {%_if_dashboard.data.header.logo_%}_[
+{{_dashboard.data.header.logo_}}]_{%_endif_%}_{%_if_dashboard.data.header.title
+%}_{{_dashboard.data.header.title_}}_{%_endif_%} {% if
+dashboard.data.header.text and not request|mobile %} {
 { dashboard.data.header.text }} {% endif %}
     * {% for action in dashboard.data.actions %}
     * {{_action.icon|icontag_}}_{{_action.label_}}
     * {% endfor %}
 {% include "dashboard/search.html" %} {% include "dashboard/tools.html" %} {%
 include "dashboard/tasks.html" %} {% include "dashboard/plus.html" %} {%
 include "dashboard/apps.html" %} {% if request.user.is_authenticated %} {%
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/messages.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% if messages %}
     <script>
         if(window['toastTimeout']) clearTimeout(window['toastTimeout']);
         window['toastTimeout'] = setTimeout(function(){$('.toast').hide();}, 10000);
     </script>
     {% for message in messages %}
-        <div class="toast align-items-center text-white bg-{{ message.tags }} border-0 show" role="alert" aria-live="assertive" aria-atomic="true" style="position:fixed; top:10; left:10">
+        <div class="toast align-items-center text-white bg-{{ message.tags }} border-0 show" role="alert" aria-live="assertive" aria-atomic="true" style="position:fixed; top:10; left:10; z-index: 1061;">
           <div class="d-flex">
             <div class="toast-body">
               {{ message }}
             </div>
             <button type="button" class="btn-close btn-close-white me-2 m-auto" data-bs-dismiss="toast" aria-label="Close" onclick="$('.toast').hide();"></button>
           </div>
         </div>
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.4/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.4/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.4/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.4/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/filter.html`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,17 @@
         $('#{{ metadata.key }}0').val($(this).find('option:selected').text().trim());
     });
     </script>
     {% endif %}
     {% if metadata.type == "boolean" %}
     <select name="{{ metadata.key }}" class="{{ metadata.key }}-{{ data.uuid }}">
         <option selected></option>
-        <option {% if metadata.value == True %}selected{% endif %} value="1">Sim</option>
-        <option {% if metadata.value == False %}selected{% endif %} value="0">Não</option>
+        <option {% if metadata.value == 'true' %}selected{% endif %} value="true">Sim</option>
+        <option {% if metadata.value == 'false' %}selected{% endif %} value="false">Não</option>
+        <option {% if metadata.value == 'null' %}selected{% endif %} value="null">Indefinido</option>
     </select>
     <script>
            $('.{{ metadata.key }}-{{ data.uuid }}').select2({
             language: 'pt-BR',
             allowClear: true,
             placeholder: 'Selecione uma opção',
            });
```

#### html2text {}

```diff
@@ -3,11 +3,12 @@
 {% for choice in metadata.choices %}
 % if metadata.value.1 == choice.id %}selected{% endif %} value="{
 { choice.id|stringformat:'s' }}">{{ choice.text }}
 {% endfor %} {% else %} {% if metadata.value %}
 {{ metadata.value.0 }}
 {% endif %} {% endif %}
 
-% if metadata.value == True %}selected{% endif %} value="1">Sim
-% if metadata.value == False %}selected{% endif %} value="0">NÃ£o
+% if metadata.value == 'true' %}selected{% endif %} value="true">Sim
+% if metadata.value == 'false' %}selected{% endif %} value="false">NÃ£o
+% if metadata.value == 'null' %}selected{% endif %} value="null">Indefinido
  {% endif %} {% if metadata.type == "date" or metadata.type == "datetime" %}
 [Unknown INPUT type] {% endif %}
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/filters.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 <style>
 {% if data.metadata.collapsed  %}
     #search-and-filters-{{ data.uuid }}.search-and-filters form{display: none}
 {% endif %}
 </style>
 
         <div class="search-and-filters" id="search-and-filters-{{ data.uuid }}">
-            <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}" style="{% if data.metadata.collapsed %}display:none{% endif %}" class="{% if data.metadata.search or data.metadata.filters %}with-filter{% endif %}">
+            <form method="get" id="form-{{ data.uuid }}" action="{{ data.path }}" style="{% if data.metadata.collapsed %}display:none{% endif %}" class="{% if data.metadata.search or data.metadata.filters %}{% if data.metadata.tree is None %}with-filter{% endif %}{% endif %}">
                 <input type="hidden" name="uuid" value="{{ data.uuid }}">
                 <input type="hidden" name="is_admin" value="{% if data.metadata.is_admin %}1{% endif %}">
                 <input type="hidden" name="collapsed" value="{% if data.metadata.collapsed %}1{% endif %}" id="collapsed-{{ data.uuid }}">
                 <input type="hidden" name="page" value="{{ data.page }}" id="pagination-{{ data.uuid }}">
                 <input type="hidden" name="compact" value="{% if compact or request.GET.compact or request|mobile %}1{%endif%}">
                 <input type="hidden" name="subset" value="{{ data.metadata.subset }}" id="subset-{{ data.uuid }}">
                 <input type="hidden" name="selected-date" value="" id="selected-date-{{ data.uuid }}">
+                <input type="hidden" name="tree-node" value="" id="tree-node-{{ data.uuid }}">
                 <!--{% for k, v in request.POST.items %}
                     {% if k != 'csrfmiddlewaretoken' %}
                         <input type="hidden" name="post__{{ k }}" value="{{ v }}">
                     {% endif %}
                 {% endfor %}-->
                 {% if data.metadata.search or data.metadata.filters %}
+                    {% if data.metadata.tree is None %}
                     <div class="filters" id="filters-{{ data.uuid }}">
                         {% if data.metadata.search %}
                             <div class="filter {% if request|mobile %}mobile{% endif %}">
                                 <label>Busca</label>
                                 <input type="text" class="form-control" pattern=".{3,}" name="q" value="{{ request.GET.q|default:'' }}" id="searchbar" title="3 ou mais caracteres" onkeypress="if(event.which==13){reload{{ data.uuid }}();return false;}" placeholder="">
                             </div>
                         {% endif %}
@@ -36,10 +38,11 @@
                                   <span class="visually-hidden">Loading...</span>
                                 </div>
                                 <i class="bi bi-funnel"></i>
                                 Filtrar
                             </button>
                         </div>
                     </div>
+                    {% endif %}
                 {% endif %}
             </form>
         </div>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load tags %}
-        {% if data.metadata.search or data.metadata.filters %}
+         {% if data.metadata.search or data.metadata.filters %} {% if
+data.metadata.tree is None %}
 {% if data.metadata.search %}
 Busca [{{ request.GET.q|default:'' }}]
 {% endif %} {% for metadata in data.metadata.filters.values %} {% include
 "queryset/filter.html" %} {% endfor %}
 Loading...
  Filtrar
-{% endif %}
+{% endif %} {% endif %}
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/queryset.html`

 * *Files 19% similar despite different names*

```diff
@@ -90,465 +90,622 @@
 00000590: 7365 7420 696e 2064 6174 612e 6174 7461  set in data.atta
 000005a0: 6368 2e76 616c 7565 7320 257d 0a20 2020  ch.values %}.   
 000005b0: 2020 2020 2020 2020 2020 203c 6c69 2063             <li c
 000005c0: 6c61 7373 3d22 6e61 762d 6974 656d 207b  lass="nav-item {
 000005d0: 7b20 7375 6273 6574 2e6b 6579 207d 7d20  { subset.key }} 
 000005e0: 7b25 2069 6620 7375 6273 6574 2e61 6374  {% if subset.act
 000005f0: 6976 6520 257d 7365 6c65 6374 6564 7b25  ive %}selected{%
-00000600: 2065 6e64 6966 2025 7d22 3e0a 2020 2020   endif %}">.    
-00000610: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-00000620: 6c61 7373 3d22 6e61 762d 6c69 6e6b 2220  lass="nav-link" 
-00000630: 6172 6961 2d63 7572 7265 6e74 3d22 7061  aria-current="pa
-00000640: 6765 2220 6872 6566 3d22 6a61 7661 7363  ge" href="javasc
-00000650: 7269 7074 3a22 206f 6e63 6c69 636b 3d22  ript:" onclick="
-00000660: 2428 2723 7061 6769 6e61 7469 6f6e 2d7b  $('#pagination-{
-00000670: 7b20 6461 7461 2e75 7569 6420 7d7d 2729  { data.uuid }}')
-00000680: 2e76 616c 2831 293b 7265 6c6f 6164 7b7b  .val(1);reload{{
-00000690: 2064 6174 612e 7575 6964 207d 7d28 277b   data.uuid }}('{
-000006a0: 7b20 7375 6273 6574 2e6b 6579 207d 7d27  { subset.key }}'
-000006b0: 2922 3e0a 2020 2020 2020 2020 2020 2020  )">.            
-000006c0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000006d0: 7373 3d22 7370 696e 6e65 722d 626f 7264  ss="spinner-bord
-000006e0: 6572 2073 7069 6e6e 6572 2d62 6f72 6465  er spinner-borde
-000006f0: 722d 736d 2064 2d6e 6f6e 6522 2072 6f6c  r-sm d-none" rol
-00000700: 653d 2273 7461 7475 7322 3e0a 2020 2020  e="status">.    
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 3c73 7061 6e20 636c 6173 733d 2276    <span class="v
-00000730: 6973 7561 6c6c 792d 6869 6464 656e 223e  isually-hidden">
-00000740: 4c6f 6164 696e 672e 2e2e 3c2f 7370 616e  Loading...</span
-00000750: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000760: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 203c 7370 616e 2063 6c61 7373 3d22 6e61   <span class="na
-00000790: 762d 6c69 6e6b 2d74 6578 7422 3e7b 7b20  v-link-text">{{ 
-000007a0: 7375 6273 6574 2e6e 616d 6520 7d7d 3c2f  subset.name }}</
-000007b0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-000007c0: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-000007d0: 636c 6173 733d 2262 6164 6765 2072 6f75  class="badge rou
-000007e0: 6e64 6564 2d70 696c 6c20 7465 7874 2d77  nded-pill text-w
-000007f0: 6869 7465 2062 672d 7072 696d 6172 7920  hite bg-primary 
-00000800: 746f 7461 6c2d 7b7b 2073 7562 7365 742e  total-{{ subset.
-00000810: 6b65 7920 7d7d 223e 7b7b 2073 7562 7365  key }}">{{ subse
-00000820: 742e 636f 756e 7420 7d7d 3c2f 7370 616e  t.count }}</span
-00000830: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00000840: 2020 3c2f 613e 0a20 2020 2020 2020 2020    </a>.         
-00000850: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
-00000860: 2020 2020 2020 2020 2020 207b 2520 656e             {% en
-00000870: 6466 6f72 2025 7d0a 2020 2020 2020 2020  dfor %}.        
-00000880: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
-00000890: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-000008a0: 207b 2520 656e 6469 6620 257d 0a0a 2020   {% endif %}..  
-000008b0: 2020 2020 2020 7b25 2066 6f72 2061 6374        {% for act
-000008c0: 696f 6e20 696e 2064 6174 612e 6163 7469  ion in data.acti
-000008d0: 6f6e 732e 696e 6c69 6e65 2025 7d0a 2020  ons.inline %}.  
-000008e0: 2020 2020 2020 2020 2020 7b25 2061 6374            {% act
-000008f0: 696f 6e20 6163 7469 6f6e 2e6b 6579 2064  ion action.key d
-00000900: 6174 612e 696e 7374 616e 7469 6174 6f72  ata.instantiator
-00000910: 2061 6374 696f 6e2e 7061 7468 2025 7d0a   action.path %}.
-00000920: 2020 2020 2020 2020 7b25 2065 6e64 666f          {% endfo
-00000930: 7220 257d 0a0a 2020 2020 2020 2020 7b25  r %}..        {%
-00000940: 2069 6620 6e6f 7420 7072 696e 7420 257d   if not print %}
-00000950: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-00000960: 696e 636c 7564 6520 2271 7565 7279 7365  include "queryse
-00000970: 742f 6669 6c74 6572 732e 6874 6d6c 2220  t/filters.html" 
-00000980: 257d 0a20 2020 2020 2020 2020 2020 203c  %}.            <
-00000990: 6469 7620 636c 6173 733d 2263 6c65 6172  div class="clear
-000009a0: 6669 7822 3e3c 2f64 6976 3e0a 2020 2020  fix"></div>.    
-000009b0: 2020 2020 2020 2020 3c73 6372 6970 743e          <script>
-000009c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009d0: 2066 756e 6374 696f 6e20 7265 6c6f 6164   function reload
-000009e0: 7b7b 2064 6174 612e 7575 6964 207d 7d28  {{ data.uuid }}(
-000009f0: 7375 6273 6574 297b 0a20 2020 2020 2020  subset){.       
-00000a00: 2020 2020 2020 2020 2020 2020 2024 2864               $(d
-00000a10: 6f63 756d 656e 742e 626f 6479 292e 6164  ocument.body).ad
-00000a20: 6443 6c61 7373 2827 7061 6765 2d6c 6f61  dClass('page-loa
-00000a30: 6469 6e67 2729 3b0a 2020 2020 2020 2020  ding');.        
-00000a40: 2020 2020 2020 2020 2020 2020 6966 2873              if(s
-00000a50: 7562 7365 743d 3d6e 756c 6c29 2073 7562  ubset==null) sub
-00000a60: 7365 7420 3d20 2428 2723 7375 6273 6574  set = $('#subset
-00000a70: 2d7b 7b20 6461 7461 2e75 7569 6420 7d7d  -{{ data.uuid }}
-00000a80: 2729 2e76 616c 2829 3b0a 2020 2020 2020  ').val();.      
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-00000aa0: 2723 7375 6273 6574 2d7b 7b20 6461 7461  '#subset-{{ data
-00000ab0: 2e75 7569 6420 7d7d 2729 2e76 616c 2873  .uuid }}').val(s
-00000ac0: 7562 7365 7429 3b0a 2020 2020 2020 2020  ubset);.        
-00000ad0: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-00000ae0: 7461 6273 2d63 6f6e 7461 696e 6572 2d7b  tabs-container-{
-00000af0: 7b20 6461 7461 2e75 7569 6420 7d7d 2729  { data.uuid }}')
-00000b00: 2e66 696e 6428 272e 6e61 762d 6974 656d  .find('.nav-item
-00000b10: 2e27 2b73 7562 7365 7429 2e66 696e 6428  .'+subset).find(
-00000b20: 272e 7370 696e 6e65 722d 626f 7264 6572  '.spinner-border
-00000b30: 2729 2e72 656d 6f76 6543 6c61 7373 2827  ').removeClass('
-00000b40: 642d 6e6f 6e65 2729 3b0a 2020 2020 2020  d-none');.      
-00000b50: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00000b60: 7220 6461 7461 203d 2024 2827 2366 6f72  r data = $('#for
-00000b70: 6d2d 7b7b 2064 6174 612e 7575 6964 207d  m-{{ data.uuid }
-00000b80: 7d27 292e 7365 7269 616c 697a 6528 293b  }').serialize();
-00000b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ba0: 2020 2020 2024 2e61 6a61 7828 7b0a 2020       $.ajax({.  
-00000bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bc0: 2020 2020 2020 7572 6c3a 277b 7b20 6461        url:'{{ da
-00000bd0: 7461 2e70 6174 687c 7361 6665 207d 7d3f  ta.path|safe }}?
-00000be0: 7b7b 2072 6571 7565 7374 7c70 6f73 745f  {{ request|post_
-00000bf0: 7175 6572 7973 7472 696e 6720 7d7d 272c  querystring }}',
-00000c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c10: 2020 2020 2020 2020 2064 6174 613a 2064           data: d
-00000c20: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
-00000c30: 2020 2020 2020 2020 2020 2020 2073 7563               suc
-00000c40: 6365 7373 3a66 756e 6374 696f 6e28 2068  cess:function( h
-00000c50: 746d 6c20 2920 7b0a 2020 2020 2020 2020  tml ) {.        
+00000600: 2065 6e64 6966 2025 7d20 7b25 2069 6620   endif %} {% if 
+00000610: 7265 7175 6573 747c 6d6f 6269 6c65 2025  request|mobile %
+00000620: 7d6d 6f62 696c 657b 2520 656e 6469 6620  }mobile{% endif 
+00000630: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+00000640: 2020 2020 203c 6120 636c 6173 733d 226e       <a class="n
+00000650: 6176 2d6c 696e 6b22 2061 7269 612d 6375  av-link" aria-cu
+00000660: 7272 656e 743d 2270 6167 6522 2068 7265  rrent="page" hre
+00000670: 663d 226a 6176 6173 6372 6970 743a 2220  f="javascript:" 
+00000680: 6f6e 636c 6963 6b3d 2224 2827 2370 6167  onclick="$('#pag
+00000690: 696e 6174 696f 6e2d 7b7b 2064 6174 612e  ination-{{ data.
+000006a0: 7575 6964 207d 7d27 292e 7661 6c28 3129  uuid }}').val(1)
+000006b0: 3b72 656c 6f61 647b 7b20 6461 7461 2e75  ;reload{{ data.u
+000006c0: 7569 6420 7d7d 2827 7b7b 2073 7562 7365  uid }}('{{ subse
+000006d0: 742e 6b65 7920 7d7d 2729 223e 0a20 2020  t.key }}')">.   
+000006e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006f0: 203c 6469 7620 636c 6173 733d 2273 7069   <div class="spi
+00000700: 6e6e 6572 2d62 6f72 6465 7220 7370 696e  nner-border spin
+00000710: 6e65 722d 626f 7264 6572 2d73 6d20 642d  ner-border-sm d-
+00000720: 6e6f 6e65 2220 726f 6c65 3d22 7374 6174  none" role="stat
+00000730: 7573 223e 0a20 2020 2020 2020 2020 2020  us">.           
+00000740: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00000750: 2063 6c61 7373 3d22 7669 7375 616c 6c79   class="visually
+00000760: 2d68 6964 6465 6e22 3e4c 6f61 6469 6e67  -hidden">Loading
+00000770: 2e2e 2e3c 2f73 7061 6e3e 0a20 2020 2020  ...</span>.     
+00000780: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000790: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+000007a0: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+000007b0: 636c 6173 733d 226e 6176 2d6c 696e 6b2d  class="nav-link-
+000007c0: 7465 7874 223e 7b7b 2073 7562 7365 742e  text">{{ subset.
+000007d0: 6e61 6d65 207d 7d3c 2f73 7061 6e3e 0a20  name }}</span>. 
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007f0: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+00000800: 6261 6467 6520 726f 756e 6465 642d 7069  badge rounded-pi
+00000810: 6c6c 2074 6578 742d 7768 6974 6520 6267  ll text-white bg
+00000820: 2d70 7269 6d61 7279 2074 6f74 616c 2d7b  -primary total-{
+00000830: 7b20 7375 6273 6574 2e6b 6579 207d 7d22  { subset.key }}"
+00000840: 3e7b 7b20 7375 6273 6574 2e63 6f75 6e74  >{{ subset.count
+00000850: 207d 7d3c 2f73 7061 6e3e 0a20 2020 2020   }}</span>.     
+00000860: 2020 2020 2020 2020 2020 203c 2f61 3e0a             </a>.
+00000870: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00000880: 6c69 3e0a 2020 2020 2020 2020 2020 2020  li>.            
+00000890: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
+000008a0: 0a20 2020 2020 2020 2020 2020 203c 2f75  .            </u
+000008b0: 6c3e 0a20 2020 2020 2020 203c 2f64 6976  l>.        </div
+000008c0: 3e0a 2020 2020 2020 2020 7b25 2065 6e64  >.        {% end
+000008d0: 6966 2025 7d0a 0a20 2020 2020 2020 207b  if %}..        {
+000008e0: 2520 666f 7220 6163 7469 6f6e 2069 6e20  % for action in 
+000008f0: 6461 7461 2e61 6374 696f 6e73 2e69 6e6c  data.actions.inl
+00000900: 696e 6520 257d 0a20 2020 2020 2020 2020  ine %}.         
+00000910: 2020 207b 2520 6163 7469 6f6e 2061 6374     {% action act
+00000920: 696f 6e2e 6b65 7920 6461 7461 2e69 6e73  ion.key data.ins
+00000930: 7461 6e74 6961 746f 7220 6163 7469 6f6e  tantiator action
+00000940: 2e70 6174 6820 257d 0a20 2020 2020 2020  .path %}.       
+00000950: 207b 2520 656e 6466 6f72 2025 7d0a 0a20   {% endfor %}.. 
+00000960: 2020 2020 2020 207b 2520 6966 206e 6f74         {% if not
+00000970: 2070 7269 6e74 2025 7d0a 2020 2020 2020   print %}.      
+00000980: 2020 2020 2020 7b25 2069 6620 6461 7461        {% if data
+00000990: 2e6d 6574 6164 6174 612e 7472 6565 2025  .metadata.tree %
+000009a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000009b0: 2020 7b25 2069 6e63 6c75 6465 2022 7175    {% include "qu
+000009c0: 6572 7973 6574 2f74 7265 652e 6874 6d6c  eryset/tree.html
+000009d0: 2220 7769 7468 2064 6174 613d 6461 7461  " with data=data
+000009e0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
+000009f0: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
+00000a00: 2020 2020 2020 2020 7b25 2069 6e63 6c75          {% inclu
+00000a10: 6465 2022 7175 6572 7973 6574 2f66 696c  de "queryset/fil
+00000a20: 7465 7273 2e68 746d 6c22 2025 7d0a 2020  ters.html" %}.  
+00000a30: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00000a40: 6c61 7373 3d22 636c 6561 7266 6978 223e  lass="clearfix">
+00000a50: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000a60: 2020 203c 7363 7269 7074 3e0a 2020 2020     <script>.    
+00000a70: 2020 2020 2020 2020 2020 2020 6675 6e63              func
+00000a80: 7469 6f6e 2072 656c 6f61 647b 7b20 6461  tion reload{{ da
+00000a90: 7461 2e75 7569 6420 7d7d 2873 7562 7365  ta.uuid }}(subse
+00000aa0: 7429 7b0a 2020 2020 2020 2020 2020 2020  t){.            
+00000ab0: 2020 2020 2020 2020 2428 646f 6375 6d65          $(docume
+00000ac0: 6e74 2e62 6f64 7929 2e61 6464 436c 6173  nt.body).addClas
+00000ad0: 7328 2770 6167 652d 6c6f 6164 696e 6727  s('page-loading'
+00000ae0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00000af0: 2020 2020 2020 2069 6628 7375 6273 6574         if(subset
+00000b00: 3d3d 6e75 6c6c 2920 7375 6273 6574 203d  ==null) subset =
+00000b10: 2024 2827 2373 7562 7365 742d 7b7b 2064   $('#subset-{{ d
+00000b20: 6174 612e 7575 6964 207d 7d27 292e 7661  ata.uuid }}').va
+00000b30: 6c28 293b 0a20 2020 2020 2020 2020 2020  l();.           
+00000b40: 2020 2020 2020 2020 2024 2827 2373 7562           $('#sub
+00000b50: 7365 742d 7b7b 2064 6174 612e 7575 6964  set-{{ data.uuid
+00000b60: 207d 7d27 292e 7661 6c28 7375 6273 6574   }}').val(subset
+00000b70: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00000b80: 2020 2020 2020 2024 2827 2374 6162 732d         $('#tabs-
+00000b90: 636f 6e74 6169 6e65 722d 7b7b 2064 6174  container-{{ dat
+00000ba0: 612e 7575 6964 207d 7d27 292e 6669 6e64  a.uuid }}').find
+00000bb0: 2827 2e6e 6176 2d69 7465 6d2e 272b 7375  ('.nav-item.'+su
+00000bc0: 6273 6574 292e 6669 6e64 2827 2e73 7069  bset).find('.spi
+00000bd0: 6e6e 6572 2d62 6f72 6465 7227 292e 7265  nner-border').re
+00000be0: 6d6f 7665 436c 6173 7328 2764 2d6e 6f6e  moveClass('d-non
+00000bf0: 6527 293b 0a20 2020 2020 2020 2020 2020  e');.           
+00000c00: 2020 2020 2020 2020 2076 6172 2064 6174           var dat
+00000c10: 6120 3d20 2428 2723 666f 726d 2d7b 7b20  a = $('#form-{{ 
+00000c20: 6461 7461 2e75 7569 6420 7d7d 2729 2e73  data.uuid }}').s
+00000c30: 6572 6961 6c69 7a65 2829 3b0a 2020 2020  erialize();.    
+00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c50: 242e 616a 6178 287b 0a20 2020 2020 2020  $.ajax({.       
 00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 2428 2723 7b7b 2064 6174 612e      $('#{{ data.
-00000c80: 6b65 7920 7d7d 2729 2e68 746d 6c28 2428  key }}').html($(
-00000c90: 6874 6d6c 292e 6669 6e64 2827 237b 7b20  html).find('#{{ 
-00000ca0: 6461 7461 2e6b 6579 207d 7d27 292e 6874  data.key }}').ht
-00000cb0: 6d6c 2829 292e 696e 6974 6961 6c69 7a65  ml()).initialize
-00000cc0: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
+00000c70: 2075 726c 3a27 7b7b 2064 6174 612e 7061   url:'{{ data.pa
+00000c80: 7468 7c73 6166 6520 7d7d 3f7b 7b20 7265  th|safe }}?{{ re
+00000c90: 7175 6573 747c 706f 7374 5f71 7565 7279  quest|post_query
+00000ca0: 7374 7269 6e67 207d 7d27 2c0a 2020 2020  string }}',.    
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 2020 2020 6461 7461 3a20 6461 7461 2c0a      data: data,.
 00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2428 646f 6375 6d65 6e74 2e62 6f64 7929  $(document.body)
-00000cf0: 2e72 656d 6f76 6543 6c61 7373 2827 7061  .removeClass('pa
-00000d00: 6765 2d6c 6f61 6469 6e67 2729 3b0a 2020  ge-loading');.  
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000d30: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d50: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00000d60: 2020 6675 6e63 7469 6f6e 2074 6f67 676c    function toggl
-00000d70: 6541 6374 696f 6e73 7b7b 2064 6174 612e  eActions{{ data.
-00000d80: 7575 6964 207d 7d28 696e 7075 7429 7b0a  uuid }}(input){.
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 2020 6966 2869 6e70 7574 2e76 616c      if(input.val
-00000db0: 7565 3d3d 2727 2920 2428 2723 7175 6572  ue=='') $('#quer
-00000dc0: 7973 6574 2d7b 7b20 6461 7461 2e75 7569  yset-{{ data.uui
-00000dd0: 6420 7d7d 2729 2e66 696e 6428 272e 6163  d }}').find('.ac
-00000de0: 7469 6f6e 2d63 6865 636b 626f 7827 292e  tion-checkbox').
-00000df0: 7072 6f70 2827 6368 6563 6b65 6427 2c20  prop('checked', 
-00000e00: 696e 7075 742e 6368 6563 6b65 6429 3b0a  input.checked);.
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 2020 6966 2824 2827 2371 7565 7279      if($('#query
-00000e30: 7365 742d 7b7b 2064 6174 612e 7575 6964  set-{{ data.uuid
-00000e40: 207d 7d27 292e 6669 6e64 2827 2e61 6374   }}').find('.act
-00000e50: 696f 6e2d 6368 6563 6b62 6f78 3a63 6865  ion-checkbox:che
-00000e60: 636b 6564 2729 2e6c 656e 6774 683e 3029  cked').length>0)
-00000e70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000e80: 2020 2020 2020 2020 2020 2428 2723 7175            $('#qu
-00000e90: 6572 7973 6574 2d7b 7b20 6461 7461 2e75  eryset-{{ data.u
-00000ea0: 7569 6420 7d7d 2729 2e66 696e 6428 272e  uid }}').find('.
-00000eb0: 6472 6f70 646f 776e 2d74 6f67 676c 652e  dropdown-toggle.
-00000ec0: 7175 6572 7973 6574 2729 2e72 656d 6f76  queryset').remov
-00000ed0: 6543 6c61 7373 2827 6469 7361 626c 6564  eClass('disabled
-00000ee0: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
-00000ef0: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
-00000f00: 7175 6572 7973 6574 2d7b 7b20 6461 7461  queryset-{{ data
-00000f10: 2e75 7569 6420 7d7d 2729 2e66 696e 6428  .uuid }}').find(
-00000f20: 272e 6472 6f70 646f 776e 2d74 6f67 676c  '.dropdown-toggl
-00000f30: 652e 696e 7374 616e 6365 2c20 2e64 726f  e.instance, .dro
-00000f40: 7064 6f77 6e2d 746f 6767 6c65 2e6d 6f64  pdown-toggle.mod
-00000f50: 656c 2729 2e61 6464 436c 6173 7328 2764  el').addClass('d
-00000f60: 6973 6162 6c65 6427 293b 0a20 2020 2020  isabled');.     
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2024 2827 2371 7565 7279 7365 742d     $('#queryset-
-00000f90: 7b7b 2064 6174 612e 7575 6964 207d 7d27  {{ data.uuid }}'
-00000fa0: 292e 6669 6e64 2827 2e62 746e 2e69 6e73  ).find('.btn.ins
-00000fb0: 7461 6e63 652c 202e 6274 6e2e 6d6f 6465  tance, .btn.mode
-00000fc0: 6c27 292e 6164 6443 6c61 7373 2827 6469  l').addClass('di
-00000fd0: 7361 626c 6564 2729 3b0a 2020 2020 2020  sabled');.      
-00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ff0: 2020 2428 2723 7175 6572 7973 6574 2d7b    $('#queryset-{
-00001000: 7b20 6461 7461 2e75 7569 6420 7d7d 2729  { data.uuid }}')
-00001010: 2e66 696e 6428 272e 6274 6e2e 7175 6572  .find('.btn.quer
-00001020: 7973 6574 2729 2e72 656d 6f76 6543 6c61  yset').removeCla
-00001030: 7373 2827 6469 7361 626c 6564 2729 3b0a  ss('disabled');.
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 2020 7d20 656c 7365 207b 0a20 2020      } else {.   
-00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 2020 2020 2024 2827 2371 7565 7279 7365       $('#queryse
-00001080: 742d 7b7b 2064 6174 612e 7575 6964 207d  t-{{ data.uuid }
-00001090: 7d27 292e 6669 6e64 2827 2e64 726f 7064  }').find('.dropd
-000010a0: 6f77 6e2d 746f 6767 6c65 2e71 7565 7279  own-toggle.query
-000010b0: 7365 7427 292e 6164 6443 6c61 7373 2827  set').addClass('
-000010c0: 6469 7361 626c 6564 2729 3b0a 2020 2020  disabled');.    
-000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010e0: 2020 2020 2428 2723 7175 6572 7973 6574      $('#queryset
-000010f0: 2d7b 7b20 6461 7461 2e75 7569 6420 7d7d  -{{ data.uuid }}
-00001100: 2729 2e66 696e 6428 272e 6472 6f70 646f  ').find('.dropdo
-00001110: 776e 2d74 6f67 676c 652e 6d6f 6465 6c2c  wn-toggle.model,
-00001120: 202e 6472 6f70 646f 776e 2d74 6f67 676c   .dropdown-toggl
-00001130: 652e 696e 7374 616e 6365 2729 2e72 656d  e.instance').rem
-00001140: 6f76 6543 6c61 7373 2827 6469 7361 626c  oveClass('disabl
-00001150: 6564 2729 3b0a 2020 2020 2020 2020 2020  ed');.          
-00001160: 2020 2020 2020 2020 2020 2020 2020 2428                $(
-00001170: 2723 7175 6572 7973 6574 2d7b 7b20 6461  '#queryset-{{ da
-00001180: 7461 2e75 7569 6420 7d7d 2729 2e66 696e  ta.uuid }}').fin
-00001190: 6428 272e 6274 6e2e 696e 7374 616e 6365  d('.btn.instance
-000011a0: 2c20 2e62 746e 2e6d 6f64 656c 2729 2e72  , .btn.model').r
-000011b0: 656d 6f76 6543 6c61 7373 2827 6469 7361  emoveClass('disa
-000011c0: 626c 6564 2729 3b0a 2020 2020 2020 2020  bled');.        
-000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2428 2723 7175 6572 7973 6574 2d7b 7b20  $('#queryset-{{ 
-000011f0: 6461 7461 2e75 7569 6420 7d7d 2729 2e66  data.uuid }}').f
-00001200: 696e 6428 272e 6274 6e2e 7175 6572 7973  ind('.btn.querys
-00001210: 6574 2729 2e61 6464 436c 6173 7328 2764  et').addClass('d
-00001220: 6973 6162 6c65 6427 293b 0a20 2020 2020  isabled');.     
-00001230: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001250: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00001260: 2020 2066 756e 6374 696f 6e20 736c 6964     function slid
-00001270: 6553 6561 7263 6841 6e64 4669 6c74 6572  eSearchAndFilter
-00001280: 737b 7b20 6461 7461 2e75 7569 6420 7d7d  s{{ data.uuid }}
-00001290: 2861 297b 0a20 2020 2020 2020 2020 2020  (a){.           
-000012a0: 2020 2020 2020 2020 2069 6628 6129 2024           if(a) $
-000012b0: 2861 292e 6669 6e64 2827 693a 6c61 7374  (a).find('i:last
-000012c0: 2d63 6869 6c64 2729 2e74 6f67 676c 6543  -child').toggleC
-000012d0: 6c61 7373 2827 6269 2d63 6865 7672 6f6e  lass('bi-chevron
-000012e0: 2d75 7027 292e 746f 6767 6c65 436c 6173  -up').toggleClas
-000012f0: 7328 2762 692d 6368 6576 726f 6e2d 646f  s('bi-chevron-do
-00001300: 776e 2729 3b0a 2020 2020 2020 2020 2020  wn');.          
-00001310: 2020 2020 2020 2020 2020 6966 2824 2827            if($('
-00001320: 2366 6f72 6d2d 7b7b 2064 6174 612e 7575  #form-{{ data.uu
-00001330: 6964 207d 7d27 292e 6373 7328 2764 6973  id }}').css('dis
-00001340: 706c 6179 2729 203d 3d20 276e 6f6e 6527  play') == 'none'
-00001350: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
-00001360: 2020 2020 2020 2020 2020 2024 2827 2366             $('#f
-00001370: 6f72 6d2d 7b7b 2064 6174 612e 7575 6964  orm-{{ data.uuid
-00001380: 207d 7d27 292e 736c 6964 6544 6f77 6e28   }}').slideDown(
-00001390: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000013a0: 2020 2020 2020 2020 2020 2024 2827 2363             $('#c
-000013b0: 6f6c 6c61 7073 6564 2d7b 7b20 6461 7461  ollapsed-{{ data
-000013c0: 2e75 7569 6420 7d7d 2729 2e76 616c 2822  .uuid }}').val("
-000013d0: 2229 3b0a 2020 2020 2020 2020 2020 2020  ");.            
-000013e0: 2020 2020 2020 2020 7d20 656c 7365 207b          } else {
-000013f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001400: 2020 2020 2020 2020 2024 2827 2366 6f72           $('#for
-00001410: 6d2d 7b7b 2064 6174 612e 7575 6964 207d  m-{{ data.uuid }
-00001420: 7d27 292e 736c 6964 6555 7028 293b 0a20  }').slideUp();. 
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2020 2020 2024 2827 2363 6f6c 6c61         $('#colla
-00001450: 7073 6564 2d7b 7b20 6461 7461 2e75 7569  psed-{{ data.uui
-00001460: 6420 7d7d 2729 2e76 616c 2831 293b 0a20  d }}').val(1);. 
-00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001480: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00001490: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-000014a0: 2020 203c 2f73 6372 6970 743e 0a20 2020     </script>.   
-000014b0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-000014c0: 0a0a 2020 2020 2020 2020 3c64 6976 2063  ..        <div c
-000014d0: 6c61 7373 3d22 7175 6572 7973 6574 2d64  lass="queryset-d
-000014e0: 6174 6122 2069 643d 2271 7565 7279 7365  ata" id="queryse
-000014f0: 742d 6461 7461 2d7b 7b20 6461 7461 2e75  t-data-{{ data.u
-00001500: 7569 6420 7d7d 223e 0a0a 2020 2020 7b25  uid }}">..    {%
-00001510: 2069 6620 6461 7461 2e6d 6574 6164 6174   if data.metadat
-00001520: 612e 7061 6769 6e61 7469 6f6e 2e74 6f74  a.pagination.tot
-00001530: 616c 206f 7220 6461 7461 2e6d 6574 6164  al or data.metad
-00001540: 6174 612e 6361 6c65 6e64 6172 2025 7d0a  ata.calendar %}.
-00001550: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00001560: 636c 6561 7266 6978 2220 6964 3d22 7061  clearfix" id="pa
-00001570: 6769 6e61 7469 6f6e 2d69 6e66 6f2d 7b7b  gination-info-{{
-00001580: 2064 6174 612e 7575 6964 207d 7d22 3e0a   data.uuid }}">.
-00001590: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000015a0: 7373 3d22 666c 6f61 742d 7374 6172 7422  ss="float-start"
-000015b0: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
-000015c0: 6976 2063 6c61 7373 3d22 6d74 2d33 206d  iv class="mt-3 m
-000015d0: 622d 3322 2073 7479 6c65 3d22 666f 6e74  b-3" style="font
-000015e0: 2d73 697a 653a 2038 3025 223e 0a20 2020  -size: 80%">.   
-000015f0: 2020 2020 2020 2020 2020 2020 2045 7869               Exi
-00001600: 6269 6e64 6f0a 2020 2020 2020 2020 2020  bindo.          
-00001610: 2020 2020 2020 7b25 2069 6620 6461 7461        {% if data
-00001620: 2e6d 6574 6164 6174 612e 7061 6769 6e61  .metadata.pagina
-00001630: 7469 6f6e 2e74 6f74 616c 203e 2064 6174  tion.total > dat
-00001640: 612e 6d65 7461 6461 7461 2e70 6167 696e  a.metadata.pagin
-00001650: 6174 696f 6e2e 696e 7465 7276 616c 2e31  ation.interval.1
-00001660: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00001670: 2020 2020 2020 2020 7b7b 2064 6174 612e          {{ data.
-00001680: 6d65 7461 6461 7461 2e70 6167 696e 6174  metadata.paginat
-00001690: 696f 6e2e 696e 7465 7276 616c 2e30 207d  ion.interval.0 }
-000016a0: 7d20 2d20 7b7b 2064 6174 612e 6d65 7461  } - {{ data.meta
-000016b0: 6461 7461 2e70 6167 696e 6174 696f 6e2e  data.pagination.
-000016c0: 696e 7465 7276 616c 2e31 207d 7d20 6465  interval.1 }} de
-000016d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016e0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-000016f0: 2020 2020 2020 2020 2020 2020 203c 7374               <st
-00001700: 726f 6e67 3e0a 2020 2020 2020 2020 2020  rong>.          
-00001710: 2020 2020 2020 2020 2020 7b7b 2064 6174            {{ dat
-00001720: 612e 6d65 7461 6461 7461 2e70 6167 696e  a.metadata.pagin
-00001730: 6174 696f 6e2e 746f 7461 6c20 7d7d 2072  ation.total }} r
-00001740: 6567 6973 7472 6f7b 2520 6966 2064 6174  egistro{% if dat
-00001750: 612e 6d65 7461 6461 7461 2e70 6167 696e  a.metadata.pagin
-00001760: 6174 696f 6e2e 746f 7461 6c20 3e20 3120  ation.total > 1 
-00001770: 257d 737b 2520 656e 6469 6620 257d 0a20  %}s{% endif %}. 
-00001780: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001790: 2f73 7472 6f6e 673e 0a20 2020 2020 2020  /strong>.       
-000017a0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000017b0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000017c0: 2020 203c 6469 7620 636c 6173 733d 2266     <div class="f
-000017d0: 6c6f 6174 2d65 6e64 223e 0a20 2020 2020  loat-end">.     
-000017e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-000017f0: 733d 226d 742d 3320 6d62 2d33 223e 0a20  s="mt-3 mb-3">. 
-00001800: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001810: 212d 2d3c 6120 6872 6566 3d22 7b7b 2064  !--<a href="{{ d
-00001820: 6174 612e 7061 7468 207d 7d3f 6578 706f  ata.path }}?expo
-00001830: 7274 3d63 7376 223e 3c69 2063 6c61 7373  rt=csv"><i class
-00001840: 3d22 6269 2062 692d 646f 776e 6c6f 6164  ="bi bi-download
-00001850: 223e 3c2f 693e 3c2f 613e 2d2d 3e0a 2020  "></i></a>-->.  
-00001860: 2020 2020 2020 2020 2020 2020 2020 3c21                <!
-00001870: 2d2d 3c61 2068 7265 663d 227b 7b20 6461  --<a href="{{ da
-00001880: 7461 2e70 6174 6820 7d7d 3f65 7870 6f72  ta.path }}?expor
-00001890: 743d 786c 7322 3e3c 6920 636c 6173 733d  t=xls"><i class=
-000018a0: 2262 6920 6269 2d66 696c 652d 6578 6365  "bi bi-file-exce
-000018b0: 6c22 3e3c 2f69 3e3c 2f61 3e2d 2d3e 0a20  l"></i></a>-->. 
-000018c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000018d0: 212d 2d3c 6120 6872 6566 3d22 7b7b 2064  !--<a href="{{ d
-000018e0: 6174 612e 7061 7468 207d 7d3f 6578 706f  ata.path }}?expo
-000018f0: 7274 3d70 6466 223e 3c69 2063 6c61 7373  rt=pdf"><i class
-00001900: 3d22 6269 2062 692d 6669 6c65 2d65 6172  ="bi bi-file-ear
-00001910: 6d61 726b 2d70 6466 223e 3c2f 693e 3c2f  mark-pdf"></i></
-00001920: 613e 2d2d 3e0a 2020 2020 2020 2020 2020  a>-->.          
-00001930: 2020 2020 2020 7b25 2069 6620 6461 7461        {% if data
-00001940: 2e6d 6574 6164 6174 612e 7365 6172 6368  .metadata.search
-00001950: 206f 7220 6461 7461 2e6d 6574 6164 6174   or data.metadat
-00001960: 612e 6669 6c74 6572 7320 257d 0a20 2020  a.filters %}.   
-00001970: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00001980: 6872 6566 3d22 6a61 7661 7363 7269 7074  href="javascript
-00001990: 3a22 3e3c 6920 636c 6173 733d 2262 6920  :"><i class="bi 
-000019a0: 6269 2d66 756e 6e65 6c22 206f 6e63 6c69  bi-funnel" oncli
-000019b0: 636b 3d22 736c 6964 6553 6561 7263 6841  ck="slideSearchA
-000019c0: 6e64 4669 6c74 6572 737b 7b20 6461 7461  ndFilters{{ data
-000019d0: 2e75 7569 6420 7d7d 2829 223e 3c2f 693e  .uuid }}()"></i>
-000019e0: 3c2f 613e 0a20 2020 2020 2020 2020 2020  </a>.           
-000019f0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00001a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a10: 203c 6120 6872 6566 3d22 6a61 7661 7363   <a href="javasc
-00001a20: 7269 7074 3a22 3e3c 6920 636c 6173 733d  ript:"><i class=
-00001a30: 2262 6920 6269 2d61 7272 6f77 2d63 6c6f  "bi bi-arrow-clo
-00001a40: 636b 7769 7365 2220 6f6e 636c 6963 6b3d  ckwise" onclick=
-00001a50: 2272 656c 6f61 647b 7b20 6461 7461 2e75  "reload{{ data.u
-00001a60: 7569 6420 7d7d 2829 3b22 3e3c 2f69 3e3c  uid }}();"></i><
-00001a70: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00001a80: 3c2f 6469 763e 0a20 2020 2020 2020 203c  </div>.        <
-00001a90: 2f64 6976 3e0a 2020 2020 3c2f 6469 763e  /div>.    </div>
-00001aa0: 0a0a 2020 2020 7b25 2069 6620 6461 7461  ..    {% if data
-00001ab0: 2e6d 6574 6164 6174 612e 6361 6c65 6e64  .metadata.calend
-00001ac0: 6172 2025 7d0a 2020 2020 2020 2020 7b25  ar %}.        {%
-00001ad0: 2069 6e63 6c75 6465 2022 7175 6572 7973   include "querys
-00001ae0: 6574 2f63 616c 656e 6461 722e 6874 6d6c  et/calendar.html
-00001af0: 2220 7769 7468 2064 6174 613d 6461 7461  " with data=data
-00001b00: 2025 7d0a 2020 2020 7b25 2065 6e64 6966   %}.    {% endif
-00001b10: 2025 7d0a 0a20 2020 207b 2520 6966 2064   %}..    {% if d
-00001b20: 6174 612e 6d65 7461 6461 7461 2e61 6767  ata.metadata.agg
-00001b30: 7265 6761 7469 6f6e 7320 257d 0a20 2020  regations %}.   
-00001b40: 2020 2020 207b 2520 666f 7220 6167 6772       {% for aggr
-00001b50: 6567 6174 696f 6e20 696e 2064 6174 612e  egation in data.
-00001b60: 6d65 7461 6461 7461 2e61 6767 7265 6761  metadata.aggrega
-00001b70: 7469 6f6e 732e 7661 6c75 6573 2025 7d0a  tions.values %}.
-00001b80: 2020 2020 2020 2020 2020 2020 3c68 3320              <h3 
-00001b90: 7374 796c 653d 2266 6c6f 6174 3a72 6967  style="float:rig
-00001ba0: 6874 3b20 6d61 7267 696e 2d6c 6566 743a  ht; margin-left:
-00001bb0: 2032 3022 3e7b 7b20 6167 6772 6567 6174   20">{{ aggregat
-00001bc0: 696f 6e2e 6e61 6d65 207d 7d3a 207b 7b20  ion.name }}: {{ 
-00001bd0: 6167 6772 6567 6174 696f 6e2e 7661 6c75  aggregation.valu
-00001be0: 657c 666f 726d 6174 207d 7d3c 2f68 333e  e|format }}</h3>
-00001bf0: 0a20 2020 2020 2020 207b 2520 656e 6466  .        {% endf
-00001c00: 6f72 2025 7d0a 2020 2020 2020 2020 3c64  or %}.        <d
-00001c10: 6976 2063 6c61 7373 3d22 636c 6561 722d  iv class="clear-
-00001c20: 6669 7822 3e26 6e62 7370 3b3c 2f64 6976  fix">&nbsp;</div
-00001c30: 3e0a 2020 2020 7b25 2065 6e64 6966 2025  >.    {% endif %
-00001c40: 7d0a 0a20 2020 207b 2520 656e 6469 6620  }..    {% endif 
-00001c50: 257d 0a0a 2020 2020 7b25 2069 6620 6461  %}..    {% if da
-00001c60: 7461 2e74 656d 706c 6174 6520 257d 0a20  ta.template %}. 
-00001c70: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00001c80: 733d 2263 6c65 6172 2d66 6978 223e 266e  s="clear-fix">&n
-00001c90: 6273 703b 3c2f 6469 763e 0a20 2020 2020  bsp;</div>.     
-00001ca0: 2020 207b 2520 696e 636c 7564 6520 6461     {% include da
-00001cb0: 7461 2e74 656d 706c 6174 6520 7769 7468  ta.template with
-00001cc0: 2064 6174 613d 6461 7461 2025 7d0a 2020   data=data %}.  
-00001cd0: 2020 7b25 2065 6c73 6520 257d 0a20 2020    {% else %}.   
-00001ce0: 2020 2020 207b 2520 696e 636c 7564 6520       {% include 
-00001cf0: 2271 7565 7279 7365 742f 6461 7461 7461  "queryset/datata
-00001d00: 626c 652e 6874 6d6c 2220 7769 7468 2064  ble.html" with d
-00001d10: 6174 613d 6461 7461 2025 7d0a 2020 2020  ata=data %}.    
-00001d20: 7b25 2065 6e64 6966 2025 7d0a 2020 2020  {% endif %}.    
-00001d30: 7b25 2069 6e63 6c75 6465 2022 7175 6572  {% include "quer
-00001d40: 7973 6574 2f61 6374 696f 6e73 2f62 6174  yset/actions/bat
-00001d50: 6368 2e68 746d 6c22 2025 7d0a 2020 2020  ch.html" %}.    
-00001d60: 7b25 2069 6620 6461 7461 2e6d 6574 6164  {% if data.metad
-00001d70: 6174 612e 7061 6769 6e61 7469 6f6e 2e70  ata.pagination.p
-00001d80: 6167 6573 7c6c 656e 6774 6820 3e20 3120  ages|length > 1 
-00001d90: 616e 6420 6e6f 7420 6461 7461 2e6d 6574  and not data.met
-00001da0: 6164 6174 612e 7363 726f 6c6c 6162 6c65  adata.scrollable
-00001db0: 2025 7d0a 0a20 2020 2020 2020 203c 6e61   %}..        <na
-00001dc0: 7620 6172 6961 2d6c 6162 656c 3d22 5061  v aria-label="Pa
-00001dd0: 6769 6e61 c3a7 c3a3 6f22 3e0a 2020 2020  gina....o">.    
-00001de0: 2020 3c75 6c20 636c 6173 733d 2270 6167    <ul class="pag
-00001df0: 696e 6174 696f 6e22 2073 7479 6c65 3d22  ination" style="
-00001e00: 6f76 6572 666c 6f77 2d78 3a68 6964 6465  overflow-x:hidde
-00001e10: 6e22 3e0a 2020 2020 2020 2020 7b25 2066  n">.        {% f
-00001e20: 6f72 2070 6167 6520 696e 2064 6174 612e  or page in data.
-00001e30: 6d65 7461 6461 7461 2e70 6167 696e 6174  metadata.paginat
-00001e40: 696f 6e2e 7061 6765 7320 257d 0a20 2020  ion.pages %}.   
-00001e50: 2020 2020 2020 2020 7b25 2069 6620 666f          {% if fo
-00001e60: 726c 6f6f 702e 636f 756e 7465 727c 6164  rloop.counter|ad
-00001e70: 643a 3320 3d3d 2064 6174 612e 6d65 7461  d:3 == data.meta
-00001e80: 6461 7461 2e70 6167 696e 6174 696f 6e2e  data.pagination.
-00001e90: 7061 6765 737c 6c65 6e67 7468 2061 6e64  pages|length and
-00001ea0: 206e 6f74 2066 6f72 6c6f 6f70 2e63 6f75   not forloop.cou
-00001eb0: 6e74 6572 203d 3d20 3520 257d 0a20 2020  nter == 5 %}.   
-00001ec0: 2020 2020 2020 2020 203c 6c69 2063 6c61           <li cla
-00001ed0: 7373 3d22 7061 6765 2d69 7465 6d20 6469  ss="page-item di
-00001ee0: 7361 626c 6564 223e 0a20 2020 2020 2020  sabled">.       
-00001ef0: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
-00001f00: 2270 6167 652d 6c69 6e6b 2220 6872 6566  "page-link" href
-00001f10: 3d22 2322 2074 6162 696e 6465 783d 222d  ="#" tabindex="-
-00001f20: 3122 2061 7269 612d 6469 7361 626c 6564  1" aria-disabled
-00001f30: 3d22 7472 7565 223e 2e2e 2e3c 2f61 3e0a  ="true">...</a>.
-00001f40: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
-00001f50: 3e0a 2020 2020 2020 2020 2020 207b 2520  >.           {% 
-00001f60: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
-00001f70: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
-00001f80: 7061 6765 2d69 7465 6d20 7b25 2069 6620  page-item {% if 
-00001f90: 7061 6765 203d 3d20 6461 7461 2e6d 6574  page == data.met
-00001fa0: 6164 6174 612e 7061 6769 6e61 7469 6f6e  adata.pagination
-00001fb0: 2e70 6167 6520 257d 6163 7469 7665 7b25  .page %}active{%
-00001fc0: 2065 6e64 6966 2025 7d22 3e0a 2020 2020   endif %}">.    
-00001fd0: 2020 2020 2020 2020 2020 2020 3c61 2063              <a c
-00001fe0: 6c61 7373 3d22 7061 6765 2d6c 696e 6b22  lass="page-link"
-00001ff0: 2068 7265 663d 226a 6176 6173 6372 6970   href="javascrip
-00002000: 743a 2220 6f6e 636c 6963 6b3d 2224 2827  t:" onclick="$('
-00002010: 2370 6167 696e 6174 696f 6e2d 7b7b 2064  #pagination-{{ d
-00002020: 6174 612e 7575 6964 207d 7d27 292e 7661  ata.uuid }}').va
-00002030: 6c28 7b7b 2070 6167 657c 7374 7269 6e67  l({{ page|string
-00002040: 666f 726d 6174 3a27 7327 207d 7d29 3b72  format:'s' }});r
-00002050: 656c 6f61 647b 7b20 6461 7461 2e75 7569  eload{{ data.uui
-00002060: 6420 7d7d 2829 3b64 6f63 756d 656e 742e  d }}();document.
-00002070: 6765 7445 6c65 6d65 6e74 4279 4964 2827  getElementById('
-00002080: 7061 6769 6e61 7469 6f6e 2d69 6e66 6f2d  pagination-info-
-00002090: 7b7b 2064 6174 612e 7575 6964 207d 7d27  {{ data.uuid }}'
-000020a0: 292e 7363 726f 6c6c 496e 746f 5669 6577  ).scrollIntoView
-000020b0: 2829 3b22 3e0a 2020 2020 2020 2020 2020  ();">.          
-000020c0: 2020 2020 2020 2020 2020 7b7b 2070 6167            {{ pag
-000020d0: 6520 7d7d 0a20 2020 2020 2020 2020 2020  e }}.           
-000020e0: 2020 2020 203c 2f61 3e0a 2020 2020 2020       </a>.      
-000020f0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
-00002100: 2020 2020 2020 7b25 2069 6620 666f 726c        {% if forl
-00002110: 6f6f 702e 636f 756e 7465 7220 3d3d 2034  oop.counter == 4
-00002120: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00002130: 3c6c 6920 636c 6173 733d 2270 6167 652d  <li class="page-
-00002140: 6974 656d 2064 6973 6162 6c65 6422 3e0a  item disabled">.
-00002150: 2020 2020 2020 2020 2020 2020 2020 3c61                <a
-00002160: 2063 6c61 7373 3d22 7061 6765 2d6c 696e   class="page-lin
-00002170: 6b22 2068 7265 663d 2223 2220 7461 6269  k" href="#" tabi
-00002180: 6e64 6578 3d22 2d31 2220 6172 6961 2d64  ndex="-1" aria-d
-00002190: 6973 6162 6c65 643d 2274 7275 6522 3e2e  isabled="true">.
-000021a0: 2e2e 3c2f 613e 0a20 2020 2020 2020 2020  ..</a>.         
-000021b0: 2020 203c 2f6c 693e 0a20 2020 2020 2020     </li>.       
-000021c0: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-000021d0: 2020 2020 2020 207b 2520 656e 6466 6f72         {% endfor
-000021e0: 2025 7d0a 2020 2020 2020 3c2f 756c 3e0a   %}.      </ul>.
-000021f0: 2020 2020 3c2f 6e61 763e 0a20 2020 207b      </nav>.    {
-00002200: 2520 656e 6469 6620 257d 0a20 2020 2020  % endif %}.     
-00002210: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00002220: 2020 3c2f 6469 763e 0a20 2020 203c 2f64    </div>.    </d
-00002230: 6976 3e0a 3c2f 6469 763e 0a7b 2520 6966  iv>.</div>.{% if
-00002240: 2064 6174 612e 6d65 7461 6461 7461 2e73   data.metadata.s
-00002250: 6372 6f6c 6c61 626c 6520 257d 0a20 2020  crollable %}.   
-00002260: 207b 2520 696e 636c 7564 6520 2271 7565   {% include "que
-00002270: 7279 7365 742f 7363 726f 6c6c 2e68 746d  ryset/scroll.htm
-00002280: 6c22 2025 7d0a 7b25 2065 6e64 6966 2025  l" %}.{% endif %
-00002290: 7d0a 3c2f 6469 763e 0a                   }.</div>.
+00000ce0: 2020 2020 2020 2020 7375 6363 6573 733a          success:
+00000cf0: 6675 6e63 7469 6f6e 2820 6874 6d6c 2029  function( html )
+00000d00: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000d10: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00000d20: 2827 237b 7b20 6461 7461 2e6b 6579 207d  ('#{{ data.key }
+00000d30: 7d27 292e 6874 6d6c 2824 2868 746d 6c29  }').html($(html)
+00000d40: 2e66 696e 6428 2723 7b7b 2064 6174 612e  .find('#{{ data.
+00000d50: 6b65 7920 7d7d 2729 2e68 746d 6c28 2929  key }}').html())
+00000d60: 2e69 6e69 7469 616c 697a 6528 293b 0a20  .initialize();. 
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2020 2020 2024 2864 6f63             $(doc
+00000d90: 756d 656e 742e 626f 6479 292e 7265 6d6f  ument.body).remo
+00000da0: 7665 436c 6173 7328 2770 6167 652d 6c6f  veClass('page-lo
+00000db0: 6164 696e 6727 293b 0a20 2020 2020 2020  ading');.       
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000dd0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00000de0: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
+00000df0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000e00: 2020 2020 2020 2020 2020 2020 2066 756e               fun
+00000e10: 6374 696f 6e20 746f 6767 6c65 4163 7469  ction toggleActi
+00000e20: 6f6e 737b 7b20 6461 7461 2e75 7569 6420  ons{{ data.uuid 
+00000e30: 7d7d 2869 6e70 7574 297b 0a20 2020 2020  }}(input){.     
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000e50: 6628 696e 7075 742e 7661 6c75 653d 3d27  f(input.value=='
+00000e60: 2729 2024 2827 2371 7565 7279 7365 742d  ') $('#queryset-
+00000e70: 7b7b 2064 6174 612e 7575 6964 207d 7d27  {{ data.uuid }}'
+00000e80: 292e 6669 6e64 2827 2e61 6374 696f 6e2d  ).find('.action-
+00000e90: 6368 6563 6b62 6f78 2729 2e70 726f 7028  checkbox').prop(
+00000ea0: 2763 6865 636b 6564 272c 2069 6e70 7574  'checked', input
+00000eb0: 2e63 6865 636b 6564 293b 0a20 2020 2020  .checked);.     
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000ed0: 6628 2428 2723 7175 6572 7973 6574 2d7b  f($('#queryset-{
+00000ee0: 7b20 6461 7461 2e75 7569 6420 7d7d 2729  { data.uuid }}')
+00000ef0: 2e66 696e 6428 272e 6163 7469 6f6e 2d63  .find('.action-c
+00000f00: 6865 636b 626f 783a 6368 6563 6b65 6427  heckbox:checked'
+00000f10: 292e 6c65 6e67 7468 3e30 297b 0a20 2020  ).length>0){.   
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f30: 2020 2020 2024 2827 2371 7565 7279 7365       $('#queryse
+00000f40: 742d 7b7b 2064 6174 612e 7575 6964 207d  t-{{ data.uuid }
+00000f50: 7d27 292e 6669 6e64 2827 2e64 726f 7064  }').find('.dropd
+00000f60: 6f77 6e2d 746f 6767 6c65 2e71 7565 7279  own-toggle.query
+00000f70: 7365 7427 292e 7265 6d6f 7665 436c 6173  set').removeClas
+00000f80: 7328 2764 6973 6162 6c65 6427 293b 0a20  s('disabled');. 
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 2020 2020 2020 2024 2827 2371 7565 7279         $('#query
+00000fb0: 7365 742d 7b7b 2064 6174 612e 7575 6964  set-{{ data.uuid
+00000fc0: 207d 7d27 292e 6669 6e64 2827 2e64 726f   }}').find('.dro
+00000fd0: 7064 6f77 6e2d 746f 6767 6c65 2e69 6e73  pdown-toggle.ins
+00000fe0: 7461 6e63 652c 202e 6472 6f70 646f 776e  tance, .dropdown
+00000ff0: 2d74 6f67 676c 652e 6d6f 6465 6c27 292e  -toggle.model').
+00001000: 6164 6443 6c61 7373 2827 6469 7361 626c  addClass('disabl
+00001010: 6564 2729 3b0a 2020 2020 2020 2020 2020  ed');.          
+00001020: 2020 2020 2020 2020 2020 2020 2020 2428                $(
+00001030: 2723 7175 6572 7973 6574 2d7b 7b20 6461  '#queryset-{{ da
+00001040: 7461 2e75 7569 6420 7d7d 2729 2e66 696e  ta.uuid }}').fin
+00001050: 6428 272e 6274 6e2e 696e 7374 616e 6365  d('.btn.instance
+00001060: 2c20 2e62 746e 2e6d 6f64 656c 2729 2e61  , .btn.model').a
+00001070: 6464 436c 6173 7328 2764 6973 6162 6c65  ddClass('disable
+00001080: 6427 293b 0a20 2020 2020 2020 2020 2020  d');.           
+00001090: 2020 2020 2020 2020 2020 2020 2024 2827               $('
+000010a0: 2371 7565 7279 7365 742d 7b7b 2064 6174  #queryset-{{ dat
+000010b0: 612e 7575 6964 207d 7d27 292e 6669 6e64  a.uuid }}').find
+000010c0: 2827 2e62 746e 2e71 7565 7279 7365 7427  ('.btn.queryset'
+000010d0: 292e 7265 6d6f 7665 436c 6173 7328 2764  ).removeClass('d
+000010e0: 6973 6162 6c65 6427 293b 0a20 2020 2020  isabled');.     
+000010f0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001100: 2065 6c73 6520 7b0a 2020 2020 2020 2020   else {.        
+00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001120: 2428 2723 7175 6572 7973 6574 2d7b 7b20  $('#queryset-{{ 
+00001130: 6461 7461 2e75 7569 6420 7d7d 2729 2e66  data.uuid }}').f
+00001140: 696e 6428 272e 6472 6f70 646f 776e 2d74  ind('.dropdown-t
+00001150: 6f67 676c 652e 7175 6572 7973 6574 2729  oggle.queryset')
+00001160: 2e61 6464 436c 6173 7328 2764 6973 6162  .addClass('disab
+00001170: 6c65 6427 293b 0a20 2020 2020 2020 2020  led');.         
+00001180: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00001190: 2827 2371 7565 7279 7365 742d 7b7b 2064  ('#queryset-{{ d
+000011a0: 6174 612e 7575 6964 207d 7d27 292e 6669  ata.uuid }}').fi
+000011b0: 6e64 2827 2e64 726f 7064 6f77 6e2d 746f  nd('.dropdown-to
+000011c0: 6767 6c65 2e6d 6f64 656c 2c20 2e64 726f  ggle.model, .dro
+000011d0: 7064 6f77 6e2d 746f 6767 6c65 2e69 6e73  pdown-toggle.ins
+000011e0: 7461 6e63 6527 292e 7265 6d6f 7665 436c  tance').removeCl
+000011f0: 6173 7328 2764 6973 6162 6c65 6427 293b  ass('disabled');
+00001200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001210: 2020 2020 2020 2020 2024 2827 2371 7565           $('#que
+00001220: 7279 7365 742d 7b7b 2064 6174 612e 7575  ryset-{{ data.uu
+00001230: 6964 207d 7d27 292e 6669 6e64 2827 2e62  id }}').find('.b
+00001240: 746e 2e69 6e73 7461 6e63 652c 202e 6274  tn.instance, .bt
+00001250: 6e2e 6d6f 6465 6c27 292e 7265 6d6f 7665  n.model').remove
+00001260: 436c 6173 7328 2764 6973 6162 6c65 6427  Class('disabled'
+00001270: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00001280: 2020 2020 2020 2020 2020 2024 2827 2371             $('#q
+00001290: 7565 7279 7365 742d 7b7b 2064 6174 612e  ueryset-{{ data.
+000012a0: 7575 6964 207d 7d27 292e 6669 6e64 2827  uuid }}').find('
+000012b0: 2e62 746e 2e71 7565 7279 7365 7427 292e  .btn.queryset').
+000012c0: 6164 6443 6c61 7373 2827 6469 7361 626c  addClass('disabl
+000012d0: 6564 2729 3b0a 2020 2020 2020 2020 2020  ed');.          
+000012e0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000012f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001300: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+00001310: 6e63 7469 6f6e 2073 6c69 6465 5365 6172  nction slideSear
+00001320: 6368 416e 6446 696c 7465 7273 7b7b 2064  chAndFilters{{ d
+00001330: 6174 612e 7575 6964 207d 7d28 6129 7b0a  ata.uuid }}(a){.
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 6966 2861 2920 2428 6129 2e66      if(a) $(a).f
+00001360: 696e 6428 2769 3a6c 6173 742d 6368 696c  ind('i:last-chil
+00001370: 6427 292e 746f 6767 6c65 436c 6173 7328  d').toggleClass(
+00001380: 2762 692d 6368 6576 726f 6e2d 7570 2729  'bi-chevron-up')
+00001390: 2e74 6f67 676c 6543 6c61 7373 2827 6269  .toggleClass('bi
+000013a0: 2d63 6865 7672 6f6e 2d64 6f77 6e27 293b  -chevron-down');
+000013b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013c0: 2020 2020 2069 6628 2428 2723 666f 726d       if($('#form
+000013d0: 2d7b 7b20 6461 7461 2e75 7569 6420 7d7d  -{{ data.uuid }}
+000013e0: 2729 2e63 7373 2827 6469 7370 6c61 7927  ').css('display'
+000013f0: 2920 3d3d 2027 6e6f 6e65 2729 7b0a 2020  ) == 'none'){.  
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 2020 2020 2020 2428 2723 666f 726d 2d7b        $('#form-{
+00001420: 7b20 6461 7461 2e75 7569 6420 7d7d 2729  { data.uuid }}')
+00001430: 2e73 6c69 6465 446f 776e 2829 3b0a 2020  .slideDown();.  
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 2020 2428 2723 636f 6c6c 6170        $('#collap
+00001460: 7365 642d 7b7b 2064 6174 612e 7575 6964  sed-{{ data.uuid
+00001470: 207d 7d27 292e 7661 6c28 2222 293b 0a20   }}').val("");. 
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 207d 2065 6c73 6520 7b0a 2020 2020     } else {.    
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2020 2020 2428 2723 666f 726d 2d7b 7b20      $('#form-{{ 
+000014c0: 6461 7461 2e75 7569 6420 7d7d 2729 2e73  data.uuid }}').s
+000014d0: 6c69 6465 5570 2829 3b0a 2020 2020 2020  lideUp();.      
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2428 2723 636f 6c6c 6170 7365 642d    $('#collapsed-
+00001500: 7b7b 2064 6174 612e 7575 6964 207d 7d27  {{ data.uuid }}'
+00001510: 292e 7661 6c28 3129 3b0a 2020 2020 2020  ).val(1);.      
+00001520: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001550: 2020 6675 6e63 7469 6f6e 2074 7265 654e    function treeN
+00001560: 6f64 657b 7b20 6461 7461 2e75 7569 6420  ode{{ data.uuid 
+00001570: 7d7d 2869 6429 7b0a 2020 2020 2020 2020  }}(id){.        
+00001580: 2020 2020 2020 2020 2020 2020 2428 646f              $(do
+00001590: 6375 6d65 6e74 2e62 6f64 7929 2e61 6464  cument.body).add
+000015a0: 436c 6173 7328 2770 6167 652d 6c6f 6164  Class('page-load
+000015b0: 696e 6727 293b 0a20 2020 2020 2020 2020  ing');.         
+000015c0: 2020 2020 2020 2020 2020 2024 2827 2371             $('#q
+000015d0: 7565 7279 7365 742d 7b7b 2064 6174 612e  ueryset-{{ data.
+000015e0: 7575 6964 207d 7d27 292e 6669 6e64 2827  uuid }}').find('
+000015f0: 696e 7075 745b 6e61 6d65 3d74 7265 652d  input[name=tree-
+00001600: 6e6f 6465 5d27 292e 7661 6c28 6964 293b  node]').val(id);
+00001610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001620: 2020 2020 2024 2e61 6a61 7828 7b0a 2020       $.ajax({.  
+00001630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001640: 2020 2020 2020 7572 6c3a 277b 7b20 6461        url:'{{ da
+00001650: 7461 2e70 6174 687c 7361 6665 207d 7d3f  ta.path|safe }}?
+00001660: 7b7b 2072 6571 7565 7374 7c70 6f73 745f  {{ request|post_
+00001670: 7175 6572 7973 7472 696e 6720 7d7d 272c  querystring }}',
+00001680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001690: 2020 2020 2020 2020 2064 6174 613a 2024           data: $
+000016a0: 2827 2366 6f72 6d2d 7b7b 2064 6174 612e  ('#form-{{ data.
+000016b0: 7575 6964 207d 7d27 292e 7365 7269 616c  uuid }}').serial
+000016c0: 697a 6528 292c 0a20 2020 2020 2020 2020  ize(),.         
+000016d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000016e0: 7563 6365 7373 3a66 756e 6374 696f 6e28  uccess:function(
+000016f0: 2068 746d 6c20 2920 7b0a 2020 2020 2020   html ) {.      
+00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001710: 2020 2020 2020 2428 2723 7175 6572 7973        $('#querys
+00001720: 6574 2d64 6174 612d 7b7b 2064 6174 612e  et-data-{{ data.
+00001730: 7575 6964 207d 7d27 292e 6874 6d6c 2824  uuid }}').html($
+00001740: 2868 746d 6c29 2e66 696e 6428 2723 7175  (html).find('#qu
+00001750: 6572 7973 6574 2d64 6174 612d 7b7b 2064  eryset-data-{{ d
+00001760: 6174 612e 7575 6964 207d 7d27 292e 6874  ata.uuid }}').ht
+00001770: 6d6c 2829 292e 696e 6974 6961 6c69 7a65  ml()).initialize
+00001780: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2428 646f 6375 6d65 6e74 2e62 6f64 7929  $(document.body)
+000017b0: 2e72 656d 6f76 6543 6c61 7373 2827 7061  .removeClass('pa
+000017c0: 6765 2d6c 6f61 6469 6e67 2729 3b0a 2020  ge-loading');.  
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000017f0: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001820: 2020 6675 6e63 7469 6f6e 2069 6e69 7469    function initi
+00001830: 616c 697a 654e 6f64 657b 7b20 6461 7461  alizeNode{{ data
+00001840: 2e75 7569 6420 7d7d 2865 6c65 6d65 6e74  .uuid }}(element
+00001850: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
+00001860: 2020 2020 2020 2065 6c65 6d65 6e74 2e66         element.f
+00001870: 696e 6428 272e 7472 6565 2d6e 6f64 6527  ind('.tree-node'
+00001880: 292e 756e 6269 6e64 2829 2e72 656d 6f76  ).unbind().remov
+00001890: 6541 7474 7228 276f 6e63 6c69 636b 2729  eAttr('onclick')
+000018a0: 2e63 6c69 636b 2866 756e 6374 696f 6e28  .click(function(
+000018b0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
+000018c0: 2020 2020 2020 2020 2020 2076 6172 2075             var u
+000018d0: 6c20 3d20 2428 7468 6973 292e 7061 7265  l = $(this).pare
+000018e0: 6e74 2829 3b0a 0a20 2020 2020 2020 2020  nt();..         
+000018f0: 2020 2020 2020 2020 2020 2020 2020 2024                 $
+00001900: 2827 2371 7565 7279 7365 742d 7b7b 2064  ('#queryset-{{ d
+00001910: 6174 612e 7575 6964 207d 7d27 292e 6669  ata.uuid }}').fi
+00001920: 6e64 2827 2e74 7265 652d 6669 6c74 6572  nd('.tree-filter
+00001930: 202e 7472 6565 2d6e 6f64 6527 292e 7265   .tree-node').re
+00001940: 6d6f 7665 436c 6173 7328 2774 6578 742d  moveClass('text-
+00001950: 7072 696d 6172 7927 293b 0a20 2020 2020  primary');.     
+00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001970: 2020 2024 2e61 6a61 7828 7b0a 2020 2020     $.ajax({.    
+00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001990: 2020 2020 2020 2020 7572 6c3a 277b 7b20          url:'{{ 
+000019a0: 6461 7461 2e70 6174 687c 7361 6665 207d  data.path|safe }
+000019b0: 7d3f 7575 6964 3d7b 7b20 6461 7461 2e75  }?uuid={{ data.u
+000019c0: 7569 6420 7d7d 2674 7265 652d 6e6f 6465  uid }}&tree-node
+000019d0: 733d 272b 7468 6973 2e69 642b 2726 7b7b  s='+this.id+'&{{
+000019e0: 2072 6571 7565 7374 7c70 6f73 745f 7175   request|post_qu
+000019f0: 6572 7973 7472 696e 6720 7d7d 272c 0a20  erystring }}',. 
+00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a10: 2020 2020 2020 2020 2020 2073 7563 6365             succe
+00001a20: 7373 3a66 756e 6374 696f 6e28 2064 6174  ss:function( dat
+00001a30: 6120 2920 7b0a 2020 2020 2020 2020 2020  a ) {.          
+00001a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a50: 2020 2020 2020 7661 7220 6c69 7320 3d20        var lis = 
+00001a60: 6461 7461 2e69 7465 6d73 2e6d 6170 2866  data.items.map(f
+00001a70: 756e 6374 696f 6e28 6974 656d 297b 7265  unction(item){re
+00001a80: 7475 726e 2027 3c6c 693e 3c69 2063 6c61  turn '<li><i cla
+00001a90: 7373 3d22 6269 2062 692d 666f 6c64 6572  ss="bi bi-folder
+00001aa0: 3222 3e3c 2f69 3e3c 7370 616e 2063 6c61  2"></i><span cla
+00001ab0: 7373 3d22 7472 6565 2d6e 6f64 6522 2069  ss="tree-node" i
+00001ac0: 643d 2227 2b69 7465 6d2e 6964 2b27 223e  d="'+item.id+'">
+00001ad0: 2027 2b69 7465 6d2e 7465 7874 2b27 3c2f   '+item.text+'</
+00001ae0: 7370 616e 3e3c 2f6c 693e 277d 292e 6a6f  span></li>'}).jo
+00001af0: 696e 2827 2729 3b0a 0a20 2020 2020 2020  in('');..       
+00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b10: 2020 2020 2020 2020 2024 2827 3c75 6c3e           $('<ul>
+00001b20: 272b 6c69 732b 273c 2f75 6c3e 2729 2e68  '+lis+'</ul>').h
+00001b30: 6964 6528 292e 6170 7065 6e64 546f 2875  ide().appendTo(u
+00001b40: 6c29 2e73 6c69 6465 446f 776e 2822 736c  l).slideDown("sl
+00001b50: 6f77 2229 3b0a 2020 2020 2020 2020 2020  ow");.          
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
+00001b80: 4e6f 6465 7b7b 2064 6174 612e 7575 6964  Node{{ data.uuid
+00001b90: 207d 7d28 756c 293b 0a20 2020 2020 2020   }}(ul);.       
+00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bb0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001bd0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00001be0: 2020 2020 2020 2020 2020 2024 2875 6c29             $(ul)
+00001bf0: 2e70 6172 656e 7428 292e 6368 696c 6472  .parent().childr
+00001c00: 656e 2827 2e6f 7065 6e65 6427 292e 6368  en('.opened').ch
+00001c10: 696c 6472 656e 2827 756c 2729 2e73 6c69  ildren('ul').sli
+00001c20: 6465 5570 2820 2273 6c6f 7722 293b 0a20  deUp( "slow");. 
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 2020 2020 2020 2075 6c2e 6164 6443 6c61         ul.addCla
+00001c50: 7373 2827 6f70 656e 6564 2729 3b0a 2020  ss('opened');.  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c70: 2020 2020 2020 2428 7468 6973 292e 6164        $(this).ad
+00001c80: 6443 6c61 7373 2827 7465 7874 2d70 7269  dClass('text-pri
+00001c90: 6d61 7279 2729 3b0a 2020 2020 2020 2020  mary');.        
+00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cb0: 7472 6565 4e6f 6465 7b7b 2064 6174 612e  treeNode{{ data.
+00001cc0: 7575 6964 207d 7d28 7468 6973 2e69 6429  uuid }}(this.id)
+00001cd0: 3b0a 0a20 2020 2020 2020 2020 2020 2020  ;..             
+00001ce0: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
+00001cf0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00001d00: 2020 2020 2020 2020 2020 2020 2069 6e69               ini
+00001d10: 7469 616c 697a 654e 6f64 657b 7b20 6461  tializeNode{{ da
+00001d20: 7461 2e75 7569 6420 7d7d 2824 2827 2371  ta.uuid }}($('#q
+00001d30: 7565 7279 7365 742d 7b7b 2064 6174 612e  ueryset-{{ data.
+00001d40: 7575 6964 207d 7d27 2929 3b0a 2020 2020  uuid }}'));.    
+00001d50: 2020 2020 2020 2020 2020 2020 2428 2723              $('#
+00001d60: 7175 6572 7973 6574 2d67 6c6f 6261 6c2d  queryset-global-
+00001d70: 6163 7469 6f6e 732d 7b7b 2064 6174 612e  actions-{{ data.
+00001d80: 7575 6964 207d 7d27 292e 6669 6e64 2827  uuid }}').find('
+00001d90: 6127 292e 636c 6963 6b28 6675 6e63 7469  a').click(functi
+00001da0: 6f6e 2829 7b0a 2020 2020 2020 2020 2020  on(){.          
+00001db0: 2020 2020 2020 2020 2020 7661 7220 7061            var pa
+00001dc0: 7261 6d73 203d 2024 2827 2366 6f72 6d2d  rams = $('#form-
+00001dd0: 7b7b 2064 6174 612e 7575 6964 207d 7d27  {{ data.uuid }}'
+00001de0: 292e 7365 7269 616c 697a 6528 293b 0a20  ).serialize();. 
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 2020 2074 6869 732e 6872 6566 203d 2074     this.href = t
+00001e10: 6869 732e 6872 6566 2e73 706c 6974 2827  his.href.split('
+00001e20: 3f27 295b 305d 202b 2027 3f27 202b 2070  ?')[0] + '?' + p
+00001e30: 6172 616d 7320 2b20 2726 676c 6f62 616c  arams + '&global
+00001e40: 5f61 6374 696f 6e3d 3127 3b0a 2020 2020  _action=1';.    
+00001e50: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
+00001e60: 2020 2020 2020 2020 2020 2020 3c2f 7363              </sc
+00001e70: 7269 7074 3e0a 2020 2020 2020 2020 7b25  ript>.        {%
+00001e80: 2065 6e64 6966 2025 7d0a 0a20 2020 2020   endif %}..     
+00001e90: 2020 203c 6469 7620 636c 6173 733d 2271     <div class="q
+00001ea0: 7565 7279 7365 742d 6461 7461 2220 6964  ueryset-data" id
+00001eb0: 3d22 7175 6572 7973 6574 2d64 6174 612d  ="queryset-data-
+00001ec0: 7b7b 2064 6174 612e 7575 6964 207d 7d22  {{ data.uuid }}"
+00001ed0: 3e0a 0a20 2020 207b 2520 6966 2064 6174  >..    {% if dat
+00001ee0: 612e 6d65 7461 6461 7461 2e70 6167 696e  a.metadata.pagin
+00001ef0: 6174 696f 6e2e 746f 7461 6c20 6f72 2064  ation.total or d
+00001f00: 6174 612e 6d65 7461 6461 7461 2e63 616c  ata.metadata.cal
+00001f10: 656e 6461 7220 257d 0a20 2020 203c 6469  endar %}.    <di
+00001f20: 7620 636c 6173 733d 2263 6c65 6172 6669  v class="clearfi
+00001f30: 7822 2069 643d 2270 6167 696e 6174 696f  x" id="paginatio
+00001f40: 6e2d 696e 666f 2d7b 7b20 6461 7461 2e75  n-info-{{ data.u
+00001f50: 7569 6420 7d7d 223e 0a20 2020 2020 2020  uid }}">.       
+00001f60: 203c 6469 7620 636c 6173 733d 2266 6c6f   <div class="flo
+00001f70: 6174 2d73 7461 7274 223e 0a20 2020 2020  at-start">.     
+00001f80: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00001f90: 733d 226d 742d 3320 6d62 2d33 2220 7374  s="mt-3 mb-3" st
+00001fa0: 796c 653d 2266 6f6e 742d 7369 7a65 3a20  yle="font-size: 
+00001fb0: 3830 2522 3e0a 2020 2020 2020 2020 2020  80%">.          
+00001fc0: 2020 2020 2020 4578 6962 696e 646f 0a20        Exibindo. 
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00001fe0: 2520 6966 2064 6174 612e 6d65 7461 6461  % if data.metada
+00001ff0: 7461 2e70 6167 696e 6174 696f 6e2e 746f  ta.pagination.to
+00002000: 7461 6c20 3e20 6461 7461 2e6d 6574 6164  tal > data.metad
+00002010: 6174 612e 7061 6769 6e61 7469 6f6e 2e69  ata.pagination.i
+00002020: 6e74 6572 7661 6c2e 3120 257d 0a20 2020  nterval.1 %}.   
+00002030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002040: 207b 7b20 6461 7461 2e6d 6574 6164 6174   {{ data.metadat
+00002050: 612e 7061 6769 6e61 7469 6f6e 2e69 6e74  a.pagination.int
+00002060: 6572 7661 6c2e 3020 7d7d 202d 207b 7b20  erval.0 }} - {{ 
+00002070: 6461 7461 2e6d 6574 6164 6174 612e 7061  data.metadata.pa
+00002080: 6769 6e61 7469 6f6e 2e69 6e74 6572 7661  gination.interva
+00002090: 6c2e 3120 7d7d 2064 650a 2020 2020 2020  l.1 }} de.      
+000020a0: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
+000020b0: 6966 2025 7d0a 2020 2020 2020 2020 2020  if %}.          
+000020c0: 2020 2020 2020 3c73 7472 6f6e 673e 0a20        <strong>. 
+000020d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020e0: 2020 207b 7b20 6461 7461 2e6d 6574 6164     {{ data.metad
+000020f0: 6174 612e 7061 6769 6e61 7469 6f6e 2e74  ata.pagination.t
+00002100: 6f74 616c 207d 7d20 7265 6769 7374 726f  otal }} registro
+00002110: 7b25 2069 6620 6461 7461 2e6d 6574 6164  {% if data.metad
+00002120: 6174 612e 7061 6769 6e61 7469 6f6e 2e74  ata.pagination.t
+00002130: 6f74 616c 203e 2031 2025 7d73 7b25 2065  otal > 1 %}s{% e
+00002140: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00002150: 2020 2020 2020 2020 3c2f 7374 726f 6e67          </strong
+00002160: 3e0a 2020 2020 2020 2020 2020 2020 3c2f  >.            </
+00002170: 6469 763e 0a20 2020 2020 2020 203c 2f64  div>.        </d
+00002180: 6976 3e0a 2020 2020 2020 2020 3c64 6976  iv>.        <div
+00002190: 2063 6c61 7373 3d22 666c 6f61 742d 656e   class="float-en
+000021a0: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
+000021b0: 3c64 6976 2063 6c61 7373 3d22 6d74 2d33  <div class="mt-3
+000021c0: 206d 622d 3322 3e0a 2020 2020 2020 2020   mb-3">.        
+000021d0: 2020 2020 2020 2020 3c21 2d2d 3c61 2068          <!--<a h
+000021e0: 7265 663d 227b 7b20 6461 7461 2e70 6174  ref="{{ data.pat
+000021f0: 6820 7d7d 3f65 7870 6f72 743d 6373 7622  h }}?export=csv"
+00002200: 3e3c 6920 636c 6173 733d 2262 6920 6269  ><i class="bi bi
+00002210: 2d64 6f77 6e6c 6f61 6422 3e3c 2f69 3e3c  -download"></i><
+00002220: 2f61 3e2d 2d3e 0a20 2020 2020 2020 2020  /a>-->.         
+00002230: 2020 2020 2020 203c 212d 2d3c 6120 6872         <!--<a hr
+00002240: 6566 3d22 7b7b 2064 6174 612e 7061 7468  ef="{{ data.path
+00002250: 207d 7d3f 6578 706f 7274 3d78 6c73 223e   }}?export=xls">
+00002260: 3c69 2063 6c61 7373 3d22 6269 2062 692d  <i class="bi bi-
+00002270: 6669 6c65 2d65 7863 656c 223e 3c2f 693e  file-excel"></i>
+00002280: 3c2f 613e 2d2d 3e0a 2020 2020 2020 2020  </a>-->.        
+00002290: 2020 2020 2020 2020 3c21 2d2d 3c61 2068          <!--<a h
+000022a0: 7265 663d 227b 7b20 6461 7461 2e70 6174  ref="{{ data.pat
+000022b0: 6820 7d7d 3f65 7870 6f72 743d 7064 6622  h }}?export=pdf"
+000022c0: 3e3c 6920 636c 6173 733d 2262 6920 6269  ><i class="bi bi
+000022d0: 2d66 696c 652d 6561 726d 6172 6b2d 7064  -file-earmark-pd
+000022e0: 6622 3e3c 2f69 3e3c 2f61 3e2d 2d3e 0a20  f"></i></a>-->. 
+000022f0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002300: 2520 6966 2064 6174 612e 6d65 7461 6461  % if data.metada
+00002310: 7461 2e73 6561 7263 6820 6f72 2064 6174  ta.search or dat
+00002320: 612e 6d65 7461 6461 7461 2e66 696c 7465  a.metadata.filte
+00002330: 7273 2025 7d0a 2020 2020 2020 2020 2020  rs %}.          
+00002340: 2020 2020 2020 3c61 2068 7265 663d 226a        <a href="j
+00002350: 6176 6173 6372 6970 743a 223e 3c69 2063  avascript:"><i c
+00002360: 6c61 7373 3d22 6269 2062 692d 6675 6e6e  lass="bi bi-funn
+00002370: 656c 2220 6f6e 636c 6963 6b3d 2273 6c69  el" onclick="sli
+00002380: 6465 5365 6172 6368 416e 6446 696c 7465  deSearchAndFilte
+00002390: 7273 7b7b 2064 6174 612e 7575 6964 207d  rs{{ data.uuid }
+000023a0: 7d28 2922 3e3c 2f69 3e3c 2f61 3e0a 2020  }()"></i></a>.  
+000023b0: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
+000023c0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+000023d0: 2020 2020 2020 2020 2020 3c61 2068 7265            <a hre
+000023e0: 663d 226a 6176 6173 6372 6970 743a 223e  f="javascript:">
+000023f0: 3c69 2063 6c61 7373 3d22 6269 2062 692d  <i class="bi bi-
+00002400: 6172 726f 772d 636c 6f63 6b77 6973 6522  arrow-clockwise"
+00002410: 206f 6e63 6c69 636b 3d22 7265 6c6f 6164   onclick="reload
+00002420: 7b7b 2064 6174 612e 7575 6964 207d 7d28  {{ data.uuid }}(
+00002430: 293b 223e 3c2f 693e 3c2f 613e 0a20 2020  );"></i></a>.   
+00002440: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00002450: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00002460: 2020 203c 2f64 6976 3e0a 0a20 2020 207b     </div>..    {
+00002470: 2520 6966 2064 6174 612e 6d65 7461 6461  % if data.metada
+00002480: 7461 2e63 616c 656e 6461 7220 257d 0a20  ta.calendar %}. 
+00002490: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
+000024a0: 6520 2271 7565 7279 7365 742f 6361 6c65  e "queryset/cale
+000024b0: 6e64 6172 2e68 746d 6c22 2077 6974 6820  ndar.html" with 
+000024c0: 6461 7461 3d64 6174 6120 257d 0a20 2020  data=data %}.   
+000024d0: 207b 2520 656e 6469 6620 257d 0a0a 2020   {% endif %}..  
+000024e0: 2020 7b25 2069 6620 6461 7461 2e6d 6574    {% if data.met
+000024f0: 6164 6174 612e 6167 6772 6567 6174 696f  adata.aggregatio
+00002500: 6e73 2025 7d0a 2020 2020 2020 2020 7b25  ns %}.        {%
+00002510: 2066 6f72 2061 6767 7265 6761 7469 6f6e   for aggregation
+00002520: 2069 6e20 6461 7461 2e6d 6574 6164 6174   in data.metadat
+00002530: 612e 6167 6772 6567 6174 696f 6e73 2e76  a.aggregations.v
+00002540: 616c 7565 7320 257d 0a20 2020 2020 2020  alues %}.       
+00002550: 2020 2020 203c 6833 2073 7479 6c65 3d22       <h3 style="
+00002560: 666c 6f61 743a 7269 6768 743b 206d 6172  float:right; mar
+00002570: 6769 6e2d 6c65 6674 3a20 3230 223e 7b7b  gin-left: 20">{{
+00002580: 2061 6767 7265 6761 7469 6f6e 2e6e 616d   aggregation.nam
+00002590: 6520 7d7d 3a20 7b7b 2061 6767 7265 6761  e }}: {{ aggrega
+000025a0: 7469 6f6e 2e76 616c 7565 7c66 6f72 6d61  tion.value|forma
+000025b0: 7420 7d7d 3c2f 6833 3e0a 2020 2020 2020  t }}</h3>.      
+000025c0: 2020 7b25 2065 6e64 666f 7220 257d 0a20    {% endfor %}. 
+000025d0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000025e0: 733d 2263 6c65 6172 2d66 6978 223e 266e  s="clear-fix">&n
+000025f0: 6273 703b 3c2f 6469 763e 0a20 2020 207b  bsp;</div>.    {
+00002600: 2520 656e 6469 6620 257d 0a0a 2020 2020  % endif %}..    
+00002610: 7b25 2065 6e64 6966 2025 7d0a 0a20 2020  {% endif %}..   
+00002620: 207b 2520 6966 2064 6174 612e 7465 6d70   {% if data.temp
+00002630: 6c61 7465 2025 7d0a 2020 2020 2020 2020  late %}.        
+00002640: 3c64 6976 2063 6c61 7373 3d22 636c 6561  <div class="clea
+00002650: 722d 6669 7822 3e26 6e62 7370 3b3c 2f64  r-fix">&nbsp;</d
+00002660: 6976 3e0a 2020 2020 2020 2020 7b25 2069  iv>.        {% i
+00002670: 6e63 6c75 6465 2064 6174 612e 7465 6d70  nclude data.temp
+00002680: 6c61 7465 2077 6974 6820 6461 7461 3d64  late with data=d
+00002690: 6174 6120 257d 0a20 2020 207b 2520 656c  ata %}.    {% el
+000026a0: 7365 2025 7d0a 2020 2020 2020 2020 7b25  se %}.        {%
+000026b0: 2069 6e63 6c75 6465 2022 7175 6572 7973   include "querys
+000026c0: 6574 2f64 6174 6174 6162 6c65 2e68 746d  et/datatable.htm
+000026d0: 6c22 2077 6974 6820 6461 7461 3d64 6174  l" with data=dat
+000026e0: 6120 257d 0a20 2020 207b 2520 656e 6469  a %}.    {% endi
+000026f0: 6620 257d 0a20 2020 207b 2520 696e 636c  f %}.    {% incl
+00002700: 7564 6520 2271 7565 7279 7365 742f 6163  ude "queryset/ac
+00002710: 7469 6f6e 732f 6261 7463 682e 6874 6d6c  tions/batch.html
+00002720: 2220 257d 0a20 2020 207b 2520 6966 2064  " %}.    {% if d
+00002730: 6174 612e 6d65 7461 6461 7461 2e70 6167  ata.metadata.pag
+00002740: 696e 6174 696f 6e2e 7061 6765 737c 6c65  ination.pages|le
+00002750: 6e67 7468 203e 2031 2061 6e64 206e 6f74  ngth > 1 and not
+00002760: 2064 6174 612e 6d65 7461 6461 7461 2e73   data.metadata.s
+00002770: 6372 6f6c 6c61 626c 6520 257d 0a0a 2020  crollable %}..  
+00002780: 2020 2020 2020 3c6e 6176 2061 7269 612d        <nav aria-
+00002790: 6c61 6265 6c3d 2250 6167 696e 61c3 a7c3  label="Pagina...
+000027a0: a36f 223e 0a20 2020 2020 203c 756c 2063  .o">.      <ul c
+000027b0: 6c61 7373 3d22 7061 6769 6e61 7469 6f6e  lass="pagination
+000027c0: 2220 7374 796c 653d 226f 7665 7266 6c6f  " style="overflo
+000027d0: 772d 783a 6869 6464 656e 223e 0a20 2020  w-x:hidden">.   
+000027e0: 2020 2020 207b 2520 666f 7220 7061 6765       {% for page
+000027f0: 2069 6e20 6461 7461 2e6d 6574 6164 6174   in data.metadat
+00002800: 612e 7061 6769 6e61 7469 6f6e 2e70 6167  a.pagination.pag
+00002810: 6573 2025 7d0a 2020 2020 2020 2020 2020  es %}.          
+00002820: 207b 2520 6966 2066 6f72 6c6f 6f70 2e63   {% if forloop.c
+00002830: 6f75 6e74 6572 7c61 6464 3a33 203d 3d20  ounter|add:3 == 
+00002840: 6461 7461 2e6d 6574 6164 6174 612e 7061  data.metadata.pa
+00002850: 6769 6e61 7469 6f6e 2e70 6167 6573 7c6c  gination.pages|l
+00002860: 656e 6774 6820 616e 6420 6e6f 7420 666f  ength and not fo
+00002870: 726c 6f6f 702e 636f 756e 7465 7220 3d3d  rloop.counter ==
+00002880: 2035 2025 7d0a 2020 2020 2020 2020 2020   5 %}.          
+00002890: 2020 3c6c 6920 636c 6173 733d 2270 6167    <li class="pag
+000028a0: 652d 6974 656d 2064 6973 6162 6c65 6422  e-item disabled"
+000028b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000028c0: 3c61 2063 6c61 7373 3d22 7061 6765 2d6c  <a class="page-l
+000028d0: 696e 6b22 2068 7265 663d 2223 2220 7461  ink" href="#" ta
+000028e0: 6269 6e64 6578 3d22 2d31 2220 6172 6961  bindex="-1" aria
+000028f0: 2d64 6973 6162 6c65 643d 2274 7275 6522  -disabled="true"
+00002900: 3e2e 2e2e 3c2f 613e 0a20 2020 2020 2020  >...</a>.       
+00002910: 2020 2020 203c 2f6c 693e 0a20 2020 2020       </li>.     
+00002920: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+00002930: 7d0a 2020 2020 2020 2020 2020 2020 3c6c  }.            <l
+00002940: 6920 636c 6173 733d 2270 6167 652d 6974  i class="page-it
+00002950: 656d 207b 2520 6966 2070 6167 6520 3d3d  em {% if page ==
+00002960: 2064 6174 612e 6d65 7461 6461 7461 2e70   data.metadata.p
+00002970: 6167 696e 6174 696f 6e2e 7061 6765 2025  agination.page %
+00002980: 7d61 6374 6976 657b 2520 656e 6469 6620  }active{% endif 
+00002990: 257d 223e 0a20 2020 2020 2020 2020 2020  %}">.           
+000029a0: 2020 2020 203c 6120 636c 6173 733d 2270       <a class="p
+000029b0: 6167 652d 6c69 6e6b 2220 6872 6566 3d22  age-link" href="
+000029c0: 6a61 7661 7363 7269 7074 3a22 206f 6e63  javascript:" onc
+000029d0: 6c69 636b 3d22 2428 2723 7061 6769 6e61  lick="$('#pagina
+000029e0: 7469 6f6e 2d7b 7b20 6461 7461 2e75 7569  tion-{{ data.uui
+000029f0: 6420 7d7d 2729 2e76 616c 287b 7b20 7061  d }}').val({{ pa
+00002a00: 6765 7c73 7472 696e 6766 6f72 6d61 743a  ge|stringformat:
+00002a10: 2773 2720 7d7d 293b 7265 6c6f 6164 7b7b  's' }});reload{{
+00002a20: 2064 6174 612e 7575 6964 207d 7d28 293b   data.uuid }}();
+00002a30: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
+00002a40: 656e 7442 7949 6428 2770 6167 696e 6174  entById('paginat
+00002a50: 696f 6e2d 696e 666f 2d7b 7b20 6461 7461  ion-info-{{ data
+00002a60: 2e75 7569 6420 7d7d 2729 2e73 6372 6f6c  .uuid }}').scrol
+00002a70: 6c49 6e74 6f56 6965 7728 293b 223e 0a20  lIntoView();">. 
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 2020 207b 7b20 7061 6765 207d 7d0a 2020     {{ page }}.  
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00002ab0: 613e 0a20 2020 2020 2020 2020 2020 203c  a>.            <
+00002ac0: 2f6c 693e 0a20 2020 2020 2020 2020 207b  /li>.          {
+00002ad0: 2520 6966 2066 6f72 6c6f 6f70 2e63 6f75  % if forloop.cou
+00002ae0: 6e74 6572 203d 3d20 3420 257d 0a20 2020  nter == 4 %}.   
+00002af0: 2020 2020 2020 2020 203c 6c69 2063 6c61           <li cla
+00002b00: 7373 3d22 7061 6765 2d69 7465 6d20 6469  ss="page-item di
+00002b10: 7361 626c 6564 223e 0a20 2020 2020 2020  sabled">.       
+00002b20: 2020 2020 2020 203c 6120 636c 6173 733d         <a class=
+00002b30: 2270 6167 652d 6c69 6e6b 2220 6872 6566  "page-link" href
+00002b40: 3d22 2322 2074 6162 696e 6465 783d 222d  ="#" tabindex="-
+00002b50: 3122 2061 7269 612d 6469 7361 626c 6564  1" aria-disabled
+00002b60: 3d22 7472 7565 223e 2e2e 2e3c 2f61 3e0a  ="true">...</a>.
+00002b70: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
+00002b80: 3e0a 2020 2020 2020 2020 2020 7b25 2065  >.          {% e
+00002b90: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
+00002ba0: 7b25 2065 6e64 666f 7220 257d 0a20 2020  {% endfor %}.   
+00002bb0: 2020 203c 2f75 6c3e 0a20 2020 203c 2f6e     </ul>.    </n
+00002bc0: 6176 3e0a 2020 2020 7b25 2065 6e64 6966  av>.    {% endif
+00002bd0: 2025 7d0a 2020 2020 2020 2020 3c2f 6469   %}.        </di
+00002be0: 763e 0a20 2020 2020 2020 203c 2f64 6976  v>.        </div
+00002bf0: 3e0a 2020 2020 3c2f 6469 763e 0a3c 2f64  >.    </div>.</d
+00002c00: 6976 3e0a 7b25 2069 6620 6461 7461 2e6d  iv>.{% if data.m
+00002c10: 6574 6164 6174 612e 7363 726f 6c6c 6162  etadata.scrollab
+00002c20: 6c65 2025 7d0a 2020 2020 7b25 2069 6e63  le %}.    {% inc
+00002c30: 6c75 6465 2022 7175 6572 7973 6574 2f73  lude "queryset/s
+00002c40: 6372 6f6c 6c2e 6874 6d6c 2220 257d 0a7b  croll.html" %}.{
+00002c50: 2520 656e 6469 6620 257d 0a3c 2f64 6976  % endif %}.</div
+00002c60: 3e0a                                     >.
```

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.4/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.4/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.4/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.4/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.4/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.4/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.4/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.4/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.4/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.4/sloth/api/templates/valueset/valueset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.4/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/urls.py` & `sloth-framework-0.1.4/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/api/views.py` & `sloth-framework-0.1.4/sloth/api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from django.shortcuts import render
 from django.template.loader import render_to_string
 from django.views.decorators.csrf import csrf_exempt
 from ..actions import Action, ACTIONS, EXPOSE
 from .templatetags.tags import is_ajax
 from ..core.queryset import QuerySet
 from sloth.api.exceptions import JsonReadyResponseException, HtmlReadyResponseException, ReadyResponseException
-from .dashboard import Dashboards
+from .dashboard import Dashboards, Dashboard
 from .. import initialize
 
 
 initialize()
 
 
 def dashboard(request, path):
@@ -221,22 +221,26 @@
     for i, token in enumerate(tokens):
         if i == 0:
             allowed_attrs.extend(EXPOSE)
         if not request.user.is_authenticated and token not in allowed_attrs and token not in extra_attrs and not token.isdigit() and '-' not in token:
             print(token, type(obj).__name__, allowed_attrs, extra_attrs)
             raise PermissionDenied()
         if token.isdigit():
+            if isinstance(obj, Dashboard):
+                obj = obj.view()
             extra_attrs = obj.metadata['actions'] + obj.metadata['inline_actions'] + ['view' if view['name'] == 'self' else view['name'] for view in obj.metadata['view']]
             obj = obj.contextualize(request).apply_role_lookups(request.user).filter(pk=token).first()
             if obj:
                 instance = obj
                 instances = None
             else:
                 raise PermissionDenied()
         elif '-' in token:
+            if isinstance(obj, Dashboard):
+                obj = obj.view()
             extra_attrs = obj.metadata['batch_actions']
             obj = obj.contextualize(request).apply_role_lookups(request.user).filter(pk__in=token.split('-'))
             instance = None
             instances = obj
             queryset = obj
         elif token in ACTIONS or token in ('add', 'edit', 'delete'):
             if token in ('edit', 'delete') and instance is None and instances is None:
@@ -273,9 +277,11 @@
                 else:
                     instantiator = obj
                     obj = getattr(obj, token)()
                 if isinstance(obj, ValueSet):
                     instance = instantiator
                 if isinstance(obj, QuerySet):
                     queryset = obj
+                    if 'global_action' in request.GET:
+                        queryset = obj.process_request(request, uuid=token).apply_role_lookups(request.user)
         allowed_attrs = obj.get_allowed_attrs()
     return obj.contextualize(request).apply_role_lookups(request.user)
```

### Comparing `sloth-framework-0.1.3/sloth/cloud/printer.py` & `sloth-framework-0.1.4/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/cloud/server.py` & `sloth-framework-0.1.4/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/conf/settings.py` & `sloth-framework-0.1.4/sloth/conf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             'EMAIL': 'email',
             'FIRST_NAME': None,
             'LAST_NAME': None
         }
     }
 }
 
-if os.environ.get('USE_REDIS') == '1':
+if os.environ.get('REDIS_HOST'):
     REDIS_HOST = os.environ.get('REDIS_HOST', 'redis')
     REDIS_PORT = os.environ.get('REDIS_PORT', 6379)
     REDIS_PASSWORD = os.environ.get('REDIS_PASSWORD', None)
     SESSION_ENGINE = 'django.contrib.sessions.backends.cache'
     SESSION_CACHE_ALIAS = 'default'
     CACHES = {
         "default": {
@@ -70,14 +70,14 @@
             "OPTIONS": {
                 "CLIENT_CLASS": "django_redis.client.DefaultClient",
                 "PASSWORD": REDIS_PASSWORD
             }
         }
     }
 
-if os.environ.get('USE_POSTGRES') == '1':
+if os.environ.get('POSTGRES_HOST'):
     DATABASES['default']['ENGINE'] = 'django.db.backends.postgresql_psycopg2'
     DATABASES['default']['NAME'] = os.environ.get('DATABASE_NAME', 'database')
     DATABASES['default']['USER'] = os.environ.get('DATABASE_USER', 'postgres')
     DATABASES['default']['PASSWORD'] = os.environ.get('DATABASE_PASSWORD', 'password')
     DATABASES['default']['HOST'] = os.environ.get('DATABASE_HOST', 'postgres')
     DATABASES['default']['PORT'] = os.environ.get('DATABASE_PORT', '5432')
```

### Comparing `sloth-framework-0.1.3/sloth/core/base.py` & `sloth-framework-0.1.4/sloth/core/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from functools import lru_cache
 import types
 from django.apps import apps
 from django.conf import settings
-from django.core.exceptions import FieldDoesNotExist
+from django.core.exceptions import FieldDoesNotExist, ValidationError
 from django.template.loader import render_to_string
 
 from sloth.actions import Action, ACTIONS
 from sloth.core.valueset import ValueSet
 from sloth.core.queryset import QuerySet
 from sloth.utils import to_snake_case, to_camel_case, getattrr
 
@@ -123,53 +123,55 @@
         tuples = set()
         for role in self.__roles__:
             if ignore_active_condition or role['active'] is None or getattrr(self, role['active'])[1]:
                 lookups = list()
                 lookups.append(role['username'])
                 if role['email']:
                     lookups.append(role['email'])
-                if model.__name__.lower() not in role['scopes']:
-                    role['scopes']['self'] = 'id'
                 lookups.extend(role['scopes'].values())
                 if role['name'].islower():
                     lookups.append(role['name'])
                 values = model.objects.filter(pk=self.pk).values(*set(lookups))
                 for value in values:
                     username = value[role['username']]
                     email = value[role['email']] if role['email'] else None
                     if username:
+                        scope_name = value[role['name']] if role['name'].islower() else role['name']
+                        tuples.add((username, email, scope_name, None, None, None))
                         for scope_key, lookup in role['scopes'].items():
-                            scope_name = value[role['name']] if role['name'].islower() else role['name']
-                            scope_type = model if lookup in ('id', 'pk') else model.get_field(lookup).related_model
+                            scope_type = model if lookup in ('pk', 'id', 'self') else model.get_field(lookup).related_model
                             scope_value = value[lookup]
                             tuples.add((username, email, scope_name, scope_type, scope_key, scope_value))
+                    # else:
+                    #     raise ValidationError('O "login" do usuário ({}) deve ser informado.'.format(role['username'].upper().replace('__', '->')))
         # print('----- {} -----'.format(self))
         # for x in tuples: print(x)
         # print('\n\n')
         return tuples
 
     def sync_roles(self, role_tuples):
         from django.contrib.auth.models import User
         role = apps.get_model('api', 'Role')
         role_tuples2 = self.get_role_tuples()
         for username, email, scope_name, scope_type, scope_key, scope_value in role_tuples2:
-            if scope_value:
+            if username:
                 user_id = User.objects.filter(username=username).values_list('id', flat=True).first()
-                scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
                 if user_id is None:
                     user = User.objects.create(username=username)
                     if email:
                         user.email = email
                     default_password = settings.DEFAULT_PASSWORD(user)
                     user.set_password(default_password)
                     user.save()
                     user_id = user.id
                 role.objects.get_or_create(
                     user_id=user_id, name=scope_name,
-                    scope_type=scope_type,
+                    scope_type='{}.{}'.format(
+                        scope_type.metaclass().app_label, scope_type.metaclass().model_name
+                    ) if scope_type else None,
                     scope_key=scope_key, scope_value=scope_value
                 )
         deleted_role_tuples = role_tuples - role_tuples2
         # print('DELETED: ', deleted_role_tuples)
         for username, email, scope_name, scope_type, scope_key, scope_value in deleted_role_tuples:
             scope_type = '{}.{}'.format(scope_type.metaclass().app_label, scope_type.metaclass().model_name)
             role.objects.filter(
@@ -221,15 +223,17 @@
             class Edit(Action):
                 class Meta:
                     model = cls
                     verbose_name = 'Editar {}'.format(cls.metaclass().verbose_name)
                     submit_label = 'Editar'
                     icon = 'pencil'
                     style = 'primary'
-                    if hasattr(cls.metaclass(), 'fieldsets'):
+                    if hasattr(cls.metaclass(), 'edit_fieldsets'):
+                        fieldsets = cls.metaclass().edit_fieldsets
+                    elif hasattr(cls.metaclass(), 'fieldsets'):
                         fieldsets = cls.metaclass().fieldsets
 
                 def has_permission(self, user):
                     return user.is_superuser or self.instance.has_edit_permission(user) or self.instance.has_permission(user)
             return Edit
 
         class Edit(form_cls):
```

### Comparing `sloth-framework-0.1.3/sloth/core/queryset.py` & `sloth-framework-0.1.4/sloth/core/queryset.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,41 @@
 
     def reset(self):
         self.metadata = dict(uuid=uuid1().hex if self.model is None else self.model.__name__.lower(), subset=None,
             display=[], view=[], filters={}, dfilters={}, search=None,
             page=1, limit=20, interval='', total=0, ignore=[], only={}, is_admin=False, ordering=[],
             actions=[], attach=[], template=None, attr=None, source=None, aggregations=[], calendar=None,
             global_actions=[], batch_actions=[], inline_actions=[], lookups=[], collapsed=True, compact=False,
-            verbose_name=None, related_field=None, scrollable=False
+            verbose_name=None, related_field=None, scrollable=False, tree=None
         )
         if self.model and getattr(self.model.metaclass(), 'autouser', False):
             self.lookups(autouser='pk')
             self.ignore('autouser')
 
     def _clone(self):
         clone = super()._clone()
         clone.request = self.request
         clone.instantiator = self.instantiator
         clone.metadata = dict(self.metadata)
         return clone
 
+    def clone(self):
+        qs = self._clone()
+        for k, v in self.metadata.items():
+            v = self.metadata[k]
+            if isinstance(v, list):
+                qs.metadata[k] = list(v)
+            elif isinstance(v, dict):
+                qs.metadata[k] = dict(v)
+        return qs
+
+    def uuid(self, value):
+        self.metadata['uuid'] = value
+        return self
+
     def first(self):
         obj = super().first()
         if self.metadata['related_field'] and isinstance(obj, self.model):
             obj.related_field = self.metadata['related_field']
         return obj
 
     def related_field(self, name):
@@ -108,16 +122,19 @@
                 if not self.request.user.roles.contains(*role_names):
                     self.ignore(field_name)
         if self.metadata['lookups']:
             lookups = []
             for name, scopes in self.metadata['lookups']:
                 if scopes:
                     for scope_value_attr, scope_key in scopes.items():
-                        for scope_value in user.roles.filter(active=True, name=name, scope_key=scope_key).values_list('scope_value', flat=True):
-                            lookups.append(Q(**{scope_value_attr: scope_value}))
+                        if scope_key == 'username':
+                            lookups.append(Q(**{scope_value_attr: user.username}))
+                        else:
+                            for scope_value in user.roles.filter(active=True, name=name, scope_key=scope_key).values_list('scope_value', flat=True):
+                                lookups.append(Q(**{scope_value_attr: scope_value}))
                 else:
                     if user.roles.contains(name):
                         return self
             if lookups:
                 return self.filter(reduce(operator.__or__, lookups))
         return self.none() if self.metadata['is_admin'] else self
 
@@ -173,14 +190,16 @@
         filters = {}
         list_filter = self.get_list_filters()
         list_filter.extend(self.metadata['dfilters'])
         if self.metadata['calendar']:
             list_filter.append(self.metadata['calendar'])
         for lookup in list_filter:
             field = self.model.get_field(lookup)
+            if field is None:
+                raise Exception('Model {} can not have a filter named {}'.format(self.model, lookup))
             formfield = field.formfield()
             filter_type = 'choices'
             if isinstance(formfield, actions.BooleanField):
                 filter_type = 'boolean'
             elif isinstance(formfield, actions.DateTimeField):
                 filter_type = 'datetime'
             elif isinstance(formfield, actions.DateField):
@@ -209,15 +228,15 @@
             else:
                 filters[key] = dict(
                     key=lookup, name=name, type=filter_type, choices=None, hidden=False, value=self.request.GET.get(lookup) if self.request else None
                 )
             if as_form:
                 filters[key].update(formfield=formfield)
             if filter_type == 'boolean':
-                filters[key]['value'] = int(filters[key]['value']) if filters[key]['value'] else None
+                filters[key]['value'] = filters[key]['value'] if filters[key]['value'] else None
 
         ordering = []
         for lookup in self.metadata['ordering']:
             field = self.model.get_field(lookup)
             ordering.append(dict(id=lookup, text=field.verbose_name))
         if ordering:
             value = None
@@ -270,44 +289,60 @@
                 else:
                     attaches[name] = dict(
                         name=verbose_name, key=name, active=name == active
                     )
         self.metadata['attach'] = attaches
         return attaches
 
+    # tree function
+
+    def tree_nodes(self):
+        qs = self.model.objects.filter(**{self.metadata['tree']: self.request.GET['tree-nodes']})
+        qs.metadata = self.metadata
+        qs.request = self.request
+        return dict(items=[dict(id=value.id, text=str(value)) for value in qs])
+
     # choices function
 
     def choices(self, request):
+        items = []
         filter_lookup = request.GET['choices']
         q = request.GET.get('term')
         field = self.model.get_field(filter_lookup)
         values = self.apply_role_lookups(request.user).values_list(
             filter_lookup, flat=True
         ).order_by(filter_lookup).order_by(filter_lookup).distinct()
+        if field.null:
+            items.append(dict(id='null', text='Indefinido'))
         if field.related_model:
             qs = field.related_model.objects.filter(id__in=values)
             qs = qs.search(q=q) if q else qs
             qs = qs.distinct()
             total = values.count()
-            items = [dict(id=value.id, text=str(value)) for value in qs[0:25]]
+            items.extend([dict(id=value.id, text=str(value)) for value in qs[0:25]])
         else:
             total = values.count()
-            items = [dict(id=value, text=str(value)) for value in values]
+            items.extend([dict(id=value, text=str(value)) for value in values])
         return dict(
             total=total, page=1, pages=math.ceil((1.0 * total) / 25),
             q=q, items=items
         )
 
     # calendar
 
     def calendar(self, name):
         self.metadata['calendar'] = name
         return self
 
+    def tree(self, name):
+        self.metadata['tree'] = name
+        return self
+
     def to_calendar(self):
+        i = 0
         days = {}
         attr_name = self.metadata['calendar']
         start = self.request.GET.get('{}__gte'.format(attr_name))
         if start:
             start = datetime.datetime.strptime(start, '%d/%m/%Y').date()
         else:
             start = self.order_by(attr_name).values_list(attr_name, flat=True).first() or datetime.date.today()
@@ -401,15 +436,15 @@
     def get_obj_actions(self, obj):
         actions = []
         for form_name in self.metadata['actions']:
             form_cls = self.model.action_form_cls(form_name)
             if form_cls is None:
                 raise BaseException('Action does not exist: {}'.format(form_name))
             if self.request is None or form_cls.check_fake_permission(
-                    request=self.request, instance=obj
+                    request=self.request, instance=obj, instantiator=self.instantiator
             ):
                 actions.append(form_cls.get_api_name())
         return actions
 
     def serialize(self, path=None, wrap=False, lazy=False):
         if wrap:
             if self.metadata['verbose_name']:
@@ -459,14 +494,16 @@
                 data['metadata'].update(
                     search=search, display=display, filters=filters, pagination=pagination,
                     collapsed=collapsed, subset=subset,
                     compact=self.metadata['compact'], is_admin=self.metadata['is_admin']# , state=self.dumps()
                 )
                 if calendar:
                     data['metadata']['calendar'] = calendar
+                if self.metadata['tree']:
+                    data['metadata']['tree'] = self.metadata['tree']
 
                 if self.metadata['aggregations']:
                     aggregations = {}
                     for aggregation in self.metadata['aggregations']:
                         aggregations[aggregation] = dict(
                             name=pretty(self.get_attr_metadata(aggregation)[0]),
                             value=getattr(self, aggregation)()
@@ -480,29 +517,29 @@
                 for view in self.metadata['view']:
                     if view['name'] == 'self':
                         view_suffix = ''
                         view_name = 'Visualizar'
                     else:
                         view_suffix = '{}/'.format(view['name'])
                         view_name = pretty(self.model.get_attr_metadata(view['name'])[0])
-                    data['actions']['instance'].append(
+                    data['actions']['instance'].insert(0,
                         dict(
                             type='view', key=view['name'], name=view_name, submit=view_name, target='instance',
                             method='get', icon=view['icon'], style='primary', ajax=False,
                             modal=view['modal'], path='{}{{id}}/{}'.format((path or '').split('?')[0], view_suffix)
                         )
                     )
                 for action_type in ('global_actions', 'actions', 'batch_actions', 'inline_actions'):
                     target = dict(global_actions='model', actions='instance', batch_actions='queryset', inline_actions='inline')[action_type]
                     for form_name in self.metadata[action_type]:
                         if form_name == 'view':
                             continue
                         form_cls = self.model.action_form_cls(form_name)
                         has_permission = self.request is None or form_cls.check_fake_permission(
-                            request=self.request, instance=self.model(), instantiator=self._hints.get('instance')
+                            request=self.request, instance=self.model(), instantiator=self._hints.get('instance', self.instantiator)
                         )
                         if action_type == 'actions' or has_permission:
                             action_path = path
                             if self.request and self.request.GET.get('subset'):
                                 action_path = '{}{}/'.format(path, self.request.GET.get('subset'))
                             action = form_cls.get_metadata(path, target)
                             data['actions'][action['target']].append(action)
@@ -551,18 +588,31 @@
             else:
                 self.metadata['view'].clear()
         return self
 
     def view(self):
         return self.all()
 
-    def display(self, *names, add_default=False):
-        if add_default:
-            names = tuple(self.model.default_list_fields()) + names
-        self.metadata['display'] = list(names)
+    def display(self, *names, add_default=False, before=None, after=None):
+        if before or after:
+            display = []
+            for name in (self.metadata['display'] or self.model.default_list_fields()):
+                if name == before:
+                    display.extend(names)
+                    display.append(name)
+                elif name == after:
+                    display.append(name)
+                    display.extend(names)
+                else:
+                    display.append(name)
+            self.metadata['display'] = display
+        else:
+            if add_default:
+                names = tuple(self.model.default_list_fields()) + names
+            self.metadata['display'] = list(names)
         return self
 
     def search(self, *names, q=None):
         if q is not None:
             lookups = []
             for search_field in self.metadata['search'] or self.model.default_search_fields():
                 lookups.append(Q(**{'{}__icontains'.format(search_field): q}))
@@ -654,51 +704,59 @@
     def page(self, n):
         self.metadata['page'] = n
         return self
 
     # action functions
 
     def actions(self, *names, clear=False):
+        qs = self._clone()
+        qs.metadata['actions'] = qs.metadata['actions'].copy()
         if clear:
-            self.metadata['actions'].clear()
+            qs.metadata['actions'].clear()
         for name in names:
             if name == 'view':
-                self.metadata['view'].append(dict(name='self', modal=False, icon='search'))
-            elif to_snake_case(name) not in self.metadata['actions']:
-                self.metadata['actions'].append(to_snake_case(name))
-        return self
+                qs.metadata['view'] = self.metadata['view'].copy()
+                qs.metadata['view'].append(dict(name='self', modal=False, icon='search'))
+            elif to_snake_case(name) not in qs.metadata['actions']:
+                qs.metadata['actions'].append(to_snake_case(name))
+        return qs
 
     def global_actions(self, *names, clear=False):
+        qs = self._clone()
+        qs.metadata['global_actions'] = qs.metadata['global_actions'].copy()
         if clear:
-            self.metadata['global_actions'].clear()
-        self.metadata['global_actions'].extend(
-            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['global_actions']]
+            qs.metadata['global_actions'].clear()
+        qs.metadata['global_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in qs.metadata['global_actions']]
         )
-        return self
+        return qs
 
     def batch_actions(self, *names, clear=False):
+        qs = self._clone()
+        qs.metadata['batch_actions'] = qs.metadata['batch_actions'].copy()
         if clear:
-            self.metadata['batch_actions'].clear()
-        self.metadata['batch_actions'].extend(
-            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['batch_actions']]
+            qs.metadata['batch_actions'].clear()
+        qs.metadata['batch_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in qs.metadata['batch_actions']]
         )
-        return self
+        return qs
 
     def inline_actions(self, *names, clear=False):
+        qs = self._clone()
+        qs.metadata['inline_actions'] = qs.metadata['inline_actions'].copy()
         if clear:
-            self.metadata['inline_actions'].clear()
-        self.metadata['inline_actions'].extend(
-            [to_snake_case(name) for name in names if to_snake_case(name) not in self.metadata['inline_actions']]
+            qs.metadata['inline_actions'].clear()
+        q.metadata['inline_actions'].extend(
+            [to_snake_case(name) for name in names if to_snake_case(name) not in qs.metadata['inline_actions']]
         )
-        return self
+        return qs
 
     def default_actions(self):
         if self.metadata['attr'] is None:
-            self.actions('view', 'edit', 'delete')
-            self.global_actions('add')
+            return self.actions('view', 'edit', 'delete').global_actions('add')
         return self
 
     # search and pagination functions
 
     def get_ordering(self):
         ordering = self.request.GET.get('ordering') if self.request else None
         if ordering:
@@ -708,14 +766,17 @@
 
     def scrollable(self, flag=True):
         self.metadata['scrollable'] = flag
         return self.datatable()
 
     def paginate(self):
         qs = self
+        if self.metadata['tree']:
+            if not [child for child in qs.query.where.children if hasattr(child, 'lhs') and child.lhs.target.name == self.metadata['tree']]:
+                qs = qs.filter(**{'{}__isnull'.format(self.metadata['tree']): True})
         if self.metadata['calendar'] and 'selected-date' in self.request.GET:
             selected_date = self.request.GET['selected-date']
             if selected_date:
                 lookups = {
                     '{}__gte'.format(self.metadata['calendar']): datetime.datetime.strptime(selected_date, '%d/%m/%Y').date(),
                     '{}__lt'.format(self.metadata['calendar']): datetime.datetime.strptime(selected_date, '%d/%m/%Y').date() + datetime.timedelta(days=1)
                 }
@@ -766,28 +827,32 @@
         if request and request.user.is_superuser and 'autouser' in self.metadata['ignore']:
             self.metadata['ignore'].remove('autouser')
         if request and self.metadata['uuid'] == request.GET.get('uuid'):
             if 'choices' in request.GET:
                 raise JsonReadyResponseException(
                     self.process_request(request).choices(request)
                 )
+            if 'tree-nodes' in request.GET:
+                raise JsonReadyResponseException(
+                    self.process_request(request).tree_nodes()
+                )
             component = self.process_request(request).apply_role_lookups(request.user)
             if request.path.startswith('/app/'):
                 raise HtmlReadyResponseException(component.html())
             else:
                 meta = request.path.startswith('/meta/')
                 raise JsonReadyResponseException(component.serialize(wrap=meta))
             return self.apply_role_lookups(request.user)
         return self
 
-    def process_request(self, request):
+    def process_request(self, request, uuid=None):
         from sloth.core.valueset import ValueSet
         page = 1
         attr_name = request.GET.get('subset', 'all')
-        self.metadata['uuid'] = request.GET.get('uuid')
+        self.metadata['uuid'] = uuid or request.GET.get('uuid')
         if attr_name == 'all':
             attach = self
         else:
             attaches = self.get_attach()
             self.metadata['subset'] = attr_name
             attach = getattr(self._clone(), attr_name)()
             attach.metadata['attach'] = attaches
@@ -808,19 +873,34 @@
             if value:
                 if item['key'] == 'ordering':
                     qs = qs.order_by(value)
                 else:
                     if item['type'] in ('date', 'datetime'):
                         value = datetime.datetime.strptime(value, '%d/%m/%Y' if '/' in value else '%Y-%m-%d')
                     if item['type'] == 'boolean':
-                        value = bool(int(value)) if value.isdigit() else value == 'true'
+                        if value == 'true':
+                            value = True
+                        elif value == 'false':
+                            value = False
+                        elif value == 'null':
+                            value = None
+                    if item['type'] == 'choices':
+                        if value == 'null':
+                            value = None
                     if item['key'] != request.GET.get('choices'):
                         qs = qs.filter(**{item['key']: value})
-        if 'q' in request.GET:
+        if 'q' in request.GET and request.GET['q']:
             qs = qs.search(q=request.GET['q'])
+        if 'tree-node' in request.GET and request.GET['tree-node']:
+            qs = qs.model.objects.filter(**{self.metadata['tree']: request.GET['tree-node']})
+            if not qs.exists():
+                qs = qs.model.objects.filter(pk=request.GET['tree-node'])
+            qs.metadata = self.metadata
+            qs.request = self.request
+            qs.tree(None)
         if 'page' in request.GET:
             page = int(request.GET['page'] or 1)
         if isinstance(attach, QuerySet):
             # if request.GET.get('is_admin') and qs.metadata['attr'] is None and request.GET.get('subset') == 'all':
             #     qs.default_actions()
             qs = qs.page(page)
             # qs.debug()
```

### Comparing `sloth-framework-0.1.3/sloth/core/statistics.py` & `sloth-framework-0.1.4/sloth/core/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         self._yfield = None
         self._xdict = {}
         self._ydict = {}
         self._values_dict = None
         self.cursor = 0
         self.request = None
         self.metadata = dict(uuid='123456', attr=None, source=None, template='', verbose_name=None)
+        self.colors = {}
 
         if '__month' in x:
             self._xdict = {i + 1: month for i, month in enumerate(MONTHS)}
         if y and '__month' in y:
             self._ydict = {i + 1: month for i, month in enumerate(MONTHS)}
 
     def verbose_name(self, name):
@@ -91,14 +92,16 @@
         else:
             values_list = self.qs.values_list(self.x).annotate(self.func(self.z))
 
         self._xfield = self.qs.model.get_field(self.x.replace('__year', '').replace('__month', ''))
         if self._xdict == {}:
             xvalues = self.qs.values_list(self.x, flat=True).order_by(self.x).distinct()
             if self._xfield.related_model:
+                if hasattr(self._xfield.related_model, 'cor'):
+                    self.colors = {pk: color for pk, color in self._xfield.related_model.objects.values_list('id', 'cor')}
                 self._xdict = {
                     obj.pk: str(obj) for obj in self._xfield.related_model.objects.filter(pk__in=xvalues)
                 }
             else:
                 self._xdict = {
                     value: value for value in self.qs.values_list(self.x, flat=True)
                 }
@@ -166,15 +169,15 @@
                 return float(value) if isinstance(value, Decimal) else value
 
             if self._ydict:
                 for i, (yk, yv) in enumerate(self._ydict.items()):
                     data = []
                     self.cursor = 0
                     for j, (xk, xv) in enumerate(self._xdict.items()):
-                        data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, yk), 0)), self.nex_color()])
+                        data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, yk), 0)), self.nex_color(xk)])
                     series.update(**{formatter.get(yv, str(self._yfield_display_value(yv))): data})
                 ty = []
                 for k, serie in series.items():
                     sy = 0
                     ly = len(serie)
                     for i, item in enumerate(serie):
                         sy += item[1]
@@ -195,15 +198,15 @@
                 elif len(tx) > 1:
                     if len(tx) > 2: ty.append(sum(ty))
                     tx = []
             else:
                 sx = 0
                 data = list()
                 for j, (xk, xv) in enumerate(self._xdict.items()):
-                    data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, None), 0)), self.nex_color()])
+                    data.append([formatter.get(xv, str(self._xfield_display_value(xv))), format_value(self._values_dict.get((xk, None), 0)), self.nex_color(xk)])
                     sx+=data[-1][1]
                 if data:
                     series['default'] = data
                 tx = [sx]
         if self.request and path is None:
             prefix = self.request.path.split('/')[1]
             path = self.request.path.replace('/{}'.format(prefix), '')
@@ -289,15 +292,17 @@
 
     def bar_chart(self):
         return self.chart('bar')
 
     def column_chart(self):
         return self.chart('column')
 
-    def nex_color(self):
+    def nex_color(self, xk=None):
+        if self.colors and xk:
+            return self.colors[xk]
         color = colors()[self.cursor]
         self.cursor += 1
         if self.cursor == len(colors()):
             self.cursor = 0
         return color
 
     def has_permission(self, user):
```

### Comparing `sloth-framework-0.1.3/sloth/core/validation.py` & `sloth-framework-0.1.4/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/core/valueset.py` & `sloth-framework-0.1.4/sloth/core/valueset.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/db/models/__init__.py` & `sloth-framework-0.1.4/sloth/db/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,19 +172,21 @@
         field.widget.formatted = self.formatted
         return field
 
 
 class ForeignKey(ForeignKey):
     def __init__(self, to, on_delete=CASCADE, **kwargs):
         self.picker = kwargs.pop('picker', None)
+        self.addable = kwargs.pop('addable', False)
         self.username_lookup = kwargs.pop('username_lookup', None)
         super().__init__(to=to, on_delete=on_delete, **kwargs)
 
     def formfield(self, **kwargs):
         field = super().formfield(**kwargs)
+        field.addable = self.addable
         if self.picker:
             field.picker = self.picker
         if self.username_lookup:
             field.username_lookup = self.username_lookup
         return field
 
 
@@ -198,18 +200,20 @@
     def __init__(self, to, **kwargs):
         if hasattr(to, 'model'):
             self.queryset = to
             to = to.model
         else:
             self.queryset = None
         self.picker = kwargs.pop('picker', None)
+        self.addable = kwargs.pop('addable', False)
         super().__init__(to, **kwargs)
 
     def formfield(self, **kwargs):
         field = super().formfield(**kwargs)
+        field.addable = self.addable
         if self.picker:
             field.picker = self.picker
         if self.queryset:
             field.queryset = self.queryset
         return field
 
 
@@ -237,14 +241,19 @@
 
 class DecimalField(models.DecimalField):
     def __init__(self, *args, **kwargs):
         decimal_places = kwargs.pop('decimal_places', 2)
         max_digits = kwargs.pop('max_digits', 9)
         super().__init__(*args, decimal_places=decimal_places, max_digits=max_digits, **kwargs)
 
+    def formfield(self, **kwargs):
+        from ...actions import DecimalField
+        kwargs.update(form_class=DecimalField)
+        return super().formfield(**kwargs)
+
 
 class Decimal3Field(models.DecimalField):
     def __init__(self, *args, **kwargs):
         decimal_places = kwargs.pop('decimal_places', 3)
         max_digits = kwargs.pop('max_digits', 9)
         super().__init__(*args, decimal_places=decimal_places, max_digits=max_digits, **kwargs)
```

### Comparing `sloth-framework-0.1.3/sloth/test/__init__.py` & `sloth-framework-0.1.4/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.4/sloth/test/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/test/selenium/browser.py` & `sloth-framework-0.1.4/sloth/test/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/__init__.py` & `sloth-framework-0.1.4/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.4/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/http/__init__.py` & `sloth-framework-0.1.4/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.4/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.4/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.4/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth/utils/log/sql.py` & `sloth-framework-0.1.4/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.3/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.4/sloth_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.3
+Version: 0.1.4
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.3/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.4/sloth_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 sloth/api/templates/queryset/filter.html
 sloth/api/templates/queryset/filters.html
 sloth/api/templates/queryset/queryset.html
 sloth/api/templates/queryset/rows.html
 sloth/api/templates/queryset/scroll.html
 sloth/api/templates/queryset/statistics.html
 sloth/api/templates/queryset/timeline.html
+sloth/api/templates/queryset/tree.html
 sloth/api/templates/queryset/actions/actions.html
 sloth/api/templates/queryset/actions/batch.html
 sloth/api/templates/queryset/actions/global.html
 sloth/api/templates/renderers/badges/badge.html
 sloth/api/templates/renderers/badges/boolean.html
 sloth/api/templates/renderers/badges/danger.html
 sloth/api/templates/renderers/badges/primary.html
@@ -162,14 +163,15 @@
 sloth/api/templates/renderers/badges/warning.html
 sloth/api/templates/renderers/boolean/thumb.html
 sloth/api/templates/renderers/calendar/calendar.html
 sloth/api/templates/renderers/calendar/events.html
 sloth/api/templates/renderers/calendar/legend.html
 sloth/api/templates/renderers/documents/document.html
 sloth/api/templates/renderers/images/banner.html
+sloth/api/templates/renderers/images/group.html
 sloth/api/templates/renderers/images/image.html
 sloth/api/templates/renderers/images/round.html
 sloth/api/templates/renderers/links/file.html
 sloth/api/templates/renderers/links/url.html
 sloth/api/templates/renderers/maps/geolocation.html
 sloth/api/templates/renderers/maps/map.html
 sloth/api/templates/renderers/messages/custom.html
@@ -178,14 +180,16 @@
 sloth/api/templates/renderers/messages/primary.html
 sloth/api/templates/renderers/messages/success.html
 sloth/api/templates/renderers/messages/warning.html
 sloth/api/templates/renderers/photos/photo.html
 sloth/api/templates/renderers/photos/round.html
 sloth/api/templates/renderers/programing/strtable.html
 sloth/api/templates/renderers/programing/terminal.html
+sloth/api/templates/renderers/progress/primary.html
+sloth/api/templates/renderers/progress/success.html
 sloth/api/templates/renderers/tags/primary.html
 sloth/api/templates/renderers/tags/tags.html
 sloth/api/templates/renderers/utils/formatted.html
 sloth/api/templates/renderers/utils/progress.html
 sloth/api/templates/renderers/utils/qrcode.html
 sloth/api/templates/renderers/utils/steps.html
 sloth/api/templates/renderers/utils/table.html
@@ -208,15 +212,14 @@
 sloth/conf/settings.py
 sloth/core/__init__.py
 sloth/core/base.py
 sloth/core/queryset.py
 sloth/core/statistics.py
 sloth/core/validation.py
 sloth/core/valueset.py
-sloth/core/views.py
 sloth/db/__init__.py
 sloth/db/models/__init__.py
 sloth/test/__init__.py
 sloth/test/selenium/__init__.py
 sloth/test/selenium/browser.py
 sloth/utils/__init__.py
 sloth/utils/formatter/__init__.py
```

