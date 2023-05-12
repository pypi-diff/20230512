# Comparing `tmp/esprepomanager-1.2.5.tar.gz` & `tmp/esprepomanager-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esprepomanager-1.2.5.tar", last modified: Sat Apr 22 15:30:04 2023, max compression
+gzip compressed data, was "esprepomanager-1.3.0.tar", last modified: Fri May 12 12:39:48 2023, max compression
```

## Comparing `esprepomanager-1.2.5.tar` & `esprepomanager-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/
--rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.2.5/LICENSE
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/PKG-INFO
--rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.2.5/README.md
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/esprepomanager/
--rw-rw-r--   0 tobias    (1012) familie    (155)    13725 2023-04-22 13:01:44.000000 esprepomanager-1.2.5/esprepomanager/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.2.5/esprepomanager/__main__.py
--rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.2.5/esprepomanager/config.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/esprepomanager/gitlab/
--rw-rw-r--   0 tobias    (1012) familie    (155)     6642 2023-04-22 13:01:44.000000 esprepomanager-1.2.5/esprepomanager/gitlab/__init__.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.2.5/esprepomanager/gitlab/group.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     7763 2023-04-22 15:30:01.000000 esprepomanager-1.2.5/esprepomanager/gitlab/project.py
--rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.2.5/esprepomanager/gitlab/user.py
--rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.2.5/esprepomanager/person.py
--rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.2.5/esprepomanager/repo.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.2.5/esprepomanager/team.py
--rw-rw-r--   0 tobias    (1012) familie    (155)     4102 2023-04-22 13:01:44.000000 esprepomanager-1.2.5/esprepomanager/utils.py
-drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/esprepomanager.egg-info/
--rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/entry_points.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-04-22 15:30:04.000000 esprepomanager-1.2.5/esprepomanager.egg-info/top_level.txt
--rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-04-22 15:30:04.939720 esprepomanager-1.2.5/setup.cfg
--rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-04-22 15:30:01.000000 esprepomanager-1.2.5/setup.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-05-12 12:39:48.689331 esprepomanager-1.3.0/
+-rw-r--r--   0 tobias    (1012) familie    (155)    35149 2023-04-11 14:23:15.000000 esprepomanager-1.3.0/LICENSE
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-05-12 12:39:48.689331 esprepomanager-1.3.0/PKG-INFO
+-rw-r--r--   0 tobias    (1012) familie    (155)      127 2023-04-14 20:13:12.000000 esprepomanager-1.3.0/README.md
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-05-12 12:39:48.685331 esprepomanager-1.3.0/esprepomanager/
+-rw-rw-r--   0 tobias    (1012) familie    (155)    13725 2023-04-22 13:01:44.000000 esprepomanager-1.3.0/esprepomanager/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      146 2023-04-11 14:32:23.000000 esprepomanager-1.3.0/esprepomanager/__main__.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)    10879 2023-04-22 11:18:34.000000 esprepomanager-1.3.0/esprepomanager/config.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-05-12 12:39:48.685331 esprepomanager-1.3.0/esprepomanager/gitlab/
+-rw-rw-r--   0 tobias    (1012) familie    (155)     6642 2023-04-22 13:01:44.000000 esprepomanager-1.3.0/esprepomanager/gitlab/__init__.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1915 2023-04-14 16:46:47.000000 esprepomanager-1.3.0/esprepomanager/gitlab/group.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     8400 2023-05-12 12:37:47.000000 esprepomanager-1.3.0/esprepomanager/gitlab/project.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      439 2023-04-13 01:24:15.000000 esprepomanager-1.3.0/esprepomanager/gitlab/user.py
+-rw-r--r--   0 tobias    (1012) familie    (155)     1850 2023-04-13 22:10:58.000000 esprepomanager-1.3.0/esprepomanager/person.py
+-rw-r--r--   0 tobias    (1012) familie    (155)      678 2023-04-12 20:47:34.000000 esprepomanager-1.3.0/esprepomanager/repo.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     1828 2023-04-22 11:18:34.000000 esprepomanager-1.3.0/esprepomanager/team.py
+-rw-rw-r--   0 tobias    (1012) familie    (155)     4102 2023-04-22 13:01:44.000000 esprepomanager-1.3.0/esprepomanager/utils.py
+drwxrwxr-x   0 tobias    (1012) familie    (155)        0 2023-05-12 12:39:48.685331 esprepomanager-1.3.0/esprepomanager.egg-info/
+-rw-rw-r--   0 tobias    (1012) familie    (155)      564 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1012) familie    (155)      558 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)        1 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       55 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/entry_points.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       14 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       15 2023-05-12 12:39:48.000000 esprepomanager-1.3.0/esprepomanager.egg-info/top_level.txt
+-rw-rw-r--   0 tobias    (1012) familie    (155)       38 2023-05-12 12:39:48.689331 esprepomanager-1.3.0/setup.cfg
+-rw-rw-r--   0 tobias    (1012) familie    (155)      768 2023-05-12 12:39:14.000000 esprepomanager-1.3.0/setup.py
```

### Comparing `esprepomanager-1.2.5/LICENSE` & `esprepomanager-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/PKG-INFO` & `esprepomanager-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.5
+Version: 1.3.0
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.5/esprepomanager/__init__.py` & `esprepomanager-1.3.0/esprepomanager/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/config.py` & `esprepomanager-1.3.0/esprepomanager/config.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/gitlab/__init__.py` & `esprepomanager-1.3.0/esprepomanager/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/gitlab/group.py` & `esprepomanager-1.3.0/esprepomanager/gitlab/group.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/gitlab/project.py` & `esprepomanager-1.3.0/esprepomanager/gitlab/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,30 +72,47 @@
         return True
 
     def tree(
         self, path: Optional[str] = None, recursive: bool = False,
         ref: Optional[str] = None, max_tries: int = 3
     ) -> List[str]:
         params = {
-            "recursive": "true" if recursive else "false"
+            "recursive": "true" if recursive else "false",
+            "pagination": "keyset",
+            "per_page": "100",
+            "order_by": "path",
+            "sort": "asc"
         }
         if path:
             params["path"] = path
         if ref:
             params["ref"] = ref
 
