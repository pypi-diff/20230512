# Comparing `tmp/nodeenv-1.6.0.tar.gz` & `tmp/nodeenv-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nodeenv-1.6.0.tar", last modified: Fri Apr  9 08:13:07 2021, max compression
+gzip compressed data, was "dist/nodeenv-1.7.0.tar", last modified: Sat Jun 25 15:38:10 2022, max compression
```

## Comparing `nodeenv-1.6.0.tar` & `nodeenv-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 kev       (1000) kev       (1000)        0 2021-04-09 08:13:07.000000 nodeenv-1.6.0/
--rw-r--r--   0 kev       (1000) kev       (1000)      216 2018-11-06 10:53:27.000000 nodeenv-1.6.0/MANIFEST.in
-drwxr-xr-x   0 kev       (1000) kev       (1000)        0 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/
--rw-r--r--   0 kev       (1000) kev       (1000)        8 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/top_level.txt
--rw-r--r--   0 kev       (1000) kev       (1000)      468 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/SOURCES.txt
--rw-r--r--   0 kev       (1000) kev       (1000)        1 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/dependency_links.txt
--rw-r--r--   0 kev       (1000) kev       (1000)    27573 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/PKG-INFO
--rw-r--r--   0 kev       (1000) kev       (1000)        1 2018-11-06 10:53:39.000000 nodeenv-1.6.0/nodeenv.egg-info/not-zip-safe
--rw-r--r--   0 kev       (1000) kev       (1000)       42 2021-04-09 08:13:07.000000 nodeenv-1.6.0/nodeenv.egg-info/entry_points.txt
--rw-r--r--   0 kev       (1000) kev       (1000)     7274 2020-08-23 18:10:51.000000 nodeenv-1.6.0/README
--rw-r--r--   0 kev       (1000) kev       (1000)     4557 2020-08-23 18:11:31.000000 nodeenv-1.6.0/Makefile
--rw-r--r--   0 kev       (1000) kev       (1000)    13332 2019-11-19 07:27:42.000000 nodeenv-1.6.0/CHANGES
--rw-r--r--   0 kev       (1000) kev       (1000)     7274 2020-08-23 18:10:51.000000 nodeenv-1.6.0/README.rst
--rw-r--r--   0 kev       (1000) kev       (1000)     6421 2018-11-06 10:53:27.000000 nodeenv-1.6.0/README.ru.rst
--rwxr-xr-x   0 kev       (1000) kev       (1000)    44896 2021-04-09 08:09:38.000000 nodeenv-1.6.0/nodeenv.py
-drwxr-xr-x   0 kev       (1000) kev       (1000)        0 2021-04-09 08:13:07.000000 nodeenv-1.6.0/debian-upstream/
--rw-r--r--   0 kev       (1000) kev       (1000)       53 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/nodeenv.links
--rw-r--r--   0 kev       (1000) kev       (1000)      345 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/nodeenv.triggers
--rw-r--r--   0 kev       (1000) kev       (1000)      752 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/control
--rw-r--r--   0 kev       (1000) kev       (1000)        2 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/compat
--rw-r--r--   0 kev       (1000) kev       (1000)     1532 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/copyright
--rwxr-xr-x   0 kev       (1000) kev       (1000)      937 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/rules
--rw-r--r--   0 kev       (1000) kev       (1000)     1392 2018-11-06 10:53:27.000000 nodeenv-1.6.0/debian-upstream/changelog
--rw-r--r--   0 kev       (1000) kev       (1000)     1532 2018-11-06 10:53:27.000000 nodeenv-1.6.0/LICENSE
--rw-r--r--   0 kev       (1000) kev       (1000)     1443 2021-04-09 08:10:57.000000 nodeenv-1.6.0/AUTHORS
--rw-r--r--   0 kev       (1000) kev       (1000)    27573 2021-04-09 08:13:07.000000 nodeenv-1.6.0/PKG-INFO
--rw-r--r--   0 kev       (1000) kev       (1000)     1796 2019-11-19 07:28:36.000000 nodeenv-1.6.0/setup.py
--rw-r--r--   0 kev       (1000) kev       (1000)       38 2021-04-09 08:13:07.000000 nodeenv-1.6.0/setup.cfg
+drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    27641 2022-06-25 15:38:10.000000 nodeenv-1.7.0/PKG-INFO
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1532 2022-04-21 19:26:06.000000 nodeenv-1.7.0/LICENSE
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1494 2022-06-25 15:33:52.000000 nodeenv-1.7.0/AUTHORS
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     4482 2022-06-25 15:30:36.000000 nodeenv-1.7.0/Makefile
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    13332 2022-04-21 19:26:06.000000 nodeenv-1.7.0/CHANGES
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      216 2022-04-21 19:26:06.000000 nodeenv-1.7.0/MANIFEST.in
+drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/debian-upstream/
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        2 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/compat
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1392 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/changelog
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       53 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/nodeenv.links
+-rwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)      937 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/rules
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1532 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/copyright
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      345 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/nodeenv.triggers
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      752 2022-04-21 19:26:06.000000 nodeenv-1.7.0/debian-upstream/control
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     7339 2022-06-25 14:04:36.000000 nodeenv-1.7.0/README
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     1819 2022-04-21 19:26:06.000000 nodeenv-1.7.0/setup.py
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    45789 2022-06-25 14:31:47.000000 nodeenv-1.7.0/nodeenv.py
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       38 2022-06-25 15:38:10.000000 nodeenv-1.7.0/setup.cfg
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     7339 2022-06-25 14:04:36.000000 nodeenv-1.7.0/README.rst
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)     6421 2022-04-21 19:26:06.000000 nodeenv-1.7.0/README.ru.rst
+drwxr-xr-x   0 shorrty  (783510019) LD\Domain Users (593637566)        0 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)    27641 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/PKG-INFO
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        1 2022-06-25 15:21:40.000000 nodeenv-1.7.0/nodeenv.egg-info/not-zip-safe
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)      498 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/SOURCES.txt
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       42 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/entry_points.txt
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)       11 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/requires.txt
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        8 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/top_level.txt
+-rw-r--r--   0 shorrty  (783510019) LD\Domain Users (593637566)        1 2022-06-25 15:38:10.000000 nodeenv-1.7.0/nodeenv.egg-info/dependency_links.txt
```

### Comparing `nodeenv-1.6.0/nodeenv.egg-info/PKG-INFO` & `nodeenv-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: nodeenv
-Version: 1.6.0
+Version: 1.7.0
 Summary: Node.js virtual environment builder
 Home-page: https://github.com/ekalinin/nodeenv
 Author: Eugene Kalinin
 Author-email: e.v.kalinin@gmail.com
 License: BSD
 Description: Node.js virtual environment
         ===========================
