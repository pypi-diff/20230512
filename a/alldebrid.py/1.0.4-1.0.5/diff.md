# Comparing `tmp/alldebrid.py-1.0.4.tar.gz` & `tmp/alldebrid.py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alldebrid.py-1.0.4.tar", last modified: Fri May 12 20:17:00 2023, max compression
+gzip compressed data, was "alldebrid.py-1.0.5.tar", last modified: Fri May 12 20:23:19 2023, max compression
```

## Comparing `alldebrid.py-1.0.4.tar` & `alldebrid.py-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 20:17:00.080112 alldebrid.py-1.0.4/
--rw-rw-rw-   0        0        0      100 2023-05-12 20:17:00.041490 alldebrid.py-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 20:16:59.647689 alldebrid.py-1.0.4/alldebrid/
--rw-rw-rw-   0        0        0      103 2023-05-12 14:57:07.000000 alldebrid.py-1.0.4/alldebrid/__init__.py
--rw-rw-rw-   0        0        0    45337 2023-05-12 20:16:55.000000 alldebrid.py-1.0.4/alldebrid/alldebrid.py
-drwxrwxrwx   0        0        0        0 2023-05-12 20:16:59.979422 alldebrid.py-1.0.4/alldebrid.py.egg-info/
--rw-rw-rw-   0        0        0      100 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 20:16:59.000000 alldebrid.py-1.0.4/alldebrid.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 20:17:00.080112 alldebrid.py-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      285 2023-05-12 20:16:46.000000 alldebrid.py-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:23:19.123904 alldebrid.py-1.0.5/
+-rw-rw-rw-   0        0        0      100 2023-05-12 20:23:19.084899 alldebrid.py-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1308 2023-05-11 11:31:41.000000 alldebrid.py-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 20:23:18.702597 alldebrid.py-1.0.5/alldebrid/
+-rw-rw-rw-   0        0        0      103 2023-05-12 14:57:07.000000 alldebrid.py-1.0.5/alldebrid/__init__.py
+-rw-rw-rw-   0        0        0    45343 2023-05-12 20:23:04.000000 alldebrid.py-1.0.5/alldebrid/alldebrid.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:23:19.021355 alldebrid.py-1.0.5/alldebrid.py.egg-info/
+-rw-rw-rw-   0        0        0      100 2023-05-12 20:23:18.000000 alldebrid.py-1.0.5/alldebrid.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-05-12 20:23:18.000000 alldebrid.py-1.0.5/alldebrid.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 20:23:18.000000 alldebrid.py-1.0.5/alldebrid.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 20:23:18.000000 alldebrid.py-1.0.5/alldebrid.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-12 20:23:18.000000 alldebrid.py-1.0.5/alldebrid.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 20:23:19.123904 alldebrid.py-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      285 2023-05-12 20:23:16.000000 alldebrid.py-1.0.5/setup.py
```

### Comparing `alldebrid.py-1.0.4/README.md` & `alldebrid.py-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `alldebrid.py-1.0.4/alldebrid/alldebrid.py` & `alldebrid.py-1.0.5/alldebrid/alldebrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1071,17 +1071,17 @@
         if not link:
             raise ValueError("No link id to save")
 
         endpoint = self.endpoints.get("save a link")
         if not endpoint:
             raise ValueError("Endpoint not found for save new link")
 
-        for l in link:
-            if not re.match(r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+', l):
-                raise InvalidLinkError(l)
+        # for l in link:
+        #     if not re.match(r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+', l):
+        #         raise InvalidLinkError(l)
 
         response = self._request(method="POST", endpoint=endpoint, links=link)
 
         if response.get("status") == "error":
             error = response["error"]
             raise APIError(error["code"], error["message"])
```

