# Comparing `tmp/vstutils-5.4.3.tar.gz` & `tmp/vstutils-5.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.3.tar", last modified: Mon Apr 17 03:38:17 2023, max compression
+gzip compressed data, was "vstutils-5.4.4.tar", last modified: Fri May 12 21:40:56 2023, max compression
```

## Comparing `vstutils-5.4.3.tar` & `vstutils-5.4.4.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.3/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4459 2023-04-17 03:38:17.474371 vstutils-5.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-18 02:33:32.000000 vstutils-5.4.3/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.3/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.3/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-13 03:48:29.000000 vstutils-5.4.3/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.3/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.3/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-13 03:48:29.000000 vstutils-5.4.3/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-03-20 21:33:20.000000 vstutils-5.4.3/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-04-17 03:38:17.478371 vstutils-5.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.438371 vstutils-5.4.3/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-04-14 03:47:13.000000 vstutils-5.4.3/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.446371 vstutils-5.4.3/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    27865 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24054 2023-02-13 06:24:20.000000 vstutils-5.4.3/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.3/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51728 2023-03-15 02:43:46.000000 vstutils-5.4.3/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    11397 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.446371 vstutils-5.4.3/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.446371 vstutils-5.4.3/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.3/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.3/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.3/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.426371 vstutils-5.4.3/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.446371 vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.446371 vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-17 03:38:17.482371 vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.450371 vstutils-5.4.3/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.450371 vstutils-5.4.3/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.450371 vstutils-5.4.3/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.3/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.3/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.3/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.450371 vstutils-5.4.3/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10704 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.3/vstutils/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.426371 vstutils-5.4.3/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.462371 vstutils-5.4.3/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   432629 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.462371 vstutils-5.4.3/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.462371 vstutils-5.4.3/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5181 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.466371 vstutils-5.4.3/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.3/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.3/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.3/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.3/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.466371 vstutils-5.4.3/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.3/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.3/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.466371 vstutils-5.4.3/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.466371 vstutils-5.4.3/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.3/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.466371 vstutils-5.4.3/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.470371 vstutils-5.4.3/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.470371 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.470371 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.470371 vstutils-5.4.3/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.470371 vstutils-5.4.3/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.3/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.3/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.3/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    17731 2023-02-13 06:24:20.000000 vstutils-5.4.3/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.474371 vstutils-5.4.3/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.3/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.3/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.3/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    44646 2023-02-09 12:14:31.000000 vstutils-5.4.3/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.3/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.3/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 03:38:17.438371 vstutils-5.4.3/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4459 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7644 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 03:37:06.000000 vstutils-5.4.3/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1942 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-17 03:38:17.000000 vstutils-5.4.3/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-12 21:40:56.159942 vstutils-5.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-18 02:33:32.000000 vstutils-5.4.4/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.4/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.4/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-13 03:48:29.000000 vstutils-5.4.4/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.4/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.4/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-13 03:48:29.000000 vstutils-5.4.4/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-03-20 21:33:20.000000 vstutils-5.4.4/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-12 21:40:56.159942 vstutils-5.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.123942 vstutils-5.4.4/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-11 10:56:05.000000 vstutils-5.4.4/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.127942 vstutils-5.4.4/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    27865 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24054 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.4/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51728 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11397 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.4/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10784 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.4/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.111942 vstutils-5.4.4/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-12 21:40:56.167942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.135942 vstutils-5.4.4/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.4/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.4/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.135942 vstutils-5.4.4/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10704 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.4/vstutils/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.115942 vstutils-5.4.4/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-12 21:40:55.000000 vstutils-5.4.4/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   432610 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.4/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.4/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.4/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.4/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.4/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    17731 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    44646 2023-02-09 12:14:31.000000 vstutils-5.4.4/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.123942 vstutils-5.4.4/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7644 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.4.3/LICENSE` & `vstutils-5.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/MANIFEST.in` & `vstutils-5.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/NOTICE` & `vstutils-5.4.4/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/PKG-INFO` & `vstutils-5.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.3
+Version: 5.4.4
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.3/README.rst` & `vstutils-5.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/requirements.txt` & `vstutils-5.4.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/setup.cfg` & `vstutils-5.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/setup.py` & `vstutils-5.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/actions.py` & `vstutils-5.4.4/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/admin.py` & `vstutils-5.4.4/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/auth.py` & `vstutils-5.4.4/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/base.py` & `vstutils-5.4.4/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/decorators.py` & `vstutils-5.4.4/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/decorators.pyi` & `vstutils-5.4.4/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/doc_generator.py` & `vstutils-5.4.4/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/endpoint.py` & `vstutils-5.4.4/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/fields.py` & `vstutils-5.4.4/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/filter_backends.py` & `vstutils-5.4.4/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/filters.py` & `vstutils-5.4.4/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/health.py` & `vstutils-5.4.4/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/meta.py` & `vstutils-5.4.4/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/metrics.py` & `vstutils-5.4.4/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0001_initial.py` & `vstutils-5.4.4/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.4.4/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.4.4/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.4.4/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.4.4/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.4.4/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/models.py` & `vstutils-5.4.4/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/pagination.py` & `vstutils-5.4.4/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/parsers.py` & `vstutils-5.4.4/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/permissions.py` & `vstutils-5.4.4/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/renderers.py` & `vstutils-5.4.4/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/responses.py` & `vstutils-5.4.4/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/responses.pyi` & `vstutils-5.4.4/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/routers.py` & `vstutils-5.4.4/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/routers.pyi` & `vstutils-5.4.4/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/schema/generators.py` & `vstutils-5.4.4/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/schema/info.py` & `vstutils-5.4.4/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/schema/inspectors.py` & `vstutils-5.4.4/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/schema/schema.py` & `vstutils-5.4.4/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/serializers.py` & `vstutils-5.4.4/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/throttling.py` & `vstutils-5.4.4/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/validators.py` & `vstutils-5.4.4/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/api/views.py` & `vstutils-5.4.4/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/asgi.py` & `vstutils-5.4.4/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/asgi_worker.py` & `vstutils-5.4.4/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/auth.py` & `vstutils-5.4.4/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/auth.pyi` & `vstutils-5.4.4/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/celery_beat_scheduler.py` & `vstutils-5.4.4/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/environment.py` & `vstutils-5.4.4/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/exceptions.py` & `vstutils-5.4.4/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/gui/context.py` & `vstutils-5.4.4/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/gui/forms.py` & `vstutils-5.4.4/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/gui/pwa_manifest.py` & `vstutils-5.4.4/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/gui/views.py` & `vstutils-5.4.4/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/ldap_utils.py` & `vstutils-5.4.4/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/_base.py` & `vstutils-5.4.4/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/celery_inspect.py` & `vstutils-5.4.4/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/dockerrun.py` & `vstutils-5.4.4/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/newproject.py` & `vstutils-5.4.4/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/run_task.py` & `vstutils-5.4.4/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/runrpc.py` & `vstutils-5.4.4/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/runserver.py` & `vstutils-5.4.4/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/management/commands/web.py` & `vstutils-5.4.4/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/middleware.py` & `vstutils-5.4.4/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/__init__.py` & `vstutils-5.4.4/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/base.py` & `vstutils-5.4.4/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/cent_notify.py` & `vstutils-5.4.4/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/custom_model.py` & `vstutils-5.4.4/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/custom_model.pyi` & `vstutils-5.4.4/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/decorators.py` & `vstutils-5.4.4/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/fields.py` & `vstutils-5.4.4/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/models/queryset.py` & `vstutils-5.4.4/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/settings.ini` & `vstutils-5.4.4/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/settings.py` & `vstutils-5.4.4/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/281.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/296.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/345.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/368.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/421.js` & `vstutils-5.4.4/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.4.4/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/618.js` & `vstutils-5.4.4/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/683.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/686.js` & `vstutils-5.4.4/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/742.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.4.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/755.js` & `vstutils-5.4.4/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/826.chunk.js` & `vstutils-5.4.4/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.4.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/844.js` & `vstutils-5.4.4/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/959.js` & `vstutils-5.4.4/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.4.4/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/app_loader.js` & `vstutils-5.4.4/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/base.js` & `vstutils-5.4.4/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.4.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.4.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/output.json` & `vstutils-5.4.4/vstutils/static/bundle/output.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964192708333334%*

 * *Differences: {"'entrypoints'": "{'spa': {'assets': {0: {'size': 432610}}, 'assetsSize': 3679153}}"}*