@@ -79,15 +79,15 @@
         
         Dependency
         ----------
         
         For nodeenv
         ^^^^^^^^^^^
         
-        * python (2.6+, 3.3+, or pypy)
+        * python (2.6+, 3.5+, or pypy)
         * make
         * tail
         
         For node.js
         ^^^^^^^^^^^
         
         * libssl-dev
@@ -134,15 +134,15 @@
             0.2.1   0.2.2   0.2.3   0.2.4   0.2.5   0.2.6   0.3.0
             0.3.2   0.3.3   0.3.4   0.3.5   0.3.6   0.3.7   0.3.8
             0.4.1   0.4.2   0.4.3   0.4.4   0.4.5   0.4.6
         
         Install node.js "0.4.3" without ssl support with 4 parallel commands 
         for compilation and npm.js "0.3.17"::
         
-            $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --jobs=4 env-4.3
+            $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --with-npm --jobs=4 env-4.3
         
         Install node.js from the source::
         
             $ nodeenv --node=0.10.25 --source env-0.10.25
         
         Install node.js from a mirror::
         
@@ -246,23 +246,25 @@
         -------------
         You can use the INI-style file ``~/.nodeenvrc`` to set default values for many options,
         the keys in that file are the long command-line option names.
         
         These are the available options and their defaults::
         
             [nodeenv]
-            debug = False
-            jobs = 2
-            make = make
-            node = latest
-            npm = latest
-            prebuilt = False
-            profile = False
+            node = 'latest'
+            npm = 'latest'
             with_npm = False
+            jobs = '2'
             without_ssl = False
+            debug = False
+            profile = False
+            make = 'make'
+            prebuilt = True
+            ignore_ssl_certs = False
+            mirror = None
         
         Alternatives
         ------------
         
         There are several alternatives that create isolated environments:
         
         * `nave <https://github.com/isaacs/nave>`_ - Virtual Environments for Node.
@@ -740,23 +742,22 @@
         
         Version 0.3.0
         --------------
         
         - Renamed nve to nodeenv
         
 Platform: any
-Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*
```

### Comparing `nodeenv-1.6.0/README` & `nodeenv-1.7.0/README`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 Dependency
 ----------
 
 For nodeenv
 ^^^^^^^^^^^
 
-* python (2.6+, 3.3+, or pypy)
+* python (2.6+, 3.5+, or pypy)
 * make
 * tail
 
 For node.js
 ^^^^^^^^^^^
 
 * libssl-dev
@@ -126,15 +126,15 @@
     0.2.1   0.2.2   0.2.3   0.2.4   0.2.5   0.2.6   0.3.0
     0.3.2   0.3.3   0.3.4   0.3.5   0.3.6   0.3.7   0.3.8
     0.4.1   0.4.2   0.4.3   0.4.4   0.4.5   0.4.6
 
 Install node.js "0.4.3" without ssl support with 4 parallel commands 
 for compilation and npm.js "0.3.17"::
 
-    $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --jobs=4 env-4.3
+    $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --with-npm --jobs=4 env-4.3
 
 Install node.js from the source::
 
     $ nodeenv --node=0.10.25 --source env-0.10.25
 
 Install node.js from a mirror::
 
@@ -238,23 +238,25 @@
 -------------
 You can use the INI-style file ``~/.nodeenvrc`` to set default values for many options,
 the keys in that file are the long command-line option names.
 
 These are the available options and their defaults::
 
     [nodeenv]
-    debug = False
-    jobs = 2
-    make = make
-    node = latest
-    npm = latest
-    prebuilt = False
-    profile = False
+    node = 'latest'
+    npm = 'latest'
     with_npm = False
+    jobs = '2'
     without_ssl = False
+    debug = False
+    profile = False
+    make = 'make'
+    prebuilt = True
+    ignore_ssl_certs = False
+    mirror = None
 
 Alternatives
 ------------
 
 There are several alternatives that create isolated environments:
 
 * `nave <https://github.com/isaacs/nave>`_ - Virtual Environments for Node.
