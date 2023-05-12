# Comparing `tmp/drb-topic-sentinel3-1.1.0.tar.gz` & `tmp/drb-topic-sentinel3-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel3-1.1.0.tar", last modified: Tue Jan  3 13:33:55 2023, max compression
+gzip compressed data, was "drb-topic-sentinel3-1.1.1.tar", last modified: Fri May 12 13:19:54 2023, max compression
```

## Comparing `drb-topic-sentinel3-1.1.0.tar` & `drb-topic-sentinel3-1.1.1.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13663 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13182 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.945198 drb-topic-sentinel3-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.945198 drb-topic-sentinel3-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.965198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Auxiliary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Auxiliary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Auxiliary/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/GNSS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/GNSS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/GNSS/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/GNSS/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/GNSS/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.953198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      716 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level0/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.957198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level1/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level1/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/level0/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/level0/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/level0/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-03 13:33:55.965198 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:33:55.961198 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13663 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2405 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-01-03 13:33:55.000000 drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-03 13:33:55.965198 drb-topic-sentinel3-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:34:08.000000 drb-topic-sentinel3-1.1.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13711 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13182 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.151354 drb-topic-sentinel3-1.1.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.151354 drb-topic-sentinel3-1.1.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.155354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Auxiliary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Auxiliary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Auxiliary/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/GNSS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/GNSS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/GNSS/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/GNSS/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/GNSS/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.159354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.163354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.163354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.163354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.167354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.167354 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.171355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.171355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.171355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.175355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.175355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.175355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level0/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.179355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.179355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.179355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.183355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level1/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level1/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.183355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.183355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.183355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/level0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/level0/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/level0/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13711 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 13:19:54.000000 drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-05-12 12:30:30.000000 drb-topic-sentinel3-1.1.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-05-12 13:19:54.187355 drb-topic-sentinel3-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3852 2023-05-12 13:19:30.000000 drb-topic-sentinel3-1.1.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-01-03 10:46:42.000000 drb-topic-sentinel3-1.1.1/versioneer.py
```

### Comparing `drb-topic-sentinel3-1.1.0/PKG-INFO` & `drb-topic-sentinel3-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel3
-Version: 1.1.0
+Version: 1.1.1
 Summary: Sentinel-3 topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/sentinel-3
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel3
 The `drb-topic-sentinel3` is a DRB plugin declaring topics about
 [Sentinel-3](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-3)
 EO satellite.
 
 ## Installation
```

### Comparing `drb-topic-sentinel3-1.1.0/README.md` & `drb-topic-sentinel3-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Auxiliary/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Auxiliary/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/DORIS/level0/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/DORIS/level0/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/MRW/level1/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/MRW/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level0/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level0/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level1/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/OLCI/level2/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/OLCI/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SLSTR/level2/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SLSTR/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level0/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level0/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level1/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SRAL/level2/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SRAL/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level1/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level1/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/SYN/level2/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/SYN/level2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/Telemetry/level0/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/Telemetry/level0/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb/topics/sentinel3/cortex.yml` & `drb-topic-sentinel3-1.1.1/drb/topics/sentinel3/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/PKG-INFO` & `drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel3
-Version: 1.1.0
+Version: 1.1.1
 Summary: Sentinel-3 topic for DRB Python
 Home-page: https://gitlab.com/drb-python/topics/sentinel-3
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # drb-topic-sentinel3
 The `drb-topic-sentinel3` is a DRB plugin declaring topics about
 [Sentinel-3](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-3)
 EO satellite.
 
 ## Installation
```

### Comparing `drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/SOURCES.txt` & `drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENCE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 drb/topics/sentinel3/__init__.py
```

### Comparing `drb-topic-sentinel3-1.1.0/drb_topic_sentinel3.egg-info/entry_points.txt` & `drb-topic-sentinel3-1.1.1/drb_topic_sentinel3.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel3-1.1.0/setup.py` & `drb-topic-sentinel3-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     author_email='drb-python@gael.fr',
     url='https://gitlab.com/drb-python/topics/sentinel-3',
     python_requires='>=3.8',
     install_requires=REQUIREMENTS,
     packages=find_namespace_packages(include=['drb.*']),
     classifiers=[
         "Programming Language :: Python :: 3.8",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: "
+        "GNU Lesser General Public License v3 (LGPLv3)",
         "Programming Language :: Python :: 3.8",
     ],
     package_data={
         'drb.topics.sentinel3': ['cortex.yml'],
 
         'drb.topics.sentinel3.OLCI': ['cortex.yml'],
         'drb.topics.sentinel3.OLCI.level0': ['cortex.yml'],
```

### Comparing `drb-topic-sentinel3-1.1.0/versioneer.py` & `drb-topic-sentinel3-1.1.1/versioneer.py`

 * *Files identical despite different names*

