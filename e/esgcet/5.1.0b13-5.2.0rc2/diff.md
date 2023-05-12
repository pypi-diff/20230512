# Comparing `tmp/esgcet-5.1.0b13.tar.gz` & `tmp/esgcet-5.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esgcet-5.1.0b13.tar", last modified: Thu Feb 16 00:31:46 2023, max compression
+gzip compressed data, was "/Users/ames4/tmpgit/esg-publisher/pkg/dist/.tmp-w67g62ms/esgcet-5.2.0rc2.tar", last modified: Fri May 12 20:42:53 2023, max compression
```

## Comparing `esgcet-5.1.0b13.tar` & `esgcet-5.2.0rc2.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-02-16 00:31:46.547199 esgcet-5.1.0b13/
--rw-r--r--   0 ames4    (36337)    36337      242 2023-02-16 00:31:46.546844 esgcet-5.1.0b13/PKG-INFO
--rw-r--r--   0 ames4    (36337)    36337     2438 2022-06-23 14:22:51.000000 esgcet-5.1.0b13/esg.ini
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-02-16 00:31:46.542489 esgcet-5.1.0b13/esgcet/
--rw-r--r--   0 ames4    (36337)    36337       25 2023-02-15 23:23:46.000000 esgcet-5.1.0b13/esgcet/__init__.py
--rw-r--r--   0 ames4    (36337)    36337     2640 2022-03-08 15:37:48.000000 esgcet-5.1.0b13/esgcet/activity_check.py
--rw-r--r--   0 ames4    (36337)    36337    12202 2023-01-06 00:49:50.000000 esgcet-5.1.0b13/esgcet/args.py
--rw-r--r--   0 ames4    (36337)    36337     2499 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/cmip5.py
--rw-r--r--   0 ames4    (36337)    36337     3573 2023-01-06 00:49:50.000000 esgcet-5.1.0b13/esgcet/cmip6.py
--rw-r--r--   0 ames4    (36337)    36337     3694 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/create_ip.py
--rw-r--r--   0 ames4    (36337)    36337      192 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/e3sm.py
--rw-r--r--   0 ames4    (36337)    36337     4511 2022-06-23 14:22:51.000000 esgcet-5.1.0b13/esgcet/esgindexpub.py
--rw-r--r--   0 ames4    (36337)    36337     2396 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/esgmapconv.py
--rw-r--r--   0 ames4    (36337)    36337     4968 2021-10-15 14:10:50.000000 esgcet-5.1.0b13/esgcet/esgmigrate.py
--rw-r--r--   0 ames4    (36337)    36337     7528 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/esgmkpubrec.py
--rw-r--r--   0 ames4    (36337)    36337     4016 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/esgpidcitepub.py
--rw-r--r--   0 ames4    (36337)    36337     6542 2022-05-09 22:14:17.000000 esgcet-5.1.0b13/esgcet/esgunpublish.py
--rw-r--r--   0 ames4    (36337)    36337     3750 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/esgupdate.py
--rw-r--r--   0 ames4    (36337)    36337     2576 2023-02-08 17:21:15.000000 esgcet-5.1.0b13/esgcet/generic_netcdf.py
--rw-r--r--   0 ames4    (36337)    36337     3625 2022-06-23 14:22:51.000000 esgcet-5.1.0b13/esgcet/generic_pub.py
--rw-r--r--   0 ames4    (36337)    36337     2808 2022-06-23 14:22:51.000000 esgcet-5.1.0b13/esgcet/index_pub.py
--rw-r--r--   0 ames4    (36337)    36337     1566 2022-06-23 14:22:51.000000 esgcet-5.1.0b13/esgcet/input4mips.py
--rw-r--r--   0 ames4    (36337)    36337     2756 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/list2json.py
--rw-r--r--   0 ames4    (36337)    36337      613 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/logger.py
--rw-r--r--   0 ames4    (36337)    36337     2156 2021-11-09 22:54:24.000000 esgcet-5.1.0b13/esgcet/mapfile.py
--rw-r--r--   0 ames4    (36337)    36337     1467 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/migratecmd.py
--rw-r--r--   0 ames4    (36337)    36337    19301 2023-02-09 22:35:15.000000 esgcet-5.1.0b13/esgcet/mk_dataset.py
--rw-r--r--   0 ames4    (36337)    36337     2013 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/mkd_cmip5.py
--rw-r--r--   0 ames4    (36337)    36337     4962 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/mkd_create_ip.py
--rw-r--r--   0 ames4    (36337)    36337     1572 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/mkd_input4mips.py
--rw-r--r--   0 ames4    (36337)    36337     3251 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/mkd_non_nc.py
--rw-r--r--   0 ames4    (36337)    36337     8857 2023-02-14 23:44:46.000000 esgcet-5.1.0b13/esgcet/pid_cite_pub.py
--rw-r--r--   0 ames4    (36337)    36337     3960 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/pub_client.py
--rw-r--r--   0 ames4    (36337)    36337     3553 2023-01-06 00:49:50.000000 esgcet-5.1.0b13/esgcet/pub_internal.py
--rw-r--r--   0 ames4    (36337)    36337      463 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/pub_test.py
--rw-r--r--   0 ames4    (36337)    36337     4479 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/publish_script.py
--rw-r--r--   0 ames4    (36337)    36337     2266 2022-03-14 16:31:36.000000 esgcet-5.1.0b13/esgcet/search_check.py
--rw-r--r--   0 ames4    (36337)    36337     4617 2022-05-09 22:14:17.000000 esgcet-5.1.0b13/esgcet/settings.py
--rw-r--r--   0 ames4    (36337)    36337     2304 2022-05-09 22:14:17.000000 esgcet-5.1.0b13/esgcet/unpublish.py
--rw-r--r--   0 ames4    (36337)    36337     4023 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/esgcet/update.py
-drwxr-xr-x   0 ames4    (36337)    36337        0 2023-02-16 00:31:46.546217 esgcet-5.1.0b13/esgcet.egg-info/
--rw-r--r--   0 ames4    (36337)    36337      242 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/PKG-INFO
--rw-r--r--   0 ames4    (36337)    36337      971 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/SOURCES.txt
--rw-r--r--   0 ames4    (36337)    36337        1 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/dependency_links.txt
--rw-r--r--   0 ames4    (36337)    36337      321 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/entry_points.txt
--rw-r--r--   0 ames4    (36337)    36337        1 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/not-zip-safe
--rw-r--r--   0 ames4    (36337)    36337       42 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/requires.txt
--rw-r--r--   0 ames4    (36337)    36337        7 2023-02-16 00:31:46.000000 esgcet-5.1.0b13/esgcet.egg-info/top_level.txt
--rw-r--r--   0 ames4    (36337)    36337       38 2023-02-16 00:31:46.547328 esgcet-5.1.0b13/setup.cfg
--rwxr-xr-x   0 ames4    (36337)    36337     3702 2021-10-15 14:07:06.000000 esgcet-5.1.0b13/setup.py
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.226019 esgcet-5.2.0rc2/
+-rw-r--r--   0 ames4    (36337)    36337      169 2023-05-12 20:42:53.225594 esgcet-5.2.0rc2/PKG-INFO
+-rw-r--r--   0 ames4    (36337)    36337     2438 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esg.ini
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.219987 esgcet-5.2.0rc2/esgcet/
+-rw-r--r--   0 ames4    (36337)    36337       25 2023-04-11 17:57:32.000000 esgcet-5.2.0rc2/esgcet/__init__.py
+-rw-r--r--   0 ames4    (36337)    36337     2640 2022-03-08 15:37:48.000000 esgcet-5.2.0rc2/esgcet/activity_check.py
+-rw-r--r--   0 ames4    (36337)    36337    12383 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/args.py
+-rw-r--r--   0 ames4    (36337)    36337     2499 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/cmip5.py
+-rw-r--r--   0 ames4    (36337)    36337     3736 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/cmip6.py
+-rw-r--r--   0 ames4    (36337)    36337     3694 2023-04-19 15:55:00.000000 esgcet-5.2.0rc2/esgcet/create_ip.py
+-rw-r--r--   0 ames4    (36337)    36337      192 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/e3sm.py
+-rw-r--r--   0 ames4    (36337)    36337     4614 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgindexpub.py
+-rw-r--r--   0 ames4    (36337)    36337     2309 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgmapconv.py
+-rw-r--r--   0 ames4    (36337)    36337     5809 2023-04-14 23:57:26.000000 esgcet-5.2.0rc2/esgcet/esgmigrate.py
+-rw-r--r--   0 ames4    (36337)    36337     7348 2023-04-26 23:13:35.000000 esgcet-5.2.0rc2/esgcet/esgmkpubrec.py
+-rw-r--r--   0 ames4    (36337)    36337     3850 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgpidcitepub.py
+-rw-r--r--   0 ames4    (36337)    36337     6400 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgunpublish.py
+-rw-r--r--   0 ames4    (36337)    36337     3639 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/esgupdate.py
+-rw-r--r--   0 ames4    (36337)    36337     3440 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/generic_netcdf.py
+-rw-r--r--   0 ames4    (36337)    36337     3625 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esgcet/generic_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     1102 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/handler_base.py
+-rw-r--r--   0 ames4    (36337)    36337     2808 2022-06-23 14:22:51.000000 esgcet-5.2.0rc2/esgcet/index_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     1598 2023-05-12 20:41:14.000000 esgcet-5.2.0rc2/esgcet/input4mips.py
+-rw-r--r--   0 ames4    (36337)    36337     2756 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/list2json.py
+-rw-r--r--   0 ames4    (36337)    36337      613 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/logger.py
+-rw-r--r--   0 ames4    (36337)    36337     2200 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/mapfile.py
+-rw-r--r--   0 ames4    (36337)    36337     1676 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/migratecmd.py
+-rw-r--r--   0 ames4    (36337)    36337    16351 2023-04-24 16:37:31.000000 esgcet-5.2.0rc2/esgcet/mk_dataset.py
+-rw-r--r--   0 ames4    (36337)    36337     4594 2023-04-24 16:37:57.000000 esgcet-5.2.0rc2/esgcet/mk_dataset_autoc.py
+-rw-r--r--   0 ames4    (36337)    36337     2349 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mk_dataset_xarray.py
+-rw-r--r--   0 ames4    (36337)    36337     1474 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_cmip5.py
+-rw-r--r--   0 ames4    (36337)    36337     4768 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_create_ip.py
+-rw-r--r--   0 ames4    (36337)    36337     1572 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/mkd_input4mips.py
+-rw-r--r--   0 ames4    (36337)    36337     2989 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/esgcet/mkd_non_nc.py
+-rw-r--r--   0 ames4    (36337)    36337     8947 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/pid_cite_pub.py
+-rw-r--r--   0 ames4    (36337)    36337     3960 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/pub_client.py
+-rw-r--r--   0 ames4    (36337)    36337     3553 2023-01-06 00:49:50.000000 esgcet-5.2.0rc2/esgcet/pub_internal.py
+-rw-r--r--   0 ames4    (36337)    36337      463 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/pub_test.py
+-rw-r--r--   0 ames4    (36337)    36337     4479 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/publish_script.py
+-rw-r--r--   0 ames4    (36337)    36337     2266 2022-03-14 16:31:36.000000 esgcet-5.2.0rc2/esgcet/search_check.py
+-rw-r--r--   0 ames4    (36337)    36337     4736 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/settings.py
+-rw-r--r--   0 ames4    (36337)    36337     2414 2023-04-11 17:56:54.000000 esgcet-5.2.0rc2/esgcet/unpublish.py
+-rw-r--r--   0 ames4    (36337)    36337     4023 2021-10-15 14:07:06.000000 esgcet-5.2.0rc2/esgcet/update.py
+drwxr-xr-x   0 ames4    (36337)    36337        0 2023-05-12 20:42:53.224982 esgcet-5.2.0rc2/esgcet.egg-info/
+-rw-r--r--   0 ames4    (36337)    36337      169 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/PKG-INFO
+-rw-r--r--   0 ames4    (36337)    36337     1049 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/SOURCES.txt
+-rw-r--r--   0 ames4    (36337)    36337        1 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/dependency_links.txt
+-rw-r--r--   0 ames4    (36337)    36337      320 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/entry_points.txt
+-rw-r--r--   0 ames4    (36337)    36337        1 2023-02-16 00:31:46.000000 esgcet-5.2.0rc2/esgcet.egg-info/not-zip-safe
+-rw-r--r--   0 ames4    (36337)    36337       69 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/requires.txt
+-rw-r--r--   0 ames4    (36337)    36337        7 2023-05-12 20:42:53.000000 esgcet-5.2.0rc2/esgcet.egg-info/top_level.txt
+-rw-r--r--   0 ames4    (36337)    36337       38 2023-05-12 20:42:53.226142 esgcet-5.2.0rc2/setup.cfg
+-rwxr-xr-x   0 ames4    (36337)    36337     3091 2023-04-24 16:37:22.000000 esgcet-5.2.0rc2/setup.py
```

### Comparing `esgcet-5.1.0b13/esg.ini` & `esgcet-5.2.0rc2/esg.ini`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/activity_check.py` & `esgcet-5.2.0rc2/esgcet/activity_check.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/args.py` & `esgcet-5.2.0rc2/esgcet/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 from pathlib import Path
 import os, sys, json
 import esgcet.esgmigrate as em
-import configparser as cfg
 from esgcet.settings import *
 import esgcet.logger as logger
+import yaml
+
+import esgcet
 
 import esgcet
 
 log = logger.Logger()
 publog = log.return_logger('Settings')
 
 DEFAULT_ESGINI = '/esg/config/esgcet'
@@ -20,163 +22,167 @@
         pass
 
     def get_args(self):
         parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
         # ANY FILE NAME INPUT: check first to make sure it exists
         home = str(Path.home())
-        def_config = home + "/.esg/esg.ini"
+        def_config = home + "/.esg/esg.yaml"
         parser.add_argument("--test", dest="test", action="store_true", help="PID registration will run in 'test' mode. Use this mode unless you are performing 'production' publications.")
         # replica stuff new... hard-coded, modify mk dataset so that it imports it instead
         parser.add_argument("--set-replica", dest="set_replica", action="store_true", help="Enable replica publication.")
         parser.add_argument("--no-replica", dest="no_replica", action="store_true", help="Disable replica publication.")
         parser.add_argument("--esgmigrate", dest="migrate", action="store_true", help="Run esgmigrate before publishing, to migrate over old config. May be left with incomplete config settings.")
         parser.add_argument("--json", dest="json", default=None, help="Load attributes from a JSON file in .json form. The attributes will override any found in the DRS structure or global attributes.")
         parser.add_argument("--data-node", dest="data_node", default=None, help="Specify data node.")
         parser.add_argument("--index-node", dest="index_node", default=None, help="Specify index node.")
         parser.add_argument("--certificate", "-c", dest="cert", default="./cert.pem", help="Use the following certificate file in .pem form for publishing (use a myproxy login to generate).")
         parser.add_argument("--project", dest="proj", default="", help="Set/overide the project for the given mapfile, for use with selecting the DRS or specific features, e.g. PrePARE, PID.")
         parser.add_argument("--cmor-tables", dest="cmor_path", default=None, help="Path to CMIP6 CMOR tables for PrePARE. Required for CMIP6 only.")
         parser.add_argument("--autocurator", dest="autocurator_path", default=None, help="Path to autocurator repository folder.")
         parser.add_argument("--map", dest="map", required=True, nargs="+", help="Mapfile or list of mapfiles.")
-        parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
+        parser.add_argument("--config", "-cfg", dest="cfg", default=def_config, help="Path to yaml config file.")
         parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
         parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
         parser.add_argument("--no-auth", dest="no_auth", action="store_true", help="Run publisher without certificate, only works on certain index nodes.")
         parser.add_argument("--verify", dest="verify", action="store_true", help="Toggle verification for publishing, default is off.")
         parser.add_argument("--version", action="version", version=f"esgpublish v{esgcet.__version__}",help="Print the version and exit")
-        
+        parser.add_argument("--xarray", dest="xarray", action="store_true", help="Use Xarray to extract metadata even if Autocurator is configured.") 
+
         pub = parser.parse_args()
 
         return pub
 
+    def load_config(self, config_path):
+        config_file = None
+        try:
+            config_file = open(config_path, 'r')  # or "a+", whatever you need
+        except IOError:
+            publog.error("Could not open file, please provide correct path to yaml config file.")
+            quit(1)
+
+        with config_file as fd:
+            conf = yaml.load(fd, Loader=yaml.SafeLoader)
+        return conf
+
     def get_dict(self, fullmap, fn_project):
 
         pub = self.get_args()
         json_file = pub.json
 
         if pub.migrate:
             em.run(DEFAULT_ESGINI, False, False)
 
-        ini_file = pub.cfg
-        config = cfg.ConfigParser()
-        if not os.path.exists(ini_file):
-            publog.error("Config file not found. " + ini_file + " does not exist.")
+        config_file = pub.cfg
+        config = self.load_config(config_file)
+        if not os.path.exists(config_file):
+            publog.error("Config file not found. " + config_file + " does not exist.")
             exit(1)
-        if os.path.isdir(ini_file):
+        if os.path.isdir(config_file):
             publog.error("Config file path is a directory. Please use a complete file path, exiting.")
             exit(1)
-        try:
-            config.read(ini_file)
-        except Exception as ex:
-            publog.exception("reading config file")
-            exit(1)
 
         if pub.proj != "":
             project = pub.proj
         else:
             try:
-                project = config['user']['project']
+                project = config['project']
                 if "none" in project:
                     project = fn_project
             except:
                 project = fn_project
 
         if not pub.silent:
             try:
-                s = config['user']['silent']
+                s = config['silent']
                 if 'true' in s or 'yes' in s:
                     silent = True
                 else:
                     silent = False
             except:
                 silent = False
         else:
             silent = True
 
         if not pub.verbose:
             if not pub.silent:
                 try:
-                    v = config['user']['verbose']
+                    v = config['verbose']
                     if 'true' in v or 'yes' in v:
                         verbose = True
                     else:
                         verbose = False
                 except:
                     verbose = False
         else:
             verbose = True
             silent = False
 
         if pub.cert == "./cert.pem":
             try:
-                cert = config['user']['cert']
+                cert = config['cert']
             except:
                 cert = pub.cert
         else:
             cert = pub.cert
 
-        conda_auto = False
-        if pub.autocurator_path is None:
-            try:
-                autocurator = config['user']['autoc_path']
-                if autocurator == "autocurator" or autocurator == "none":
-                    autocurator = "autocurator"
-                    conda_auto = True
-            except:
-                autocurator = "autocurator"
-                conda_auto = True
+        if pub.xarray:
+            autocurator = None
+        elif pub.autocurator_path is None:
+            autocurator = config.get('autoc_path', None)
+            if autocurator == "none":
+                autocurator = None
         else:
             autocurator = pub.autocurator_path
 
         if pub.index_node is None:
             try:
-                index_node = config['user']['index_node']
+                index_node = config['index_node']
             except:
                 publog.exception("Index node not defined. Use the --index-node option or define in esg.ini.")
                 exit(1)
         else:
             index_node = pub.index_node
 
         if pub.data_node is None:
             try:
-                data_node = config['user']['data_node']
+                data_node = config['data_node']
             except:
                 publog.exception("Data node not defined. Use --data-node option or define in esg.ini.")
                 exit(1)
         else:
             data_node = pub.data_node
         try:
-            data_roots = json.loads(config['user']['data_roots'])
+            data_roots = config['data_roots']
             if data_roots == 'none':
-                publog.error("Data roots undefined. Define in esg.ini to create file metadata.")
+                publog.error("Data roots undefined. Define in config file to create file metadata.")
                 exit(1)
         except:
-            publog.exception("Data roots undefined. Define in esg.ini to create file metadata.")
+            publog.exception("Data roots undefined. Define in config file to create file metadata.")
             exit(1)
 
         try:
-            globus = config['user']['globus_uuid']
+            globus = config['globus_uuid']
         except:
             globus = "none"
 
         try:
-            dtn = config['user']['data_transfer_node']
+            dtn = config['data_transfer_node']
         except:
             dtn = "none"
 
         skip_prepare = False
         try:
-            skip_prep_str = config['user']['skip_prepare'].lower()
+            skip_prep_str = config['skip_prepare'].lower()
             skip_prepare = (skip_prep_str in ["true", "yes"])
         except:
             pass
         force_prepare = False
         try:
-            force_prep_str = config['user']['force_prepare'].lower()
+            force_prep_str = config['force_prepare'].lower()
             force_prepare = (force_prep_str in ["true", "yes"])
         except:
             pass
         if skip_prepare and force_prepare:
             publog.error("PrePARE simultaneously skipped and forced.")
             exit(1)
 
@@ -185,15 +191,15 @@
             exit(1)
         elif pub.set_replica:
             replica = True
         elif pub.no_replica:
             replica = False
         else:
             try:
-                r = config['user']['set_replica'].lower()
+                r = config['set_replica'].lower()
                 if 'yes' in r or 'true' in r:
                     replica = True
                 elif 'no' in r or 'false' in r:
                     replica = False
                 else:
                     publog.error("Config file error: set_replica must be true, false, yes, or no.")
                     exit(1)
@@ -201,21 +207,16 @@
                 publog.exception("Set_replica not defined. Use --set-replica or --no-replica or define in esg.ini.")
                 exit(1)
 
         test = False
         if pub.test:
             test = True
 
-        if not conda_auto:
-            autoc_command = autocurator + "/bin/autocurator"  # concatenate autocurator command
-        else:
-            autoc_command = autocurator
-        
         try:
-            proj_config = json.loads(config['user']['user_project_config'])
+            proj_config = config['user_project_config']
         except:
             publog.warning("User project config missing or could not be parsed.")
             proj_config = {}
 
         os.system("cert_path=" + cert)
 
         if pub.verify:
@@ -225,74 +226,81 @@
 
         if pub.no_auth:
             auth = False
         else:
             auth = True
 
         try:
-            non_netcdf = config['user']['non_netcdf'].lower()
+            non_netcdf = config['non_netcdf'].lower()
             if 'yes' in non_netcdf or 'true' in non_netcdf:
                 non_nc = True
             else:
                 non_nc = False
         except:
             non_nc = False
 
         try:
-            mountpoints = json.loads(config['user']['mountpoint_map'])
+            mountpoints = config['mountpoint_map']
             if mountpoints == "none":
                 mountpoints = None
         except:
             mountpoints = None
 
         if globus == "none" and not silent:
             publog.info("No Globus UUID defined.")
 
         if dtn == "none" and not silent:
             publog.info("No data transfer node defined.")
 
         argdict = {"fullmap": fullmap, "silent": silent, "verbose": verbose,
                    "cert": cert,
-                   "autoc_command": autoc_command, "index_node": index_node, "data_node": data_node,
+                   "autoc_command": autocurator, "index_node": index_node, "data_node": data_node,
                    "data_roots": data_roots, "globus": globus, "dtn": dtn, "replica": replica,
                    "json_file": json_file, "test": test, "user_project_config": proj_config, "verify": verify,
                    "auth": auth, "skip_prepare": skip_prepare, "force_prepare": force_prepare,
                    "non_nc": non_nc, "mountpoints": mountpoints}
 
         if project and "none" not in project:
             argdict["proj"] = project
 
         project = project.lower()
         if project == "cmip6":
             if pub.cmor_path is None:
                 try:
-                    argdict["cmor_tables"] = config['user']['cmor_path']
+                    argdict["cmor_tables"] = config['cmor_path']
                 except:
                     publog.exception("No path for CMOR tables defined. Use --cmor-tables option or define in config file.")
                     exit(1)
             else:
                 argdict["cmor_tables"] = pub.cmor_path
         if project == "cmip6" or project == "input4mips" or (project in proj_config and "pid_prefix" in proj_config[project]):  
             try:
-                argdict["pid_creds"] = json.loads(config['user']['pid_creds'])
+                # Unpack the PID credentials format from the yaml to be compatible with the legacy format
+                pid_creds = config['pid_creds']
+                creds_lst = []
+                for it in pid_creds:
+                    rec = pid_creds[it]
+                    rec['url'] = it
+                    creds_lst.append(rec)
+                argdict['pid_creds'] = creds_lst
             except:
                 publog.exception("PID credentials not defined. Define in config file esg.ini.")
                 exit(1)
-        if "cmip6_clone" in config['user'] and project == config['user']['cmip6_clone'].lower():
+        if "cmip6_clone" in config and project == config['cmip6_clone'].lower():
             if "pid_creds" in argdict:
                 argdict["cmip6-clone"] = project
             if not argdict["user_project_config"]:
                 argdict["user_project_config"] = {}
             argdict["user_project_config"]["clone_project"] = "cmip6"
-        if "enable_archive" in config['user'] and config['user'].get("enable_archive", False):
+        if "enable_archive" in config and config.get("enable_archive", False):
             try:
                 argdict["enable_archive"] = True
 
-                argdict["archive_path"] = config["user"]["archive_location"]
-                argdict["archive_path_length"] = config["user"]["archive_depth"]
+                argdict["archive_path"] = config["archive_location"]
+                argdict["archive_path_length"] = config["archive_depth"]
                 if not os.path.isdir(argdict["archive_path"]):
                     publog.exception(f"Error with archive path {argdict['archive_path']}")
                     exit(1)
             except:
                 publog.exception("Configuration file error: check archive (and other) settings")
                 exit(1)
         else:
```