```

### Comparing `nodeenv-1.6.0/CHANGES` & `nodeenv-1.7.0/CHANGES`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/README.rst` & `nodeenv-1.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 Dependency
 ----------
 
 For nodeenv
 ^^^^^^^^^^^
 
-* python (2.6+, 3.3+, or pypy)
+* python (2.6+, 3.5+, or pypy)
 * make
 * tail
 
 For node.js
 ^^^^^^^^^^^
 
 * libssl-dev
@@ -126,15 +126,15 @@
     0.2.1   0.2.2   0.2.3   0.2.4   0.2.5   0.2.6   0.3.0
     0.3.2   0.3.3   0.3.4   0.3.5   0.3.6   0.3.7   0.3.8
     0.4.1   0.4.2   0.4.3   0.4.4   0.4.5   0.4.6
 
 Install node.js "0.4.3" without ssl support with 4 parallel commands 
 for compilation and npm.js "0.3.17"::
 
-    $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --jobs=4 env-4.3
+    $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --with-npm --jobs=4 env-4.3
 
 Install node.js from the source::
 
     $ nodeenv --node=0.10.25 --source env-0.10.25
 
 Install node.js from a mirror::
 
@@ -238,23 +238,25 @@
 -------------
 You can use the INI-style file ``~/.nodeenvrc`` to set default values for many options,
 the keys in that file are the long command-line option names.
 
 These are the available options and their defaults::
 
     [nodeenv]
-    debug = False
-    jobs = 2
-    make = make
-    node = latest
-    npm = latest
-    prebuilt = False
-    profile = False
+    node = 'latest'
+    npm = 'latest'
     with_npm = False
+    jobs = '2'
     without_ssl = False
+    debug = False
+    profile = False
+    make = 'make'
+    prebuilt = True
+    ignore_ssl_certs = False
+    mirror = None
 
 Alternatives
 ------------
 
 There are several alternatives that create isolated environments:
 
 * `nave <https://github.com/isaacs/nave>`_ - Virtual Environments for Node.
