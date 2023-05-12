# Comparing `tmp/netbox-bgp-0.8.1.tar.gz` & `tmp/netbox-bgp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netbox-bgp/netbox-bgp/dist/tmpvbaqr3r5/netbox-bgp-0.8.1.tar", last modified: Fri Sep 16 08:22:09 2022, max compression
+gzip compressed data, was "/home/runner/work/netbox-bgp/netbox-bgp/dist/.tmp-blmz1rad/netbox-bgp-0.9.0.tar", last modified: Wed Jan 25 08:20:34 2023, max compression
```

## Comparing `netbox-bgp-0.8.1.tar` & `netbox-bgp-0.9.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (116)    10174 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       45 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1865 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1421 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/
--rw-r--r--   0 runner    (1001) docker     (116)      515 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      713 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/api/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5981 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (116)      633 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     1295 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/api/views.py
--rw-r--r--   0 runner    (1001) docker     (116)     2323 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/choices.py
--rw-r--r--   0 runner    (1001) docker     (116)     6647 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/filters.py
--rw-r--r--   0 runner    (1001) docker     (116)    11295 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/forms.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1438 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     4121 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)      962 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0002_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2061 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0003_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      526 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0004_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      352 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0005_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      405 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0006_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      406 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0007_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0008_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      422 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0009_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1486 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0010_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2011 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0011_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      544 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0012_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      433 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0013_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      321 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0014_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      957 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0015_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      670 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0016_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1027 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0017_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1060 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0018_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      519 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0019_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      518 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0020_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3470 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0021_netbox32_support.py
--rw-r--r--   0 runner    (1001) docker     (116)     2013 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0022_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3110 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0023_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1098 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0024_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)      689 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0025_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)     2185 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/0026_netbox_bgp.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10084 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     2588 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/navigation.py
--rw-r--r--   0 runner    (1001) docker     (116)     4128 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/tables.py
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/
--rw-r--r--   0 runner    (1001) docker     (116)     3349 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/bgppeergroup.html
--rw-r--r--   0 runner    (1001) docker     (116)     6746 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/bgpsession.html
--rw-r--r--   0 runner    (1001) docker     (116)     3175 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/community.html
--rw-r--r--   0 runner    (1001) docker     (116)      242 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/device_extend.html
--rw-r--r--   0 runner    (1001) docker     (116)     3272 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/prefixlist.html
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/prefixlistrule.html
--rw-r--r--   0 runner    (1001) docker     (116)     3293 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/routingpolicy.html
--rw-r--r--   0 runner    (1001) docker     (116)     2649 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/routingpolicyrule.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11248 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      685 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (116)     5785 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (116)     5459 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/version.py
--rw-r--r--   0 runner    (1001) docker     (116)     9517 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/netbox_bgp/views.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1865 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2192 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/netbox_bgp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-16 08:22:09.000000 netbox-bgp-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1212 2022-09-16 08:21:58.000000 netbox-bgp-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)    10174 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       45 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1892 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1448 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/
+-rw-r--r--   0 runner    (1001) docker     (116)      549 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      713 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/api/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5981 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      806 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1815 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2333 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/choices.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8528 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/filters.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11295 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1438 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (116)     4121 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (116)      962 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0002_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2061 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0003_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      526 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0004_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      352 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0005_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      405 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0006_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      406 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0007_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1673 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0008_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      422 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0009_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1486 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0010_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2011 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0011_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      544 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0012_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      433 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0013_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      321 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0014_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      957 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0015_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      670 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0016_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1027 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0017_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1060 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0018_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      519 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0019_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      518 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0020_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3470 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0021_netbox32_support.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2013 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0022_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3110 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0023_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1098 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0024_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)      689 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0025_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2185 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0026_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1847 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/0027_netbox_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10084 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2911 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4128 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/tables.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1021 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/
+-rw-r--r--   0 runner    (1001) docker     (116)     3349 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/bgppeergroup.html
+-rw-r--r--   0 runner    (1001) docker     (116)     6746 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/bgpsession.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3175 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/community.html
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/device_extend.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3286 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/prefixlist.html
+-rw-r--r--   0 runner    (1001) docker     (116)     2133 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/prefixlistrule.html
+-rw-r--r--   0 runner    (1001) docker     (116)     3314 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/routingpolicy.html
+-rw-r--r--   0 runner    (1001) docker     (116)     2649 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/routingpolicyrule.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11248 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (116)      685 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5785 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5459 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9515 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/netbox_bgp/views.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1892 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2233 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/netbox_bgp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-25 08:20:34.000000 netbox-bgp-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1212 2023-01-25 08:20:26.000000 netbox-bgp-0.9.0/setup.py
```

### Comparing `netbox-bgp-0.8.1/LICENSE` & `netbox-bgp-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/PKG-INFO` & `netbox-bgp-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-bgp
-Version: 0.8.1
+Version: 0.9.0
 Summary: BGP related stuff
 Home-page: https://github.com/k01ek/netbox-bgp
 Author: Nikolay Yuzefovich
 Author-email: mgk.kolek@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
