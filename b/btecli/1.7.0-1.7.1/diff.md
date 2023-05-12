# Comparing `tmp/btecli-1.7.0.tar.gz` & `tmp/btecli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btecli-1.7.0.tar", last modified: Fri May 12 18:56:13 2023, max compression
+gzip compressed data, was "btecli-1.7.1.tar", last modified: Fri May 12 20:58:43 2023, max compression
```

## Comparing `btecli-1.7.0.tar` & `btecli-1.7.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.651691 btecli-1.7.0/
--rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.7.0/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.7.0/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:56:13.651221 btecli-1.7.0/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.7.0/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.638698 btecli-1.7.0/btecli/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    10909 2023-05-12 18:55:02.000000 btecli-1.7.0/btecli/cli.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.640884 btecli-1.7.0/btecli/lib/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.641851 btecli-1.7.0/btecli/lib/cryptography/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/cryptography/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/cryptography/aes.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/cryptography/wincred.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.642311 btecli-1.7.0/btecli/lib/defaults/
--rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/defaults/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.642921 btecli-1.7.0/btecli/lib/dictutils/
--rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.7.0/btecli/lib/dictutils/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.643613 btecli-1.7.0/btecli/lib/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.644367 btecli-1.7.0/btecli/lib/input/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/input/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/input/streams.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.644787 btecli-1.7.0/btecli/lib/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.645452 btecli-1.7.0/btecli/lib/options/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/options/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/options/mexclusive.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.647283 btecli-1.7.0/btecli/lib/plugin/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/plugin/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-1.7.0/btecli/lib/plugin/finder.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-1.7.0/btecli/lib/plugin/metadata.py
--rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-1.7.0/btecli/lib/plugin/plugins.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.648143 btecli-1.7.0/btecli/lib/proc/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/proc/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5063 2023-05-12 18:51:53.000000 btecli-1.7.0/btecli/lib/proc/local_invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.649679 btecli-1.7.0/btecli/lib/shell/
--rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-1.7.0/btecli/lib/shell/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/shell/bash_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.7.0/btecli/lib/shell/which.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.640575 btecli-1.7.0/btecli.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      976 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      252 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-12 18:56:13.000000 btecli-1.7.0/btecli.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.7.0/ecli.config.yaml.example
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.632439 btecli-1.7.0/resources/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:56:13.650329 btecli-1.7.0/resources/icons/
--rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.7.0/resources/icons/admin.ico
--rw-r--r--   0 etejeda    (501) staff       (20)       38 2023-05-12 18:56:13.651909 btecli-1.7.0/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.7.0/setup.iss
--rw-r--r--   0 etejeda    (501) staff       (20)     1201 2023-05-12 18:55:10.000000 btecli-1.7.0/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 18:55:33.000000 btecli-1.7.0/version.rc
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.069913 btecli-1.7.1/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.7.1/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.7.1/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 20:58:43.069570 btecli-1.7.1/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.7.1/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.057683 btecli-1.7.1/btecli/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    10909 2023-05-12 20:58:36.000000 btecli-1.7.1/btecli/cli.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.059918 btecli-1.7.1/btecli/lib/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.060887 btecli-1.7.1/btecli/lib/cryptography/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/aes.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/cryptography/wincred.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.061346 btecli-1.7.1/btecli/lib/defaults/
+-rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/defaults/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.061832 btecli-1.7.1/btecli/lib/dictutils/
+-rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.7.1/btecli/lib/dictutils/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.062399 btecli-1.7.1/btecli/lib/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.063063 btecli-1.7.1/btecli/lib/input/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/input/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/input/streams.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.063467 btecli-1.7.1/btecli/lib/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.064097 btecli-1.7.1/btecli/lib/options/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/options/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/options/mexclusive.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.065987 btecli-1.7.1/btecli/lib/plugin/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/plugin/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-1.7.1/btecli/lib/plugin/finder.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-1.7.1/btecli/lib/plugin/metadata.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-1.7.1/btecli/lib/plugin/plugins.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.066788 btecli-1.7.1/btecli/lib/proc/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/proc/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5063 2023-05-12 18:51:53.000000 btecli-1.7.1/btecli/lib/proc/local_invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.068518 btecli-1.7.1/btecli/lib/shell/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-1.7.1/btecli/lib/shell/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/shell/bash_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.7.1/btecli/lib/shell/which.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.059563 btecli-1.7.1/btecli.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      976 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      252 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-12 20:58:42.000000 btecli-1.7.1/btecli.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.7.1/ecli.config.yaml.example
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.052405 btecli-1.7.1/resources/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 20:58:43.069022 btecli-1.7.1/resources/icons/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.7.1/resources/icons/admin.ico
+-rw-r--r--   0 etejeda    (501) staff       (20)       38 2023-05-12 20:58:43.070016 btecli-1.7.1/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.7.1/setup.iss
+-rw-r--r--   0 etejeda    (501) staff       (20)     1201 2023-05-12 20:58:31.000000 btecli-1.7.1/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 20:58:25.000000 btecli-1.7.1/version.rc
```

### Comparing `btecli-1.7.0/.gitignore` & `btecli-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/LICENSE` & `btecli-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/README.md` & `btecli-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/cli.py` & `btecli-1.7.1/btecli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from btecli.lib.plugin import plugins
 from btecli.lib.input.streams import Streams
 from btecli.lib.dictutils import Struct
 from btconfig import Config
 
 # Private variables
 __author__ = 'Bert Tejeda'
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 # Configuration Files
 config_file_name = 'ecli.config.yaml'
 # Initialize App Config
 config = Config(
     config_file_uri=config_file_name,
     default_value=default_config
 ).read()
