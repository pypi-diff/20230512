# Comparing `tmp/btecli-1.6.4.tar.gz` & `tmp/btecli-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btecli-1.6.4.tar", last modified: Fri May 12 18:27:41 2023, max compression
+gzip compressed data, was "btecli-1.6.5.tar", last modified: Fri May 12 18:44:42 2023, max compression
```

## Comparing `btecli-1.6.4.tar` & `btecli-1.6.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.468907 btecli-1.6.4/
--rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.6.4/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.6.4/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:27:41.468563 btecli-1.6.4/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.6.4/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.456501 btecli-1.6.4/btecli/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    10889 2023-05-12 18:26:58.000000 btecli-1.6.4/btecli/cli.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.459096 btecli-1.6.4/btecli/lib/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.460121 btecli-1.6.4/btecli/lib/cryptography/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/cryptography/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/cryptography/aes.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/cryptography/wincred.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.460584 btecli-1.6.4/btecli/lib/defaults/
--rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/defaults/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.461097 btecli-1.6.4/btecli/lib/dictutils/
--rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.6.4/btecli/lib/dictutils/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.461642 btecli-1.6.4/btecli/lib/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.462321 btecli-1.6.4/btecli/lib/input/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/input/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/input/streams.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.462783 btecli-1.6.4/btecli/lib/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.463444 btecli-1.6.4/btecli/lib/options/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/options/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/options/mexclusive.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.465066 btecli-1.6.4/btecli/lib/plugin/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/plugin/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3247 2023-05-11 01:05:54.000000 btecli-1.6.4/btecli/lib/plugin/finder.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2009 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/plugin/metadata.py
--rw-r--r--   0 etejeda    (501) staff       (20)     7614 2023-05-11 11:59:34.000000 btecli-1.6.4/btecli/lib/plugin/plugins.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.465868 btecli-1.6.4/btecli/lib/proc/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/proc/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5057 2023-05-11 11:59:38.000000 btecli-1.6.4/btecli/lib/proc/local_invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.467537 btecli-1.6.4/btecli/lib/shell/
--rw-r--r--   0 etejeda    (501) staff       (20)     2453 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/shell/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/shell/bash_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.6.4/btecli/lib/shell/which.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.458769 btecli-1.6.4/btecli.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      976 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      252 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-12 18:27:41.000000 btecli-1.6.4/btecli.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.6.4/ecli.config.yaml.example
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.450137 btecli-1.6.4/resources/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:27:41.467948 btecli-1.6.4/resources/icons/
--rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.6.4/resources/icons/admin.ico
--rw-r--r--   0 etejeda    (501) staff       (20)       38 2023-05-12 18:27:41.469014 btecli-1.6.4/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.6.4/setup.iss
--rw-r--r--   0 etejeda    (501) staff       (20)     1201 2023-05-12 18:26:53.000000 btecli-1.6.4/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 18:26:48.000000 btecli-1.6.4/version.rc
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.893649 btecli-1.6.5/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.6.5/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.6.5/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:44:42.893044 btecli-1.6.5/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.6.5/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.876445 btecli-1.6.5/btecli/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    10889 2023-05-12 18:44:08.000000 btecli-1.6.5/btecli/cli.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.878984 btecli-1.6.5/btecli/lib/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.879886 btecli-1.6.5/btecli/lib/cryptography/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/cryptography/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/cryptography/aes.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/cryptography/wincred.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.880329 btecli-1.6.5/btecli/lib/defaults/
+-rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/defaults/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.880738 btecli-1.6.5/btecli/lib/dictutils/
+-rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.6.5/btecli/lib/dictutils/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.881630 btecli-1.6.5/btecli/lib/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.882679 btecli-1.6.5/btecli/lib/input/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/input/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/input/streams.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.883212 btecli-1.6.5/btecli/lib/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.884310 btecli-1.6.5/btecli/lib/options/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/options/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/options/mexclusive.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.886723 btecli-1.6.5/btecli/lib/plugin/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/plugin/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3247 2023-05-11 01:05:54.000000 btecli-1.6.5/btecli/lib/plugin/finder.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2009 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/plugin/metadata.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     7614 2023-05-11 11:59:34.000000 btecli-1.6.5/btecli/lib/plugin/plugins.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.887916 btecli-1.6.5/btecli/lib/proc/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/proc/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5057 2023-05-11 11:59:38.000000 btecli-1.6.5/btecli/lib/proc/local_invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.891403 btecli-1.6.5/btecli/lib/shell/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2453 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/shell/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/shell/bash_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.6.5/btecli/lib/shell/which.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.878676 btecli-1.6.5/btecli.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      976 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      252 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-12 18:44:42.000000 btecli-1.6.5/btecli.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.6.5/ecli.config.yaml.example
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.871610 btecli-1.6.5/resources/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 18:44:42.892216 btecli-1.6.5/resources/icons/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.6.5/resources/icons/admin.ico
+-rw-r--r--   0 etejeda    (501) staff       (20)       38 2023-05-12 18:44:42.893808 btecli-1.6.5/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.6.5/setup.iss
+-rw-r--r--   0 etejeda    (501) staff       (20)     1201 2023-05-12 18:43:50.000000 btecli-1.6.5/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 18:43:59.000000 btecli-1.6.5/version.rc
```

### Comparing `btecli-1.6.4/.gitignore` & `btecli-1.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/LICENSE` & `btecli-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/README.md` & `btecli-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/cli.py` & `btecli-1.6.5/btecli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ecli.lib.plugin import plugins
 from ecli.lib.input.streams import Streams
 from ecli.lib.dictutils import Struct
 from btconfig import Config
 
 # Private variables
 __author__ = 'Bert Tejeda'