### Comparing `esgcet-5.1.0b13/esgcet/cmip5.py` & `esgcet-5.2.0rc2/esgcet/cmip5.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/cmip6.py` & `esgcet-5.2.0rc2/esgcet/cmip6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from esgcet.pid_cite_pub import ESGPubPidCite
 from esgcet.activity_check import FieldCheck
 import tempfile
 import json
-from cmip6_cv import PrePARE
+
 from esgcet.generic_pub import BasePublisher
 from esgcet.generic_netcdf import GenericPublisher
 import sys, os
 import esgcet.logger as logger
 
 log = logger.Logger()
 
@@ -28,14 +28,15 @@
         if self.replica:
             self.skip_prepare = not argdict["force_prepare"]
         else:
             self.skip_prepare = argdict["skip_prepare"]
         self.publog = log.return_logger('CMIP6', self.silent, self.verbose)
 
     def prepare_internal(self, json_map, cmor_tables):
+        from cmip6_cv import PrePARE
         try:
             assert(len(cmor_tables) > 0, f"{cmor_tables} are specified from config")
             assert(os.path.isdir(cmor_tables), f"{cmor_tables} exists and is a directory")
             self.publog.info("Iterating through filenames for PrePARE (internal version)...")
             validator = PrePARE.PrePARE
             for info in json_map:
                 filename = info[1]