```diff
@@ -26,15 +26,15 @@
             "filteredAuxiliaryAssets": 0,
             "name": "base"
         },
         "spa": {
             "assets": [
                 {
                     "name": "vstutils.js",
-                    "size": 432629
+                    "size": 432610
                 },
                 {
                     "name": "755.js",
                     "size": 89997
                 },
                 {
                     "name": "421.js",
@@ -57,15 +57,15 @@
                     "size": 1798980
                 },
                 {
                     "name": "spa.js",
                     "size": 3597
                 }
             ],
-            "assetsSize": 3679172,
+            "assetsSize": 3679153,
             "auxiliaryAssetsSize": 117924,
             "filteredAssets": 0,
             "filteredAuxiliaryAssets": 2,
             "name": "spa"
         }
     },
     "errors": []
```

### Comparing `vstutils-5.4.3/vstutils/static/bundle/spa.js` & `vstutils-5.4.4/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static/bundle/vstutils.js` & `vstutils-5.4.4/vstutils/static/bundle/vstutils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2062,23 +2062,22 @@
                 w = n(44589),
                 x = n.n(w),
                 C = n(87305),
                 S = {};
             S.styleTagTransform = x(), S.setAttributes = _(), S.insert = v().bind(null, "head"), S.domAPI = h(), S.insertStyleElement = y(), p()(C.Z, S), C.Z && C.Z.locals && C.Z.locals;
             var k = (0, n(51900).Z)(d, r, [], !1, null, "38a98dfb", null).exports,
                 F = n(66044),