-__version__ = '1.6.4'
+__version__ = '1.6.5'
 # Configuration Files
 config_file_name = 'ecli.config.yaml'
 # Initialize App Config
 config = Config(
     config_file_uri=config_file_name,
     default_value=default_config
 ).read()
```

### Comparing `btecli-1.6.4/btecli/lib/cryptography/aes.py` & `btecli-1.6.5/btecli/lib/cryptography/aes.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/cryptography/wincred.py` & `btecli-1.6.5/btecli/lib/cryptography/wincred.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/formatting/__init__.py` & `btecli-1.6.5/btecli/lib/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/logger/__init__.py` & `btecli-1.6.5/btecli/lib/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/options/mexclusive.py` & `btecli-1.6.5/btecli/lib/options/mexclusive.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/plugin/finder.py` & `btecli-1.6.5/btecli/lib/plugin/finder.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/plugin/metadata.py` & `btecli-1.6.5/btecli/lib/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/plugin/plugins.py` & `btecli-1.6.5/btecli/lib/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/proc/local_invocation.py` & `btecli-1.6.5/btecli/lib/proc/local_invocation.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/shell/__init__.py` & `btecli-1.6.5/btecli/lib/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli/lib/shell/which.py` & `btecli-1.6.5/btecli/lib/shell/which.py`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/btecli.egg-info/SOURCES.txt` & `btecli-1.6.5/btecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/resources/icons/admin.ico` & `btecli-1.6.5/resources/icons/admin.ico`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/setup.iss` & `btecli-1.6.5/setup.iss`

 * *Files identical despite different names*

### Comparing `btecli-1.6.4/setup.py` & `btecli-1.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 if '--show-packages' in ' '.join(sys.argv):
     for p in required_packages:
         print(p.split('=')[0])
     sys.exit()    
 
 setup(
     name='btecli',
-    version='1.6.4',
+    version='1.6.5',
     packages=find_packages(),
     include_package_data=True,
     install_requires=required_packages,
     package_data={'': extra_files},
     entry_points='''
         [core_package.cli_plugins]
         [console_scripts]
```

### Comparing `btecli-1.6.4/version.rc` & `btecli-1.6.5/version.rc`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 VSVersionInfo(
     ffi=FixedFileInfo(
-    filevers=(1, 6, 4, 0),
-    prodvers=(1, 6, 4, 0),
+    filevers=(1, 6, 5, 0),
+    prodvers=(1, 6, 5, 0),
     mask=0x3f,
     flags=0x0,
     OS=0x40004,
     fileType=0x1,
     subtype=0x0,
     date=(0, 0)),
     kids=[StringFileInfo([StringTable(
     u'040904B0',
     [StringStruct(u'FileDescription', u'ecli'),
-    StringStruct(u'FileVersion', u'1.6.4'),
+    StringStruct(u'FileVersion', u'1.6.5'),
     StringStruct(u'InternalName', u'ecli'),
     StringStruct(u'LegalCopyright', u''),
     StringStruct(u'OriginalFilename', u'ecli'),
     StringStruct(u'ProductName', u'Extensible Command-line'),
-    StringStruct(u'ProductVersion', u'1.6.4'),
+    StringStruct(u'ProductVersion', u'1.6.5'),
     StringStruct(u'Language', u'Language Neutral'),
     StringStruct(u'LegalTrademarks', u'')])]), 
     VarFileInfo([VarStruct(u'Translation', [1033, 1200])])]
 )
```

