# Comparing `tmp/cellmaps_utils-0.1.0a6.tar.gz` & `tmp/cellmaps_utils-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.1.0a6.tar", last modified: Thu May 11 18:39:04 2023, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.1.0a7.tar", last modified: Thu May 11 22:07:40 2023, max compression
```

## Comparing `cellmaps_utils-0.1.0a6.tar` & `cellmaps_utils-0.1.0a7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.743704 cellmaps_utils-0.1.0a6/
--rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a6/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a6/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 18:39:04.743832 cellmaps_utils-0.1.0a6/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a6/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.736841 cellmaps_utils-0.1.0a6/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-10 17:28:17.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     3858 2023-05-11 18:35:27.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/music_utils.py
--rw-r--r--   0 churas     (504) staff       (20)    11676 2023-05-05 20:36:20.000000 cellmaps_utils-0.1.0a6/cellmaps_utils/provenance.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.738078 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       51 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-11 18:39:04.000000 cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.741841 cellmaps_utils-0.1.0a6/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.732271 cellmaps_utils-0.1.0a6/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.732383 cellmaps_utils-0.1.0a6/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.742818 cellmaps_utils-0.1.0a6/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a6/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a6/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a6/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-11 18:39:04.744266 cellmaps_utils-0.1.0a6/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1787 2023-05-05 21:20:31.000000 cellmaps_utils-0.1.0a6/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 18:39:04.743511 cellmaps_utils-0.1.0a6/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a6/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a6/tests/test_logutils.py
--rw-r--r--   0 churas     (504) staff       (20)    12542 2023-05-09 21:54:19.000000 cellmaps_utils-0.1.0a6/tests/test_provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.431299 cellmaps_utils-0.1.0a7/
+-rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a7/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a7/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 22:07:40.431436 cellmaps_utils-0.1.0a7/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a7/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.422410 cellmaps_utils-0.1.0a7/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-11 22:06:22.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     3858 2023-05-11 18:35:27.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)      234 2023-05-05 00:31:11.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/music_utils.py
+-rw-r--r--   0 churas     (504) staff       (20)    12991 2023-05-11 21:55:18.000000 cellmaps_utils-0.1.0a7/cellmaps_utils/provenance.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.423871 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     4577 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      979 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       60 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-11 22:07:40.000000 cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.429479 cellmaps_utils-0.1.0a7/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.417825 cellmaps_utils-0.1.0a7/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.417893 cellmaps_utils-0.1.0a7/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.430283 cellmaps_utils-0.1.0a7/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      838 2023-05-05 00:54:50.000000 cellmaps_utils-0.1.0a7/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a7/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-11 22:07:40.432051 cellmaps_utils-0.1.0a7/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1796 2023-05-11 20:55:28.000000 cellmaps_utils-0.1.0a7/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-11 22:07:40.431040 cellmaps_utils-0.1.0a7/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a7/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a7/tests/test_logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     7029 2023-05-11 21:02:45.000000 cellmaps_utils-0.1.0a7/tests/test_provenance.py
```

### Comparing `cellmaps_utils-0.1.0a6/CONTRIBUTING.rst` & `cellmaps_utils-0.1.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/LICENSE` & `cellmaps_utils-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/PKG-INFO` & `cellmaps_utils-0.1.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_utils
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a6/README.rst` & `cellmaps_utils-0.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils/constants.py` & `cellmaps_utils-0.1.0a7/cellmaps_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils/logutils.py` & `cellmaps_utils-0.1.0a7/cellmaps_utils/logutils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.1.0a7/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils/provenance.py` & `cellmaps_utils-0.1.0a7/cellmaps_utils/provenance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 
 import os
 import subprocess
 import logging
+import uuid
 from datetime import date
 
 from cellmaps_utils.exceptions import CellMapsProvenanceError
 logger = logging.getLogger(__name__)
 
 
 class ProvenanceUtil(object):
