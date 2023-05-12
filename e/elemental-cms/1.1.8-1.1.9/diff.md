# Comparing `tmp/elemental-cms-1.1.8.tar.gz` & `tmp/elemental-cms-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elemental-cms-1.1.8.tar", last modified: Sun Sep  4 18:22:32 2022, max compression
+gzip compressed data, was "elemental-cms-1.1.9.tar", last modified: Mon Sep  5 14:20:29 2022, max compression
```

## Comparing `elemental-cms-1.1.8.tar` & `elemental-cms-1.1.9.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elemental_cms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-04 18:22:32.000000 elemental-cms-1.1.8/elemental_cms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/
--rw-r--r--   0 runner    (1001) docker     (121)     6923 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/admin/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/admin/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.348483 elemental-cms-1.1.8/elementalcms/admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/admin/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/core/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/core/elementalcontext.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/core/flaskcontext.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/core/mongodbcontext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/extends/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/extends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/extends/actionsdecorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/extends/actionsmapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/extends/applet.py
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/extends/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/management/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldeps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/globaldepscommands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/media.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/management/mediacommands/
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/mediacommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/mediacommands/delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/mediacommands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/mediacommands/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/mediacommands/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/management/pagescommands/
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/pagescommands/unpublish.py
--rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/management/snippetscommands/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/snippetscommands/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/management/staticcommands/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/staticcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/staticcommands/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/staticcommands/delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/management/staticcommands/list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/persistence/models/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/models/mongosession.py
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/mongodbconnectionmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/mongosessioninterface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/persistence/repositories/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/draftsrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/genericrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/globaldepsrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/pagesrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/sessionsrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/persistence/repositories/snippetsrepository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/presenter/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/presenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/presenter/presenter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/presenter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/presenter/templates/presenter/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/presenter/templates/presenter/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.356483 elemental-cms-1.1.8/elementalcms/services/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/services/global_deps/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/getall.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/getme.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/getone.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/removeone.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/global_deps/updateone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/services/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/getall.py
--rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/gethome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/getme.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/getone.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/removeone.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/pages/updateone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/services/sessions/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/sessions/createexpirationindex.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/sessions/getme.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/sessions/upsertme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/services/snippets/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/getall.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/getmany.py
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/getme.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/getone.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/removeone.py
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/snippets/updateone.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/usecaseresult.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/services/users/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/services/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/static/admin/client-stack/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/static/admin/client-stack/modules/
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/static/admin/client-stack/modules/html-editor.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.352483 elemental-cms-1.1.8/elementalcms/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/elementalcms/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/elementalcms/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 18:22:32.360483 elemental-cms-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-09-04 18:22:25.000000 elemental-cms-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elemental_cms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-05 14:20:29.000000 elemental-cms-1.1.9/elemental_cms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/
+-rw-r--r--   0 runner    (1001) docker     (121)     6923 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/admin/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/admin/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.326061 elemental-cms-1.1.9/elementalcms/admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/admin/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/core/elementalcontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/core/flaskcontext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/core/mongodbcontext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/extends/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/extends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/extends/actionsdecorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/extends/actionsmapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/extends/applet.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/extends/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.334061 elemental-cms-1.1.9/elementalcms/management/
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4900 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3166 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldeps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.334061 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2734 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/globaldepscommands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/media.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.334061 elemental-cms-1.1.9/elementalcms/management/mediacommands/
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/mediacommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/mediacommands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/mediacommands/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/mediacommands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/mediacommands/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4229 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pages.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.338061 elemental-cms-1.1.9/elementalcms/management/pagescommands/
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      637 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4396 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2079 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/pagescommands/unpublish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2643 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.338061 elemental-cms-1.1.9/elementalcms/management/snippetscommands/
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3032 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/snippetscommands/remove.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/static.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.338061 elemental-cms-1.1.9/elementalcms/management/staticcommands/
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/staticcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2616 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/staticcommands/collect.py
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/staticcommands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/management/staticcommands/list.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/persistence/
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/persistence/models/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/models/mongosession.py
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/mongodbconnectionmanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/mongosessioninterface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/persistence/repositories/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/draftsrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/genericrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/globaldepsrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/pagesrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/sessionsrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/persistence/repositories/snippetsrepository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/presenter/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/presenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5244 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/presenter/presenter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.326061 elemental-cms-1.1.9/elementalcms/presenter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/presenter/templates/presenter/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/presenter/templates/presenter/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/services/
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.342061 elemental-cms-1.1.9/elementalcms/services/global_deps/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/getall.py
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/getme.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/getone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/removeone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/global_deps/updateone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/services/pages/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/getall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1664 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/gethome.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/getme.py
+-rw-r--r--   0 runner    (1001) docker     (121)      655 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/getone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/removeone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/pages/updateone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/services/sessions/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/sessions/createexpirationindex.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/sessions/getme.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/sessions/upsertme.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/services/snippets/
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/getall.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/getmany.py
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/getme.py
+-rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/getone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/removeone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/snippets/updateone.py
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/usecaseresult.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/services/users/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/services/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.326061 elemental-cms-1.1.9/elementalcms/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.326061 elemental-cms-1.1.9/elementalcms/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/static/admin/client-stack/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/static/admin/client-stack/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/static/admin/client-stack/modules/html-editor.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/translations/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.330061 elemental-cms-1.1.9/elementalcms/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/elementalcms/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/elementalcms/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 14:20:29.346061 elemental-cms-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-09-05 14:20:15.000000 elemental-cms-1.1.9/setup.py
```

### Comparing `elemental-cms-1.1.8/LICENSE` & `elemental-cms-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/PKG-INFO` & `elemental-cms-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elemental-cms
-Version: 1.1.8
+Version: 1.1.9
 Summary: Flask + MongoDB Web CMS for Developers.
 Home-page: https://github.com/paranoid-software/elemental-cms
 Author: Paranoid Software
 Author-email: info@paranoid.software
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `elemental-cms-1.1.8/elemental_cms.egg-info/PKG-INFO` & `elemental-cms-1.1.9/elemental_cms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elemental-cms
-Version: 1.1.8
+Version: 1.1.9
 Summary: Flask + MongoDB Web CMS for Developers.
 Home-page: https://github.com/paranoid-software/elemental-cms
 Author: Paranoid Software
 Author-email: info@paranoid.software
 License: MPL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `elemental-cms-1.1.8/elemental_cms.egg-info/SOURCES.txt` & `elemental-cms-1.1.9/elemental_cms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/__init__.py` & `elemental-cms-1.1.9/elementalcms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from elementalcms.persistence import MongoSessionInterface
 from elementalcms.services.snippets import GetMe
 
 from elementalcms.admin import admin
 from elementalcms.presenter import presenter
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 
 class Elemental:
 
     __applets = {}
 
     def get_view_for(self, applet_name, controller_name, action_name):