```

### Comparing `nodeenv-1.6.0/README.ru.rst` & `nodeenv-1.7.0/README.ru.rst`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/nodeenv.py` & `nodeenv-1.7.0/nodeenv.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sys
 import os
 import re
 import ssl
 import stat
 import logging
 import operator
-import optparse
+import argparse
 import subprocess
 import tarfile
 import pipes
 import platform
 import zipfile
 import shutil
 import sysconfig
@@ -43,15 +43,15 @@
     import urllib.request as urllib2
     iteritems = operator.methodcaller('items')
     import http
     IncompleteRead = http.client.IncompleteRead
 
 from pkg_resources import parse_version
 
-nodeenv_version = '1.6.0'
+nodeenv_version = '1.7.0'
 
 join = os.path.join
 abspath = os.path.abspath
 src_base_url = None
 
 is_PY3 = sys.version_info[0] >= 3
 is_WIN = platform.system() == 'Windows'
@@ -96,20 +96,22 @@
     jobs = '2'
     without_ssl = False
     debug = False
     profile = False
     make = 'make'
     prebuilt = True
     ignore_ssl_certs = False
+    mirror = None
 
     @classmethod
     def _load(cls, configfiles, verbose=False):
         """
         Load configuration from the given files in reverse order,
         if they exist and have a [nodeenv] section.
+        Additionally, load version from .node-version if file exists.
         """
         for configfile in reversed(configfiles):
             configfile = os.path.expanduser(configfile)
             if not os.path.exists(configfile):
                 continue
 
             ini_file = ConfigParser()
@@ -129,14 +131,18 @@
                     val = ini_file.get(section, attr)
 
                 if verbose:
                     print('CONFIG {0}: {1} = {2}'.format(
                         os.path.basename(configfile), attr, val))
                 setattr(cls, attr, val)
 
+        if os.path.exists(".node-version"):
+            with open(".node-version", "r") as v_file:
+                setattr(cls, "node", v_file.readlines(1)[0].strip())
+
     @classmethod
     def _dump(cls):
         """
         Print defaults for the README.
         """
         print("    [nodeenv]")
         print("    " + "\n    ".join(
@@ -160,24 +166,24 @@
 def remove_env_bin_from_path(env, env_bin_dir):
     """
     Remove bin directory of the current environment from PATH
     """
     return env.replace(env_bin_dir + ':', '')
 
 
-def node_version_from_opt(opt):
+def node_version_from_args(args):
     """
-    Parse the node version from the optparse options
+    Parse the node version from the argparse args
     """
-    if opt.node == 'system':
+    if args.node == 'system':
         out, err = subprocess.Popen(
             ["node", "--version"], stdout=subprocess.PIPE).communicate()
         return parse_version(clear_output(out).replace('v', ''))
 
-    return parse_version(opt.node)
+    return parse_version(args.node)
 
 
 def create_logger():
     """
     Create logger for diagnostic
     """
     # create logger
@@ -206,180 +212,190 @@
     loggr.addHandler(ch)
     return loggr
 
 
 logger = create_logger()
 
 
-def parse_args(check=True):
+def make_parser():
     """
-    Parses command line arguments.
-
-    Set `check` to False to skip validation checks.
+    Make a command line argument parser.
     """
-    parser = optparse.OptionParser(
-        version=nodeenv_version,
-        usage="%prog [OPTIONS] ENV_DIR")
+    parser = argparse.ArgumentParser(
+        usage="%(prog)s [OPTIONS] DEST_DIR")
 
-    parser.add_option(
+    parser.add_argument(
+        '--version', action='version', version=nodeenv_version)
+
+    parser.add_argument(
         '-n', '--node', dest='node', metavar='NODE_VER', default=Config.node,
         help='The node.js version to use, e.g., '
         '--node=0.4.3 will use the node-v0.4.3 '
         'to create the new environment. '
         'The default is last stable version (`latest`). '
         'Use `lts` to use the latest LTS release. '
         'Use `system` to use system-wide node.')
 
-    parser.add_option(
+    parser.add_argument(
         '--mirror',
-        action="store", dest='mirror',
+        action="store", dest='mirror', default=Config.mirror,
         help='Set mirror server of nodejs.org to download from.')
 
     if not is_WIN:
-        parser.add_option(
+        parser.add_argument(
             '-j', '--jobs', dest='jobs', default=Config.jobs,
             help='Sets number of parallel commands at node.js compilation. '
             'The default is 2 jobs.')
 
-        parser.add_option(
+        parser.add_argument(
             '--load-average', dest='load_average',
             help='Sets maximum load average for executing parallel commands '
             'at node.js compilation.')
 
-        parser.add_option(
+        parser.add_argument(
             '--without-ssl', dest='without_ssl',
             action='store_true', default=Config.without_ssl,
             help='Build node.js without SSL support')
 
-        parser.add_option(
+        parser.add_argument(
             '--debug', dest='debug',
             action='store_true', default=Config.debug,
             help='Build debug variant of the node.js')
 
-        parser.add_option(
+        parser.add_argument(
             '--profile', dest='profile',
             action='store_true', default=Config.profile,
             help='Enable profiling for node.js')
 
-        parser.add_option(
+        parser.add_argument(
             '--make', '-m', dest='make_path',
             metavar='MAKE_PATH',
             help='Path to make command',
             default=Config.make)
 
-        parser.add_option(
+        parser.add_argument(
             '--source', dest='prebuilt',
             action='store_false', default=Config.prebuilt,
             help='Install node.js from the source')
 
-    parser.add_option(
+    parser.add_argument(
         '-v', '--verbose',
         action='store_true', dest='verbose', default=False,
         help="Verbose mode")
 
-    parser.add_option(
+    parser.add_argument(
         '-q', '--quiet',
         action='store_true', dest='quiet', default=False,
         help="Quiet mode")
 
-    parser.add_option(
+    parser.add_argument(
         '-C', '--config-file', dest='config_file', default=None,
         help="Load a different file than '~/.nodeenvrc'. "
         "Pass an empty string for no config (use built-in defaults).")
 
-    parser.add_option(
+    parser.add_argument(
         '-r', '--requirements',
         dest='requirements', default='', metavar='FILENAME',
         help='Install all the packages listed in the given requirements file.')
 
-    parser.add_option(
+    parser.add_argument(
         '--prompt', dest='prompt',
         help='Provides an alternative prompt prefix for this environment')
 
-    parser.add_option(
+    parser.add_argument(
         '-l', '--list', dest='list',
         action='store_true', default=False,
         help='Lists available node.js versions')
 
-    parser.add_option(
+    parser.add_argument(
         '--update', dest='update',
         action='store_true', default=False,
         help='Install npm packages from file without node')
 
-    parser.add_option(
+    parser.add_argument(
         '--with-npm', dest='with_npm',
         action='store_true', default=Config.with_npm,
         help='Build without installing npm into the new virtual environment. '
         'Required for node.js < 0.6.3. By default, the npm included with '
         'node.js is used. Under Windows, this defaults to true.')
 
-    parser.add_option(
+    parser.add_argument(
         '--npm', dest='npm',
         metavar='NPM_VER', default=Config.npm,
         help='The npm version to use, e.g., '
         '--npm=0.3.18 will use the npm-0.3.18.tgz '
         'tarball to install. '
         'The default is last available version (`latest`).')
 
-    parser.add_option(
+    parser.add_argument(
         '--no-npm-clean', dest='no_npm_clean',
         action='store_true', default=False,
         help='Skip the npm 0.x cleanup.  Cleanup is enabled by default.')
 
-    parser.add_option(
+    parser.add_argument(
         '--python-virtualenv', '-p', dest='python_virtualenv',
         action='store_true', default=False,
         help='Use current python virtualenv')
 
-    parser.add_option(
+    parser.add_argument(
         '--clean-src', '-c', dest='clean_src',
         action='store_true', default=False,
         help='Remove "src" directory after installation')
 
-    parser.add_option(
+    parser.add_argument(
         '--force', dest='force',
         action='store_true', default=False,
         help='Force installation in a pre-existing directory')
 
-    parser.add_option(
+    parser.add_argument(
         '--prebuilt', dest='prebuilt',
         action='store_true', default=Config.prebuilt,
         help='Install node.js from prebuilt package (default)')
 
-    parser.add_option(
+    parser.add_argument(
         '--ignore_ssl_certs', dest='ignore_ssl_certs',
         action='store_true', default=Config.ignore_ssl_certs,
         help='Ignore certificates for package downloads. - UNSAFE -')
 
-    options, args = parser.parse_args()
+    parser.add_argument(
+        metavar='DEST_DIR', dest='env_dir', nargs='?',
+        help='Destination directory')
+
+    return parser
 
-    if options.config_file is None:
-        options.config_file = ["./tox.ini", "./setup.cfg", "~/.nodeenvrc"]
-    elif not options.config_file:
-        options.config_file = []
+
+def parse_args(check=True):
+    """
+    Parses command line arguments.
+
+    Set `check` to False to skip validation checks.
+    """
+    parser = make_parser()
+    args = parser.parse_args()
+
+    if args.config_file is None:
+        args.config_file = ["./tox.ini", "./setup.cfg", "~/.nodeenvrc"]
+    elif not args.config_file:
+        args.config_file = []
     else:
         # Make sure that explicitly provided files exist
-        if not os.path.exists(options.config_file):
+        if not os.path.exists(args.config_file):
             parser.error("Config file '{0}' doesn't exist!".format(
-                options.config_file))
-        options.config_file = [options.config_file]
+                args.config_file))
+        args.config_file = [args.config_file]
 
     if not check:
-        return options, args
+        return args
 
-    if not options.list and not options.python_virtualenv:
-        if not args:
+    if not args.list:
+        if not args.python_virtualenv and not args.env_dir:
             parser.error('You must provide a DEST_DIR or '
                          'use current python virtualenv')
 
-        if len(args) > 1:
-            parser.error('There must be only one argument: DEST_DIR '
-                         '(you gave: {0})'.format(' '.join(args)))
-
-    return options, args
+    return args
 
 
 def mkdir(path):
     """
     Create directory
     """
     if not os.path.exists(path):
@@ -557,15 +573,15 @@
     tf = tarfile.open(*args, **kwargs)
     try:
         yield tf
     finally:
         tf.close()
 
 
-def download_node_src(node_url, src_dir, opt):
+def download_node_src(node_url, src_dir, args):
     """
     Download source code
     """
     logger.info('.', extra=dict(continued=True))
     try:
         dl_contents = io.BytesIO(urlopen(node_url).read())
     except IncompleteRead as e:
@@ -580,15 +596,15 @@
         member_name = lambda s: s  # noqa: E731
     else:
         ctx = tarfile_open(fileobj=dl_contents)
         members = operator.methodcaller('getmembers')
         member_name = operator.attrgetter('name')
 
     with ctx as archive:
-        node_ver = re.escape(opt.node)
+        node_ver = re.escape(args.node)
         rexp_string = r"node-v%s[^/]*/(README\.md|CHANGELOG\.md|LICENSE)"\
             % node_ver
         extract_list = [
             member
             for member in members(archive)
             if re.match(rexp_string, member_name(member)) is None
         ]
@@ -596,15 +612,17 @@
 
 
 def urlopen(url):
     home_url = "https://github.com/ekalinin/nodeenv/"
     headers = {'User-Agent': 'nodeenv/%s (%s)' % (nodeenv_version, home_url)}
     req = urllib2.Request(url, None, headers)
     if ignore_ssl_certs:
-        context = ssl.SSLContext()
+        # py27: protocol required, py3: optional
+        # https://github.com/ekalinin/nodeenv/issues/296
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
         context.verify_mode = ssl.CERT_NONE
         return urllib2.urlopen(req, context=context)
     return urllib2.urlopen(req)
 
 # ---------------------------------------------------------
 # Virtual environment functions
 
@@ -652,34 +670,34 @@
             filename = join(env_dir, 'bin', filename)
             if os.path.exists(filename):
                 make_executable(filename)
 
     logger.info('.', extra=dict(continued=True))
 
 
-def build_node_from_src(env_dir, src_dir, node_src_dir, opt):
+def build_node_from_src(env_dir, src_dir, node_src_dir, args):
     env = {}
     make_param_names = ['load-average', 'jobs']
     make_param_values = map(
-        lambda x: getattr(opt, x.replace('-', '_')),
+        lambda x: getattr(args, x.replace('-', '_')),
         make_param_names)
     make_opts = [
         '--{0}={1}'.format(name, value)
         if len(value) > 0 else '--{0}'.format(name)
         for name, value in zip(make_param_names, make_param_values)
         if value is not None
     ]
 
     if getattr(sys.version_info, 'major', sys.version_info[0]) > 2:
         # Currently, the node.js build scripts are using python2.*,
         # therefore we need to temporarily point python exec to the
         # python 2.* version in this case.
         try:
             _, which_python2_output = callit(
-                ['which', 'python2'], opt.verbose, True, node_src_dir, env
+                ['which', 'python2'], args.verbose, True, node_src_dir, env
             )
             python2_path = which_python2_output[0]
         except (OSError, IndexError):
             raise OSError(
                 'Python >=3.0 virtualenv detected, but no python2 '
                 'command (required for building node.js) was found'
             )
@@ -692,109 +710,115 @@
         env['PATH'] = '{}:{}'.format(node_tmpbin_dir,
                                      os.environ.get('PATH', ''))
 
     conf_cmd = [
         './configure',
         '--prefix=%s' % pipes.quote(env_dir)
     ]
-    if opt.without_ssl:
+    if args.without_ssl:
         conf_cmd.append('--without-ssl')
-    if opt.debug:
+    if args.debug:
         conf_cmd.append('--debug')
-    if opt.profile:
+    if args.profile:
         conf_cmd.append('--profile')
 
-    make_cmd = opt.make_path
+    make_cmd = args.make_path
 
-    callit(conf_cmd, opt.verbose, True, node_src_dir, env)
+    callit(conf_cmd, args.verbose, True, node_src_dir, env)
     logger.info('.', extra=dict(continued=True))
-    callit([make_cmd] + make_opts, opt.verbose, True, node_src_dir, env)
+    callit([make_cmd] + make_opts, args.verbose, True, node_src_dir, env)
     logger.info('.', extra=dict(continued=True))
-    callit([make_cmd + ' install'], opt.verbose, True, node_src_dir, env)
+    callit([make_cmd + ' install'], args.verbose, True, node_src_dir, env)
 
 
-def install_node(env_dir, src_dir, opt):
+def install_node(env_dir, src_dir, args):
     """
     Download source code for node.js, unpack it
     and install it in virtual environment.
     """
     try:
-        install_node_wrapped(env_dir, src_dir, opt)
+        install_node_wrapped(env_dir, src_dir, args)
     except BaseException:
         # this restores the newline suppressed by continued=True
         logger.info('')
         raise
 
 
-def install_node_wrapped(env_dir, src_dir, opt):
+def install_node_wrapped(env_dir, src_dir, args):
     env_dir = abspath(env_dir)
-    node_src_dir = join(src_dir, to_utf8('node-v%s' % opt.node))
-    src_type = "prebuilt" if opt.prebuilt else "source"
+    node_src_dir = join(src_dir, to_utf8('node-v%s' % args.node))
+    src_type = "prebuilt" if args.prebuilt else "source"
 
-    logger.info(' * Install %s node (%s) ' % (src_type, opt.node),
+    logger.info(' * Install %s node (%s) ' % (src_type, args.node),
                 extra=dict(continued=True))
 
-    if opt.prebuilt:
-        node_url = get_node_bin_url(opt.node)
+    if args.prebuilt:
+        node_url = get_node_bin_url(args.node)
     else:
-        node_url = get_node_src_url(opt.node)
+        node_url = get_node_src_url(args.node)
 
     # get src if not downloaded yet
     if not os.path.exists(node_src_dir):
-        download_node_src(node_url, src_dir, opt)
+        try:
+            download_node_src(node_url, src_dir, args)
+        except urllib2.HTTPError:
+            if "arm64" in node_url:
+                # if arm64 not found, try x64
+                download_node_src(node_url.replace('arm64', 'x64'),
+                                  src_dir, args)
 
     logger.info('.', extra=dict(continued=True))
 
-    if opt.prebuilt:
-        copy_node_from_prebuilt(env_dir, src_dir, opt.node)
+    if args.prebuilt:
+        copy_node_from_prebuilt(env_dir, src_dir, args.node)
     else:
-        build_node_from_src(env_dir, src_dir, node_src_dir, opt)
+        build_node_from_src(env_dir, src_dir, node_src_dir, args)
 
     logger.info(' done.')
 
 
-def install_npm(env_dir, _src_dir, opt):
+def install_npm(env_dir, _src_dir, args):
     """
     Download source code for npm, unpack it
     and install it in virtual environment.
     """
-    logger.info(' * Install npm.js (%s) ... ' % opt.npm,
+    logger.info(' * Install npm.js (%s) ... ' % args.npm,
                 extra=dict(continued=True))
     env = dict(
         os.environ,
-        clean='no' if opt.no_npm_clean else 'yes',
-        npm_install=opt.npm,
+        clean='no' if args.no_npm_clean else 'yes',
+        npm_install=args.npm,
     )
     proc = subprocess.Popen(
         (
             'bash', '-c',
             '. {0} && npm install -g npm@{1}'.format(
                 pipes.quote(join(env_dir, 'bin', 'activate')),
-                opt.npm,
+                args.npm,
             )
         ),
         env=env,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
     )
     out, _ = proc.communicate()
-    if opt.verbose:
+    if args.verbose:
         logger.info(out)
     logger.info('done.')
 
 
-def install_npm_win(env_dir, src_dir, opt):
+def install_npm_win(env_dir, src_dir, args):
     """
     Download source code for npm, unpack it
     and install it in virtual environment.
     """
-    logger.info(' * Install npm.js (%s) ... ' % opt.npm,
+    logger.info(' * Install npm.js (%s) ... ' % args.npm,
                 extra=dict(continued=True))
-    npm_url = 'https://github.com/npm/cli/archive/v%s.zip' % opt.npm
+    npm_url = 'https://github.com/npm/cli/archive/v%s.zip' % args.npm
     npm_contents = io.BytesIO(urlopen(npm_url).read())
 
     bin_path = join(env_dir, 'Scripts')
     node_modules_path = join(bin_path, 'node_modules', 'npm')
 
     if os.path.exists(node_modules_path):
         shutil.rmtree(node_modules_path)
@@ -804,59 +828,59 @@
 
     if os.path.exists(join(bin_path, 'npm-cli.js')):
         os.remove(join(bin_path, 'npm-cli.js'))
 
     with zipfile.ZipFile(npm_contents, 'r') as zipf:
         zipf.extractall(src_dir)
 
-    npm_ver = 'cli-%s' % opt.npm
+    npm_ver = 'cli-%s' % args.npm
     shutil.copytree(join(src_dir, npm_ver), node_modules_path)
     shutil.copy(join(src_dir, npm_ver, 'bin', 'npm.cmd'),
                 join(bin_path, 'npm.cmd'))
     shutil.copy(join(src_dir, npm_ver, 'bin', 'npm-cli.js'),
                 join(bin_path, 'npm-cli.js'))
 
     if is_CYGWIN:
         shutil.copy(join(bin_path, 'npm-cli.js'),
                     join(env_dir, 'bin', 'npm-cli.js'))
         shutil.copytree(join(bin_path, 'node_modules'),
                         join(env_dir, 'bin', 'node_modules'))
         npm_gh_url = 'https://raw.githubusercontent.com/npm/cli'
-        npm_bin_url = '{}/{}/bin/npm'.format(npm_gh_url, opt.npm)
+        npm_bin_url = '{}/{}/bin/npm'.format(npm_gh_url, args.npm)
         writefile(join(env_dir, 'bin', 'npm'), urlopen(npm_bin_url).read())
 
 
-def install_packages(env_dir, opt):
+def install_packages(env_dir, args):
     """
     Install node.js packages via npm
     """
     logger.info(' * Install node.js packages ... ',
                 extra=dict(continued=True))
     packages = [package.strip() for package in
-                open(opt.requirements).readlines()]
+                open(args.requirements).readlines()]
     activate_path = join(env_dir, 'bin', 'activate')
-    real_npm_ver = opt.npm if opt.npm.count(".") == 2 else opt.npm + ".0"
-    if opt.npm == "latest" or real_npm_ver >= "1.0.0":
+    real_npm_ver = args.npm if args.npm.count(".") == 2 else args.npm + ".0"
+    if args.npm == "latest" or real_npm_ver >= "1.0.0":
         cmd = '. ' + pipes.quote(activate_path) + \
               ' && npm install -g %(pack)s'
     else:
         cmd = '. ' + pipes.quote(activate_path) + \
               ' && npm install %(pack)s' + \
               ' && npm activate %(pack)s'
 
     for package in packages:
         if not package:
             continue
         callit(cmd=[
-            cmd % {"pack": package}], show_stdout=opt.verbose, in_shell=True)
+            cmd % {"pack": package}], show_stdout=args.verbose, in_shell=True)
 
     logger.info('done.')
 
 
-def install_activate(env_dir, opt):
+def install_activate(env_dir, args):
     """
     Install virtual environment activation script
     """
     if is_WIN:
         files = {
             'activate.bat': ACTIVATE_BAT,
             "deactivate.bat": DEACTIVATE_BAT,
@@ -873,21 +897,21 @@
         }
         bin_dir = join(env_dir, 'bin')
         shim_node = join(bin_dir, "node")
         shim_nodejs = join(bin_dir, "nodejs")
     if is_CYGWIN:
         mkdir(bin_dir)
 
-    if opt.node == "system":
+    if args.node == "system":
         files["node"] = SHIM
 
     mod_dir = join('lib', 'node_modules')
-    prompt = opt.prompt or '(%s)' % os.path.basename(os.path.abspath(env_dir))
+    prompt = args.prompt or '(%s)' % os.path.basename(os.path.abspath(env_dir))
 
-    if opt.node == "system":
+    if args.node == "system":
         env = os.environ.copy()
         env.update({'PATH': remove_env_bin_from_path(env['PATH'], bin_dir)})
         for candidate in ("nodejs", "node"):
             which_node_output, _ = subprocess.Popen(
                 ["which", candidate],
                 stdout=subprocess.PIPE, env=env).communicate()
             shim_node = clear_output(which_node_output)
@@ -911,18 +935,18 @@
         else:
             content = content.replace('__NPM_CONFIG_PREFIX__',
                                       '$NODE_VIRTUAL_ENV')
         # if we call in the same environment:
         #   $ nodeenv -p --prebuilt
         #   $ nodeenv -p --node=system
         # we should get `bin/node` not as binary+string.
-        # `bin/activate` should be appended if we inside
+        # `bin/activate` should be appended if we're inside
         # existing python's virtual environment
         need_append = False
-        if opt.python_virtualenv:
+        if args.python_virtualenv:
             disable_prompt = DISABLE_PROMPT.get(name, '')
             enable_prompt = ENABLE_PROMPT.get(name, '')
             content = disable_prompt + content + enable_prompt
             need_append = bool(disable_prompt)
         writefile(file_path, content, append=need_append)
 
     if not os.path.exists(shim_nodejs):
@@ -937,44 +961,44 @@
 
 def set_predeactivate_hook(env_dir):
     if not is_WIN:
         with open(join(env_dir, 'bin', 'predeactivate'), 'a') as hook:
             hook.write(PREDEACTIVATE_SH)
 
 
-def create_environment(env_dir, opt):
+def create_environment(env_dir, args):
     """
     Creates a new environment in ``env_dir``.
     """
-    if os.path.exists(env_dir) and not opt.python_virtualenv:
+    if os.path.exists(env_dir) and not args.python_virtualenv:
         logger.info(' * Environment already exists: %s', env_dir)
-        if not opt.force:
+        if not args.force:
             sys.exit(2)
     src_dir = to_utf8(abspath(join(env_dir, 'src')))
     mkdir(src_dir)
 
-    if opt.node != "system":
-        install_node(env_dir, src_dir, opt)
+    if args.node != "system":
+        install_node(env_dir, src_dir, args)
     else:
         mkdir(join(env_dir, 'bin'))
         mkdir(join(env_dir, 'lib'))
         mkdir(join(env_dir, 'lib', 'node_modules'))
     # activate script install must be
     # before npm install, npm use activate
     # for install
-    install_activate(env_dir, opt)
-    if node_version_from_opt(opt) < parse_version("0.6.3") or opt.with_npm:
+    install_activate(env_dir, args)
+    if node_version_from_args(args) < parse_version("0.6.3") or args.with_npm:
         instfunc = install_npm_win if is_WIN or is_CYGWIN else install_npm
-        instfunc(env_dir, src_dir, opt)
-    if opt.requirements:
-        install_packages(env_dir, opt)
-    if opt.python_virtualenv:
+        instfunc(env_dir, src_dir, args)
+    if args.requirements:
+        install_packages(env_dir, args)
+    if args.python_virtualenv:
         set_predeactivate_hook(env_dir)
     # Cleanup
-    if opt.clean_src:
+    if args.clean_src:
         shutil.rmtree(src_dir)
 
 
 def _get_versions_json():
     response = urlopen('%s/index.json' % src_base_url)
     return json.loads(response.read().decode('UTF-8'))
 
@@ -1002,85 +1026,86 @@
     return _get_versions_json()[0]['version'].lstrip('v')
 
 
 def get_last_lts_node_version():
     """
     Return the last node.js version marked as LTS
     """
-    return next((v['version'].lstrip('v') for v in _get_versions_json() if v['lts']), None)
+    return next((v['version'].lstrip('v')
+                 for v in _get_versions_json() if v['lts']), None)
 
 
-def get_env_dir(opt, args):
-    if opt.python_virtualenv:
+def get_env_dir(args):
+    if args.python_virtualenv:
         if hasattr(sys, 'real_prefix'):
             res = sys.prefix
         elif hasattr(sys, 'base_prefix') and sys.base_prefix != sys.prefix:
             res = sys.prefix
         elif 'CONDA_PREFIX' in os.environ:
             res = sys.prefix
         else:
             logger.error('No python virtualenv is available')
             sys.exit(2)
     else:
-        res = args[0]
+        res = args.env_dir
     return to_utf8(res)
 
 
 # noinspection PyProtectedMember
 def main():
     """
     Entry point
     """
     # quick&dirty way to help update the README
     if "--dump-config-defaults" in sys.argv:
         Config._dump()
         return
 
-    opt, args = parse_args(check=False)
+    args = parse_args(check=False)
     # noinspection PyProtectedMember
-    Config._load(opt.config_file, opt.verbose)
+    Config._load(args.config_file, args.verbose)
 
-    opt, args = parse_args()
+    args = parse_args()
 
-    if opt.node.lower() == 'system' and is_WIN:
+    if args.node.lower() == 'system' and is_WIN:
         logger.error('Installing system node.js on win32 is not supported!')
         exit(1)
 
     global src_base_url
     global ignore_ssl_certs
 
-    ignore_ssl_certs = opt.ignore_ssl_certs
+    ignore_ssl_certs = args.ignore_ssl_certs
 
     src_domain = None
-    if opt.mirror:
-        if '://' in opt.mirror:
-            src_base_url = opt.mirror
+    if args.mirror:
+        if '://' in args.mirror:
+            src_base_url = args.mirror
         else:
-            src_domain = opt.mirror
+            src_domain = args.mirror
     # use unofficial builds only if musl and no explicitly chosen mirror
     elif is_x86_64_musl():
         src_domain = 'unofficial-builds.nodejs.org'
     else:
         src_domain = 'nodejs.org'
     if src_base_url is None:
         src_base_url = 'https://%s/download/release' % src_domain
 
-    if not opt.node or opt.node.lower() == 'latest':
-        opt.node = get_last_stable_node_version()
-    elif opt.node.lower() == 'lts':
-        opt.node = get_last_lts_node_version()
+    if not args.node or args.node.lower() == 'latest':
+        args.node = get_last_stable_node_version()
+    elif args.node.lower() == 'lts':
+        args.node = get_last_lts_node_version()
 
-    if opt.list:
+    if args.list:
         print_node_versions()
-    elif opt.update:
-        env_dir = get_env_dir(opt, args)
-        install_packages(env_dir, opt)
+    elif args.update:
+        env_dir = get_env_dir(args)
+        install_packages(env_dir, args)
     else:
-        env_dir = get_env_dir(opt, args)
-        create_environment(env_dir, opt)
+        env_dir = get_env_dir(args)
+        create_environment(env_dir, args)
 
 
 # ---------------------------------------------------------
 # Shell scripts content
 
 DISABLE_PROMPT = {
     'activate': """
@@ -1370,16 +1395,16 @@
     if test -n "$_OLD_NODE_FISH_PROMPT_OVERRIDE"
         # Set an empty local `$fish_function_path` to allow the removal of
         # `fish_prompt` using `functions -e`.
         set -l fish_function_path
 
         # Erase virtualenv's `fish_prompt` and restore the original.
         functions -e fish_prompt
-        functions -c _old_fish_prompt fish_prompt
-        functions -e _old_fish_prompt
+        functions -c _node_old_fish_prompt fish_prompt
+        functions -e _node_old_fish_prompt
         set -e _OLD_NODE_FISH_PROMPT_OVERRIDE
     end
 
     set -e NODE_VIRTUAL_ENV
 
     if test (count $argv) = 0 -o "$argv[1]" != "nondestructive"
         # Self destruct!
@@ -1446,16 +1471,16 @@
 
 if set -q npm_config_prefix
     set -gx _OLD_npm_config_prefix $npm_config_prefix
 end
 set -gx npm_config_prefix "__NPM_CONFIG_PREFIX__"
 
 if test -z "$NODE_VIRTUAL_ENV_DISABLE_PROMPT"
-    # Copy the current `fish_prompt` function as `_old_fish_prompt`.
-    functions -c fish_prompt _old_fish_prompt
+    # Copy the current `fish_prompt` function as `_node_old_fish_prompt`.
+    functions -c fish_prompt _node_old_fish_prompt
 
     function fish_prompt
         # Save the current $status, for fish_prompts that display it.
         set -l old_status $status
 
         # Prompt override provided?
         # If not, just prepend the environment name.
```

