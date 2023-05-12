# Comparing `tmp/irails-1.3.3.tar.gz` & `tmp/irails-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.3.tar", last modified: Thu May 11 15:40:33 2023, max compression
+gzip compressed data, was "irails-1.3.4.tar", last modified: Thu May 11 15:42:52 2023, max compression
```

## Comparing `irails-1.3.3.tar` & `irails-1.3.4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.834063 irails-1.3.3/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-11 15:40:33.833052 irails-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.748280 irails-1.3.3/irails/
--rw-rw-rw-   0        0        0      306 2023-05-11 15:40:26.000000 irails-1.3.3/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.3/irails/_i18n.py
--rw-rw-rw-   0        0        0     2445 2023-05-11 15:39:57.000000 irails-1.3.3/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.3/irails/_utils.py
--rw-rw-rw-   0        0        0    11722 2023-05-11 15:21:25.000000 irails-1.3.3/irails/auth.py
--rw-rw-rw-   0        0        0    12404 2023-05-11 15:21:09.000000 irails-1.3.3/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.762242 irails-1.3.3/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.763240 irails-1.3.3/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.3/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.3/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.3/irails/cbv.py
--rw-rw-rw-   0        0        0     6065 2023-05-11 15:19:41.000000 irails-1.3.3/irails/config.py
--rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.3/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32262 2023-05-11 15:20:13.000000 irails-1.3.3/irails/core.py
--rw-rw-rw-   0        0        0     6409 2023-05-11 15:21:34.000000 irails-1.3.3/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.3/irails/log.py
--rw-rw-rw-   0        0        0     8673 2023-05-11 15:20:30.000000 irails-1.3.3/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.3/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.3/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.3/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.776220 irails-1.3.3/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.3/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7811 2023-05-11 15:34:41.000000 irails-1.3.3/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.3/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.3/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.3/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1556 2023-05-11 05:57:14.000000 irails-1.3.3/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.3/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     1855 2023-05-11 12:33:17.000000 irails-1.3.3/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.707195 irails-1.3.3/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.791165 irails-1.3.3/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.3/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.3/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.3/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.3/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.3/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.3/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.3/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.3/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.794158 irails-1.3.3/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.3/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.796151 irails-1.3.3/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.3/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.810114 irails-1.3.3/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.3/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.3/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.3/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.3/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.3/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.3/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.3/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.3/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.3/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.710179 irails-1.3.3/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.814104 irails-1.3.3/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.3/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.3/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.3/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      277 2023-05-11 11:03:51.000000 irails-1.3.3/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.817096 irails-1.3.3/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.3/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.3/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.821087 irails-1.3.3/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.714167 irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.825076 irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.829064 irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.715165 irails-1.3.3/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.831057 irails-1.3.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2677 2023-05-11 15:20:54.000000 irails-1.3.3/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:40:33.758254 irails-1.3.3/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2326 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-11 15:40:33.000000 irails-1.3.3/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 15:40:33.834063 irails-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.925829 irails-1.3.4/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-11 15:42:52.924831 irails-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.844469 irails-1.3.4/irails/
+-rw-rw-rw-   0        0        0      306 2023-05-11 15:42:44.000000 irails-1.3.4/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.3.4/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2445 2023-05-11 15:39:57.000000 irails-1.3.4/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.3.4/irails/_utils.py
+-rw-rw-rw-   0        0        0    11722 2023-05-11 15:21:25.000000 irails-1.3.4/irails/auth.py
+-rw-rw-rw-   0        0        0    12404 2023-05-11 15:21:09.000000 irails-1.3.4/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.859428 irails-1.3.4/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.860426 irails-1.3.4/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.3.4/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.4/irails/cbv.py
+-rw-rw-rw-   0        0        0     6065 2023-05-11 15:19:41.000000 irails-1.3.4/irails/config.py
+-rw-rw-rw-   0        0        0    12326 2023-05-11 05:06:13.000000 irails-1.3.4/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32262 2023-05-11 15:20:13.000000 irails-1.3.4/irails/core.py
+-rw-rw-rw-   0        0        0     6409 2023-05-11 15:21:34.000000 irails-1.3.4/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.4/irails/log.py
+-rw-rw-rw-   0        0        0     8673 2023-05-11 15:20:30.000000 irails-1.3.4/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.4/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.4/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.4/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.873573 irails-1.3.4/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.4/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-05-11 15:34:41.000000 irails-1.3.4/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.3.4/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6934 2023-05-11 05:34:35.000000 irails-1.3.4/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.4/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1553 2023-05-11 15:41:47.000000 irails-1.3.4/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.4/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     1855 2023-05-11 12:33:17.000000 irails-1.3.4/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.784701 irails-1.3.4/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.885544 irails-1.3.4/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.4/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.4/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.4/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.4/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.3.4/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.3.4/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.3.4/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.4/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.889534 irails-1.3.4/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.4/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.890530 irails-1.3.4/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.4/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.904885 irails-1.3.4/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.4/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.3.4/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.4/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.4/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.4/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.4/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.4/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.4/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.4/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.788617 irails-1.3.4/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.907881 irails-1.3.4/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.4/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.4/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.4/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.4/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.910869 irails-1.3.4/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.4/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.4/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.912864 irails-1.3.4/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.792607 irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.915856 irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.920842 irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.793604 irails-1.3.4/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.922836 irails-1.3.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2677 2023-05-11 15:20:54.000000 irails-1.3.4/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:42:52.856437 irails-1.3.4/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-11 15:42:52.000000 irails-1.3.4/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:42:52.925829 irails-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.4/setup.py
```

### Comparing `irails-1.3.3/PKG-INFO` & `irails-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.3.3 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.4 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.3/README.md` & `irails-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/_i18n.py` & `irails-1.3.4/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/_loader.py` & `irails-1.3.4/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/_utils.py` & `irails-1.3.4/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/auth.py` & `irails-1.3.4/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/base_controller.py` & `irails-1.3.4/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.4/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/cbv.py` & `irails-1.3.4/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/config.py` & `irails-1.3.4/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/controller_utils.py` & `irails-1.3.4/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/core.py` & `irails-1.3.4/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/database.py` & `irails-1.3.4/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/log.py` & `irails-1.3.4/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/midware.py` & `irails-1.3.4/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/midware_casbin.py` & `irails-1.3.4/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/midware_session.py` & `irails-1.3.4/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/mvc_router.py` & `irails-1.3.4/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/_app.py` & `irails-1.3.4/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/_controller.py` & `irails-1.3.4/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/_i18n.py` & `irails-1.3.4/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/_project.py` & `irails-1.3.4/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/_run.py` & `irails-1.3.4/irails/scripts/_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,11 +32,11 @@
         apps_dirs = app_cfg.get("appdir") 
         kwargs['reload_dirs'] = apps_dirs
         kwargs['reload_includes'] = ['*.po']
     # module_path = 'main.py'
     # spec = importlib.util.spec_from_file_location(module_path, module_path)
     # module = importlib.util.module_from_spec(spec)
     # spec.loader.exec_module(module) 
-    from irails.config import _log
+    from irails.log import _log
     kwargs['log_level'] = _log.level
     uvicorn.run(app="irails.core:generate_mvc_app",**kwargs)
```

### Comparing `irails-1.3.3/irails/scripts/_shell.py` & `irails-1.3.4/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/main.py` & `irails-1.3.4/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.4/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/app/home.tpl` & `irails-1.3.4/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.4/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.4/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.4/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.4/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.4/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.4/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails/view.py` & `irails-1.3.4/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails.egg-info/PKG-INFO` & `irails-1.3.4/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.3
+Version: 1.3.4
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.3.3 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.3.4 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.3.3/irails.egg-info/SOURCES.txt` & `irails-1.3.4/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/irails.egg-info/requires.txt` & `irails-1.3.4/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.3/setup.py` & `irails-1.3.4/setup.py`

 * *Files identical despite different names*

