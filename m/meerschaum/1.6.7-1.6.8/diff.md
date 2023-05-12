# Comparing `tmp/meerschaum-1.6.7.tar.gz` & `tmp/meerschaum-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerschaum-1.6.7.tar", last modified: Thu May 11 18:21:26 2023, max compression
+gzip compressed data, was "meerschaum-1.6.8.tar", last modified: Fri May 12 06:36:15 2023, max compression
```

## Comparing `meerschaum-1.6.7.tar` & `meerschaum-1.6.8.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.271268 meerschaum-1.6.7/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.7/LICENSE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.7/NOTICE
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-11 18:21:26.270268 meerschaum-1.6.7/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.7/README.md
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.254268 meerschaum-1.6.7/meerschaum/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.7/meerschaum/__main__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.254268 meerschaum-1.6.7/meerschaum/_internal/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.7/meerschaum/_internal/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.255268 meerschaum-1.6.7/meerschaum/_internal/arguments/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.7/meerschaum/_internal/arguments/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/_internal/arguments/_parse_arguments.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12624 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/_internal/arguments/_parser.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.255268 meerschaum-1.6.7/meerschaum/_internal/docs/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/_internal/docs/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/docs/index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/_internal/entry.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.255268 meerschaum-1.6.7/meerschaum/_internal/gui/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/gui/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.255268 meerschaum-1.6.7/meerschaum/_internal/gui/app/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/gui/app/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.7/meerschaum/_internal/gui/app/_windows.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/gui/app/actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/gui/app/pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.256268 meerschaum-1.6.7/meerschaum/_internal/shell/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/_internal/shell/Shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.7/meerschaum/_internal/shell/ShellCompleter.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.7/meerschaum/_internal/shell/ValidAutoSuggest.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/shell/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.256268 meerschaum-1.6.7/meerschaum/_internal/shell/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/_internal/shell/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.256268 meerschaum-1.6.7/meerschaum/_internal/term/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.7/meerschaum/_internal/term/TermPageHandler.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.7/meerschaum/_internal/term/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/_internal/term/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.258268 meerschaum-1.6.7/meerschaum/actions/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.7/meerschaum/actions/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/actions/api.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/actions/bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.7/meerschaum/actions/clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/actions/copy.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/actions/delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/actions/drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/actions/edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.7/meerschaum/actions/install.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/actions/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.7/meerschaum/actions/os.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/actions/python.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/actions/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/actions/reload.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/actions/setup.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.7/meerschaum/actions/sh.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.7/meerschaum/actions/show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/actions/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/actions/stack.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.7/meerschaum/actions/start.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.7/meerschaum/actions/stop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.7/meerschaum/actions/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.7/meerschaum/actions/uninstall.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.7/meerschaum/actions/upgrade.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.7/meerschaum/actions/verify.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.258268 meerschaum-1.6.7/meerschaum/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/api/_chain.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.7/meerschaum/api/_events.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.7/meerschaum/api/_oauth2.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.7/meerschaum/api/_websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.259268 meerschaum-1.6.7/meerschaum/api/dash/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.7/meerschaum/api/dash/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/dash/actions.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.260268 meerschaum-1.6.7/meerschaum/api/dash/assets/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/ansi_up.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/banner_1920x320.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/favicon.ico
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/logo_48x48.png
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/assets/logo_500x500.png
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.260268 meerschaum-1.6.7/meerschaum/api/dash/callbacks/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/callbacks/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/dash/callbacks/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.7/meerschaum/api/dash/callbacks/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/callbacks/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/api/dash/callbacks/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/dash/components.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/dash/connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/graphs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/dash/keys.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.260268 meerschaum-1.6.7/meerschaum/api/dash/pages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/dashboard.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/error.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/pages/register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.7/meerschaum/api/dash/pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.7/meerschaum/api/dash/users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/dash/websockets.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.261268 meerschaum-1.6.7/meerschaum/api/models/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/models/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/models/_interfaces.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/models/_locations.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/models/_metrics.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.7/meerschaum/api/models/_pipes.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.261268 meerschaum-1.6.7/meerschaum/api/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.261268 meerschaum-1.6.7/meerschaum/api/resources/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.261268 meerschaum-1.6.7/meerschaum/api/resources/static/css/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/css/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/css/bootstrap.min.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.7/meerschaum/api/resources/static/css/dash.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/css/dbc_dark.css
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/css/styles.css
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.261268 meerschaum-1.6.7/meerschaum/api/resources/static/ico/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/ico/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/ico/logo.ico
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.262268 meerschaum-1.6.7/meerschaum/api/resources/static/js/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/js/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/js/action_button.js
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/js/main.js
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.262268 meerschaum-1.6.7/meerschaum/api/resources/static/png/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/static/png/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.262268 meerschaum-1.6.7/meerschaum/api/resources/templates/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/templates/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/templates/index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/templates/old_index.html
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/resources/templates/secret.html
--rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.7/meerschaum/api/resources/templates/termpage.html
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.263268 meerschaum-1.6.7/meerschaum/api/routes/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/api/routes/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/api/routes/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/api/routes/_connectors.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/api/routes/_index.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/routes/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/routes/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.7/meerschaum/api/routes/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/routes/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/api/routes/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/api/routes/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.263268 meerschaum-1.6.7/meerschaum/api/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/api/tables/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.7/meerschaum/config/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.6.7/meerschaum/config/_default.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.7/meerschaum/config/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.7/meerschaum/config/_environment.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.7/meerschaum/config/_formatting.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/config/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.7/meerschaum/config/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/config/_paths.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/config/_preprocess.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.7/meerschaum/config/_read_config.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.7/meerschaum/config/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/config/_sync.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-05-11 18:21:19.000000 meerschaum-1.6.7/meerschaum/config/_version.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/config/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/stack/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/config/stack/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/stack/grafana/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.7/meerschaum/config/stack/grafana/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/stack/mosquitto/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/config/stack/mosquitto/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/stack/mosquitto/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/config/stack/mosquitto/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.264268 meerschaum-1.6.7/meerschaum/config/stack/resources/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/config/stack/resources/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.265268 meerschaum-1.6.7/meerschaum/config/static/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/config/static/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.265268 meerschaum-1.6.7/meerschaum/connectors/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/Connector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.266268 meerschaum-1.6.7/meerschaum/connectors/api/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/api/APIConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/connectors/api/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.7/meerschaum/connectors/api/_actions.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/connectors/api/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.7/meerschaum/connectors/api/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/connectors/api/_get.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.7/meerschaum/connectors/api/_login.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/connectors/api/_misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/connectors/api/_patch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.7/meerschaum/connectors/api/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.7/meerschaum/connectors/api/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/connectors/api/_post.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.7/meerschaum/connectors/api/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.7/meerschaum/connectors/api/_users.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.7/meerschaum/connectors/parse.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.266268 meerschaum-1.6.7/meerschaum/connectors/plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/connectors/plugin/PluginConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/connectors/plugin/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/poll.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.267268 meerschaum-1.6.7/meerschaum/connectors/sql/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/SQLConnector.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/connectors/sql/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_cli.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_create_engine.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11901 2023-05-05 21:44:39.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    88433 2023-05-09 02:50:23.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_plugins.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24635 2023-05-08 21:38:02.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_uri.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/_users.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.267268 meerschaum-1.6.7/meerschaum/connectors/sql/tables/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/connectors/sql/tables/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/connectors/sql/tables/types.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/connectors/sql/tools.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.267268 meerschaum-1.6.7/meerschaum/core/
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.268268 meerschaum-1.6.7/meerschaum/core/Pipe/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14991 2023-05-11 17:47:16.000000 meerschaum-1.6.7/meerschaum/core/Pipe/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_attributes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_bootstrap.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_clear.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6847 2022-11-13 04:57:20.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_data.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_delete.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_drop.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-05-08 21:38:02.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_dtypes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_edit.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2585 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_fetch.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_register.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_show.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25015 2023-05-11 17:47:16.000000 meerschaum-1.6.7/meerschaum/core/Pipe/_sync.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.268268 meerschaum-1.6.7/meerschaum/core/Plugin/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/core/Plugin/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.268268 meerschaum-1.6.7/meerschaum/core/User/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/core/User/_User.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/core/User/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.7/meerschaum/core/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.268268 meerschaum-1.6.7/meerschaum/plugins/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.7/meerschaum/plugins/_Plugin.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/plugins/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.269268 meerschaum-1.6.7/meerschaum/utils/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.7/meerschaum/utils/__init__.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.269268 meerschaum-1.6.7/meerschaum/utils/daemon/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/utils/daemon/Daemon.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.7/meerschaum/utils/daemon/Log.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.7/meerschaum/utils/daemon/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/utils/daemon/_names.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/utils/debug.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.270268 meerschaum-1.6.7/meerschaum/utils/formatting/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/utils/formatting/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/utils/formatting/_jobs.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/utils/formatting/_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.7/meerschaum/utils/formatting/_pprint.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/utils/formatting/_shell.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.7/meerschaum/utils/get_pipes.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.7/meerschaum/utils/interactive.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    61453 2023-05-08 21:38:02.000000 meerschaum-1.6.7/meerschaum/utils/misc.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.7/meerschaum/utils/networking.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.270268 meerschaum-1.6.7/meerschaum/utils/packages/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-05-08 21:38:02.000000 meerschaum-1.6.7/meerschaum/utils/packages/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-05-11 18:21:19.000000 meerschaum-1.6.7/meerschaum/utils/packages/_packages.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.7/meerschaum/utils/packages/lazy_loader.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.7/meerschaum/utils/pool.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/utils/process.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.7/meerschaum/utils/prompt.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.7/meerschaum/utils/schedule.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34688 2023-05-09 02:50:23.000000 meerschaum-1.6.7/meerschaum/utils/sql.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/utils/threading.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2517 2023-05-05 21:42:47.000000 meerschaum-1.6.7/meerschaum/utils/typing.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.270268 meerschaum-1.6.7/meerschaum/utils/venv/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.7/meerschaum/utils/venv/_Venv.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.7/meerschaum/utils/venv/__init__.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.7/meerschaum/utils/warnings.py
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.7/meerschaum/utils/yaml.py
-drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-11 18:21:26.254268 meerschaum-1.6.7/meerschaum.egg-info/
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/PKG-INFO
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/SOURCES.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/dependency_links.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/entry_points.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/requires.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/top_level.txt
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-11 18:21:26.000000 meerschaum-1.6.7/meerschaum.egg-info/zip-safe
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-05-11 18:21:26.271268 meerschaum-1.6.7/setup.cfg
--rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-05-11 18:21:19.000000 meerschaum-1.6.7/setup.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.390143 meerschaum-1.6.8/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11359 2021-12-27 13:50:47.000000 meerschaum-1.6.8/LICENSE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      114 2021-12-27 13:50:47.000000 meerschaum-1.6.8/NOTICE
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 06:36:15.389143 meerschaum-1.6.8/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9248 2022-07-13 02:48:08.000000 meerschaum-1.6.8/README.md
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.374143 meerschaum-1.6.8/meerschaum/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1236 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2774 2022-10-22 06:28:47.000000 meerschaum-1.6.8/meerschaum/__main__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      169 2022-04-23 01:15:00.000000 meerschaum-1.6.8/meerschaum/_internal/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/arguments/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      519 2022-10-22 06:25:53.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9741 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/_parse_arguments.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12375 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/_internal/arguments/_parser.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/docs/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      126 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/_internal/docs/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7719 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/docs/index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4625 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/_internal/entry.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum/_internal/gui/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1332 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/gui/app/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1565 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2632 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/_windows.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1016 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1678 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/gui/app/pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/shell/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    31489 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/_internal/shell/Shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2981 2022-10-22 06:28:01.000000 meerschaum-1.6.8/meerschaum/_internal/shell/ShellCompleter.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1280 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/_internal/shell/ValidAutoSuggest.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      281 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/shell/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/shell/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/_internal/shell/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.376143 meerschaum-1.6.8/meerschaum/_internal/term/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      612 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/_internal/term/TermPageHandler.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1495 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/_internal/term/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      788 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/_internal/term/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.378143 meerschaum-1.6.8/meerschaum/actions/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8129 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/actions/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10996 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/api.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14529 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4857 2022-08-23 06:14:42.000000 meerschaum-1.6.8/meerschaum/actions/clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6095 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/actions/copy.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15245 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2701 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/actions/drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9492 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7380 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/actions/install.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4206 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2251 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/actions/os.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2395 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/python.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11219 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/actions/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      605 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/reload.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3211 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/actions/setup.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2026 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/actions/sh.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    23468 2023-01-11 06:27:06.000000 meerschaum-1.6.8/meerschaum/actions/show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4224 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/actions/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5501 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/actions/stack.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18247 2022-11-22 01:55:36.000000 meerschaum-1.6.8/meerschaum/actions/start.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3948 2023-01-16 21:21:28.000000 meerschaum-1.6.8/meerschaum/actions/stop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15339 2022-12-15 02:09:06.000000 meerschaum-1.6.8/meerschaum/actions/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6073 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/actions/uninstall.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6307 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/actions/upgrade.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3348 2022-10-26 04:20:20.000000 meerschaum-1.6.8/meerschaum/actions/verify.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.378143 meerschaum-1.6.8/meerschaum/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7638 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      875 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/_chain.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      966 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/api/_events.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/api/_oauth2.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1226 2022-11-05 03:38:45.000000 meerschaum-1.6.8/meerschaum/api/_websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.379143 meerschaum-1.6.8/meerschaum/api/dash/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2238 2023-01-09 08:57:26.000000 meerschaum-1.6.8/meerschaum/api/dash/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9600 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/actions.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.380143 meerschaum-1.6.8/meerschaum/api/dash/assets/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21923 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/ansi_up.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   338636 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/banner_1920x320.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/favicon.ico
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10218 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/logo_48x48.png
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    67702 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/assets/logo_500x500.png
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/dash/callbacks/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      283 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24874 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2529 2023-01-09 09:04:18.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2777 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3446 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/api/dash/callbacks/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6771 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/components.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      843 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/dash/connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2072 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/graphs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3544 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13682 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/keys.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/dash/pages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      273 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3838 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/dashboard.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      598 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/error.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4601 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1425 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2398 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/pages/register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15039 2022-10-31 14:15:34.000000 meerschaum-1.6.8/meerschaum/api/dash/pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3054 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      504 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      886 2022-07-26 06:45:25.000000 meerschaum-1.6.8/meerschaum/api/dash/users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      924 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/dash/websockets.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/models/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      276 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      263 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_interfaces.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      304 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_locations.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      295 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/models/_metrics.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      463 2021-11-20 21:54:59.000000 meerschaum-1.6.8/meerschaum/api/models/_pipes.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      115 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.381143 meerschaum-1.6.8/meerschaum/api/resources/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/css/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)   180286 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/bootstrap.min.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1592 2022-10-31 13:18:31.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/dash.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6087 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/dbc_dark.css
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       81 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/css/styles.css
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/ico/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/ico/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9662 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/ico/logo.ico
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.382143 meerschaum-1.6.8/meerschaum/api/resources/static/js/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      540 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/action_button.js
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/js/main.js
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/resources/static/png/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/static/png/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/resources/templates/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1019 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1711 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/old_index.html
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      141 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/secret.html
+-rwxr-xr-x   0 bmeares   (1000) bmeares   (1000)     2082 2021-12-09 07:32:03.000000 meerschaum-1.6.8/meerschaum/api/resources/templates/termpage.html
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/routes/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      734 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/api/routes/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1803 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_connectors.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      578 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/routes/_index.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1882 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1702 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    21169 2023-01-21 08:00:50.000000 meerschaum-1.6.8/meerschaum/api/routes/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6152 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7239 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/api/routes/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      825 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/api/routes/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.383143 meerschaum-1.6.8/meerschaum/api/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      615 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/api/tables/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11629 2023-01-11 04:28:52.000000 meerschaum-1.6.8/meerschaum/config/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5135 2023-05-05 04:35:54.000000 meerschaum-1.6.8/meerschaum/config/_default.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8807 2022-07-13 02:48:16.000000 meerschaum-1.6.8/meerschaum/config/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4507 2022-10-22 07:29:33.000000 meerschaum-1.6.8/meerschaum/config/_environment.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5556 2022-05-02 19:58:56.000000 meerschaum-1.6.8/meerschaum/config/_formatting.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      647 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1508 2023-01-11 05:57:34.000000 meerschaum-1.6.8/meerschaum/config/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6648 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/_paths.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1220 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/config/_preprocess.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    14567 2022-10-14 04:34:51.000000 meerschaum-1.6.8/meerschaum/config/_read_config.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3589 2021-11-21 05:32:46.000000 meerschaum-1.6.8/meerschaum/config/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4968 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/config/_sync.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       71 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/config/_version.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8233 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/config/stack/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/grafana/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2010 2022-11-01 03:52:40.000000 meerschaum-1.6.8/meerschaum/config/stack/grafana/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      186 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.384142 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/mosquitto/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/config/stack/resources/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        0 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/config/stack/resources/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/config/static/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3679 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/config/static/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.385143 meerschaum-1.6.8/meerschaum/connectors/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6381 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/Connector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12064 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/api/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4022 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/APIConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      205 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/api/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2759 2022-10-22 06:21:34.000000 meerschaum-1.6.8/meerschaum/connectors/api/_actions.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      945 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2056 2022-11-01 03:12:07.000000 meerschaum-1.6.8/meerschaum/connectors/api/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1572 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_get.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2054 2022-11-18 03:44:05.000000 meerschaum-1.6.8/meerschaum/connectors/api/_login.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1185 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/_misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      933 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_patch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    19986 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/connectors/api/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5227 2022-06-27 01:07:31.000000 meerschaum-1.6.8/meerschaum/connectors/api/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      922 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/connectors/api/_post.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1489 2022-07-25 06:37:48.000000 meerschaum-1.6.8/meerschaum/connectors/api/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5303 2022-08-19 04:59:44.000000 meerschaum-1.6.8/meerschaum/connectors/api/_users.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4048 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/connectors/parse.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2084 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/connectors/plugin/PluginConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      198 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/plugin/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7215 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/poll.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.386143 meerschaum-1.6.8/meerschaum/connectors/sql/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8592 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/SQLConnector.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      175 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/connectors/sql/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3495 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_cli.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10197 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_create_engine.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12650 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    88433 2023-05-09 02:50:23.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7921 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_plugins.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    26869 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3312 2022-10-18 01:38:49.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_uri.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9972 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/_users.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/connectors/sql/tables/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6482 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tables/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1573 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tables/types.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      187 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/connectors/sql/tools.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/Pipe/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    15032 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    13202 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_attributes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7613 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_bootstrap.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2112 2022-11-13 04:57:20.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_clear.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10716 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_data.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1854 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_delete.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1052 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_drop.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3146 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_dtypes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8471 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_edit.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2877 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_fetch.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2240 2023-01-16 21:21:28.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_register.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1352 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_show.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    25706 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/core/Pipe/_sync.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/Plugin/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      137 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/Plugin/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.387143 meerschaum-1.6.8/meerschaum/core/User/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2362 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/User/_User.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      161 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/User/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      251 2022-04-24 10:29:36.000000 meerschaum-1.6.8/meerschaum/core/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.388142 meerschaum-1.6.8/meerschaum/plugins/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    33813 2023-01-21 08:00:50.000000 meerschaum-1.6.8/meerschaum/plugins/_Plugin.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    18398 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/plugins/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.388142 meerschaum-1.6.8/meerschaum/utils/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)      444 2021-11-08 16:07:48.000000 meerschaum-1.6.8/meerschaum/utils/__init__.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/daemon/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    24801 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/daemon/Daemon.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3170 2023-01-09 03:01:33.000000 meerschaum-1.6.8/meerschaum/utils/daemon/Log.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     5355 2023-01-09 09:50:51.000000 meerschaum-1.6.8/meerschaum/utils/daemon/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4302 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/daemon/_names.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3690 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/debug.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/formatting/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     9387 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/formatting/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2939 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_jobs.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    12729 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3032 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_pprint.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3844 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/formatting/_shell.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    11791 2022-12-05 04:26:42.000000 meerschaum-1.6.8/meerschaum/utils/get_pipes.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3419 2022-10-18 06:13:35.000000 meerschaum-1.6.8/meerschaum/utils/interactive.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    61453 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/utils/misc.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1006 2022-02-28 20:55:01.000000 meerschaum-1.6.8/meerschaum/utils/networking.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/packages/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    53718 2023-05-08 21:38:02.000000 meerschaum-1.6.8/meerschaum/utils/packages/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     8054 2023-05-12 06:36:03.000000 meerschaum-1.6.8/meerschaum/utils/packages/_packages.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2540 2022-07-25 06:37:48.000000 meerschaum-1.6.8/meerschaum/utils/packages/lazy_loader.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2781 2022-08-23 06:14:42.000000 meerschaum-1.6.8/meerschaum/utils/pool.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7098 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/process.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    16060 2022-05-02 19:58:56.000000 meerschaum-1.6.8/meerschaum/utils/prompt.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     1635 2022-08-29 21:54:10.000000 meerschaum-1.6.8/meerschaum/utils/schedule.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    34702 2023-05-12 06:36:07.000000 meerschaum-1.6.8/meerschaum/utils/sql.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2152 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/threading.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     2517 2023-05-05 21:42:47.000000 meerschaum-1.6.8/meerschaum/utils/typing.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.389143 meerschaum-1.6.8/meerschaum/utils/venv/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3479 2022-10-25 06:38:00.000000 meerschaum-1.6.8/meerschaum/utils/venv/_Venv.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    22150 2023-04-26 08:12:59.000000 meerschaum-1.6.8/meerschaum/utils/venv/__init__.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     6610 2023-04-25 23:57:31.000000 meerschaum-1.6.8/meerschaum/utils/warnings.py
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3162 2023-01-09 09:23:24.000000 meerschaum-1.6.8/meerschaum/utils/yaml.py
+drwxr-xr-x   0 bmeares   (1000) bmeares   (1000)        0 2023-05-12 06:36:15.375143 meerschaum-1.6.8/meerschaum.egg-info/
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)    10798 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/PKG-INFO
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     7834 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/SOURCES.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/dependency_links.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       88 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/entry_points.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     4703 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/requires.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       11 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/top_level.txt
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)        1 2023-05-12 06:36:15.000000 meerschaum-1.6.8/meerschaum.egg-info/zip-safe
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)       38 2023-05-12 06:36:15.390143 meerschaum-1.6.8/setup.cfg
+-rw-r--r--   0 bmeares   (1000) bmeares   (1000)     3056 2023-05-12 06:36:03.000000 meerschaum-1.6.8/setup.py
```

### Comparing `meerschaum-1.6.7/LICENSE` & `meerschaum-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/PKG-INFO` & `meerschaum-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.7
+Version: 1.6.8
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.7/README.md` & `meerschaum-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/__init__.py` & `meerschaum-1.6.8/meerschaum/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/__main__.py` & `meerschaum-1.6.8/meerschaum/__main__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/arguments/__init__.py` & `meerschaum-1.6.8/meerschaum/_internal/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/arguments/_parse_arguments.py` & `meerschaum-1.6.8/meerschaum/_internal/arguments/_parse_arguments.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/arguments/_parser.py` & `meerschaum-1.6.8/meerschaum/_internal/arguments/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,19 +231,14 @@
 )
 groups['sync'].add_argument(
     '--chunksize', type=int, help=(
         "Specify the chunksize for syncing and retrieving data. Defaults to 900."
     ),
 )
 groups['sync'].add_argument(
-    '--sync-chunks', action='store_true',
-    help="Sync chunks while fetching data instead of waiting until all have arrived. " +
-    "Similar to --async. WARNING! This can be very dangerous when used with --async.",
-)
-groups['sync'].add_argument(
     '--skip-check-existing', '--allow-duplicates', action='store_true',
     help = (
         "Skip checking for duplicate rows when syncing. " +
         "This drastically improves performance when all rows to be synced are unique. " +
         "For example, this setting is highly recommended for use with IoT devices."
     )
 )