@@ -76,22 +77,24 @@
         map_json_data = self.mapfile()
 
         # step two: PrePARE
         if not self.skip_prepare:
             self.prepare_internal(map_json_data, self.cmor_tables)
 
         # step three: autocurator
-        self.publog.info("Running autocurator...")
-        self.autocurator(map_json_data)
+#        self.publog.info("Running autocurator...")
+#        self.autocurator(map_json_data)
+        # step two: autocurator
+        self.publog.info(f"Running Extraction... {str(self.extract_method)}")
+        self.extract_method(map_json_data)
 
         # step four: make dataset
         self.publog.info("Making dataset...")
         out_json_data = self.mk_dataset(map_json_data)
 
-
         # step five: assign PID
         self.publog.info("Assigning PID...")
         new_json_data = self.pid(out_json_data)
 
         # step six: update record if exists
         self.publog.info("Updating...")
         self.update(new_json_data)
```

### Comparing `esgcet-5.1.0b13/esgcet/create_ip.py` & `esgcet-5.2.0rc2/esgcet/create_ip.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/esgindexpub.py` & `esgcet-5.2.0rc2/esgcet/esgindexpub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import sys, json, os
 from esgcet.index_pub import ESGPubIndex
 import argparse
-import configparser as cfg
 from pathlib import Path
 import esgcet.logger as logger
+import esgcet.args as pub_args
 
 log = logger.Logger()
 publog = log.return_logger('esgindexpub')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     home = str(Path.home())
-    def_config = home + "/.esg/esg.ini"
+    def_config = home + "/.esg/esg.yaml"
     parser.add_argument("--index-node", dest="index_node", default=None, help="Specify index node.")
     parser.add_argument("--certificate", "-c", dest="cert", default="./cert.pem",
                         help="Use the following certificate file in .pem form for publishing (use a myproxy login to generate).")
     parser.add_argument("--pub-rec", dest="json_data", default=None,
                         help="JSON file output from esgpidcitepub or esgmkpubrec.")