-                Z = n(90548),
-                A = n(42950);
+                Z = n(90548);
             s.pp.once("models[_UserSettings].fields.beforeInit", (e => {
                 e.custom.title = "Custom settings", e.main.title = "Main settings"
             }));
-            const T = "/user/",
-                P = "".concat(T, "{id}/");
+            const A = "/user/",
+                T = "".concat(A, "{id}/");
 
-            function E(e) {
+            function P(e) {
                 e.actions.set("generate_password", {
                     name: "generate_password",
                     title: "Generate password",
                     handler: () => {
                         const e = (0, u.getApp)(),
                             t = (0, u.generatePassword)();
                         e.store.page.setFieldValue({
@@ -2091,37 +2090,37 @@
                     }
                 })
             }
             s.pp.once("app.afterInit", (e => {
                 let {
                     app: t
                 } = e;
-                const n = "".concat(T).concat(t.api.getUserId()),
+                const n = "".concat(A).concat(t.api.getUserId()),
                     i = "/profile";
                 t.router.beforeEach(((e, t, s) => {
                     e.path.startsWith(i) ? s({
                         path: e.path.replace(i, n)
                     }) : s()
                 }))
             })), s.pp.once("openapi.loaded", (e => {
-                e.paths["".concat(P, "twofa/")]["x-edit-style"] = !0
+                e.paths["".concat(T, "twofa/")]["x-edit-style"] = !0
             })), s.pp.once("allModels.created", (e => {
                 let {
                     models: t
                 } = e;
                 t.get("TwoFA").viewField = null
             })), s.pp.once("allViews.created", (e => {
                 let {
                     views: t
                 } = e;
-                const n = t.get(P);
+                const n = t.get(T);
                 n.sublinks.delete("_settings");
                 const s = n.sublinks.get("twofa");
                 s.title = "Two factor authentication", s.iconClasses = ["fas", "fa-lock"];
-                const a = t.get("".concat(P, "twofa/"));
+                const a = t.get("".concat(T, "twofa/"));
                 a.mixins.push(k), a.params.method = "PUT", a.title = "Two factor authentication", a.extendStore((e => {
                     const t = (0, u.getApp)(),
                         n = (0, i.computed)((() => {
                             if (e.sandbox.value.secret) {
                                 const n = t.user.getViewFieldValue();
                                 return "otpauth://totp/".concat(n, "@").concat(t.config.projectName, "?secret=").concat(e.sandbox.secret)
                             }
@@ -2147,59 +2146,55 @@
                                     value: t.join(","),
                                     markChanged: !1
                                 })
                             }
                         },
                         secretUri: n
                     }
-                })), t.get("".concat(P, "_settings/")).hidden = !0;
+                })), t.get("".concat(T, "_settings/")).hidden = !0;
                 const r = t.get("/user/{id}/change_password/");
-                r && E(r);
+                r && P(r);
                 const o = t.get("/user/new/");
-                o && E(o)
+                o && P(o)
             })), s.pp.connect("</user/{id}/twofa/>filterActions", (e => {
                 const t = (0, u.getApp)();
                 e.actions = [{
                     name: "save",
                     title: e.data.enabled ? "Disable" : "Enable",
                     async handler() {
                         try {
                             t.store.page.validateAndSetInstanceData()
                         } catch (e) {
                             return void t.error_handler.defineErrorAndShow(e)
                         }
                         t.store.page.loading = !0;
                         const e = t.store.page.instance;
                         try {
-                            await e.update("put"), t.store.page.loading = !1, t.store.page.changedFields = [], Z.guiPopUp.success(t.i18n.t(Z.pop_up_msg.instance.success.save, ["", "TFA"])), (0, u.openPage)({
-                                path: (0, A.B8)({
-                                    instance: e
-                                })
-                            })
+                            await e.update("put"), t.store.page.loading = !1, t.store.page.changedFields = [], Z.guiPopUp.success(t.i18n.t(Z.pop_up_msg.instance.success.save, ["", "TFA"])), await (0, l.useViewStore)().fetchData()
                         } catch (e) {
                             t.store.page.loading = !1;
                             let n = t.error_handler.errorToString(e),
                                 i = t.i18n.t(Z.pop_up_msg.instance.error.save, [n]);
                             t.error_handler.showError(i, n)
                         }
                     }
                 }]
             }));