```

### Comparing `elemental-cms-1.1.8/elementalcms/admin/admin.py` & `elemental-cms-1.1.9/elementalcms/admin/admin.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/admin/templates/admin/index.html` & `elemental-cms-1.1.9/elementalcms/admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/core/flaskcontext.py` & `elemental-cms-1.1.9/elementalcms/core/flaskcontext.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/core/mongodbcontext.py` & `elemental-cms-1.1.9/elementalcms/core/mongodbcontext.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/extends/actionsdecorators.py` & `elemental-cms-1.1.9/elementalcms/extends/actionsdecorators.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/extends/actionsmapper.py` & `elemental-cms-1.1.9/elementalcms/extends/actionsmapper.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/cli.py` & `elemental-cms-1.1.9/elementalcms/management/cli.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldeps.py` & `elemental-cms-1.1.9/elementalcms/management/globaldeps.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldepscommands/create.py` & `elemental-cms-1.1.9/elementalcms/management/globaldepscommands/create.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldepscommands/list.py` & `elemental-cms-1.1.9/elementalcms/management/globaldepscommands/list.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldepscommands/pull.py` & `elemental-cms-1.1.9/elementalcms/management/globaldepscommands/pull.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldepscommands/push.py` & `elemental-cms-1.1.9/elementalcms/management/globaldepscommands/push.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/globaldepscommands/remove.py` & `elemental-cms-1.1.9/elementalcms/management/globaldepscommands/remove.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/media.py` & `elemental-cms-1.1.9/elementalcms/management/media.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/mediacommands/delete.py` & `elemental-cms-1.1.9/elementalcms/management/mediacommands/delete.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/mediacommands/list.py` & `elemental-cms-1.1.9/elementalcms/management/mediacommands/list.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/mediacommands/pull.py` & `elemental-cms-1.1.9/elementalcms/management/mediacommands/pull.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/mediacommands/push.py` & `elemental-cms-1.1.9/elementalcms/management/mediacommands/push.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pages.py` & `elemental-cms-1.1.9/elementalcms/management/pages.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/create.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/create.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/list.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/list.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/publish.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/publish.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/pull.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/pull.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/push.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/push.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/remove.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/remove.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/pagescommands/unpublish.py` & `elemental-cms-1.1.9/elementalcms/management/pagescommands/unpublish.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippets.py` & `elemental-cms-1.1.9/elementalcms/management/snippets.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippetscommands/create.py` & `elemental-cms-1.1.9/elementalcms/management/snippetscommands/create.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippetscommands/list.py` & `elemental-cms-1.1.9/elementalcms/management/snippetscommands/list.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippetscommands/pull.py` & `elemental-cms-1.1.9/elementalcms/management/snippetscommands/pull.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippetscommands/push.py` & `elemental-cms-1.1.9/elementalcms/management/snippetscommands/push.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/snippetscommands/remove.py` & `elemental-cms-1.1.9/elementalcms/management/snippetscommands/remove.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/static.py` & `elemental-cms-1.1.9/elementalcms/management/static.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/staticcommands/collect.py` & `elemental-cms-1.1.9/elementalcms/management/staticcommands/collect.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/staticcommands/delete.py` & `elemental-cms-1.1.9/elementalcms/management/staticcommands/delete.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/management/staticcommands/list.py` & `elemental-cms-1.1.9/elementalcms/management/staticcommands/list.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/persistence/mongodbconnectionmanager.py` & `elemental-cms-1.1.9/elementalcms/persistence/mongodbconnectionmanager.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/persistence/mongosessioninterface.py` & `elemental-cms-1.1.9/elementalcms/persistence/mongosessioninterface.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/persistence/repositories/genericrepository.py` & `elemental-cms-1.1.9/elementalcms/persistence/repositories/genericrepository.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/persistence/repositories/sessionsrepository.py` & `elemental-cms-1.1.9/elementalcms/persistence/repositories/sessionsrepository.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/presenter/presenter.py` & `elemental-cms-1.1.9/elementalcms/presenter/presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     if 'langCode' not in session or session['langCode'] != lang_mode:
         session['langCode'] = lang_code
 
     return render_template('presenter/index.html',
                            page=get_page_model(result.value()))
 
 