-    parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
+    parser.add_argument("--config", "-cfg", dest="cfg", default=def_config, help="Path to yaml config file.")
     parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
     parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
     parser.add_argument("--no-auth", dest="no_auth", action="store_true",
                         help="Run publisher without certificate, only works on certain index nodes.")
     parser.add_argument("--verify", dest="verify", action="store_true",
                         help="Toggle server certificate verification for publishing, default is off.")
     parser.add_argument("--xml-list", dest="xml_list", default=None,
@@ -39,60 +39,60 @@
     ini_file = a.cfg
     if not os.path.exists(ini_file):
         publog.error("Config file not found. " + ini_file + " does not exist.")
         exit(1)
     if os.path.isdir(ini_file):
         publog.error("Config file path is a directory. Please use a complete file path.")
         exit(1)
-    config = cfg.ConfigParser()
-    try:
-        config.read(ini_file)
-    except Exception as ex:
-        publog.exception("config file")
+    args = pub_args.PublisherArgs()
+    config = args.load_config(ini_file)
+
+    if not (a.json_data or a.xml_list):
+        publog.error("Input data argument missing.  Please provide either records in .json form or a list of xml files for index publishing")
         exit(1)
 
     if not (a.json_data or a.xml_list):
         publog.error("Input data argument missing.  Please provide either records in .json form or a list of xml files for index publishing")
         exit(1)
 
     if not a.silent:
         try:
-            s = config['user']['silent']
+            s = config['silent']
             if 'true' in s or 'yes' in s:
                 silent = True
             else:
                 silent = False
         except:
             silent = False
     else:
         silent = True
 
     if not a.verbose:
         try:
-            v = config['user']['verbose']
+            v = config['verbose']
             if 'true' in v or 'yes' in v:
                 verbose = True
             else:
                 verbose = False
         except:
             verbose = False
     else:
         verbose = True
 
     if a.cert == "./cert.pem":
         try:
-            cert = config['user']['cert']
+            cert = config['cert']
         except:
             cert = a.cert
     else:
         cert = a.cert
 
     if a.index_node is None:
         try:
-            index_node = config['user']['index_node']
+            index_node = config['index_node']
         except:
             publog.exception("Index node not defined. Use the --index-node option or define in esg.ini.")
             exit(1)
     else:
         index_node = a.index_node
 
     if a.verify:
```

### Comparing `esgcet-5.1.0b13/esgcet/esgmapconv.py` & `esgcet-5.2.0rc2/esgcet/esgmapconv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,58 @@
 import sys
 from esgcet.mapfile import ESGPubMapConv
 import json
 import os
-import configparser as cfg
 import argparse
 from pathlib import Path
 import esgcet.logger as logger
+import esgcet.args as pub_args
 
 log = logger.Logger()
 publog = log.return_logger('esgmapconv')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     home = str(Path.home())
-    def_config = home + "/.esg/esg.ini"
+    def_config = home + "/.esg/esg.yaml"
     parser.add_argument("--project", dest="proj", default="", help="Set/overide the project for the given mapfile, for use with selecting the DRS or specific features, e.g. PrePARE, PID.")
     parser.add_argument("--map", dest="map", required=True, help="Mapfile ending in .map extension, contains metadata about the record.")
     parser.add_argument("--out-file", dest="out_file", help="Output file for map data in JSON format. Default is printed to standard out.")
-    parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
+    parser.add_argument("--config", "-cfg", dest="cfg", default=def_config, help="Path to yaml config file.")
 
     pub = parser.parse_args()
 
     return pub
 
 
 def run():
     a = get_args()
     ini_file = a.cfg
-    config = cfg.ConfigParser()
     if not os.path.exists(ini_file):
         publog.error("Config file not found. " + ini_file + " does not exist.")
         exit(1)
     if os.path.isdir(ini_file):
         publog.error("Config file path is a directory. Please use a complete file path.")
         exit(1)
-    try:
-        config.read(ini_file)
-    except Exception as ex:
-        publog.exception("Could not read config file")
-        exit(1)
 
+    args = pub_args.PublisherArgs()
+    config = args.load_config(ini_file)
     p = True
     if a.out_file is not None:
         p = False
         outfile = a.out_file
 
     proj = None
     if a.proj != "":
         proj = a.proj
     else:
         try:
-            proj = config['user']['project']
+            proj = config['project']
         except:
             pass
 
     try:
         fullmap = a.map
     except:
         publog.exception("Argparse error. Exiting.")
```

### Comparing `esgcet-5.1.0b13/esgcet/esgmigrate.py` & `esgcet-5.2.0rc2/esgcet/esgmigrate.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,34 +3,54 @@
 import os, sys
 from urllib.parse import urlparse
 import shutil
 from datetime import date
 from pathlib import Path
 import json
 import esgcet.logger as logger
+import yaml
 
 log = logger.Logger()
 
 DEFAULT_ESGINI = '/esg/config/esgcet/'
-CONFIG_FN_DEST = "~/.esg/esg.ini"
+CONFIG_FN_DEST = "~/.esg/esg.yaml"
 
+# These are the keys that 
+MIGRATE_KEYS = ['pid_creds', 'data_roots', 'user_project_config']
 
 def project_list(cfg_obj):
     return [x[0] for x in cfg_obj.get_options_from_table('project_options')]
 
-
 class ESGPubMigrate(object):
 
     def __init__(self, i, newpath, silent=False, verbose=False):
         self.ini_path = i
         self.silent = silent
         self.verbose = verbose
         self.save_path = newpath
         self.publog = log.return_logger('esgmigrate', silent, verbose)
 
+    def migrate_new(self):
+
+        config = cfg.ConfigParser()
+        ini_file = self.ini_path
+        if os.path.isdir(ini_file):
+            ini_file = os.path.join(ini_file, 'esg.ini')
+        config.read(ini_file)        
+        cf_user = config['user']
+
+        cf_dict = {}
+        for key in cf_user:
+            if key in MIGRATE_KEYS:
+                cf_dict[key] = json.loads(cf_user[key])
+            else:
+                cf_dict[key] = cf_user[key]
+        del cf_dict['note']
+        self.write_config(cf_dict)
+
     def project_migrate(self, project):
 
         if not project:
             return None
         path = self.ini_path
         SP = SectionParser("project:{}".format(project), directory=path)
         SP.parse(path)
@@ -57,17 +77,27 @@
             self.publog.exception("Exception encountered.")
             return
 
         thredds_url = sp.get("thredds_url")
         res = urlparse(thredds_url)
         data_node = res.netloc
 
-        index_url = sp.get('rest_service_url')
-        res = urlparse(index_url)
-        index_node = res.netloc
+
+        index_node =''
+        if 'rest_service_url' in sp:
+            index_url = sp.get('rest_service_url')
+            res = urlparse(index_url)
+            index_node = res.netloc
+        else:
+            self.publog.warning("No REST publishing url found in old config, will need to set index_node setting")
+        
+        try:
+            cmor_path = sp.get('cmor_table_path')
+        except:
+            cmor_path = "/usr/local/cmip6-cmor-tables/Tables"
 
         
         try:
             cmor_path = sp.get('cmor_table_path')
         except:
             cmor_path = "/usr/local/cmip6-cmor-tables/Tables"
 
@@ -109,51 +139,49 @@
             if line[0] == "GridFTP":
                 res = urlparse(line[1])
                 DATA_TRANSFER_NODE = res.netloc
             elif line[0] == "Globus":
                 parts= line[1].split(':')
                 GLOBUS_UUID = parts[1][0:36] # length of UUID
 
-        cert_base = sp.get('hessian_service_certfile')
-
+        cert_base = 'none'
+        if 'heshessian_service_certfile' in sp:
+            cert_base = sp.get('hessian_service_certfile')
+        
         CERT_FN = cert_base.replace('%(home)s', '~')
 
         self.publog.debug(str(dr_dict))
         self.publog.debug(str(pid_creds))
         self.publog.debug(data_node)
         self.publog.debug(index_node)
         self.publog.debug(CERT_FN)
         self.publog.debug(DATA_TRANSFER_NODE)
         self.publog.debug(GLOBUS_UUID)
         self.publog.debug(project)
 
         project_config = {project: self.project_migrate(project)}
+        new_config = {"data_node": data_node, "index_node": index_node, "data_roots": dr_dict, "cert": CERT_FN,
+                      "globus_uuid": GLOBUS_UUID, "data_transfer_node": DATA_TRANSFER_NODE, "pid_creds": pid_creds,
+                      "cmor_path" : cmor_path }
+        if project_config:
+            new_config["project_cfg"] = project_config
+        self.write_config(new_config)
+
+    def write_config(self, new_config):
+
+        pid_creds = new_config['pid_creds']
+        new_creds = {}
+        for it in pid_creds:
+            url = it['url']
+            del it['url']
+            new_creds[url] = it
+        new_config['pid_creds'] = new_creds
 
         d = date.today()
         t = d.strftime("%y%m%d")
-        home = str(Path.home())
         config_file = self.save_path
         if os.path.exists(self.save_path):
-            backup = self.save_path + ".bak"
+            backup = f"{self.save_path}.{t}.bak"
             shutil.copyfile(config_file, backup)
-        Path(config_file).touch()
-        config = cfg.ConfigParser()
-        config.read(config_file)
-        new_config = {"data_node": data_node, "index_node": index_node, "data_roots": json.dumps(dr_dict), "cert": CERT_FN,
-                      "globus_uuid": GLOBUS_UUID, "data_transfer_node": DATA_TRANSFER_NODE, "pid_creds": json.dumps(pid_creds),
-                      "cmor_path" : cmor_path }
-
-        try:
-            test = config['user']['data_node']
-            if project_config:
-                new_config["project_cfg"] = json.dumps(project_config)
-            for key, value in new_config.items():
-                if value:
-                    config.set('user', key, value)
-        except:
-            config.add_section('user')
-            for key, value in new_config.items():
-                if value:
-                    config.set('user', key, value)
-        with open(config_file, "w") as cf:
-            config.write(cf)
 
+        with open(config_file, 'w') as f:
+            yaml.dump(new_config, f)
```

### Comparing `esgcet-5.1.0b13/esgcet/esgmkpubrec.py` & `esgcet-5.2.0rc2/esgcet/esgmkpubrec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,120 +1,118 @@
 from esgcet.args import PublisherArgs
 import argparse
 from pathlib import Path
-import configparser as cfg
 import sys
+import esgcet.args as pub_args
 import json
 import os
 import esgcet.logger as logger
 
 log = logger.Logger()
 publog = log.return_logger('esgmkpubrec')
 
+from esgcet.mk_dataset_autoc import ESGPubAutocHandler
+from esgcet.mk_dataset_xarray import ESGPubXArrayHandler
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
 
     # ANY FILE NAME INPUT: check first to make sure it exists
     home = str(Path.home())
-    def_config = home + "/.esg/esg.ini"
+    def_config = home + "/.esg/esg.yaml"
     parser.add_argument("--set-replica", dest="set_replica", action="store_true", help="Enable replica publication.")
     parser.add_argument("--no-replica", dest="no_replica", action="store_true", help="Disable replica publication.")
     parser.add_argument("--json", dest="json", default=None,
                         help="Load attributes from a JSON file in .json form. The attributes will override any found in the DRS structure or global attributes.")
-    parser.add_argument("--scan-file", dest="scan_file", required=True, help="JSON output file from autocurator.")
+    parser.add_argument("--scan-file", dest="scan_file", help="JSON output file from autocurator.  If not set will use XArray to load data from files")
     parser.add_argument("--map-data", dest="map_data", required=True,
                         help="Mapfile json data converted using esgmapconv.")
     parser.add_argument("--out-file", dest="out_file", default=None,
                         help="Optional output file destination. Default is stdout.")
     parser.add_argument("--data-node", dest="data_node", default=None, help="Specify data node.")
     parser.add_argument("--index-node", dest="index_node", default=None, help="Specify index node.")
     parser.add_argument("--project", dest="proj", default="",
                         help="Set/overide the project for the given mapfile, for use with selecting the DRS or specific features, e.g. PrePARE, PID.")
-    parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
+    parser.add_argument("--config", "-cfg", dest="cfg", default=def_config, help="Path to yaml config file.")
     parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
     parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
 
     pub = parser.parse_args()
 
     return pub
 
 
 def run():
 
     a = get_args()
     ini_file = a.cfg
-    config = cfg.ConfigParser()
-    config.read(ini_file)
     if not os.path.exists(ini_file):
         publog.error("Config file not found. " + ini_file + " does not exist.")
         exit(1)
     if os.path.isdir(ini_file):
         publog.error("Config file path is a directory. Please use a complete file path.")
         exit(1)
-    try:
-        config.read(ini_file)
-    except Exception as ex:
-        publog.exception("Could not read config file")
-        exit(1)
-
+    args = pub_args.PublisherArgs()
+    config = args.load_config(ini_file)
 
     p = True
     if a.out_file is not None:
         p = False
         outfile = a.out_file
 
     if not a.silent:
         try:
-            s = config['user']['silent']
+            s = config['silent']
             if 'true' in s or 'yes' in s:
                 silent = True
             else:
                 silent = False
         except:
             silent = False
     else:
         silent = True
-
+        
     if not a.verbose:
         try:
-            v = config['user']['verbose']
+            v = config['verbose']
             if 'true' in v or 'yes' in v:
                 verbose = True
             else:
                     verbose = False
         except:
             verbose = False
     else:
         verbose = True
 
     try:
         map_json_data = json.load(open(a.map_data, 'r'))
     except:
-        publog.exception("Argparse error. Exiting.")
+        publog.exception("Missing required  Exiting.")
         exit(1)
 
-    try:
-        scanfn = a.scan_file
-    except:
-        publog.exception("Argparse error. Exiting.")
-        exit(1)
+    scanarg = a.scan_file
+    
+    if scanarg:
+        format_handler = ESGPubAutocHandler
+    else:
+        format_handler = ESGPubXArrayHandler
+        scanarg = format_handler.xarray_load(map_json_data)
 
     if a.data_node is None:
         try:
-            data_node = config['user']['data_node']
+            data_node = config['data_node']
         except:
             publog.exception("Data node not supplied in config or command line. Exiting.")
             exit(1)
     else:
         data_node = a.data_node
 
     if a.index_node is None:
         try:
-            index_node = config['user']['index_node']
+            index_node = config['index_node']
         except:
             publog.exception("Index node not supplied in config or command line. Exiting.")
             exit(1)
     else:
         index_node = a.index_node
 
     if a.set_replica and a.no_replica:
@@ -122,94 +120,98 @@
         exit(1)
     elif a.set_replica:
         replica = True
     elif a.no_replica:
         replica = False
     else:
         try:
-            r = config['user']['set_replica']
+            r = config['set_replica']
             if 'yes' in r or 'true' in r:
                 replica = True
             elif 'no' in r or 'false' in r:
                 replica = False
             else:
                 publog.error("Set_replica must be true, false, yes, or no.")
                 exit(1)
         except:
             publog.exception("Set_replica not defined. Use --set-replica or --no-replica or define in config file.")
             exit(1)
 
     try:
-        data_roots = json.loads(config['user']['data_roots'])
+        data_roots = config['data_roots']
         if data_roots == 'none':
             publog.error("Data roots undefined. Define in config file to create file metadata.")
             exit(1)
     except:
         publog.exception("Data roots undefined. Define in config file to create file metadata.")
         exit(1)
 
     try:
-        globus = json.loads(config['user']['globus_uuid'])
+        globus = json.loads(config['globus_uuid'])
     except:
         # globus undefined
         globus = "none"
 
     try:
-        dtn = config['user']['data_transfer_node']
+        dtn = config['data_transfer_node']
     except:
         # dtn undefined
         dtn = "none"
 
     json_file = None
     if a.json is not None:
         json_file = a.json
 
     if a.proj != "":
         project = a.proj
     else:
         try:
-            project = config['user']['project']
+            project = config['project']
         except:
             project = None
 
     try:
-        non_netcdf = config['user']['non_netcdf'].lower()
+        non_netcdf = config['non_netcdf'].lower()
         if 'yes' in non_netcdf or 'true' in non_netcdf:
             non_nc = True
         else:
             non_nc = False
     except:
         non_nc = False
 
     try:
-        proj_config = json.loads(config['user']['user_project_config'])
+        proj_config = json.loads(config['user_project_config'])
     except:
         proj_config = None
 
+
+    construct = None
+
     if project == "create-ip":
         from esgcet.mkd_create_ip import ESGPubMKDCreateIP
-        mkd = ESGPubMKDCreateIP(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose, False)
+        construct = ESGPubMKDCreateIP
     elif project == "cmip5":
         from esgcet.mkd_cmip5 import ESGPubMKDCmip5
-        mkd = ESGPubMKDCmip5(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose, False)
+        construct = ESGPubMKDCmip5
     elif project == "input4mips":
         from esgcet.mkd_input4mips import ESGPubMKDinput4MIPs
-        mkd = ESGPubMKDinput4MIPs(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose)
+        construct = ESGPubMKDinput4MIPs
     elif non_nc:
         from esgcet.mkd_non_nc import ESGPubMKDNonNC
-        mkd = ESGPubMKDNonNC(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose)
+        construct = ESGPubMKDNonNC
     else:
         from esgcet.mk_dataset import ESGPubMakeDataset
-        mkd = ESGPubMakeDataset(data_node, index_node, replica, globus, data_roots, dtn, silent, verbose)
+        construct = ESGPubMakeDataset
+    mkd = construct(data_node, index_node, replica, globus, data_roots, dtn, format_handler, silent, verbose)
 
     try:
         if non_nc:
             out_json_data = mkd.get_records(map_json_data, json_file)
         else:
-            out_json_data = mkd.get_records(map_json_data, scanfn, json_file, user_project=proj_config)
+            out_json_data = mkd.get_records(map_json_data, scanarg, json_file, user_project=proj_config)
 
     except Exception as ex:
         publog.exception("Failed to make dataset")
         exit(1)
 
     if p:
         print(json.dumps(out_json_data))
```

### Comparing `esgcet-5.1.0b13/esgcet/esgpidcitepub.py` & `esgcet-5.2.0rc2/esgcet/esgupdate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,121 @@
-from esgcet.pid_cite_pub import ESGPubPidCite
-import argparse
+import os
+from esgcet.update import ESGPubUpdate
 import sys
 import json
+import argparse
 from pathlib import Path
-import configparser as cfg
-import os
+import esgcet.args as pub_args
 import esgcet.logger as logger
 
 log = logger.Logger()
-publog = log.return_logger('esgpidcitepub')
+publog = log.return_logger('esgupdate')
 
 
 def get_args():
     parser = argparse.ArgumentParser(description="Publish data sets to ESGF databases.")
+
     home = str(Path.home())
-    def_config = home + "/.esg/esg.ini"
-    parser.add_argument("--data-node", dest="data_node", default=None, help="Specify data node.")
+    def_config = home + "/.esg/esg.yaml"
+    parser.add_argument("--index-node", dest="index_node", default=None, help="Specify index node.")
+    parser.add_argument("--certificate", "-c", dest="cert", default="./cert.pem",
+                        help="Use the following certificate file in .pem form for publishing (use a myproxy login to generate).")
     parser.add_argument("--pub-rec", dest="json_data", required=True,
-                        help="Dataset and file json data; output from esgmkpubrec.")
-    parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
-    parser.add_argument("--out-file", dest="out_file", default=None,
-                        help="Optional output file destination. Default is stdout.")
+                        help="JSON file output from esgpidcitepub or esgmkpubrec.")
+    parser.add_argument("--config", "-cfg", dest="cfg", default=def_config, help="Path to yaml config file.")
     parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
     parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