```

### Comparing `meerschaum-1.6.7/meerschaum/_internal/docs/index.py` & `meerschaum-1.6.8/meerschaum/_internal/docs/index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/entry.py` & `meerschaum-1.6.8/meerschaum/_internal/entry.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/gui/__init__.py` & `meerschaum-1.6.8/meerschaum/_internal/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/gui/app/__init__.py` & `meerschaum-1.6.8/meerschaum/_internal/gui/app/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/gui/app/_windows.py` & `meerschaum-1.6.8/meerschaum/_internal/gui/app/_windows.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/gui/app/actions.py` & `meerschaum-1.6.8/meerschaum/_internal/gui/app/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/gui/app/pipes.py` & `meerschaum-1.6.8/meerschaum/_internal/gui/app/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/shell/Shell.py` & `meerschaum-1.6.8/meerschaum/_internal/shell/Shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/shell/ShellCompleter.py` & `meerschaum-1.6.8/meerschaum/_internal/shell/ShellCompleter.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/shell/ValidAutoSuggest.py` & `meerschaum-1.6.8/meerschaum/_internal/shell/ValidAutoSuggest.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/term/TermPageHandler.py` & `meerschaum-1.6.8/meerschaum/_internal/term/TermPageHandler.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/term/__init__.py` & `meerschaum-1.6.8/meerschaum/_internal/term/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/_internal/term/tools.py` & `meerschaum-1.6.8/meerschaum/_internal/term/tools.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/__init__.py` & `meerschaum-1.6.8/meerschaum/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/api.py` & `meerschaum-1.6.8/meerschaum/actions/api.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/bootstrap.py` & `meerschaum-1.6.8/meerschaum/actions/bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/clear.py` & `meerschaum-1.6.8/meerschaum/actions/clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/copy.py` & `meerschaum-1.6.8/meerschaum/actions/copy.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/delete.py` & `meerschaum-1.6.8/meerschaum/actions/delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/drop.py` & `meerschaum-1.6.8/meerschaum/actions/drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/edit.py` & `meerschaum-1.6.8/meerschaum/actions/edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/install.py` & `meerschaum-1.6.8/meerschaum/actions/install.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/login.py` & `meerschaum-1.6.8/meerschaum/actions/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/os.py` & `meerschaum-1.6.8/meerschaum/actions/os.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/python.py` & `meerschaum-1.6.8/meerschaum/actions/python.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/register.py` & `meerschaum-1.6.8/meerschaum/actions/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/reload.py` & `meerschaum-1.6.8/meerschaum/actions/reload.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/setup.py` & `meerschaum-1.6.8/meerschaum/actions/setup.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/sh.py` & `meerschaum-1.6.8/meerschaum/actions/sh.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/show.py` & `meerschaum-1.6.8/meerschaum/actions/show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/sql.py` & `meerschaum-1.6.8/meerschaum/actions/sql.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/stack.py` & `meerschaum-1.6.8/meerschaum/actions/stack.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/start.py` & `meerschaum-1.6.8/meerschaum/actions/start.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/stop.py` & `meerschaum-1.6.8/meerschaum/actions/stop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/sync.py` & `meerschaum-1.6.8/meerschaum/actions/sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/uninstall.py` & `meerschaum-1.6.8/meerschaum/actions/uninstall.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/upgrade.py` & `meerschaum-1.6.8/meerschaum/actions/upgrade.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/actions/verify.py` & `meerschaum-1.6.8/meerschaum/actions/verify.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/__init__.py` & `meerschaum-1.6.8/meerschaum/api/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/_chain.py` & `meerschaum-1.6.8/meerschaum/api/_chain.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/_events.py` & `meerschaum-1.6.8/meerschaum/api/_events.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/_oauth2.py` & `meerschaum-1.6.8/meerschaum/api/_oauth2.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/_websockets.py` & `meerschaum-1.6.8/meerschaum/api/_websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/__init__.py` & `meerschaum-1.6.8/meerschaum/api/dash/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/actions.py` & `meerschaum-1.6.8/meerschaum/api/dash/actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/assets/ansi_up.js` & `meerschaum-1.6.8/meerschaum/api/dash/assets/ansi_up.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/assets/banner_1920x320.png` & `meerschaum-1.6.8/meerschaum/api/dash/assets/banner_1920x320.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/assets/favicon.ico` & `meerschaum-1.6.8/meerschaum/api/dash/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/assets/logo_48x48.png` & `meerschaum-1.6.8/meerschaum/api/dash/assets/logo_48x48.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/assets/logo_500x500.png` & `meerschaum-1.6.8/meerschaum/api/dash/assets/logo_500x500.png`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/callbacks/dashboard.py` & `meerschaum-1.6.8/meerschaum/api/dash/callbacks/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/callbacks/login.py` & `meerschaum-1.6.8/meerschaum/api/dash/callbacks/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/callbacks/plugins.py` & `meerschaum-1.6.8/meerschaum/api/dash/callbacks/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/callbacks/register.py` & `meerschaum-1.6.8/meerschaum/api/dash/callbacks/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/components.py` & `meerschaum-1.6.8/meerschaum/api/dash/components.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/connectors.py` & `meerschaum-1.6.8/meerschaum/api/dash/connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/graphs.py` & `meerschaum-1.6.8/meerschaum/api/dash/graphs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/jobs.py` & `meerschaum-1.6.8/meerschaum/api/dash/jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/keys.py` & `meerschaum-1.6.8/meerschaum/api/dash/keys.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pages/dashboard.py` & `meerschaum-1.6.8/meerschaum/api/dash/pages/dashboard.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pages/error.py` & `meerschaum-1.6.8/meerschaum/api/dash/pages/error.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pages/login.py` & `meerschaum-1.6.8/meerschaum/api/dash/pages/login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pages/plugins.py` & `meerschaum-1.6.8/meerschaum/api/dash/pages/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pages/register.py` & `meerschaum-1.6.8/meerschaum/api/dash/pages/register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/pipes.py` & `meerschaum-1.6.8/meerschaum/api/dash/pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/plugins.py` & `meerschaum-1.6.8/meerschaum/api/dash/plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/users.py` & `meerschaum-1.6.8/meerschaum/api/dash/users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/dash/websockets.py` & `meerschaum-1.6.8/meerschaum/api/dash/websockets.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/static/css/bootstrap.min.css` & `meerschaum-1.6.8/meerschaum/api/resources/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/static/css/dash.css` & `meerschaum-1.6.8/meerschaum/api/resources/static/css/dash.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/static/css/dbc_dark.css` & `meerschaum-1.6.8/meerschaum/api/resources/static/css/dbc_dark.css`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/static/ico/logo.ico` & `meerschaum-1.6.8/meerschaum/api/resources/static/ico/logo.ico`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/static/js/action_button.js` & `meerschaum-1.6.8/meerschaum/api/resources/static/js/action_button.js`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/templates/index.html` & `meerschaum-1.6.8/meerschaum/api/resources/templates/index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/templates/old_index.html` & `meerschaum-1.6.8/meerschaum/api/resources/templates/old_index.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/resources/templates/termpage.html` & `meerschaum-1.6.8/meerschaum/api/resources/templates/termpage.html`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/__init__.py` & `meerschaum-1.6.8/meerschaum/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_actions.py` & `meerschaum-1.6.8/meerschaum/api/routes/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_connectors.py` & `meerschaum-1.6.8/meerschaum/api/routes/_connectors.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_index.py` & `meerschaum-1.6.8/meerschaum/api/routes/_index.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_login.py` & `meerschaum-1.6.8/meerschaum/api/routes/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_misc.py` & `meerschaum-1.6.8/meerschaum/api/routes/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_pipes.py` & `meerschaum-1.6.8/meerschaum/api/routes/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_plugins.py` & `meerschaum-1.6.8/meerschaum/api/routes/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_users.py` & `meerschaum-1.6.8/meerschaum/api/routes/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/routes/_version.py` & `meerschaum-1.6.8/meerschaum/api/routes/_version.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/api/tables/__init__.py` & `meerschaum-1.6.8/meerschaum/api/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/__init__.py` & `meerschaum-1.6.8/meerschaum/config/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_default.py` & `meerschaum-1.6.8/meerschaum/config/_default.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_edit.py` & `meerschaum-1.6.8/meerschaum/config/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_environment.py` & `meerschaum-1.6.8/meerschaum/config/_environment.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_formatting.py` & `meerschaum-1.6.8/meerschaum/config/_formatting.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_jobs.py` & `meerschaum-1.6.8/meerschaum/config/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_patch.py` & `meerschaum-1.6.8/meerschaum/config/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_paths.py` & `meerschaum-1.6.8/meerschaum/config/_paths.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_preprocess.py` & `meerschaum-1.6.8/meerschaum/config/_preprocess.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_read_config.py` & `meerschaum-1.6.8/meerschaum/config/_read_config.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_shell.py` & `meerschaum-1.6.8/meerschaum/config/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/_sync.py` & `meerschaum-1.6.8/meerschaum/config/_sync.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/stack/__init__.py` & `meerschaum-1.6.8/meerschaum/config/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/stack/grafana/__init__.py` & `meerschaum-1.6.8/meerschaum/config/stack/grafana/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/config/static/__init__.py` & `meerschaum-1.6.8/meerschaum/config/static/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/Connector.py` & `meerschaum-1.6.8/meerschaum/connectors/Connector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/__init__.py` & `meerschaum-1.6.8/meerschaum/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/APIConnector.py` & `meerschaum-1.6.8/meerschaum/connectors/api/APIConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_actions.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_actions.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_delete.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_fetch.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_fetch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_get.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_get.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_login.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_login.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_misc.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_patch.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_patch.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_pipes.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_plugins.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_post.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_post.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_uri.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/api/_users.py` & `meerschaum-1.6.8/meerschaum/connectors/api/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/parse.py` & `meerschaum-1.6.8/meerschaum/connectors/parse.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/plugin/PluginConnector.py` & `meerschaum-1.6.8/meerschaum/connectors/plugin/PluginConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/poll.py` & `meerschaum-1.6.8/meerschaum/connectors/poll.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/SQLConnector.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/SQLConnector.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_cli.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_cli.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_create_engine.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_create_engine.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_fetch.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_fetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 def fetch(
         self,
         pipe: meerschaum.Pipe,
         begin: Union[datetime.datetime, str, None] = '',
         end: Union[datetime.datetime, str, None] = None,
         chunk_hook: Optional[Callable[[pd.DataFrame], Any]] = None,
         chunksize: Optional[int] = -1,
+        workers: Optional[int] = None,
         debug: bool = False,
         **kw: Any
-    ) -> Union['pd.DataFrame', None]:
+    ) -> Union['pd.DataFrame', List[Any], None]:
     """Execute the SQL definition and return a Pandas DataFrame.
 
     Parameters
     ----------
     pipe: meerschaum.Pipe
         The pipe object which contains the `fetch` metadata.
         
@@ -42,38 +43,51 @@
         Most recent datatime to search for data.
         If `backtrack_minutes` is provided, subtract `backtrack_minutes`.
 
     end: Union[datetime.datetime, str, None], default None
         The latest datetime to search for data.
         If `end` is `None`, do not bound 
 
+    chunk_hook: Callable[[pd.DataFrame], Any], default None
+        A function to pass to `SQLConnector.read()` that accepts a Pandas DataFrame.
+
+    chunksize: Optional[int], default -1
+        How many rows to load into memory at once (when `chunk_hook` is provided).
+        Otherwise the entire result set is loaded into memory.
+
+    workers: Optional[int], default None
+        How many threads to use when consuming the generator (when `chunk_hook is provided).
+        Defaults to the number of cores.
+
     debug: bool, default False
         Verbosity toggle.
        
     Returns
     -------
     A pandas DataFrame or `None`.
