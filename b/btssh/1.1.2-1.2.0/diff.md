# Comparing `tmp/btssh-1.1.2.tar.gz` & `tmp/btssh-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btssh-1.1.2.tar", last modified: Thu May 11 11:52:00 2023, max compression
+gzip compressed data, was "btssh-1.2.0.tar", last modified: Fri May 12 14:40:16 2023, max compression
```

## Comparing `btssh-1.1.2.tar` & `btssh-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:52:00.323388 btssh-1.1.2/
--rw-r--r--   0 etejeda    (501) staff       (20)     1291 2023-05-11 11:48:18.000000 btssh-1.1.2/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:48:18.000000 btssh-1.1.2/AUTHORS.rst
--rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:48:18.000000 btssh-1.1.2/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:48:18.000000 btssh-1.1.2/MANIFEST.in
--rw-r--r--   0 etejeda    (501) staff       (20)     4732 2023-05-11 11:52:00.323590 btssh-1.1.2/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     4083 2023-05-11 11:48:18.000000 btssh-1.1.2/README.md
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:52:00.321112 btssh-1.1.2/btssh/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5769 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/client.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1834 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/dictutils.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1683 2023-05-11 11:51:18.000000 btssh-1.1.2/btssh/invocation.py
--rw-r--r--   0 etejeda    (501) staff       (20)      690 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/logger.py
--rw-r--r--   0 etejeda    (501) staff       (20)     7635 2023-05-11 11:51:20.000000 btssh-1.1.2/btssh/provider.py
--rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/scp.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3193 2023-05-11 11:48:18.000000 btssh-1.1.2/btssh/sync.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-11 11:52:00.323108 btssh-1.1.2/btssh.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     4732 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      402 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-05-11 11:52:00.000000 btssh-1.1.2/btssh.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:48:18.000000 btssh-1.1.2/requirements.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      955 2023-05-11 11:52:00.324388 btssh-1.1.2/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:48:18.000000 btssh-1.1.2/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:48:18.000000 btssh-1.1.2/tox.ini
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 14:40:16.153251 btssh-1.2.0/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1291 2023-05-11 11:48:18.000000 btssh-1.2.0/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)      175 2023-05-11 11:48:18.000000 btssh-1.2.0/AUTHORS.rst
+-rw-r--r--   0 etejeda    (501) staff       (20)     1097 2023-05-11 11:48:18.000000 btssh-1.2.0/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)      224 2023-05-11 11:48:18.000000 btssh-1.2.0/MANIFEST.in
+-rw-r--r--   0 etejeda    (501) staff       (20)     4732 2023-05-12 14:40:16.153543 btssh-1.2.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     4083 2023-05-11 11:48:18.000000 btssh-1.2.0/README.md
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 14:40:16.149824 btssh-1.2.0/btssh/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5769 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/client.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1834 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/dictutils.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1683 2023-05-11 11:51:18.000000 btssh-1.2.0/btssh/invocation.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      690 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/logger.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     7635 2023-05-11 11:51:20.000000 btssh-1.2.0/btssh/provider.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    16240 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/scp.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3193 2023-05-11 11:48:18.000000 btssh-1.2.0/btssh/sync.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-12 14:40:16.152754 btssh-1.2.0/btssh.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     4732 2023-05-12 14:40:15.000000 btssh-1.2.0/btssh.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      402 2023-05-12 14:40:16.000000 btssh-1.2.0/btssh.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-12 14:40:15.000000 btssh-1.2.0/btssh.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:52:00.000000 btssh-1.2.0/btssh.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)       72 2023-05-12 14:40:15.000000 btssh-1.2.0/btssh.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        6 2023-05-12 14:40:15.000000 btssh-1.2.0/btssh.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-11 11:48:18.000000 btssh-1.2.0/requirements.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      955 2023-05-12 14:40:16.154702 btssh-1.2.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)       36 2023-05-11 11:48:18.000000 btssh-1.2.0/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      315 2023-05-11 11:48:18.000000 btssh-1.2.0/tox.ini
```

### Comparing `btssh-1.1.2/.gitignore` & `btssh-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/LICENSE` & `btssh-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/PKG-INFO` & `btssh-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btssh
-Version: 1.1.2
+Version: 1.2.0
 Summary: Utility library for command invocation via ssh
 Home-page: https://github.com/berttejeda/bert.sshutil.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: ssh,command,python,invoke,remote,invocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btssh-1.1.2/README.md` & `btssh-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/client.py` & `btssh-1.2.0/btssh/client.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/dictutils.py` & `btssh-1.2.0/btssh/dictutils.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/invocation.py` & `btssh-1.2.0/btssh/invocation.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/logger.py` & `btssh-1.2.0/btssh/logger.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/provider.py` & `btssh-1.2.0/btssh/provider.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/scp.py` & `btssh-1.2.0/btssh/scp.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh/sync.py` & `btssh-1.2.0/btssh/sync.py`

 * *Files identical despite different names*

### Comparing `btssh-1.1.2/btssh.egg-info/PKG-INFO` & `btssh-1.2.0/btssh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btssh
-Version: 1.1.2
+Version: 1.2.0
 Summary: Utility library for command invocation via ssh
 Home-page: https://github.com/berttejeda/bert.sshutil.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: ssh,command,python,invoke,remote,invocation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `btssh-1.1.2/setup.cfg` & `btssh-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = btssh
 author = Engelbert Tejeda
 author_email = berttejeda@gmail.com
 description = Utility library for command invocation via ssh
-version = 1.1.2
+version = 1.2.0
 url = https://github.com/berttejeda/bert.sshutil.git
 keywords = 
 	ssh
 	command
 	python
 	invoke
 	remote
```