-    parser.add_argument("--test", dest="test", action="store_true",
-                        help="PID registration will run in 'test' mode. Use this mode unless you are performing 'production' publications.")
+    parser.add_argument("--no-auth", dest="no_auth", action="store_true",
+                        help="Run publisher without certificate, only works on certain index nodes.")
+    parser.add_argument("--verify", dest="verify", action="store_true",
+                        help="Toggle verification for publishing, default is off.")
 
     pub = parser.parse_args()
 
     return pub
 
 
 def run():
     a = get_args()
+
     ini_file = a.cfg
-    config = cfg.ConfigParser()
-    config.read(ini_file)
     if not os.path.exists(ini_file):
         publog.error("Config file not found. " + ini_file + " does not exist.")
         exit(1)
     if os.path.isdir(ini_file):
         publog.error("Config file path is a directory. Please use a complete file path.")
         exit(1)
-    try:
-        config.read(ini_file)
-    except Exception as ex:
-        publog.exception("Could not read config file")
-        exit(1)
-
-
-    p = True
-    if a.out_file is not None:
-        p = False
-        outfile = a.out_file
-
-    if a.data_node is None:
-        try:
-            data_node = config['user']['data_node']
-        except:
-            publog.exception("Data node not supplied in config or command line. Exiting.")
-            exit(1)
+    args = pub_args.PublisherArgs()
+    config = args.load_config(ini_file)
 
     if not a.silent:
         try:
-            s = config['user']['silent']
+            s = config['silent']
             if 'true' in s or 'yes' in s:
                 silent = True
             else:
                 silent = False
         except:
             silent = False
     else:
         silent = True
 
     if not a.verbose:
         try:
-            v = config['user']['verbose']
+            v = config['verbose']
             if 'true' in v or 'yes' in v:
                 verbose = True
             else:
                 verbose = False
         except:
             verbose = False
     else:
         verbose = True
 
-    if a.data_node is None:
+    if a.cert == "./cert.pem":
         try:
-            data_node = config['user']['data_node']
+            cert = config['cert']
         except:
-            publog.exception("Data node not supplied in config or command line. Exiting.")
-            exit(1)
+            cert = a.cert
     else:
-        data_node = a.data_node
+        cert = a.cert
 
-    test = False
-    if a.test:
-        test = True
+    if a.verify:
+        verify = True
+    else:
+        verify = False
 
-    try:
-        pid_creds = json.loads(config['user']['pid_creds'])
-    except:
-        publog.exception("PID credentials not defined. Define in config file esg.ini.")
-        exit(1)
+    if a.no_auth:
+        auth = False
+    else:
+        auth = True
+
+    if a.index_node is None:
+        try:
+            index_node = config['index_node']
+        except:
+            publog.exception("Index node not defined. Use the --index-node option or define in esg.ini.")
+            exit(1)
+    else:
+        index_node = a.index_node
 
     try:
-        out_json_data = json.load(open(a.json_data))
+        new_json_data = json.load(open(a.json_data))
     except:
-        publog.exception("Could not open JSON file. Exiting.")
+        publog.exception("Could not open json file. Exiting.")
         exit(1)
 
-    pid = ESGPubPidCite(out_json_data, pid_creds, data_node, test=test, silent=silent,
-                        verbose=verbose)
-
+    up = ESGPubUpdate(index_node, cert, silent=silent, verbose=verbose, verify=verify,
+                      auth=auth)
     try:
-        new_json_data = pid.do_pidcite()
+        up.run(new_json_data)
     except Exception as ex:
-        publog.exception("Failed assigning pid or running activity check")
+        publog.exception("Failed to update record")
         exit(1)
 
-    if p:
-        print(json.dumps(new_json_data))
-    else:
-        with open(outfile, 'w') as of:
-            json.dump(new_json_data, of)
-
 
 def main():
     run()
 
 
 if __name__ == '__main__':
     sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
```

### Comparing `esgcet-5.1.0b13/esgcet/esgunpublish.py` & `esgcet-5.2.0rc2/esgcet/esgunpublish.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import esgcet.unpublish as upub
 import os
 import sys
 import json
 import argparse
-import configparser as cfg
 from pathlib import Path
+import esgcet.args as pub_args
 import esgcet.logger as logger
 
 from esgcet.mapfile import ESGPubMapConv
 
 log = logger.Logger()
 publog = log.return_logger('esgunpublish')
 
 import esgcet
 
 def get_args():
     parser = argparse.ArgumentParser(description="Unpublish data sets from ESGF databases.")
 
     home = str(Path.home())
-    def_config = home + "/.esg/esg.ini"
+    def_config = home + "/.esg/esg.yaml"
     parser.add_argument("--index-node", dest="index_node", default=None, help="Specify index node.")
     parser.add_argument("--data-node", dest="data_node", default=None, help="Specify data node.")
     parser.add_argument("--certificate", "-c", dest="cert", default="./cert.pem",
                         help="Use the following certificate file in .pem form for unpublishing (use a myproxy login to generate).")
     parser.add_argument("--delete", dest="delete", action="store_true", help="Specify deletion of dataset (default is retraction).")
     parser.add_argument("--dset-id", dest="dset_id", default=None,
                         help="Dataset ID for dataset to be retracted or deleted.")
     parser.add_argument("--map", dest="map", default=None, nargs="+",
                         help="Path(s) to a mapfile or directory(s) containing mapfiles.")    
     parser.add_argument("--use-list", dest="dset_list", default=None,
                         help="Path to a file containing list of dataset_ids.")
-    parser.add_argument("--ini", "-i", dest="cfg", default=def_config, help="Path to config file.")
+    parser.add_argument("--config", "-i", dest="cfg", default=def_config, help="Path to config file.")
     parser.add_argument("--version", action="version", version=f"esgunpublish v{esgcet.__version__}",help="Print the version and exit")
     parser.add_argument("--no-auth", dest="no_auth", action="store_true", help="Run publisher without certificate, only works on certain index nodes.")
     parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
     parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
 
     pub = parser.parse_args()
 
@@ -67,135 +67,121 @@
                         dset_list.append(dataset_id)
         else:
             dataset_id = map_to_dataset(m)
             dset_list.append(dataset_id)
 
     return dset_list
 
-
 def run():
     a = get_args()
 
-    ini_file = a.cfg
-    config = cfg.ConfigParser()
-    if not os.path.exists(ini_file):
-        publog.error("Config file not found. " + ini_file + " does not exist.")
-        exit(1)
-    if os.path.isdir(ini_file):
-        publog.error("Config file path is a directory. Please use a complete file path.")
-        exit(1)
-    try:
-        config.read(ini_file)
-    except Exception as ex:
-        publog.exception("Could not read config file")
-        exit(1)
-
+    cfg_file = a.cfg
+    if os.path.isdir(cfg_file):
+        cfg_file = os.path.join(cfg_file, "esg.yaml")
+    if not os.path.exists(cfg_file):
+        publog.error(f"Config file not found. {cfg_file} does not exist.")
+        raise RuntimeError(f"Config file not found. {cfg_file} does not exist.")
 
+    args = pub_args.PublisherArgs()
+    config = args.load_config(cfg_file)
     if a.cert == "./cert.pem":
         try:
-            cert = config['user']['cert']
+            cert = config['cert']
         except:
             cert = a.cert
     else:
         cert = a.cert
 
     if a.index_node is None:
         try:
-            index_node = config['user']['index_node']
+            index_node = config['index_node']
         except:
             publog.exception("Index node not defined. Use the --index-node option or define in esg.ini.")
             exit(1)
     else:
         index_node = a.index_node
 
-
     dset_id = ""
-
     if a.dset_id:
-
         dset_id = a.dset_id
 
     if not '|' in dset_id or (a.map):
         if a.data_node is None:
             try:
-                data_node = config['user']['data_node']
+                data_node = config['data_node']
             except:
                 publog.exception("Data node not defined. Use the --data-node option or define in esg.ini.")
                 exit(1)
         else:
             data_node = a.data_node
     else:
         data_node = None
 