+@presenter.route('/<path:slug>', methods=['GET'])
 @presenter.route('/<path:slug>/', methods=['GET'])
 def render(slug: str, lang_code: str = None):
 
     draft = request.args.get('draft')
     lang_mode = current_app.config['LANGUAGE_MODE']
 
     if lang_code is None and lang_mode == 'single':
```

### Comparing `elemental-cms-1.1.8/elementalcms/services/global_deps/getall.py` & `elemental-cms-1.1.9/elementalcms/services/global_deps/getall.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/global_deps/getme.py` & `elemental-cms-1.1.9/elementalcms/services/global_deps/getme.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/global_deps/getone.py` & `elemental-cms-1.1.9/elementalcms/services/global_deps/getone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/global_deps/updateone.py` & `elemental-cms-1.1.9/elementalcms/services/global_deps/updateone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/getall.py` & `elemental-cms-1.1.9/elementalcms/services/pages/getall.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/gethome.py` & `elemental-cms-1.1.9/elementalcms/services/pages/gethome.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/getme.py` & `elemental-cms-1.1.9/elementalcms/services/pages/getme.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/getone.py` & `elemental-cms-1.1.9/elementalcms/services/pages/getone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/removeone.py` & `elemental-cms-1.1.9/elementalcms/services/pages/removeone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/pages/updateone.py` & `elemental-cms-1.1.9/elementalcms/services/pages/updateone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/sessions/getme.py` & `elemental-cms-1.1.9/elementalcms/services/sessions/getme.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/sessions/upsertme.py` & `elemental-cms-1.1.9/elementalcms/services/sessions/upsertme.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/snippets/getall.py` & `elemental-cms-1.1.9/elementalcms/services/snippets/getall.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/snippets/getmany.py` & `elemental-cms-1.1.9/elementalcms/services/snippets/getmany.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/snippets/getme.py` & `elemental-cms-1.1.9/elementalcms/services/snippets/getme.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/snippets/getone.py` & `elemental-cms-1.1.9/elementalcms/services/snippets/getone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/snippets/updateone.py` & `elemental-cms-1.1.9/elementalcms/services/snippets/updateone.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/services/usecaseresult.py` & `elemental-cms-1.1.9/elementalcms/services/usecaseresult.py`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/static/admin/client-stack/modules/html-editor.js` & `elemental-cms-1.1.9/elementalcms/static/admin/client-stack/modules/html-editor.js`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/templates/base.html` & `elemental-cms-1.1.9/elementalcms/templates/base.html`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/elementalcms/translations/es/LC_MESSAGES/messages.po` & `elemental-cms-1.1.9/elementalcms/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `elemental-cms-1.1.8/setup.py` & `elemental-cms-1.1.9/setup.py`

 * *Files identical despite different names*