```

### Comparing `btecli-1.7.0/btecli/lib/cryptography/aes.py` & `btecli-1.7.1/btecli/lib/cryptography/aes.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/cryptography/wincred.py` & `btecli-1.7.1/btecli/lib/cryptography/wincred.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/formatting/__init__.py` & `btecli-1.7.1/btecli/lib/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/logger/__init__.py` & `btecli-1.7.1/btecli/lib/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/options/mexclusive.py` & `btecli-1.7.1/btecli/lib/options/mexclusive.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/plugin/finder.py` & `btecli-1.7.1/btecli/lib/plugin/finder.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/plugin/metadata.py` & `btecli-1.7.1/btecli/lib/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/plugin/plugins.py` & `btecli-1.7.1/btecli/lib/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/proc/local_invocation.py` & `btecli-1.7.1/btecli/lib/proc/local_invocation.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/shell/__init__.py` & `btecli-1.7.1/btecli/lib/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli/lib/shell/which.py` & `btecli-1.7.1/btecli/lib/shell/which.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/btecli.egg-info/SOURCES.txt` & `btecli-1.7.1/btecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/resources/icons/admin.ico` & `btecli-1.7.1/resources/icons/admin.ico`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/setup.iss` & `btecli-1.7.1/setup.iss`

 * *Files identical despite different names*

### Comparing `btecli-1.7.0/setup.py` & `btecli-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
 extra_files = package_files('btecli.plugins')
 
 required_packages = [
-        'btconfig>=4.4.0,<5.0.0',
+        'btconfig>=4.3.0,<5.0.0',
         'bs4>=0.0.1,<0.1.0',
         'click>=8.1.3,<9.0.0',
         'click-plugins==1.1.1',
         'colorama==0.4.3',
         'first==2.0.2',
         'jello==1.2.10',
         'lxml==4.9.1',
@@ -31,15 +31,15 @@
 if '--show-packages' in ' '.join(sys.argv):
     for p in required_packages:
         print(p.split('=')[0])
     sys.exit()    
 
 setup(
     name='btecli',
-    version='1.7.0',
+    version='1.7.1',
     packages=find_packages(),
     include_package_data=True,
     install_requires=required_packages,
     package_data={'': extra_files},
     entry_points='''
         [core_package.cli_plugins]
         [console_scripts]
```

### Comparing `btecli-1.7.0/version.rc` & `btecli-1.7.1/version.rc`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 VSVersionInfo(
     ffi=FixedFileInfo(
-    filevers=(1, 7, 0, 0),
-    prodvers=(1, 7, 0, 0),
+    filevers=(1, 7, 0, 1),
+    prodvers=(1, 7, 0, 1),
     mask=0x3f,
     flags=0x0,
     OS=0x40004,
     fileType=0x1,
     subtype=0x0,
     date=(0, 0)),
     kids=[StringFileInfo([StringTable(
     u'040904B0',
     [StringStruct(u'FileDescription', u'ecli'),
-    StringStruct(u'FileVersion', u'1.7.0'),
+    StringStruct(u'FileVersion', u'1.7.1'),
     StringStruct(u'InternalName', u'ecli'),
     StringStruct(u'LegalCopyright', u''),
     StringStruct(u'OriginalFilename', u'ecli'),
     StringStruct(u'ProductName', u'Extensible Command-line'),
-    StringStruct(u'ProductVersion', u'1.7.0'),
+    StringStruct(u'ProductVersion', u'1.7.1'),
     StringStruct(u'Language', u'Language Neutral'),
     StringStruct(u'LegalTrademarks', u'')])]), 
     VarFileInfo([VarStruct(u'Translation', [1033, 1200])])]
 )
```