-
     if a.delete:
         d = True
     else:
         d = False
 
     if a.no_auth:
         auth = False
     else:
         auth = True
-
+        
     if not a.silent:
         try:
-            s = config['user']['silent']
+            s = config['silent']
             if 'true' in s or 'yes' in s:
                 silent = True
             else:
                 silent = False
         except:
             silent = False
     else:
         silent = True
 
     if not a.verbose:
         if not a.silent:
             try:
-                v = config['user']['verbose']
+                v = config['verbose']
                 if 'true' in v or 'yes' in v:
                     verbose = True
                 else:
                     verbose = False
             except:
                 verbose = False
     else:
         verbose = True
         silent = False
 
-
-    args = {    "delete": d, 
+    args = { "delete": d, 
              "data_node": data_node, 
              "index_node": index_node, 
              "cert": cert, 
              "auth" :auth, 
              "verbose" : verbose,
              "silent" :silent }
 
-
     if len(dset_id) > 0:
         args["dataset_id_lst"] = [dset_id]
     elif a.map:
-
         args["dataset_id_lst"] = maps_to_dataset_list(a.map)
     elif a.dset_list:
         try:
             dset_arr = [line.rstrip() for line in open(a.dset_list)]
         except:
             publog.exception(f"Error opening {args['dset_list']} file.")
 
         args["dataset_id_lst"] = dset_arr
     else:
         publog.error("No unpublish input method specified.  Please use from one of the following arguments: --map --use-list --dset-id ; type esgunpublish --help for more info")
         exit(1)
 
     if (upub.check_for_pid_proj(args["dataset_id_lst"])):
         try:
-            pid_creds = json.loads(config['user']['pid_creds'])
+            pid_creds = config['pid_creds']
             args["pid_creds"] = pid_creds
         except:
             publog.exception("PID credentials not defined. Define in config file esg.ini.")
             exit(1)    
 
     status = 0
     try:
```

### Comparing `esgcet-5.1.0b13/esgcet/generic_netcdf.py` & `esgcet-5.2.0rc2/esgcet/generic_netcdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from esgcet.mk_dataset_autoc import ESGPubAutocHandler
+from esgcet.mk_dataset_xarray import ESGPubXArrayHandler
 from esgcet.mk_dataset import ESGPubMakeDataset
+
 import json, os, sys
 import tempfile
 from esgcet.generic_pub import BasePublisher
 import traceback
 import esgcet.logger as logger
 
 log = logger.Logger()
@@ -10,56 +13,82 @@
 class GenericPublisher(BasePublisher):
 
     scan_file = tempfile.NamedTemporaryFile()  # create a temporary file which is deleted afterward for autocurator
     scanfn = scan_file.name
 
     def __init__(self, argdict):
         super().__init__(argdict)
-        self.autoc_command = argdict["autoc_command"]
-        self.MKD_Construct = ESGPubMakeDataset
+
+        self.MKD_Construct = ESGPubMakeDataset        
+        if argdict["autoc_command"]:
+            self.autoc_command = argdict["autoc_command"]
+            self.format_handler = ESGPubAutocHandler
+            self.extract_method = self.autocurator
+        else:
+            self.autoc_command = None
+            self.extract_method = self.xarray_load
+            self.format_handler = ESGPubXArrayHandler
+
         self.publog = log.return_logger('Generic NetCDF Publisher', self.silent, self.verbose)
 
     def cleanup(self):
         self.scan_file.close()
 
+    def xarray_load(self, map_json_data):
+        """
+        Xarray Load
+        """
+        self.xarray_set = self.format_handler.xarray_load(map_json_data)
+
+
     def autocurator(self, map_json_data):
+        """
+        Autocurator
+        """
         datafile = map_json_data[0][1]
 
         destpath = os.path.dirname(datafile)
         outname = os.path.basename(datafile)
         idx = outname.rfind('.')
 
         autstr = self.autoc_command + ' --out_pretty --out_json {} --files "{}/*.nc"'
+        self.publog.debug(f"RUNNING {autstr}")
         stat = os.system(autstr.format(self.scanfn, destpath))
         if os.WEXITSTATUS(stat) != 0:
             self.publog.error("Autocurator exited with exit code: " + str(os.WEXITSTATUS(stat)))
             self.cleanup()
             exit(os.WEXITSTATUS(stat))
 
     def mk_dataset(self, map_json_data):
         mkd = self.MKD_Construct(self.data_node, self.index_node, self.replica, self.globus, self.data_roots, self.dtn,
-                                self.silent, self.verbose)
+                                self.format_handler, self.silent, self.verbose)
         mkd.set_project(self.project)
+
+        if self.autoc_command:
+            scan_arg = json.load(open(self.scanfn))
+        else:
+            scan_arg = self.xarray_set
+
         try:
-            out_json_data = mkd.get_records(map_json_data, self.scanfn, self.json_file, user_project=self.proj_config)
+            out_json_data = mkd.get_records(map_json_data, scan_arg, self.json_file, user_project=self.proj_config)
         except Exception as ex:
             self.publog.exception("Failed to make dataset")
             self.cleanup()
             exit(1)
         return out_json_data
 
     def workflow(self):
 
         # step one: convert mapfile
         self.publog.info("Converting mapfile...")
         map_json_data = self.mapfile()
 
         # step two: autocurator
-        self.publog.info("Running autocurator...")
-        self.autocurator(map_json_data)
+        self.publog.info(f"Running Extraction... {str(self.extract_method)}")
+        self.extract_method(map_json_data)
 
         # step three: make dataset
         self.publog.info("Making dataset...")
         out_json_data = self.mk_dataset(map_json_data)
 
         # step four: update record if exists
         self.publog.info("Updating...")
@@ -67,8 +96,8 @@
 
         # step five: publish to database
         self.publog.info("Running index pub...")
         rc = self.index_pub(out_json_data)
 
         self.publog.info("Done. Cleaning up.")
         self.cleanup()
-        return rc
+        return rc
```

### Comparing `esgcet-5.1.0b13/esgcet/generic_pub.py` & `esgcet-5.2.0rc2/esgcet/generic_pub.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/index_pub.py` & `esgcet-5.2.0rc2/esgcet/index_pub.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/input4mips.py` & `esgcet-5.2.0rc2/esgcet/input4mips.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 
     def workflow(self):
 
         # step one: convert mapfile
         self.publog.info("Converting mapfile...")
         map_json_data = self.mapfile()
 
-        # step three: autocurator
-        self.publog.info("Running autocurator...")
-        self.autocurator(map_json_data)
+        # step three: extract data
+        self.publog.info(f"Running Extraction... {str(self.extract_method)}")
+        self.extract_method(map_json_data)
 
         # step four: make dataset
         self.publog.info("Making dataset...")
         out_json_data = self.mk_dataset(map_json_data)
 
         # step five: assign PID
         self.publog.info("Assigning PID...")
@@ -45,8 +45,8 @@
 
         # step seven: publish to database
         self.publog.info("Running index pub...")
         rc = self.index_pub(new_json_data)
 
         self.publog.info("Done. Cleaning up.")
         self.cleanup()
-        return rc
+        return rc
```

### Comparing `esgcet-5.1.0b13/esgcet/list2json.py` & `esgcet-5.2.0rc2/esgcet/list2json.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/logger.py` & `esgcet-5.2.0rc2/esgcet/logger.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/mapfile.py` & `esgcet-5.2.0rc2/esgcet/mapfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         ret = []
         for line in self.map_data:
 
             parts = line.rstrip().split(' | ')
             if mountpoints and self.project:
                 mapstr = parts[1]
                 root = mapstr.split(self.project)[0][:-1]
-                parts[1] = mapstr.replace(root, mountpoints[root])
+                if root in mountpoints:
+                    parts[1] = mapstr.replace(root, mountpoints[root])
 
             ret.append(parts)
 
         self.map_data_arr = ret
         return ret
 
     def set_map_arr(self, maparr):
```

### Comparing `esgcet-5.1.0b13/esgcet/migratecmd.py` & `esgcet-5.2.0rc2/esgcet/migratecmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     parser = argparse.ArgumentParser(description="Migrate old config settings into new format.")
 
     parser.add_argument("--old-config", dest="cfg", default=DEFAULT_ESGINI, help="Path to directory containing old config file to migrate.")
     parser.add_argument("--silent", dest="silent", action="store_true", help="Enable silent mode.")
     parser.add_argument("--verbose", dest="verbose", action="store_true", help="Enable verbose mode.")
     parser.add_argument("--project", dest="project", default=None, help='Name of a particular legacy project to migrate.')
     parser.add_argument("--destination", dest='dest', default=home+'/.esg/esg.ini', help="Destination for new config file.")
-
+    parser.add_argument("--v5", dest="newcfg", action="store_true", help="Migrate a v5 esg.ini rather than a legacy version (v4 or earlier)")
     pub = parser.parse_args()
 
     return pub
 
 
 def main():
 
@@ -32,15 +32,18 @@
     silent = a.silent
     verbose = a.verbose
     project = a.project
     filepath = a.dest
 
     try:
         em = ESGPubMigrate(ini_path, filepath, silent=silent, verbose=verbose)
-        em.migrate(project)
+        if a.newcfg:
+            em.migrate_new()
+        else:
+            em.migrate(project)
     except:
         publog.exception("Failed to migrate old config")
 
 
 if __name__ == "__main__":
     sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
     main()
```

### Comparing `esgcet-5.1.0b13/esgcet/mk_dataset.py` & `esgcet-5.2.0rc2/esgcet/mk_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 
 from esgcet.settings import *
 from pathlib import Path
 import esgcet.logger as logger
 
 log = logger.Logger()
 
-
 class ESGPubMakeDataset:
-
+    """
+    Base class (abstract) to assemble the ESGF index records (dataset and file records).
+    """
     def init_project(self, proj):
+        """
+        Intialize the specific project metadata based on a stock or custom configuration
+
+        proj: Name of the project to be process
+        """
         project = proj
 
         if project in DRS:
             self.DRS = DRS[project]
             if project in CONST_ATTR:
                 self.CONST_ATTR = CONST_ATTR[project]
         elif self.user_project and "clone_project" in self.user_project:
@@ -35,15 +41,30 @@
             if 'DRS' in self.user_project[project]:
                 self.DRS = self.user_project[project]['DRS']
             if 'CONST_ATTR' in self.user_project[project]:
                 self.CONST_ATTR = self.user_project[project]['CONST_ATTR']
         else:
             raise (BaseException(f"Error: Project {project} Data Record Syntax (DRS) not defined. Define in esg.ini"))
 
-    def __init__(self, data_node, index_node, replica, globus, data_roots, dtn, silent=False, verbose=False, limit_exceeded=False, user_project=None):
+    def __init__(self, data_node, index_node, replica, globus, data_roots, dtn, handler_class, silent=False, verbose=False, limit_exceeded=False, user_project=None):
+        """
+        Constructor
+
+        data_node (string):  ESGF Data Node to host the data 
+        index_node (string):  ESGF Index Node to 
+        replica (bool):  Is data a replca
+        globus (string):  Globus endpoint UUID
+        data_roots (dict): mapping of logical to file system roots for data
+        dtn (string):  legacy server name for gridftp urls
+        handler_class (class):  class type of the handler to construct the (format) handler object
+        silent (bool):  Run in silent mode (suppress all output but errors)
+        verbose (bool):  Print verbose (debug), 
+        limit_exceeded (bool):
+        user_project (dict):  User-defined project config info
+        """
         self.silent = silent
         self.verbose = verbose
         self.data_roots = data_roots
         self.globus = globus
         self.data_node = data_node
         self.index_node = index_node
         self.replica = replica
