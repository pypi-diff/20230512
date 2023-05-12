# Comparing `tmp/alldebrid.py-1.0.3.tar.gz` & `tmp/alldebrid.py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alldebrid.py-1.0.3.tar", last modified: Fri May 12 15:13:36 2023, max compression
+gzip compressed data, was "alldebrid.py-1.0.4.tar", last modified: Fri May 12 20:17:00 2023, max compression
```

## Comparing `alldebrid.py-1.0.3.tar` & `alldebrid.py-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 15:13:36.301828 alldebrid.py-1.0.3/
--rw-rw-rw-   0        0        0      100 2023-05-12 15:13:36.251725 alldebrid.py-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 15:13:35.840057 alldebrid.py-1.0.3/alldebrid/
--rw-rw-rw-   0        0        0      103 2023-05-12 14:57:07.000000 alldebrid.py-1.0.3/alldebrid/__init__.py
--rw-rw-rw-   0        0        0    45490 2023-05-12 15:13:08.000000 alldebrid.py-1.0.3/alldebrid/alldebrid.py
-drwxrwxrwx   0        0        0        0 2023-05-12 15:13:36.174496 alldebrid.py-1.0.3/alldebrid.py.egg-info/
--rw-rw-rw-   0        0        0      100 2023-05-12 15:13:35.000000 alldebrid.py-1.0.3/alldebrid.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-12 15:13:35.000000 alldebrid.py-1.0.3/alldebrid.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 15:13:35.000000 alldebrid.py-1.0.3/alldebrid.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 15:13:35.000000 alldebrid.py-1.0.3/alldebrid.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 15:13:35.000000 alldebrid.py-1.0.3/alldebrid.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 15:13:36.301828 alldebrid.py-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      285 2023-05-12 15:13:18.000000 alldebrid.py-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:17:00.080112 alldebrid.py-1.0.4/
+-rw-rw-rw-   0        0        0      100 2023-05-12 20:17:00.041490 alldebrid.py-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 20:16:59.647689 alldebrid.py-1.0.4/alldebrid/
+-rw-rw-rw-   0        0        0      103 2023-05-12 14:57:07.000000 alldebrid.py-1.0.4/alldebrid/__init__.py
+-rw-rw-rw-   0        0        0    45337 2023-05-12 20:16:55.000000 alldebrid.py-1.0.4/alldebrid/alldebrid.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:16:59.979422 alldebrid.py-1.0.4/alldebrid.py.egg-info/
+-rw-rw-rw-   0        0        0      100 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 20:17:00.080112 alldebrid.py-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      285 2023-05-12 20:16:46.000000 alldebrid.py-1.0.4/setup.py
```

### Comparing `alldebrid.py-1.0.3/README.md` & `alldebrid.py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alldebrid.py-1.0.3/alldebrid/alldebrid.py` & `alldebrid.py-1.0.4/alldebrid/alldebrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1410,15 +1410,8 @@
             data=data,
             params=params,
             files=files,
             timeout=timeout,
             session=session,
         )
 
-        return response
-
-
-ad = AllDebrid(apikey="tXQQw2JPx8iKEyeeOoJE")
-try:
-    response = ad.save_new_link("invalid_link")
-except InvalidLinkError as e:
-    print(e)
+        return response
```