@@ -17,25 +18,26 @@
         Constructor
 
         :param fairscape_binary: `FAIRSCAPE <https://github.com/fairscape/fairscape-cli>`__ command line binary
         :type fairscape_binary: str
         """
         self._binary = fairscape_binary
 
-    def _run_cmd(self, cmd, timeout=360):
+    def _run_cmd(self, cmd, cwd=None, timeout=360):
         """
         Runs command as a command line process
 
         :param cmd_to_run: command to run as list
         :type cmd_to_run: list
         :return: (return code, standard out, standard error)
         :rtype: tuple
         """
-        logger.debug('Running command: ' + str(cmd))
-        p = subprocess.Popen(cmd,
+        logger.debug('Running command under ' + str(cwd) +
+                     ' path: ' + str(cmd))
+        p = subprocess.Popen(cmd, cwd=cwd,
                              stdout=subprocess.PIPE,
                              stderr=subprocess.PIPE)
         try:
             out, err = p.communicate(timeout=timeout)
         except subprocess.TimeoutExpired:
             logger.warning('Timeout reached. Killing process')
             p.kill()
@@ -76,46 +78,54 @@
                                'used-by': '?',
                                'derived-from': '?',
                                'associated-publication': '?',
                                'additional-documentation': '?'})
         return field_dict
 
     def register_rocrate(self, rocrate_path, name='',
-                         organization_name='', project_name=''):
+                         organization_name='', project_name='',
+                         guid=None):
         """
         Creates/registers rocreate in directory specified by **rocrate_path**
         Upon completion a ``ro-crate-metadata.json`` file will be created
         in the directory
 
         :param rocrate_path:
         :type rocrate_path: str
         :param name:
         :param organization_name:
         :param project_name:
         :return:
         """
-        cmd = [self._binary, 'rocrate', 'create',
+        cmd = [self._binary, 'rocrate', 'init',
                '--name', name,
                '--organization-name', organization_name,
-               '--project-name', project_name,
-               rocrate_path]
+               '--project-name', project_name]
 
-        exit_code, out_str, err_str = self._run_cmd(cmd, timeout=30)
+        if guid is None:
+            guid = str(uuid.uuid4())
+
+        cmd.append('--guid')
+        cmd.append(guid)
+
+        exit_code, out_str, err_str = self._run_cmd(cmd, cwd=rocrate_path,
+                                                    timeout=30)
         logger.debug('creation of crate stdout: ' + str(out_str))
         logger.debug('creation of crate stdout: ' + str(err_str))
         logger.debug('creation of crate exit code: ' + str(exit_code))
         if exit_code != 0:
             raise CellMapsProvenanceError('Error creating crate: ' +
                                           str(out_str) + ' : ' + str(err_str))
 
     def register_computation(self, rocrate_path, name='',
                              run_by='', command='',
                              date_created=date.today().strftime('%m-%d-%Y'),
-                             description='', used_software=[],
-                             used_dataset=[], generated=[]):
+                             description='Must be at least 10 characters', used_software=[],
+                             used_dataset=[], generated=[],
+                             guid=None):
 
         """
         Registers computation adding information to
         ``ro-crate-metadata.json`` file stored in **rocrate_path**
         directory.
 
         :param rocrate_path: Path to existing rocrate directory
@@ -136,20 +146,26 @@
                              by this computation
         :type used_dataset: list
         :param generated: list of `FAIRSCAPE <https://fairscape.github.io>`__ dataset ids for datasets
                           generated by this computation
         :type generated: list
         :return:
         """
-        cmd = [self._binary, 'rocrate', 'add', 'computation',
+        cmd = [self._binary, 'rocrate', 'register', 'computation',
                '--name', name,
                '--run-by', run_by,
                '--date-created', date_created,
                '--command', command,
                '--description', description]
+        if guid is None:
+            guid = str(uuid.uuid4())
+
+        cmd.append('--guid')
+        cmd.append(guid)
+
         if used_software is not None:
             for entry in used_software:
                 cmd.append('--used-software')
                 cmd.append(entry)
         if used_dataset is not None:
             for entry in used_dataset:
                 cmd.append('--used-dataset')
@@ -167,16 +183,19 @@
             raise CellMapsProvenanceError('Error adding dataset: ' +
                                           str(out_str) + ' : ' + str(err_str))
 
         logger.debug('add data set out_str: ' + str(out_str))
         logger.debug('add data set err_str: ' + str(err_str))
         return out_str
 
-    def register_software(self, rocrate_path, name='unknown', description='',
-                          author='', version='', file_format='', url=''):
+    def register_software(self, rocrate_path, name='unknown',
+                          description='Must be at least 10 characters',
+                          author='', version='', file_format='', url='',
+                          date_modified='01-01-1969',
+                          guid=None):
         """
         Registers software by adding information to
         ``ro-crate-metadata.json`` file stored in **rocrate_path**
         directory.
 
         .. warning::
 