@@ -28,14 +28,15 @@
 |-------------|-------|
 | NetBox 2.10 | 0.3.9 |
 | NetBox 2.11 | 0.3.9 |
 | NetBox 3.0  | 0.4.3 |
 | NetBox 3.1  | 0.5.0 |
 | NetBox 3.2  | >= 0.6.0 |
 | NetBox 3.3  | >= 0.8.1 |
+| NetBox 3.4  | >= 0.9.0 |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip  
 
 ```
 pip install netbox-bgp
```

### Comparing `netbox-bgp-0.8.1/README.md` & `netbox-bgp-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 |-------------|-------|
 | NetBox 2.10 | 0.3.9 |
 | NetBox 2.11 | 0.3.9 |
 | NetBox 3.0  | 0.4.3 |
 | NetBox 3.1  | 0.5.0 |
 | NetBox 3.2  | >= 0.6.0 |
 | NetBox 3.3  | >= 0.8.1 |
+| NetBox 3.4  | >= 0.9.0 |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip  
 
 ```
 pip install netbox-bgp
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/__init__.py` & `netbox-bgp-0.9.0/netbox_bgp/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     verbose_name = 'BGP'
     description = 'Subsystem for tracking bgp related objects'
     version = __version__
     author = 'Nikolay Yuzefovich'
     author_email = 'mgk.kolek@gmail.com'
     base_url = 'bgp'
     required_settings = []
-    min_version = '3.2.0'
-    max_version = '3.3.99'
+    min_version = '3.4.0'
+    max_version = '3.4.99'
     default_settings = {
         'device_ext_page': 'right',
+        'top_level_menu' : False,
     }
 
 
 config = BGPConfig # noqa
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/admin.py` & `netbox-bgp-0.9.0/netbox_bgp/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/api/serializers.py` & `netbox-bgp-0.9.0/netbox_bgp/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/api/urls.py` & `netbox-bgp-0.9.0/netbox_bgp/api/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from rest_framework import routers
 
 from .views import (
     BGPSessionViewSet, RoutingPolicyViewSet, BGPPeerGroupViewSet, CommunityViewSet,
-    PrefixListViewSet
+    PrefixListViewSet, PrefixListRuleViewSet, RoutingPolicyRuleViewSet
 )
 
 router = routers.DefaultRouter()
 router.register('session', BGPSessionViewSet, 'session')
 router.register('bgpsession', BGPSessionViewSet, 'bgpsession')
 router.register('routing-policy', RoutingPolicyViewSet)
+router.register('routing-policy-rule', RoutingPolicyRuleViewSet)
 router.register('peer-group', BGPPeerGroupViewSet, 'peergroup')
 router.register('bgppeergroup', BGPPeerGroupViewSet, 'bgppeergroup')
 router.register('community', CommunityViewSet)
 router.register('prefix-list', PrefixListViewSet)
+router.register('prefix-list-rule', PrefixListRuleViewSet)
 
 
 urlpatterns = router.urls
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/choices.py` & `netbox-bgp-0.9.0/netbox_bgp/choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,14 @@
         (AFISAFI_VPNV6_MULTICAST, 'VPNv6 Multicast'),
         (AFISAFI_VPNV6_FLOWSPEC, 'VPNv6 Flowspec')
     )
 
 
 class IPAddressFamilyChoices(ChoiceSet):
 
-    FAMILY_4 = 4
-    FAMILY_6 = 6
+    FAMILY_4 = 'ipv4'
+    FAMILY_6 = 'ipv6'
 
     CHOICES = (
         (FAMILY_4, 'IPv4'),
         (FAMILY_6, 'IPv6'),
     )
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/filters.py` & `netbox-bgp-0.9.0/netbox_bgp/filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import django_filters
 import netaddr
 from django.db.models import Q
 from netaddr.core import AddrFormatError
 from extras.filters import TagFilter
+from netbox.filtersets import NetBoxModelFilterSet
 
-from .models import Community, BGPSession, RoutingPolicy, BGPPeerGroup, PrefixList
+from .models import Community, BGPSession, RoutingPolicy, RoutingPolicyRule, BGPPeerGroup, PrefixList, PrefixListRule
 from ipam.models import IPAddress, ASN
 from dcim.models import Device
 
 
-class CommunityFilterSet(django_filters.FilterSet):
+class CommunityFilterSet(NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
     tag = TagFilter()
 
     class Meta:
@@ -28,35 +29,35 @@
                 Q(id__icontains=value)
                 | Q(value__icontains=value)
                 | Q(description__icontains=value)
         )
         return queryset.filter(qs_filter)
 
 
-class BGPSessionFilterSet(django_filters.FilterSet):
+class BGPSessionFilterSet(NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
     tag = TagFilter()
 
     remote_as = django_filters.ModelMultipleChoiceFilter(
-        field_name='remote_as__number',
+        field_name='remote_as__asn',
         queryset=ASN.objects.all(),
         to_field_name='asn',
         label='Remote AS (Number)',
     )
     remote_as_id = django_filters.ModelMultipleChoiceFilter(
         field_name='remote_as__id',
         queryset=ASN.objects.all(),
         to_field_name='id',
         label='Remote AS (ID)',
     )
     local_as = django_filters.ModelMultipleChoiceFilter(
-        field_name='local_as__number',
+        field_name='local_as__asn',
         queryset=ASN.objects.all(),
         to_field_name='asn',
         label='Local AS (Number)',
     )
     local_as_id = django_filters.ModelMultipleChoiceFilter(
         field_name='local_as__id',
         queryset=ASN.objects.all(),
@@ -122,17 +123,17 @@
         fields = ['name', 'description', 'status', 'tenant']
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = (
-                Q(remote_as__number__icontains=value)
+                Q(remote_as__asn__icontains=value)
                 | Q(name__icontains=value)
-                | Q(local_as__number__icontains=value)
+                | Q(local_as__asn__icontains=value)
                 | Q(description__icontains=value)
         )
         return queryset.filter(qs_filter)
 
     def search_by_remote_ip(self, queryset, name, value):
         if not value.strip():
             return queryset
@@ -148,15 +149,15 @@
         try:
             query = str(netaddr.IPNetwork(value).cidr)
             return queryset.filter(local_address__address=query)
         except (AddrFormatError, ValueError):
             return queryset.none()
 
 
-class RoutingPolicyFilterSet(django_filters.FilterSet):
+class RoutingPolicyFilterSet(NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
     tag = TagFilter()
 
     class Meta:
@@ -170,14 +171,40 @@
         qs_filter = (
                 Q(name__icontains=value)
                 | Q(description__icontains=value)
         )
         return queryset.filter(qs_filter)
 
 
+class RoutingPolicyRuleFilterSet(django_filters.FilterSet):
+    q = django_filters.CharFilter(
+        method='search',
+        label='Search',
+    )
+    tag = TagFilter()
+
+    class Meta:
+        model = RoutingPolicyRule
+        fields = ['id', 'index', 'action', 'description', 'routing_policy_id', 'continue_entry']
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = (
+                Q(id__icontains=value)
+                | Q(index__icontains=value)
+                | Q(action__icontains=value)
+                | Q(description__icontains=value)
+                | Q(routing_policy_id__icontains=value)
+                | Q(continue_entry__icontains=value)
+        )
+        return queryset.filter(qs_filter)
+
+
 class BGPPeerGroupFilterSet(django_filters.FilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
     tag = TagFilter()
 
@@ -192,15 +219,15 @@
         qs_filter = (
                 Q(name__icontains=value)
                 | Q(description__icontains=value)
         )
         return queryset.filter(qs_filter)
 
 
-class PrefixListFilterSet(django_filters.FilterSet):
+class PrefixListFilterSet(NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method='search',
         label='Search',
     )
     tag = TagFilter()
 
     class Meta:
@@ -212,7 +239,35 @@
         if not value.strip():
             return queryset
         qs_filter = (
                 Q(name__icontains=value)
                 | Q(description__icontains=value)
         )
         return queryset.filter(qs_filter)
+
+class PrefixListRuleFilterSet(django_filters.FilterSet):
+    q = django_filters.CharFilter(
+        method='search',
+        label='Search',
+    )
+    tag = TagFilter()
+
+    class Meta:
+        model = PrefixListRule
+        #fields = ['index', 'action', 'prefix_custom', 'ge', 'le', 'prefix_list', 'prefix_list_id']
+        fields = ['id', 'index', 'action', 'ge', 'le', 'prefix_list', 'prefix_list_id']
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        qs_filter = (
+                Q(id__icontains=value)
+                | Q(index__icontains=value)
+                | Q(action__icontains=value)
+                #| Q(prefix_custom__icontains=value)
+                | Q(ge__icontains=value)
+                | Q(le__icontains=value)
+                | Q(prefix_list__icontains=value)
+                | Q(prefix_list_id__icontains=value)
+        )
+        return queryset.filter(qs_filter)
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/forms.py` & `netbox-bgp-0.9.0/netbox_bgp/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/graphql.py` & `netbox-bgp-0.9.0/netbox_bgp/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0001_initial.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0002_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0002_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0003_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0003_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0004_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0004_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0008_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0008_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0010_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0010_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0011_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0011_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0012_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0012_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0015_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0015_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0016_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0016_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0017_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0017_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0018_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0018_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0019_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0019_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0020_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0020_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0021_netbox32_support.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0021_netbox32_support.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0022_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0022_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0023_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0023_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0024_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0024_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0025_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0025_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/migrations/0026_netbox_bgp.py` & `netbox-bgp-0.9.0/netbox_bgp/migrations/0026_netbox_bgp.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/models.py` & `netbox-bgp-0.9.0/netbox_bgp/models.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/navigation.py` & `netbox-bgp-0.9.0/netbox_bgp/navigation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from extras.plugins import PluginMenuButton, PluginMenuItem
+from django.conf import settings
+
+from extras.plugins import PluginMenuButton, PluginMenuItem, PluginMenu
 from utilities.choices import ButtonColorChoices
 
-menu_items = (
+
+_menu_items = (
     PluginMenuItem(
         link='plugins:netbox_bgp:community_list',
         link_text='Communities',
         permissions=['netbox_bgp.view_community'],
         buttons=(
             PluginMenuButton(
                 link='plugins:netbox_bgp:community_add',
@@ -69,7 +72,18 @@
                 icon_class='mdi mdi-plus-thick',
                 color=ButtonColorChoices.GREEN,
                 permissions=['netbox_bgp.add_bgppeergroup'],
             ),
         ),
     )
 )
+
+plugin_settings = settings.PLUGINS_CONFIG.get('netbox_bgp', {})
+
+if plugin_settings.get('top_level_menu'):
+    menu = PluginMenu(  
+        label="BGP",
+        groups=(("BGP", _menu_items),),
+        icon_class="mdi mdi-bootstrap",
+    )
+else:
+    menu_items = _menu_items
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/tables.py` & `netbox-bgp-0.9.0/netbox_bgp/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/template_content.py` & `netbox-bgp-0.9.0/netbox_bgp/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/bgppeergroup.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/bgppeergroup.html`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/bgpsession.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/bgpsession.html`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/community.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/community.html`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/prefixlist.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/prefixlist.html`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 {% block controls %}
 <div class="pull-right noprint">
     {% if perms.netbox_bgp.change_prefixlist %}
     <a href="{% url 'plugins:netbox_bgp:prefixlistrule_add' %}?prefix_list={{ object.pk }}" class="btn btn-success">
         <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Rule
     </a>
     {% endif %}
-    {% if perms.netbox_bgp.change_policy %}
+    {% if perms.netbox_bgp.change_routingpolicy %}
     <a href="{% url 'plugins:netbox_bgp:prefixlist_edit' pk=object.pk %}" class="btn btn-warning">
         <span class="mdi mdi-pencil" aria-hidden="true"></span> Edit
     </a>
     {% endif %}
-    {% if perms.netbox_bgp.delete_policy %}
+    {% if perms.netbox_bgp.delete_routingpolicy %}
     <a href="{% url 'plugins:netbox_bgp:prefixlist_delete' pk=object.pk %}" class="btn btn-danger">
         <span class="mdi mdi-trash-can-outline" aria-hidden="true"></span> Delete
     </a>
     {% endif %}
 </div>
 {% endblock controls %}
 {% block tabs %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load custom_links %}
 {% load helpers %} {% load plugins %} {% load render_table from django_tables2
 %} {% block breadcrumbs %}
 Prefix_Lists
 {% endblock %} {% block controls %}
 {% if perms.netbox_bgp.change_prefixlist %} _Rule {% endif %} {% if
-perms.netbox_bgp.change_policy %} _Edit {% endif %} {% if
-perms.netbox_bgp.delete_policy %} _Delete {% endif %}
+perms.netbox_bgp.change_routingpolicy %} _Edit {% endif %} {% if
+perms.netbox_bgp.delete_routingpolicy %} _Delete {% endif %}
 {% endblock controls %} {% block tabs %}
     * {% block tab_items %}
     * {{_object|meta:"verbose_name"|bettertitle_}}
     * {% endblock tab_items %} {% if perms.extras.view_objectchange %}
     * Change_Log
     * {% endif %}
 {% endblock tabs %} {% block content %}
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/prefixlistrule.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/prefixlistrule.html`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/routingpolicy.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/routingpolicy.html`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 {% load render_table from django_tables2 %}
 
 {% block breadcrumbs %}
 <li class="breadcrumb-item"><a href="{% url 'plugins:netbox_bgp:routingpolicy_list' %}">Routing Policies</a></li>
 {% endblock %}
 {% block controls %}
 <div class="pull-right noprint">
-    {% if perms.netbox_bgp.change_policy %}
+    {% if perms.netbox_bgp.change_routingpolicy %}
     <a href="{% url 'plugins:netbox_bgp:routingpolicyrule_add' %}?routing_policy={{ object.pk }}" class="btn btn-success">
         <span class="mdi mdi-plus-thick" aria-hidden="true"></span> Rule
     </a>
     {% endif %}
-    {% if perms.netbox_bgp.change_policy %}
+    {% if perms.netbox_bgp.change_routingpolicy %}
     <a href="{% url 'plugins:netbox_bgp:routingpolicy_edit' pk=object.pk %}" class="btn btn-warning">
         <span class="mdi mdi-pencil" aria-hidden="true"></span> Edit
     </a>
     {% endif %}
-    {% if perms.netbox_bgp.delete_policy %}
+    {% if perms.netbox_bgp.delete_routingpolicy %}
     <a href="{% url 'plugins:netbox_bgp:routingpolicy_delete' pk=object.pk %}" class="btn btn-danger">
         <span class="mdi mdi-trash-can-outline" aria-hidden="true"></span> Delete
     </a>
     {% endif %}
 </div>
 {% endblock controls %}
 {% block tabs %}
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {% extends 'generic/object.html' %} {% load buttons %} {% load custom_links %}
 {% load helpers %} {% load plugins %} {% load render_table from django_tables2
 %} {% block breadcrumbs %}
 Routing_Policies
 {% endblock %} {% block controls %}
-{% if perms.netbox_bgp.change_policy %} _Rule {% endif %} {% if
-perms.netbox_bgp.change_policy %} _Edit {% endif %} {% if
-perms.netbox_bgp.delete_policy %} _Delete {% endif %}
+{% if perms.netbox_bgp.change_routingpolicy %} _Rule {% endif %} {% if
+perms.netbox_bgp.change_routingpolicy %} _Edit {% endif %} {% if
+perms.netbox_bgp.delete_routingpolicy %} _Delete {% endif %}
 {% endblock controls %} {% block tabs %}
     * {% block tab_items %}
     * {{_object|meta:"verbose_name"|bettertitle_}}
     * {% endblock tab_items %} {% if perms.extras.view_objectchange %}
     * Change_Log
     * {% endif %}
 {% endblock tabs %} {% block content %}
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp/templates/netbox_bgp/routingpolicyrule.html` & `netbox-bgp-0.9.0/netbox_bgp/templates/netbox_bgp/routingpolicyrule.html`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/tests/test_api.py` & `netbox-bgp-0.9.0/netbox_bgp/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/tests/test_forms.py` & `netbox-bgp-0.9.0/netbox_bgp/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/tests/test_models.py` & `netbox-bgp-0.9.0/netbox_bgp/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/urls.py` & `netbox-bgp-0.9.0/netbox_bgp/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-bgp-0.8.1/netbox_bgp/views.py` & `netbox-bgp-0.9.0/netbox_bgp/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,20 @@
 
 
 class BGPSessionView(generic.ObjectView):
     queryset = BGPSession.objects.all()
     template_name = 'netbox_bgp/bgpsession.html'
 
     def get_extra_context(self, request, instance):