-
+    If `chunk_hook` is not None, return a list of the hook function's results.
     """
     meta_def = self.get_pipe_metadef(
         pipe,
         begin = begin,
         end = end,
         debug = debug,
         **kw
     )
+    as_hook_results = chunk_hook is not None
     chunks = self.read(
         meta_def,
         chunk_hook = chunk_hook,
+        as_hook_results = as_hook_results,
         chunksize = chunksize,
-        as_iterator = True,
+        workers = workers,
         debug = debug,
     )
     ### if sqlite, parse for datetimes
-    if self.flavor == 'sqlite':
+    if not as_hook_results and self.flavor == 'sqlite':
         from meerschaum.utils.misc import parse_df_datetimes
         ignore_cols = [
             col
             for col, dtype in pipe.dtypes.items()
             if 'datetime' not in str(dtype)
         ]
         return (
```

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_pipes.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_plugins.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_plugins.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_sql.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 def read(
         self,
         query_or_table: Union[str, sqlalchemy.Query],
         params: Optional[Dict[str, Any], List[str]] = None,
         dtype: Optional[Dict[str, Any]] = None,
         chunksize: Optional[int] = -1,
+        workers: Optional[int] = None,
         chunk_hook: Optional[Callable[[pandas.DataFrame], Any]] = None,
         as_hook_results: bool = False,
         chunks: Optional[int] = None,
         as_chunks: bool = False,
         as_iterator: bool = False,
         silent: bool = False,
         debug: bool = False,
@@ -60,14 +61,18 @@
 
     chunksize: Optional[int], default -1
         How many chunks to read at a time. `None` will read everything in one large chunk.
         Defaults to system configuration.
 
         **NOTE:** DuckDB does not allow for chunking.
 
+    workers: Optional[int], default None
+        How many threads to use when consuming the generator.
+        Only applies if `chunk_hook` is provided.
+
     chunk_hook: Optional[Callable[[pandas.DataFrame], Any]], default None
         Hook function to execute once per chunk, e.g. writing and reading chunks intermittently.
         See `--sync-chunks` for an example.
         **NOTE:** `as_iterator` MUST be False (default).
 
     as_hook_results: bool, default False
         If `True`, return a `List` of the outputs of the hook function.
@@ -101,16 +106,18 @@
     or `None` if something breaks.
 
     """
     if chunks is not None and chunks <= 0:
         return []
     from meerschaum.utils.sql import sql_item_name, truncate_item_name
     from meerschaum.utils.packages import attempt_import, import_pandas