### Comparing `nodeenv-1.6.0/debian-upstream/control` & `nodeenv-1.7.0/debian-upstream/control`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/debian-upstream/copyright` & `nodeenv-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/debian-upstream/rules` & `nodeenv-1.7.0/debian-upstream/rules`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/debian-upstream/changelog` & `nodeenv-1.7.0/debian-upstream/changelog`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/LICENSE` & `nodeenv-1.7.0/debian-upstream/copyright`

 * *Files identical despite different names*

### Comparing `nodeenv-1.6.0/PKG-INFO` & `nodeenv-1.7.0/nodeenv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: nodeenv
-Version: 1.6.0
+Version: 1.7.0
 Summary: Node.js virtual environment builder
 Home-page: https://github.com/ekalinin/nodeenv
 Author: Eugene Kalinin
 Author-email: e.v.kalinin@gmail.com
 License: BSD
 Description: Node.js virtual environment
         ===========================
@@ -79,15 +79,15 @@
         
         Dependency
         ----------
         
         For nodeenv
         ^^^^^^^^^^^
         
-        * python (2.6+, 3.3+, or pypy)
+        * python (2.6+, 3.5+, or pypy)
         * make
         * tail
         
         For node.js
         ^^^^^^^^^^^
         
         * libssl-dev
@@ -134,15 +134,15 @@
             0.2.1   0.2.2   0.2.3   0.2.4   0.2.5   0.2.6   0.3.0
             0.3.2   0.3.3   0.3.4   0.3.5   0.3.6   0.3.7   0.3.8
             0.4.1   0.4.2   0.4.3   0.4.4   0.4.5   0.4.6
         
         Install node.js "0.4.3" without ssl support with 4 parallel commands 
         for compilation and npm.js "0.3.17"::
         