-        if instance.peer_group:
-            import_policies_qs = instance.import_policies.all() | instance.peer_group.import_policies.all()
-            export_policies_qs = instance.export_policies.all() | instance.peer_group.export_policies.all()
-        else:
-            import_policies_qs = instance.import_policies.all()
-            export_policies_qs = instance.export_policies.all()
+        import_policies_qs = instance.import_policies.all()
+        if not import_policies_qs and instance.peer_group:
+            import_policies_qs = instance.peer_group.import_policies.all()
+        export_policies_qs = instance.export_policies.all()
+        if not export_policies_qs and instance.peer_group:
+            export_policies_qs = instance.peer_group.export_policies.all()
 
         import_policies_table = tables.RoutingPolicyTable(
             import_policies_qs,
             orderable=False
         )
         export_policies_table = tables.RoutingPolicyTable(
             export_policies_qs,
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp.egg-info/PKG-INFO` & `netbox-bgp-0.9.0/netbox_bgp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-bgp
-Version: 0.8.1
+Version: 0.9.0
 Summary: BGP related stuff
 Home-page: https://github.com/k01ek/netbox-bgp
 Author: Nikolay Yuzefovich
 Author-email: mgk.kolek@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
@@ -28,14 +28,15 @@
 |-------------|-------|
 | NetBox 2.10 | 0.3.9 |
 | NetBox 2.11 | 0.3.9 |
 | NetBox 3.0  | 0.4.3 |
 | NetBox 3.1  | 0.5.0 |
 | NetBox 3.2  | >= 0.6.0 |
 | NetBox 3.3  | >= 0.8.1 |
+| NetBox 3.4  | >= 0.9.0 |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip  
 
 ```
 pip install netbox-bgp
```

### Comparing `netbox-bgp-0.8.1/netbox_bgp.egg-info/SOURCES.txt` & `netbox-bgp-0.9.0/netbox_bgp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 netbox_bgp/migrations/0020_netbox_bgp.py
 netbox_bgp/migrations/0021_netbox32_support.py
 netbox_bgp/migrations/0022_netbox_bgp.py
 netbox_bgp/migrations/0023_netbox_bgp.py
 netbox_bgp/migrations/0024_netbox_bgp.py
 netbox_bgp/migrations/0025_netbox_bgp.py
 netbox_bgp/migrations/0026_netbox_bgp.py
+netbox_bgp/migrations/0027_netbox_bgp.py
 netbox_bgp/migrations/__init__.py
 netbox_bgp/templates/netbox_bgp/bgppeergroup.html
 netbox_bgp/templates/netbox_bgp/bgpsession.html
 netbox_bgp/templates/netbox_bgp/community.html
 netbox_bgp/templates/netbox_bgp/device_extend.html
 netbox_bgp/templates/netbox_bgp/prefixlist.html
 netbox_bgp/templates/netbox_bgp/prefixlistrule.html
```

### Comparing `netbox-bgp-0.8.1/setup.py` & `netbox-bgp-0.9.0/setup.py`

 * *Files identical despite different names*