-        for _ in range(max_tries):
-            resp = self.send_request("GET", "repository/tree", params_=params)
-            j_resp = resp.json()
-            if resp.ok:
-                return [x["path"] for x in j_resp]
-            log.debug(j_resp)
-            time.sleep(1)
+        link: Optional[str] = None
+        ret_list: List[str] = []
+        next_page: bool = True
+        while next_page:
+            for _ in range(max_tries):
+                if link:
+                    resp = requests.get(link)
+                else:
+                    resp = self.send_request("GET", "repository/tree", params_=params)
+                j_resp = resp.json()
+                if resp.ok:
+                    ret_list.extend(x["path"] for x in j_resp)
+                    if resp.links.get("next"):
+                        link = resp.links.get("next")["url"]  # type: ignore
+                    else:
+                        next_page = False
+                    break
+                else:
+                    log.debug(j_resp)
+                    time.sleep(1)
 
-        return []
+        return ret_list
 
     def members(self) -> List[User]:
         resp = self.send_request("GET", "members", params_={"per_page": "100"})
         if not resp.ok:
             log.debug(resp.json())
             return []
         return [User.from_json(x) for x in resp.json()]
```

### Comparing `esprepomanager-1.2.5/esprepomanager/person.py` & `esprepomanager-1.3.0/esprepomanager/person.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/repo.py` & `esprepomanager-1.3.0/esprepomanager/repo.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/team.py` & `esprepomanager-1.3.0/esprepomanager/team.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager/utils.py` & `esprepomanager-1.3.0/esprepomanager/utils.py`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/esprepomanager.egg-info/PKG-INFO` & `esprepomanager-1.3.0/esprepomanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esprepomanager
-Version: 1.2.5
+Version: 1.3.0
 Summary: manager for git repos
 Home-page: https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager
 Author: Teichi
 Author-email: tobias@teichmann.top
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `esprepomanager-1.2.5/esprepomanager.egg-info/SOURCES.txt` & `esprepomanager-1.3.0/esprepomanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esprepomanager-1.2.5/setup.py` & `esprepomanager-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="esprepomanager",
-    version="1.2.5",
+    version="1.3.0",
     author="Teichi",
     author_email="tobias@teichmann.top",
     description="manager for git repos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.tugraz.at/esp-oop1-dev/pyrepomanager",
     packages=setuptools.find_packages(),
```