@@ -52,60 +73,75 @@
 
         self.mapconv = ESGPubMapConv("")
         self.dataset = {}
         self.project = None
         self.user_project = user_project
         self.DRS = None
         self.CONST_ATTR = None
+        #  The default for variables, specific projects may use "variable" instead
         self.variable_name = "variable_id"
         self.publog = log.return_logger('Make Dataset', self.silent, self.verbose)
         self.xattr = None
         self.tracking_id_set = set()
+        self.handler = handler_class(self.publog)
 
     def set_project(self, project_in):
+        """
+        Configure the project
+        """
         self.project = project_in
 
-    def unpack_values(self, invals):
-        for x in invals:
-            if x['values']:
-                yield x['values']
-
     def prune_list(self, ll):
+        """
+        Shorten the list only actual items (no Nones)
+
+        ll (list):  input list
+
+        return list
+        """
         for x in ll:
             if not x is None:
                 yield (x)
 
     def load_xattr(self, xattrfn):
+        """
+        Load a set of "extended attributes" ie. additional key-value pairs for the dataset record from a file
+        Default method, specific projects may format attributes diffeerntly
+        xattrfn (string):  Full path to a .json file containing the pairs
+        """
         if self.xattr:
             return
         if (xattrfn):
             self.xattr = json.load(open(xattrfn))
         else:
             self.xattr = {}
 
     def proc_xattr(self, xattrfn):
+        """
+        Load and process the extended attributes
+        """
         self.load_xattr(xattrfn)
         if len(self.xattr) > 0:
             tmp_xattr = self.xattr_handler()
             for key in tmp_xattr:
                 self.dataset[key] = tmp_xattr[key]
 
     def xattr_handler(self):
+        """
+        Base method for handling the extended attributes
+        """
         return self.xattr
 
     def get_dataset(self, mapdata, scanobj):
 
         master_id, version = mapdata.split('#')
-
         parts = master_id.split('.')
-
         projkey = parts[0]
         self.first_val = projkey
-        scandata = scanobj['dataset']
-
+        scandata = self.handler.get_attrs_dict(scanobj)
 
         if self.project:
             projkey = self.project
         self.init_project(projkey.lower())
 
         facets = self.DRS  # depends on Init_project to initialize
 
@@ -244,158 +280,77 @@
                     root_found = True
                     break
             if not root_found:
                 self.publog.error('The file system root {} not found.  Please check your configuration.'.format(proj_root))
                 exit(1)
 
         ret["url"] = self.gen_urls(self.data_roots[proj_root], rel_path)
-        ret["publish_path"] = f"{self.data_roots[proj_root]}/{rel_path}"
+        ret["publish_path"] = f"{self.data_roots[proj_root]}/{rel_path}" 
         if "number_of_files" in ret:
             ret.pop("number_of_files")
         else:
             self.publog.warning("No files present")
         if "datetime_start" in ret:
             ret.pop("datetime_start")
             ret.pop("datetime_end")
 
         return ret
 
-    def get_scanfile_dict(self, scandata):
-        ret = {}
-        for key in scandata:
-            rec = scandata[key]
-            ret[rec['name']] = rec
-        return ret
-
-    def update_metadata(self, record, scanobj):
-        if "variables" in scanobj:
-            if self.variable_name in record:
-
-                vid = record[self.variable_name]
-                try:
-                    if vid in scanobj["variables"]:
-                        var_rec = scanobj["variables"][vid]
-                        if "long_name" in var_rec.keys():
-                            record["variable_long_name"] = var_rec["long_name"]
+    def set_variables(self, record, scanobj):
+        variables = self.handler.get_variables(scanobj)
+        # use the correct facet id string to get the variable if pre-specified in the record
+        vid = record[self.variable_name]
+        if vid in variables:
+            var_rec = variables[vid]
+            if "long_name" in var_rec:
+                record["variable_long_name"] = var_rec["long_name"]
+            elif "info" in var_rec:
+                record["variable_long_name"] = var_rec["info"]
+            if "standard_name" in var_rec:
+                record["cf_standard_name"] = var_rec["standard_name"]
+            if "units" in var_rec:
+                record["variable_units"] = var_rec["units"]
+            record[self.variable_name] = vid
+            if self.variable_name == "variable_id":
+                record["variable"] = vid
+        else:
+            var_list = self.handler.get_variable_list(variables)
+            if len(var_list) < VARIABLE_LIMIT:
+                init_lst = [self.variable_name, "variable_long_name"]
+                if "variable_id" in init_lst:
+                    init_lst.append("variable")
+                for kid in init_lst:
+                    record[kid] = []
+                units_list = []
+                cf_list = []
+                for vk in var_list:
+                    if not vk in VARIABLE_EXCLUDES:
+                        var_rec = variables[vk]
+                        if "long_name" in var_rec:
+                            record["variable_long_name"].append(var_rec["long_name"])
                         elif "info" in var_rec:
-                            record["variable_long_name"] = var_rec["info"]
-                        if "standard_name" in var_rec:
-                            record["cf_standard_name"] = var_rec["standard_name"]
-                        record["variable_units"] = var_rec["units"]
-                        record[self.variable_name] = vid
-                        if self.variable_name == "variable_id":
-                            record["variable"] = vid
-                    else:
-                        var_list = list(scanobj["variables"].keys())
-                        if len(var_list) < VARIABLE_LIMIT:
-                            init_lst = [self.variable_name, "variable_long_name"]
-                            if "variable_id" in init_lst:
-                                init_lst.append("variable")
-                            for kid in init_lst:
-                                record[kid] = []
-                            units_list = []
-                            cf_list = []
-                            for vk in var_list:
-                                if not vk in VARIABLE_EXCLUDES:
-                                    var_rec = scanobj["variables"][vk]
-                                    if "long_name" in var_rec.keys():
-                                        record["variable_long_name"].append(var_rec["long_name"])
-                                    elif "info" in var_rec:
-                                        record["variable_long_name"].append(var_rec["info"])
-                                    if "standard_name" in var_rec and len(var_rec["standard_name"]) > 0:
-                                        cf_list.append(var_rec["standard_name"])          
-                                    if var_rec["units"] != "1" and len(var_rec["units"]) > 0:
-                                        units_list.append(var_rec["units"])
-                                    record["variable"].append(vk)
-
-                            if self.variable_name == "variable_id":
-                                record[self.variable_name] = "Multiple"
-                            record["variable_units"] = list(set(units_list))
-                            record["cf_standard_name"] = list(set(cf_list))
-                    
-                        if self.variable_name == "variable_id":
-                            record["variable"] = "Multiple"
-
-                except Exception as ex:
-                    self.publog.exception("Variable could not be extracted, exception encountered")
-                    record[self.variable_name] = "none"
-            else:
-                self.publog.warning("TODO check project settings for variable extraction")
-                record[self.variable_name] = "Multiple"
+                            record["variable_long_name"].append(var_rec["info"])
+                        if "standard_name" in var_rec and len(var_rec["standard_name"]) > 0:
+                            cf_list.append(var_rec["standard_name"])          
+                        if var_rec["units"] != "1" and len(var_rec["units"]) > 0:
+                            units_list.append(var_rec["units"])
+                        record["variable"].append(vk)
+
                 if self.variable_name == "variable_id":
-                    record["variable"] = "Multiple"
-        else:
-            self.publog.warning("No variables were extracted (is this CF compliant?)")
+                    record[self.variable_name] = "Multiple"
+                record["variable_units"] = list(set(units_list))
+                record["cf_standard_name"] = list(set(cf_list))
+        
+            if self.variable_name == "variable_id":
+                record["variable"] = "Multiple"
 
-        geo_units = []
-        if "axes" in scanobj:
-            axes = scanobj["axes"]
-            if "lat" in axes:
-                lat = axes["lat"]
-                geo_units.append(lat["units"])
-                if 'values' not in lat.keys():
-                    record["north_degrees"] = lat['subaxes']['0']["values"][-1]
-                    record["south_degrees"] = lat['subaxes']['0']["values"][0]
-                else:
-                    record["north_degrees"] = lat["values"][-1]
-                    record["south_degrees"] = lat["values"][0]
-            if "lon" in axes:
-                lon = axes["lon"]
-                geo_units.append(lon["units"])
-                if 'values' not in lon.keys():
-                    record["east_degrees"] = lon['subaxes']['0']["values"][-1]
-                    record["west_degrees"] = lon['subaxes']['0']["values"][0]
-                else:
-                    record["east_degrees"] = lon["values"][-1]
-                    record["west_degrees"] = lon["values"][0]
-            if "time" in axes:
-                time_obj = axes["time"]
-                time_units = time_obj["units"]
-                tu_parts = []
-                if type(time_units) is str:
-                    tu_parts = time_units.split()
-                if len(tu_parts) > 2 and tu_parts[0] == "days" and tu_parts[1] == "since":
-                    proc_time = True
-                    tu_date = tu_parts[2]  # can we ignore time component?
-                    if "subaxes" in time_obj:
-                        subaxes = time_obj["subaxes"]
-                        sub_values = sorted([x for x in self.unpack_values(subaxes.values())])
-
-                        tu_start_inc = int(sub_values[0][0])
-                        tu_end_inc = int(sub_values[-1][-1])
-                    elif "values" in time_obj:
-                        tu_start_inc = time_obj["values"][0]
-                        tu_end_inc = time_obj["values"][-1]
-                    else:
-                        self.publog.warning("Time values not located...")
-                        proc_time = False
-                    if proc_time:
-                        try:
-                            days_since_dt = datetime.strptime(tu_date.split("T")[0], "%Y-%m-%d")
-                        except:
-                            tu_date = '0' + tu_date
-                            while len(tu_date.split('-')[0]) < 4:
-                                tu_date = '0' + tu_date
-                            days_since_dt = datetime.strptime(tu_date.split("T")[0], "%Y-%m-%d")
-                        dt_start = days_since_dt + timedelta(days=tu_start_inc)
-                        dt_end = days_since_dt + timedelta(days=tu_end_inc)
-                        if dt_start.microsecond >= 500000:
-                            dt_start = dt_start + timedelta(seconds=1)
-                        dt_start = dt_start.replace(microsecond=0)
-                        record["datetime_start"] = "{}Z".format(dt_start.isoformat())
-                        record["datetime_end"] = "{}Z".format(dt_end.isoformat())
-
-            if "plev" in axes:
-                plev = axes["plev"]
-                if "units" in plev and "values" in plev:
-                    record["height_units"] = plev["units"]
-                    record["height_top"] = plev["values"][0]
-                    record["height_bottom"] = plev["values"][-1]
-        else:
-            self.publog.warning("No axes extracted from data files")
+    def update_metadata(self, record, scanobj):
+
+        self.set_variables(record, scanobj)
+        self.handler.set_bounds(record, scanobj)
 
     def iterate_files(self, mapdata, scandata):
         ret = []
         sz = 0
         last_file = None
 
         for maprec in mapdata:
@@ -416,43 +371,41 @@
             if x:
                 lst.append(x)
         last_file["url"] = lst
         access = [x.split("|")[2] for x in last_file["url"]]
 
         return ret, sz, access
 