@@ -197,34 +216,44 @@
         :type url: str
         :param rocrate_path: Path to directory with registered rocrate
         :type rocrate_path: str
         :raises CellMapsProvenanceError: If `FAIRSCAPE <https://fairscape.github.io>`__ call fails
         :return: guid of software from `FAIRSCAPE <https://fairscape.github.io>`__
         :rtype: str
         """
-        cmd = [self._binary, 'rocrate', 'add', 'software',
+        cmd = [self._binary, 'rocrate', 'register', 'software',
                '--name', name,
                '--description', description,
                '--author', author,
                '--version', version,
                '--file-format', file_format,
                '--url', url,
-               rocrate_path]
+               '--date-modified', date_modified]
+        if guid is None:
+            guid = str(uuid.uuid4())
+
+        cmd.append('--guid')
+        cmd.append(guid)
+
+        cmd.append('--filepath')
+        cmd.append(url)
+        cmd.append(rocrate_path)
         exit_code, out_str, err_str = self._run_cmd(cmd, timeout=30)
 
         logger.debug('add software exit code: ' + str(exit_code))
         if exit_code != 0:
             raise CellMapsProvenanceError('Error adding software: ' +
                                           str(out_str) + ' : ' + str(err_str))
         logger.debug('add software out_str: ' + str(out_str))
         logger.debug('add software err_str: ' + str(err_str))
         return out_str
 
     def register_dataset(self, rocrate_path, data_dict=None,
-                         source_file=None, skip_copy=True):
+                         source_file=None, skip_copy=True,
+                         guid=None):
         """
         Adds a dataset to existing rocrate specified by **rocrate_path**
         by adding information to ``ro-crate-metadata.json`` file
 
         Information about dataset should be specified in the **data_dict**
         dict passed in.
 
@@ -256,28 +285,45 @@
         :type source_file: str
         :param skip_copy: If ``True`` skip the copy of source file into
                           **crate_path**. Use this when source file already
                           resides in **crate_path**
         :return: id of dataset from `FAIRSCAPE <https://fairscape.github.io>`__
         :rtype: str
         """
-        cmd = [self._binary, 'rocrate', 'add', 'dataset',
+        operation_name = 'register'
+        if skip_copy is not None and skip_copy is False:
+            operation_name = 'add'
+
+        cmd = [self._binary, 'rocrate', operation_name,
+               'dataset',
                '--name', data_dict['name'],
                '--version', data_dict['version'],
                '--data-format', data_dict['data-format'],
                '--description', data_dict['description'],
                '--date-published', data_dict['date-published'],
-               '--author', data_dict['author'],
-               '--source-filepath', source_file]
+               '--author', data_dict['author']]
+
+        if guid is None:
+            guid = str(uuid.uuid4())
+
+        cmd.append('--guid')
+        cmd.append(guid)
+
         if skip_copy is not None and skip_copy is False:
+            cmd.append('--source-filepath')
+            cmd.append(source_file)
             cmd.append('--destination-filepath')
             cmd.append(os.path.join(rocrate_path,
                                     os.path.basename(source_file)))
+        else:
+            cmd.append('--filepath')
+            cmd.append(source_file)
+
         cmd.append(rocrate_path)
         exit_code, out_str, err_str = self._run_cmd(cmd, timeout=30)
-        logger.debug('add dataset exit code: ' + str(exit_code))
+        logger.debug(operation_name + ' dataset exit code: ' + str(exit_code))
         if exit_code != 0:
             raise CellMapsProvenanceError('Error adding dataset: ' +
                                           str(out_str) + ' : ' + str(err_str))
-        logger.debug('add data set out_str: ' + str(out_str))
-        logger.debug('add data set err_str: ' + str(err_str))
+        logger.debug(operation_name + ' data set out_str: ' + str(out_str))
+        logger.debug(operation_name + ' data set err_str: ' + str(err_str))
         return out_str
```

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-utils
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a6/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.1.0a7/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/Makefile` & `cellmaps_utils-0.1.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/cellmaps_utils.rst` & `cellmaps_utils-0.1.0a7/docs/cellmaps_utils.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/conf.py` & `cellmaps_utils-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/index.rst` & `cellmaps_utils-0.1.0a7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/installation.rst` & `cellmaps_utils-0.1.0a7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/make.bat` & `cellmaps_utils-0.1.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/newrelease.rst` & `cellmaps_utils-0.1.0a7/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/pypircfile.rst` & `cellmaps_utils-0.1.0a7/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/docs/versioningscheme.rst` & `cellmaps_utils-0.1.0a7/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a6/setup.py` & `cellmaps_utils-0.1.0a7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['fairscape-cli',
+requirements = ['fairscape-cli==0.1.5a1',
                 'scipy',
                 'scikit-learn',
                 'pandas',
                 'numpy',
                 'dill']
 
 setup_requirements = [ ]
```

### Comparing `cellmaps_utils-0.1.0a6/tests/test_logutils.py` & `cellmaps_utils-0.1.0a7/tests/test_logutils.py`

 * *Files identical despite different names*