+    from meerschaum.utils.pool import get_pool
     import warnings
     import inspect
+    import traceback
     pd = import_pandas()
     sqlalchemy = attempt_import("sqlalchemy")
     default_chunksize = self._sys_config.get('chunksize', None)
     chunksize = chunksize if chunksize != -1 else default_chunksize
     if chunksize is None and as_iterator:
         if not silent and self.flavor not in _disallow_chunks_flavors:
             warn(
@@ -162,59 +169,95 @@
         formatted_query = sqlalchemy.text("SELECT * FROM " + str(query_or_table))
     else:
         try:
             formatted_query = sqlalchemy.text(query_or_table)
         except Exception as e:
             formatted_query = query_or_table
 
+    chunk_list = []
+    chunk_hook_results = []
     try:
+        stream_results = not as_iterator and chunk_hook is not None and chunksize is not None
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', 'case sensitivity issues')
-            with self.engine.begin() as connection:
-                chunk_generator = pd.read_sql_query(
-                    formatted_query,
-                    connection,
-                    params = params,
-                    chunksize = chunksize,
-                    dtype = dtype,
-                )
+            with self.engine.begin() as transaction:
+                with transaction.execution_options(stream_results=stream_results) as connection:
+                    chunk_generator = pd.read_sql_query(
+                        formatted_query,
+                        connection,
+                        params = params,
+                        chunksize = chunksize,
+                        dtype = dtype,
+                    )
+
+                    ### `stream_results` must be False (will load everything into memory).
+                    if as_iterator or chunksize is None:
+                        return chunk_generator
+
+                    ### We must consume the generator in this context if using server-side cursors.
+                    if stream_results:
+
+                        pool = get_pool(workers=workers)
+
+                        def _process_chunk(_chunk, _retry_on_failure: bool = True):
+                            if not as_hook_results:
+                                chunk_list.append(_chunk)
+                            result = None
+                            if chunk_hook is not None:
+                                try:
+                                    result = chunk_hook(
+                                        _chunk,
+                                        workers = workers,
+                                        chunksize = chunksize,
+                                        debug = debug,
+                                        **kw
+                                    )
+                                except Exception as e:
+                                    result = False, traceback.format_exc()
+                                    from meerschaum.utils.formatting import get_console
+                                    get_console().print_exception()
+
+                                ### If the chunk fails to process, try it again one more time.
+                                if isinstance(result, tuple) and result[0] is False:
+                                    if _retry_on_failure:
+                                        return _process_chunk(_chunk, _retry_on_failure=False)
+
+                            return result
+
+                        chunk_hook_results = list(pool.imap(_process_chunk, chunk_generator))
+                        if as_hook_results:
+                            return chunk_hook_results
+
     except Exception as e:
         if debug:
             dprint(f"[{self}] Failed to execute query:\n\n{query_or_table}\n\n")
         if not silent:
             warn(str(e), stacklevel=3)
         from meerschaum.utils.formatting import get_console
         get_console().print_exception()
 
         return None
 
-    chunk_list = []
     read_chunks = 0
-    chunk_hook_results = []
-    if chunksize is None:
-        chunk_list.append(chunk_generator)
-    elif as_iterator:
-        return chunk_generator
-    else:
-        try:
-            for chunk in chunk_generator:
-                if chunk_hook is not None:
-                    chunk_hook_results.append(
-                        chunk_hook(chunk, chunksize=chunksize, debug=debug, **kw)
-                    )
-                chunk_list.append(chunk)
-                read_chunks += 1
-                if chunks is not None and read_chunks >= chunks:
-                    break
-        except Exception as e:
-            warn(f"[{self}] Failed to retrieve query results:\n" + str(e), stacklevel=3)
-            from meerschaum.utils.formatting import get_console
-            get_console().print_exception()
+    try:
+        for chunk in chunk_generator:
+            if chunk_hook is not None:
+                chunk_hook_results.append(
+                    chunk_hook(chunk, chunksize=chunksize, debug=debug, **kw)
+                )
+            chunk_list.append(chunk)
+            read_chunks += 1
+            if chunks is not None and read_chunks >= chunks:
+                break
+    except Exception as e:
+        warn(f"[{self}] Failed to retrieve query results:\n" + str(e), stacklevel=3)
+        from meerschaum.utils.formatting import get_console
+        get_console().print_exception()
 
-            return None
+        return None
 
     ### If no chunks returned, read without chunks
     ### to get columns
     if len(chunk_list) == 0:
         with warnings.catch_warnings():
             warnings.filterwarnings('ignore', 'case sensitivity issues')
             with self.engine.begin() as connection:
```

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_uri.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_uri.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/_users.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/_users.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/tables/__init__.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/connectors/sql/tables/types.py` & `meerschaum-1.6.8/meerschaum/connectors/sql/tables/types.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/__init__.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     >>> import pandas as pd
     >>> df = pd.read_csv('weather.csv')
     >>> pipe.sync(df)
     ```
     """
 
     from ._fetch import fetch
-    from ._data import get_data, get_backtrack_data, get_rowcount
+    from ._data import get_data, get_backtrack_data, get_rowcount, _get_data_as_iterator
     from ._register import register
     from ._attributes import (
         attributes,
         parameters,
         columns,
         dtypes,
         get_columns,
@@ -100,15 +100,15 @@
         children,
         target,
         _target_legacy,
         guess_datetime,
     )
     from ._show import show
     from ._edit import edit, edit_definition, update
-    from ._sync import sync, get_sync_time, exists, filter_existing
+    from ._sync import sync, get_sync_time, exists, filter_existing, _get_chunk_label
     from ._delete import delete
     from ._drop import drop
     from ._clear import clear
     from ._bootstrap import bootstrap
     from ._dtypes import enforce_dtypes, infer_dtypes
 
     def __init__(
```

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_attributes.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_attributes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_bootstrap.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_clear.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_clear.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_data.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 # vim:fenc=utf-8
 
 """
 Retrieve Pipes' data from instances.
 """
 
 from __future__ import annotations
-from meerschaum.utils.typing import Optional, Dict, Any, Union
+import datetime
+from meerschaum.utils.typing import Optional, Dict, Any, Union, Generator
 
 def get_data(
         self,
         begin: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         params: Optional[Dict[str, Any]] = None,
+        as_iterator: bool = False,
+        as_chunks: bool = False,
+        chunk_interval: Union[datetime.datetime, int, None] = None,
         fresh: bool = False,
         debug: bool = False,
         **kw: Any
-    ) -> Union['pd.DataFrame', None]:
+    ) -> Union['pd.DataFrame', Generator['pd.DataFrame'], None]:
     """
     Get a pipe's data from the instance connector.
 
     Parameters
     ----------
     begin: Optional[datetime.datetime], default None
         Lower bound datetime to begin searching for data (inclusive).
@@ -33,14 +37,27 @@
         Translates to a `WHERE` clause like `WHERE datetime < end`.
         Defaults to `None`.
 
     params: Optional[Dict[str, Any]], default None
         Filter the retrieved data by a dictionary of parameters.
         See `meerschaum.utils.sql.build_where` for more details. 
 
+    as_iterator: bool, default False
+        If `True`, return a generator of chunks of pipe data.
+
+    as_chunks: bool, default False
+        Alias for `as_iterator`.
+
+    chunk_interval: int, default None
+        If `as_iterator`, then return chunks with `begin` and `end` separated by this interval.
+        By default, use a timedelta of 1 day.
+        If the `datetime` axis is an integer, default to the configured chunksize.
+        Note that because `end` is always non-inclusive,
+        there will be `chunk_interval - 1` rows per chunk for integers.
+
     fresh: bool, default True
         If `True`, skip local cache and directly query the instance connector.
         Defaults to `True`.
 
     debug: bool, default False
         Verbosity toggle.
         Defaults to `False`.
@@ -49,19 +66,33 @@
     -------
     A `pd.DataFrame` for the pipe's data corresponding to the provided parameters.
 
     """
     from meerschaum.utils.warnings import warn
     from meerschaum.utils.venv import Venv
     from meerschaum.connectors import get_connector_plugin
+    from meerschaum.utils.misc import iterate_chunks
+    from meerschaum.config import get_config
     kw.update({'begin': begin, 'end': end, 'params': params,})
 
+    as_iterator = as_iterator or as_chunks
+
+    if as_iterator or as_chunks:
+        return self._get_data_as_iterator(
+            begin = begin,
+            end = end,
+            params = params,
+            chunk_interval = chunk_interval,
+            fresh = fresh,
+            debug = debug,
+        )
+
     if not self.exists(debug=debug):
         return None
-
+       
     if self.cache_pipe is not None:
         if not fresh:
             _sync_cache_tuple = self.cache_pipe.sync(debug=debug, **kw)
             if not _sync_cache_tuple[0]:
                 warn(f"Failed to sync cache for {self}:\n" + _sync_cache_tuple[1])
                 fresh = True
             else: ### Successfully synced cache.
@@ -78,14 +109,104 @@
                 debug = debug,
                 **kw
             ),
             debug = debug,
         )
 
 
+def _get_data_as_iterator(
+        self,
+        begin: Optional[datetime.datetime] = None,
+        end: Optional[datetime.datetime] = None,
+        params: Optional[Dict[str, Any]] = None,
+        chunk_interval: Union[datetime.datetime, int, None] = None,
+        fresh: bool = False,
+        debug: bool = False,
+        **kw: Any
+    ) -> Generator['pd.DataFrame']:
+    """
+    Return a pipe's data as a generator.
+    """
+    from meerschaum.utils.misc import round_time
+    parse_begin = isinstance(begin, str)
+    parse_end = isinstance(end, str)
+    if parse_begin or parse_end:
+        from meerschaum.utils.packages import attempt_import
+        dateutil_parser = attempt_import('dateutil.parser')
+    if parse_begin:
+        begin = dateutil_parser.parse(begin)
+    if parse_end:
+        end = dateutil_parser.parse(end)
+    _ = kw.pop('as_chunks', None)
+    _ = kw.pop('as_iterator', None)
+    min_dt = (
+        begin if begin is not None
+        else self.get_sync_time(round_down=False, newest=False, params=params, debug=debug)
+    )
+    max_dt = (
+        end if end is not None
+        else self.get_sync_time(round_down=False, newest=True, params=params, debug=debug)
+    )
+
+    ### We want to search just past the maximum value.
+    if end is None:
+        if isinstance(max_dt, int):
+            max_dt += 1
+        elif isinstance(max_dt, datetime.datetime):
+            max_dt = round_time(max_dt + datetime.timedelta(minutes=1))
+
+    if chunk_interval is None:
+        chunk_interval = (
+            get_config('system', 'connectors', 'sql', 'chunksize')
+            if isinstance(min_dt, int)
+            else datetime.timedelta(days=1)
+        )
+
+
+    ### If we can't determine bounds
+    ### or if chunk_interval exceeds the max,
+    ### return a single chunk.
+    if (
+        (min_dt is None and max_dt is None)
+        or
+        (min_dt + chunk_interval) > max_dt
+    ):
+        return (
+            self.get_data(
+                begin = begin,
+                end = end,
+                params = params,
+                fresh = fresh,
+                debug = debug,
+            ) for i in range(1)
+        )
+
+    chunk_begin = min_dt
+    chunk_end = min_dt + chunk_interval
+    while chunk_end < max_dt:
+        yield self.get_data(
+            begin = chunk_begin,
+            end = chunk_end,
+            params = params,
+            fresh = fresh,
+            debug = debug,
+        )
+        chunk_begin = chunk_end
+        chunk_end += chunk_interval
+
+    if chunk_begin <= max_dt:
+        yield self.get_data(
+            begin = chunk_begin,
+            end = max_dt,
+            params = params,
+            fresh = fresh,
+            debug = debug,
+        )
+
+
 def get_backtrack_data(
         self,
         backtrack_minutes: int = 0,
         begin: Optional['datetime.datetime'] = None,
         fresh: bool = False,
         debug: bool = False,
         **kw: Any
```

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_delete.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_delete.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_drop.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_drop.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_dtypes.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_edit.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_edit.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_fetch.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_fetch.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,30 +58,36 @@
         plugin_name = (
             self.connector.label if self.connector.type == 'plugin'
             else self.connector.__module__.replace('plugins.', '').split('.')[0]
         )
         connector_plugin = Plugin(plugin_name)
         connector_plugin.activate_venv(debug=debug)
     
-    _chunk_hook = kw.pop('chunk_hook') if 'chunk_hook' in kw else None
+    _chunk_hook = kw.pop('chunk_hook', None)
+    if sync_chunks and _chunk_hook is None:
+
+        def _chunk_hook(chunk, **kw) -> SuccessTuple:
+            """
+            Wrap `Pipe.sync()` with a custom chunk label prepended to the message.
+            """
+            chunk_success, chunk_message = self.sync(chunk, **kw)
+            chunk_label = self._get_chunk_label(chunk, self.columns.get('datetime', None))
+            if chunk_label:
+                chunk_message = '\n' + chunk_label + '\n' + chunk_message
+            return chunk_success, chunk_message
 
     df = self.connector.fetch(
         self,
         begin = begin,
         end = end,
-        chunk_hook = (
-            self.sync if sync_chunks and _chunk_hook is None
-            else _chunk_hook
-        ),
+        chunk_hook = _chunk_hook,
         debug = debug,
         **kw
     )
     if (
         self.connector.type == 'plugin'
         or
         self.connector.type in custom_types
     ):
         connector_plugin.deactivate_venv(debug=debug)
-    ### Return True if we're syncing in parallel, else continue as usual.
-    if sync_chunks:
-        return True
+
     return df
```

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_register.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_register.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_show.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_show.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/core/Pipe/_sync.py` & `meerschaum-1.6.8/meerschaum/core/Pipe/_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         min_seconds: int = 1,
         check_existing: bool = True,
         blocking: bool = True,
         workers: Optional[int] = None,
         callback: Optional[Callable[[Tuple[bool, str]], Any]] = None,
         error_callback: Optional[Callable[[Exception], Any]] = None,
         chunksize: Optional[int] = -1,
-        sync_chunks: bool = False,
+        sync_chunks: bool = True,
         debug: bool = False,
         **kw: Any
     ) -> SuccessTuple:
     """
     Fetch new data from the source and update the pipe's table with new data.
     
     Get new remote data via fetch, get existing data in the same time period,
@@ -94,17 +94,16 @@
 
     chunksize: int, default -1
         Specify the number of rows to sync per chunk.
         If `-1`, resort to system configuration (default is `900`).
         A `chunksize` of `None` will sync all rows in one transaction.
         Defaults to `-1`.
 
-    sync_chunks: bool, default False
+    sync_chunks: bool, default True
         If possible, sync chunks while fetching them into memory.
-        Defaults to `False`.
 
     debug: bool, default False
         Verbosity toggle. Defaults to False.
 
     Returns
     -------
     A `SuccessTuple` of success (`bool`) and message (`str`).
@@ -122,15 +121,18 @@
     import datetime
     import time
     if (callback is not None or error_callback is not None) and blocking:
         warn("Callback functions are only executed when blocking = False. Ignoring...")
 
     _checkpoint(_total=2, **kw)
 
-    ### NOTE: Setting begin to the sync time for Simple Sync.
+    if chunksize == 0:
+        chunksize = None
+        sync_chunks = False
+
     ### TODO: Add flag for specifying syncing method.
     begin = _determine_begin(self, begin, debug=debug)
     kw.update({
         'begin': begin, 'end': end, 'force': force, 'retries': retries, 'min_seconds': min_seconds,
         'check_existing': check_existing, 'blocking': blocking, 'workers': workers,
         'callback': callback, 'error_callback': error_callback, 'sync_chunks': sync_chunks,
         'chunksize': chunksize,
@@ -239,14 +241,24 @@
                 msg = f"Failed to fetch data from {p.connector}:\n    {e}"
                 df = None
 
             if df is None:
                 p._exists = None
                 return False, f"No data were fetched for {p}."
 
+            if isinstance(df, list):
+                if len(df) == 0:
+                    return True, f"No new rows were returned for {p}."
+
+                ### May be a chunk hook results list.
+                if isinstance(df[0], tuple):
+                    success = all([_success for _success, _ in df])
+                    message = '\n'.join([_message for _, _message in df])
+                    return success, message
+
             ### TODO: Depreciate async?
             if df is True:
                 p._exists = None
                 return True, f"{p} is being synced in parallel."
 
         ### CHECKPOINT: Retrieved the DataFrame.
         _checkpoint(**kw)
@@ -254,15 +266,14 @@
         ### Allow for dataframe generators or iterables.
         if (
             not isinstance(df, (dict, list, str))
             and 'DataFrame' not in str(type(df))
             and isinstance(df, (Generator, Iterable))
         ):
             from meerschaum.utils.pool import get_pool
-            from meerschaum.utils.misc import get_datetime_bound_from_df
             import threading
             engine_pool_size = (
                 p.instance_connector.engine.pool.size()
                 if p.instance_connector.type == 'sql'
                 else 1
             )
             current_num_threads = len(threading.enumerate())
@@ -270,44 +281,39 @@
             desired_workers = min(workers or engine_pool_size, engine_pool_size)
             kw['workers'] = max(
                 (desired_workers - current_num_threads),
                 1,
             )
 
             dt_col = p.columns.get('datetime', None)
-            def get_chunk_label(_chunk) -> str:
-                min_dt = get_datetime_bound_from_df(_chunk, dt_col)
-                max_dt = get_datetime_bound_from_df(_chunk, dt_col, minimum=False)
-                return (
-                    f"{min_dt} - {max_dt}"
-                    if min_dt is not None and max_dt is not None
-                    else ''
-                )
 
 
             pool = get_pool(workers=kw.get('workers', 1))
             if debug:
                 dprint(f"Received {type(df)}. Attempting to sync first chunk...")
-            chunk = next(df)
+            try:
+                chunk = next(df)
+            except StopIteration:
+                return True, "Received an empty generator; nothing to do."
             chunk_success, chunk_msg = _sync(p, chunk)
-            chunk_msg = '\n' + get_chunk_label(chunk) + '\n' + chunk_msg
+            chunk_msg = '\n' + self._get_chunk_label(chunk, dt_col) + '\n' + chunk_msg
             if not chunk_success:
                 return chunk_success, f"Unable to sync initial chunk for {p}:\n{chunk_msg}"
             if debug:
                 dprint(f"Successfully synced the first chunk, attemping the rest...")
 
             failed_chunks = []
             def _process_chunk(_chunk):
                 try:
                     _chunk_success, _chunk_msg = _sync(p, _chunk)
                 except Exception as e:
                     _chunk_success, _chunk_msg = False, str(e)
                 if not _chunk_success:
                     failed_chunks.append(_chunk)
-                return _chunk_success, '\n' + get_chunk_label(_chunk) + '\n' + _chunk_msg
+                return _chunk_success, '\n' + self._get_chunk_label(_chunk, dt_col) + '\n' + _chunk_msg
 
 
             results = sorted(
                 [(chunk_success, chunk_msg)] + list(pool.imap(_process_chunk, df))
             )
             chunk_messages = [chunk_msg for _, chunk_msg in results]
             success_bools = [chunk_success for chunk_success, _ in results]
@@ -707,7 +713,29 @@
         joined_df
         .where(~new_rows_mask)
         .dropna(how='all')[cols]
         .reset_index(drop=True)
     ) if on_cols else None
 
     return unseen_df, update_df, delta_df
+
+
+@staticmethod
+def _get_chunk_label(
+        chunk: Union[
+            'pd.DataFrame',
+            List[Dict[str, Any]],
+            Dict[str, List[Any]]
+        ],
+        dt_col: str,
+    ) -> str:
+    """
+    Return the min - max label for the chunk.
+    """
+    from meerschaum.utils.misc import get_datetime_bound_from_df
+    min_dt = get_datetime_bound_from_df(chunk, dt_col)
+    max_dt = get_datetime_bound_from_df(chunk, dt_col, minimum=False)
+    return (
+        f"{min_dt} - {max_dt}"
+        if min_dt is not None and max_dt is not None
+        else ''
+    )
```

### Comparing `meerschaum-1.6.7/meerschaum/core/User/_User.py` & `meerschaum-1.6.8/meerschaum/core/User/_User.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/plugins/_Plugin.py` & `meerschaum-1.6.8/meerschaum/plugins/_Plugin.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/plugins/__init__.py` & `meerschaum-1.6.8/meerschaum/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/daemon/Daemon.py` & `meerschaum-1.6.8/meerschaum/utils/daemon/Daemon.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/daemon/Log.py` & `meerschaum-1.6.8/meerschaum/utils/daemon/Log.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/daemon/__init__.py` & `meerschaum-1.6.8/meerschaum/utils/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/daemon/_names.py` & `meerschaum-1.6.8/meerschaum/utils/daemon/_names.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/debug.py` & `meerschaum-1.6.8/meerschaum/utils/debug.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/formatting/__init__.py` & `meerschaum-1.6.8/meerschaum/utils/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/formatting/_jobs.py` & `meerschaum-1.6.8/meerschaum/utils/formatting/_jobs.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/formatting/_pipes.py` & `meerschaum-1.6.8/meerschaum/utils/formatting/_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/formatting/_pprint.py` & `meerschaum-1.6.8/meerschaum/utils/formatting/_pprint.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/formatting/_shell.py` & `meerschaum-1.6.8/meerschaum/utils/formatting/_shell.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/get_pipes.py` & `meerschaum-1.6.8/meerschaum/utils/get_pipes.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/interactive.py` & `meerschaum-1.6.8/meerschaum/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/misc.py` & `meerschaum-1.6.8/meerschaum/utils/misc.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/networking.py` & `meerschaum-1.6.8/meerschaum/utils/networking.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/packages/__init__.py` & `meerschaum-1.6.8/meerschaum/utils/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/packages/_packages.py` & `meerschaum-1.6.8/meerschaum/utils/packages/_packages.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/packages/lazy_loader.py` & `meerschaum-1.6.8/meerschaum/utils/packages/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/pool.py` & `meerschaum-1.6.8/meerschaum/utils/pool.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/process.py` & `meerschaum-1.6.8/meerschaum/utils/process.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/prompt.py` & `meerschaum-1.6.8/meerschaum/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/schedule.py` & `meerschaum-1.6.8/meerschaum/utils/schedule.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/sql.py` & `meerschaum-1.6.8/meerschaum/utils/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,25 +493,25 @@
     "CAST('2022-01-01 00:00:00' AS TIMESTAMP) + INTERVAL '1 day'"
 
     """
     from meerschaum.utils.debug import dprint
     from meerschaum.utils.packages import attempt_import
     from meerschaum.utils.warnings import error
     import datetime
-    dateutil = attempt_import('dateutil')
+    dateutil_parser = attempt_import('dateutil.parser')
     if 'int' in str(type(begin)).lower():
         return str(begin)
     if not begin:
         return None
     _original_begin = begin
     begin_time = None
     ### Sanity check: make sure `begin` is a valid datetime before we inject anything.
     if not isinstance(begin, datetime.datetime):
         try:
-            begin_time = dateutil.parser.parse(begin)
+            begin_time = dateutil_parser.parse(begin)
         except Exception:
             begin_time = None
     else:
         begin_time = begin
 
     ### Unable to parse into a datetime.
     if begin_time is None:
```

### Comparing `meerschaum-1.6.7/meerschaum/utils/threading.py` & `meerschaum-1.6.8/meerschaum/utils/threading.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/typing.py` & `meerschaum-1.6.8/meerschaum/utils/typing.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/venv/_Venv.py` & `meerschaum-1.6.8/meerschaum/utils/venv/_Venv.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/venv/__init__.py` & `meerschaum-1.6.8/meerschaum/utils/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/warnings.py` & `meerschaum-1.6.8/meerschaum/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum/utils/yaml.py` & `meerschaum-1.6.8/meerschaum/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum.egg-info/PKG-INFO` & `meerschaum-1.6.8/meerschaum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meerschaum
-Version: 1.6.7
+Version: 1.6.8
 Summary: Sync Time-Series Pipes with Meerschaum
 Home-page: https://meerschaum.io
 Author: Bennett Meares
 Author-email: bennett.meares@gmail.com
 Maintainer-email: bennett.meares@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.meerschaum.io
```

### Comparing `meerschaum-1.6.7/meerschaum.egg-info/SOURCES.txt` & `meerschaum-1.6.8/meerschaum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/meerschaum.egg-info/requires.txt` & `meerschaum-1.6.8/meerschaum.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `meerschaum-1.6.7/setup.py` & `meerschaum-1.6.8/setup.py`

 * *Files identical despite different names*

