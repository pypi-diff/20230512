# Comparing `tmp/certbot-dns-netcup-1.1.4.tar.gz` & `tmp/certbot-dns-netcup-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-netcup-1.1.4.tar", last modified: Wed Apr 20 00:22:44 2022, max compression
+gzip compressed data, was "certbot-dns-netcup-1.2.0.tar", last modified: Sun Nov 27 11:15:54 2022, max compression
```

## Comparing `certbot-dns-netcup-1.1.4.tar` & `certbot-dns-netcup-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:22:44.225656 certbot-dns-netcup-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    10786 2022-04-20 00:22:30.000000 certbot-dns-netcup-1.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-04-20 00:22:30.000000 certbot-dns-netcup-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-04-20 00:22:44.225656 certbot-dns-netcup-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6451 2022-04-20 00:22:30.000000 certbot-dns-netcup-1.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:22:44.225656 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7740 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-20 00:22:44.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-04-20 00:22:30.000000 certbot-dns-netcup-1.1.4/certbot_dns_netcup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-04-20 00:22:44.225656 certbot-dns-netcup-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-04-20 00:22:30.000000 certbot-dns-netcup-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 11:15:54.813825 certbot-dns-netcup-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2022-11-27 11:15:47.000000 certbot-dns-netcup-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2022-11-27 11:15:47.000000 certbot-dns-netcup-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2022-11-27 11:15:54.813825 certbot-dns-netcup-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2022-11-27 11:15:47.000000 certbot-dns-netcup-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 11:15:54.813825 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-11-27 11:15:54.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2022-11-27 11:15:47.000000 certbot-dns-netcup-1.2.0/certbot_dns_netcup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2022-11-27 11:15:54.813825 certbot-dns-netcup-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2022-11-27 11:15:47.000000 certbot-dns-netcup-1.2.0/setup.py
```

### Comparing `certbot-dns-netcup-1.1.4/LICENSE.txt` & `certbot-dns-netcup-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-netcup-1.1.4/PKG-INFO` & `certbot-dns-netcup-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: certbot-dns-netcup
-Version: 1.1.4
+Version: 1.2.0
 Summary: netcup DNS Authenticator plugin for Certbot
 Home-page: https://github.com/coldfix/certbot-dns-netcup
 Author: Thomas Gläßle
 Author-email: thomas@coldfix.de
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -197,9 +196,7 @@
 .. |License| image::   https://img.shields.io/pypi/l/certbot-dns-netcup.svg
    :target:            https://github.com/coldfix/certbot-dns-netcup/blob/master/LICENSE.txt
    :alt:               License: Apache
 
 .. |ImageSize| image:: https://img.shields.io/docker/image-size/coldfix/certbot-dns-netcup
    :target:            https://hub.docker.com/repository/docker/coldfix/certbot-dns-netcup
    :alt:               Docker image size
-
-
```

### Comparing `certbot-dns-netcup-1.1.4/README.rst` & `certbot-dns-netcup-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-netcup-1.1.4/certbot_dns_netcup.egg-info/PKG-INFO` & `certbot-dns-netcup-1.2.0/certbot_dns_netcup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: certbot-dns-netcup
-Version: 1.1.4
+Version: 1.2.0
 Summary: netcup DNS Authenticator plugin for Certbot
 Home-page: https://github.com/coldfix/certbot-dns-netcup
 Author: Thomas Gläßle
 Author-email: thomas@coldfix.de
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -197,9 +196,7 @@
 .. |License| image::   https://img.shields.io/pypi/l/certbot-dns-netcup.svg
    :target:            https://github.com/coldfix/certbot-dns-netcup/blob/master/LICENSE.txt
    :alt:               License: Apache
 
 .. |ImageSize| image:: https://img.shields.io/docker/image-size/coldfix/certbot-dns-netcup
    :target:            https://hub.docker.com/repository/docker/coldfix/certbot-dns-netcup
    :alt:               Docker image size
-
-
```

### Comparing `certbot-dns-netcup-1.1.4/certbot_dns_netcup.py` & `certbot-dns-netcup-1.2.0/certbot_dns_netcup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 """
 This module defines a certbot plugin to automate the process of completing a
 ``dns-01`` challenge (`~acme.challenges.DNS01`) by creating, and subsequently
 removing, TXT records using the netcup CCP API.
 """
 
 # Keep metadata before any imports (for setup.py)!
-__version__ = '1.1.4'
+__version__ = '1.2.0'
 __url__     = 'https://github.com/coldfix/certbot-dns-netcup'
 __all__     = ['Authenticator']
 
 from lexicon.providers import netcup
-import zope.interface
 
-from certbot import interfaces
 from certbot.plugins import dns_common
 from certbot.plugins import dns_common_lexicon
 
+try:                    # certbot 1.x, required until <=1.17
+    import zope.interface
+    from certbot.interfaces import IAuthenticator, IPluginFactory
+
+    def implement_authenticator(cls):
+        cls = zope.interface.provider(IPluginFactory)(cls)
+        cls = zope.interface.implementer(IAuthenticator)(cls)
+        return cls
+except ImportError:     # certbot 2.x, compatible with >=1.18
+    def implement_authenticator(cls):
+        return cls
+
+
 CCP_API_URL = 'https://www.netcup-wiki.de/wiki/CCP_API'
 
 
-@zope.interface.implementer(interfaces.IAuthenticator)
-@zope.interface.provider(interfaces.IPluginFactory)
+@implement_authenticator
 class Authenticator(dns_common.DNSAuthenticator):
     """DNS Authenticator for netcup
 
     This Authenticator uses the netcup API to fulfill a dns-01 challenge.
     """
 
     description = ('Obtain certificates using a DNS TXT record (if you are '
```

### Comparing `certbot-dns-netcup-1.1.4/setup.cfg` & `certbot-dns-netcup-1.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [options]
 py_modules = certbot_dns_netcup
 python_requires = >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 install_requires = 
-	acme>=0.31.0
 	certbot>=0.31.0
 	dns-lexicon>=3.2.3
-	zope.interface
 
 [options.entry_points]
 certbot.plugins = 
 	dns-netcup = certbot_dns_netcup:Authenticator
 
 [metadata]
 name = certbot-dns-netcup
```

### Comparing `certbot-dns-netcup-1.1.4/setup.py` & `certbot-dns-netcup-1.2.0/setup.py`

 * *Files identical despite different names*