-            class V extends F.IntegerField {
+            class E extends F.IntegerField {
                 toInner() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return "profile" === this._getValueFromData(e) ? "profile" : super.toInner(e)
                 }
             }
             s.pp.once("allViews.created", (e => {
                 let {
                     views: t
                 } = e;
                 const n = new Set(Array.from(t.values()).filter((e => e.path.startsWith("/user/{id}/") && e.objects)).map((e => e.objects)));
-                for (const e of n) e.pathParams.length > 0 && (e.pathParams[0] = new V(e.pathParams[0].options))
+                for (const e of n) e.pathParams.length > 0 && (e.pathParams[0] = new E(e.pathParams[0].options))
             }))
         },
         32465: function(e, t, n) {
             n.d(t, {
                 Nv: function() {
                     return N
                 },
```

### Comparing `vstutils-5.4.3/vstutils/static/img/anonymous.png` & `vstutils-5.4.4/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/static_files.py` & `vstutils-5.4.4/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/tasks.py` & `vstutils-5.4.4/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/auth/base.html` & `vstutils-5.4.4/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/auth/language_selector.html` & `vstutils-5.4.4/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/auth/tfa.html` & `vstutils-5.4.4/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/base.html` & `vstutils-5.4.4/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/gui/base.html` & `vstutils-5.4.4/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/gui/offline.html` & `vstutils-5.4.4/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/gui/service-worker.js` & `vstutils-5.4.4/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.4.4/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/package.json.template` & `vstutils-5.4.4/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.4.4/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/setup.py.template` & `vstutils-5.4.4/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/test.py.template` & `vstutils-5.4.4/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.4.4/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.4.4/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.4.4/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/registration/confirm_email.html` & `vstutils-5.4.4/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.4.4/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.4.4/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/registration/user_registration.html` & `vstutils-5.4.4/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/rest_framework/admin.html` & `vstutils-5.4.4/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.4.4/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templatetags/request_static.py` & `vstutils-5.4.4/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templatetags/translation.py` & `vstutils-5.4.4/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.4.4/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.4.4/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/templatetags/vstconfigs.py` & `vstutils-5.4.4/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/tests.py` & `vstutils-5.4.4/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/tools.py` & `vstutils-5.4.4/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/translations/cn.py` & `vstutils-5.4.4/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/translations/ru.py` & `vstutils-5.4.4/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/translations/vi.py` & `vstutils-5.4.4/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/urls.py` & `vstutils-5.4.4/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/utils.py` & `vstutils-5.4.4/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/web.ini` & `vstutils-5.4.4/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils/wsgi.py` & `vstutils-5.4.4/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils.egg-info/PKG-INFO` & `vstutils-5.4.4/vstutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.3
+Version: 5.4.4
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.3/vstutils.egg-info/SOURCES.txt` & `vstutils-5.4.4/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.3/vstutils.egg-info/requires.txt` & `vstutils-5.4.4/vstutils.egg-info/requires.txt`

 * *Files identical despite different names*