-            $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --jobs=4 env-4.3
+            $ nodeenv --without-ssl --node=0.4.3 --npm=0.3.17 --with-npm --jobs=4 env-4.3
         
         Install node.js from the source::
         
             $ nodeenv --node=0.10.25 --source env-0.10.25
         
         Install node.js from a mirror::
         
@@ -246,23 +246,25 @@
         -------------
         You can use the INI-style file ``~/.nodeenvrc`` to set default values for many options,
         the keys in that file are the long command-line option names.
         
         These are the available options and their defaults::
         
             [nodeenv]
-            debug = False
-            jobs = 2
-            make = make
-            node = latest
-            npm = latest
-            prebuilt = False
-            profile = False
+            node = 'latest'
+            npm = 'latest'
             with_npm = False
+            jobs = '2'
             without_ssl = False
+            debug = False
+            profile = False
+            make = 'make'
+            prebuilt = True
+            ignore_ssl_certs = False
+            mirror = None
         
         Alternatives
         ------------
         
         There are several alternatives that create isolated environments:
         
         * `nave <https://github.com/isaacs/nave>`_ - Virtual Environments for Node.
@@ -740,23 +742,22 @@
         
         Version 0.3.0
         --------------
         
         - Renamed nve to nodeenv
         
 Platform: any
-Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*
```