-    def get_records(self, mapdata, scanfilename, xattrfn=None, user_project=None):
+    def get_records(self, mapdata, scanobj, xattrfn=None, user_project=None):
 
         self.user_project = user_project
         self.load_xattr(xattrfn)
 
         if isinstance(mapdata, str):
             mapobj = json.load(open(mapdata))
         else:
             mapobj = mapdata
-        scanobj = json.load(open(scanfilename))
 
         self.get_dataset(mapobj[0][0], scanobj)
         self.update_metadata(self.dataset, scanobj)
         self.dataset["number_of_files"] = len(mapobj)  # place this better
         project = self.dataset['project']
 
         self.proc_xattr(xattrfn)
 
         self.publog.debug("Record:\n" + json.dumps(self.dataset, indent=4))
-        print()
 
         self.mapconv.set_map_arr(mapobj)
         mapdict = self.mapconv.parse_map_arr()
 
-        self.publog.debug('Mapfile dictionary:\n' + json.dumps(mapdict, indent=4))
-        print()
-        scandict = self.get_scanfile_dict(scanobj['file'])
-        self.publog.debug('Autocurator Scanfile dictionary:\n' + json.dumps(scandict, indent=4))
-        print()
+        #self.publog.debug('Mapfile dictionary:\n' + json.dumps(mapdict, indent=1)) # Superverbose
+       
+        scandict = self.handler.get_scanfile_dict(scanobj, mapdict)
+        #self.publog.debug('Autocurator Scanfile dictionary:\n' + json.dumps(scandict, indent=1))  # Superverbose
+
         ret, sz, access = self.iterate_files(mapdict, scandict)
         self.dataset["size"] = sz
         self.dataset["access"] = access
         ret.append(self.dataset)
         return ret
 
     @staticmethod
```

### Comparing `esgcet-5.1.0b13/esgcet/mkd_create_ip.py` & `esgcet-5.2.0rc2/esgcet/mkd_create_ip.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,40 +17,25 @@
     def init_project(self, s, l):
 
         self.project = "CREATE-IP"
         if s in self.source_ids:
             self.DRS = DRS["create-ip-src"]
         elif l == 7:
             self.DRS = DRS["create-ip-model"]
+        elif l == 8:
+            self.DRS = DRS["create-ip-var"]
         else:
             self.DRS = DRS["create-ip-exp"]
 
-    def __init__(self, data_node, index_node, replica, globus, data_roots, dtn, silent=False, verbose=False, limit_exceeded=False, user_project=None):
-        self.silent = silent
-        self.verbose = verbose
-        self.data_roots = data_roots
-        self.globus = globus
-        self.data_node = data_node
-        self.index_node = index_node
-        self.replica = replica
-        self.dtn = dtn
-        self.limit_exceeded = limit_exceeded
-
-        self.mapconv = ESGPubMapConv("")
-        self.dataset = {}
-        self.project = None
-        self.user_project = user_project
-        self.DRS = None
-        self.CONST_ATTR = None
-        self.variable_name = "variable_id"
-        self.variable = None
-
-        self.source_ids = ["CCSM-CAM", "CFSR", "CREATE-MRE2models", "CREATE-MRE3models", "CREATE-MREmodels", "GEOS-5",
+    def __init__(self, *args, **kwargs):
+        super(ESGPubMakeDataset,self).__init__(args, kwargs)
+        self.models = ["CCSM-CAM", "CFSR", "CREATE-MRE2models", "CREATE-MRE3models", "CREATE-MREmodels", "GEOS-5",
                    "IFS-Cy31r2", "IFS-Cy41r2", "JRA-25", "JRA-55", "MITgcm", "MOM3", "MOM4", "MRICOMv3",
                    "NCEP-Global-Operational-Model", "NEMOv3", "NEMOv32-LIM2", "NEMOv34-LIM2", "ORAmodels", "ensda-v351"]
+        self.source_ids = [ "20CRv2c", "C-GLORSv5", "CERA-20C", "CFSR", "CREATE-MRE", "ECDAv31", "ERA-Interim", "ERA40-CRUTS3-10", "ERA5", "ERAInterim-CRUTS3-10", "GECCO2", "GODAS", "JRA-25", "JRA-55," "JRA-55-mdl-iso", "MERRA", "MERRA-CRUTS3-10", "MERRA2", "MERRA2-ASM", "MOVE-G2i", "MRE2ensemble", "NCEP-NCAR-CRUTS3-10", "ORAP5", "ORAS4", "ORAensemble"]
         self.publog = log.return_logger('Make Dataset CREATE-IP', self.silent, self.verbose)
 
     def get_dataset(self, mapdata, scanobj):
 
         master_id, version = mapdata.split('#')
 
         parts = master_id.split('.')
```

### Comparing `esgcet-5.1.0b13/esgcet/mkd_input4mips.py` & `esgcet-5.2.0rc2/esgcet/mkd_input4mips.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/mkd_non_nc.py` & `esgcet-5.2.0rc2/esgcet/mkd_non_nc.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,42 +59,29 @@
 
         access = [x.split("|")[2] for x in last_file["url"]]
 
         return ret, sz, access
 
     def get_records(self, mapdata, xattrfn=None, user_project=None):
         self.user_project = user_project
-        self.load_xattr(xattrfn)
 
         if isinstance(mapdata, str):
             mapobj = json.load(open(mapdata))
         else:
             mapobj = mapdata
 
         self.get_dataset(mapobj[0][0])
 
-
         self.dataset["number_of_files"] = len(mapobj)  # place this better
         project = self.dataset['project']
 
-        if xattrfn:
-            xattrobj = json.load(open(xattrfn))
-        else:
-            xattrobj = {}
-
-        if len(xattrobj) > 0:
-            xattrobj = self.xattr_handler()
-
-        for key in xattrobj:
-            self.dataset[key] = xattrobj[key]
-
+        self.proc_xattr(xattrfn)
         self.publog.debug("Record:\n" + json.dumps(self.dataset, indent=4))
         print()
 
-
         self.mapconv.set_map_arr(mapobj)
         mapdict = self.mapconv.parse_map_arr()
         self.publog.debug('Mapfile dictionary:\n' + json.dumps(mapdict, indent=4))
         print()
 
         ret, sz, access = self.iterate_files(mapdict)
```

### Comparing `esgcet-5.1.0b13/esgcet/pid_cite_pub.py` & `esgcet-5.2.0rc2/esgcet/pid_cite_pub.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         """ Constructor
             ds_rec - a dataset record (dictionary/json)
             pid_creds - credentials typically loaded from config file, contains PID server, password, etc.
             silent, verbose - suppress info msgs, extend print
             test - register PID in test mode, essential for testing """
         self.ds_records = ds_recs
         self.pid_creds = pid_creds
+        if type(self.pid_creds) == dict:
+            self.pid_creds = [ self.pid_creds, ]
         self.silent = silent
         self.verbose = verbose
         self.test_publication = test
         self.pid_prefix = pid_prefix
         self.project_family = project_family
         self.data_node = data_node
         self.publog = log.return_logger('PID Citation', silent, verbose)
```

### Comparing `esgcet-5.1.0b13/esgcet/pub_client.py` & `esgcet-5.2.0rc2/esgcet/pub_client.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/pub_internal.py` & `esgcet-5.2.0rc2/esgcet/pub_internal.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/publish_script.py` & `esgcet-5.2.0rc2/esgcet/publish_script.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/search_check.py` & `esgcet-5.2.0rc2/esgcet/search_check.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet/settings.py` & `esgcet-5.2.0rc2/esgcet/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 DRS = { 'cmip6' : [ 'mip_era' , 'activity_drs','institution_id','source_id','experiment_id','member_id','table_id','variable_id','grid_label'],
          'e3sm' : [ 'source', 'model_version', 'experiment', 'grid_resolution', 'realm', 'regridding', 'data_type', 'time_frequency', 'ensemble_member'],
     'input4mips' : ['activity_id', 'mip_era', 'target_mip', 'institution_id', 'source_id', 'realm', 'frequency', 'variable_id', 'grid_label'],
     'cordex' : ['project', 'product', 'domain', 'institute', 'driving_model', 'experiment', 'ensemble', 'rcm_model', 'rcm_version', 'time_frequency', 'variable' ],
     'create-ip-exp' : ['project', 'product', 'institute', 'experiment', 'realm', 'time_frequency'],
     'create-ip-src': ['project', 'product', 'institute', 'source_id', 'realm', 'time_frequency'],
     'create-ip-model': ['project', 'product', 'institute', 'model', 'source_id', 'realm', 'time_frequency'],
+    'create-ip-var': ['project', 'product', 'institute', 'model', 'source_id', 'time_frequency', 'realm', 'variable'],
         'cmip5' : ['project', 'product', 'institute', 'model', 'experiment', 'realm', 'time_frequency',  'ensemble']}
 
 SPLIT_FACET = { 'e3sm' : { 'delim' : '_' , 'facet' : 'grid_resolution', 0 : ''}  }
 
 # Global attributes expected to be read for a particular project.  For now a simple list.  
 GA = { 'cmip6' : ['frequency',
                      'realm',
```

### Comparing `esgcet-5.1.0b13/esgcet/unpublish.py` & `esgcet-5.2.0rc2/esgcet/unpublish.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 from esgcet.search_check import ESGSearchCheck
 
 
 import esgcet.logger as logger
 
 log = logger.Logger()
 
-
-
 def check_for_pid_proj(dset_arr):
 
     for dset in dset_arr:
 
         parts = dset.split('.')
         if parts[0].lower() in ["cmip6", "input4mips"]:
             return True            
 
     return False
 
 
 def run(args):
 
     hostname = args["index_node"]
+    data_node = args["data_node"]
     verbose = args["verbose"]    
     silent = args["silent"]
-    
+    auth = args["auth"]
+    cert_fn = args["cert"]
+    do_delete = args["delete"]
+
     pub_log = log.return_logger('Unpublish', args["silent"], args["verbose"])
     searchcheck = ESGSearchCheck(hostname, silent, verbose)
     status = 0
 
     for dset_id in args["dataset_id_lst"]:
 
         status += single_unpublish(dset_id, args, pub_log, searchcheck)
```

### Comparing `esgcet-5.1.0b13/esgcet/update.py` & `esgcet-5.2.0rc2/esgcet/update.py`

 * *Files identical despite different names*

### Comparing `esgcet-5.1.0b13/esgcet.egg-info/SOURCES.txt` & `esgcet-5.2.0rc2/esgcet.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,24 @@
 esgcet/esgmigrate.py
 esgcet/esgmkpubrec.py
 esgcet/esgpidcitepub.py
 esgcet/esgunpublish.py
 esgcet/esgupdate.py
 esgcet/generic_netcdf.py
 esgcet/generic_pub.py
+esgcet/handler_base.py
 esgcet/index_pub.py
 esgcet/input4mips.py
 esgcet/list2json.py
 esgcet/logger.py
 esgcet/mapfile.py
 esgcet/migratecmd.py
 esgcet/mk_dataset.py
+esgcet/mk_dataset_autoc.py
+esgcet/mk_dataset_xarray.py
 esgcet/mkd_cmip5.py
 esgcet/mkd_create_ip.py
 esgcet/mkd_input4mips.py
 esgcet/mkd_non_nc.py
 esgcet/pid_cite_pub.py
 esgcet/pub_client.py
 esgcet/pub_internal.py
```

