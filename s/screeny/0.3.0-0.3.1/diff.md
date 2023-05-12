# Comparing `tmp/screeny-0.3.0.tar.gz` & `tmp/screeny-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.3.0.tar", last modified: Fri May 12 15:35:50 2023, max compression
+gzip compressed data, was "screeny-0.3.1.tar", last modified: Fri May 12 18:46:54 2023, max compression
```

## Comparing `screeny-0.3.0.tar` & `screeny-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.385030 screeny-0.3.0/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.3.0/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:34:47.000000 screeny-0.3.0/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 15:35:50.385191 screeny-0.3.0/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)     2544 2023-05-12 15:23:58.000000 screeny-0.3.0/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.3.0/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.382243 screeny-0.3.0/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)      195 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)     4454 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/image.py
--rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 14:29:39.000000 screeny-0.3.0/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 15:08:56.000000 screeny-0.3.0/screeny/screeny.py
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 15:35:50.384601 screeny-0.3.0/screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-12 15:35:50.000000 screeny-0.3.0/screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-05-12 15:35:50.385824 screeny-0.3.0/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 18:46:54.129767 screeny-0.3.1/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.3.1/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:40:17.000000 screeny-0.3.1/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 18:46:54.129906 screeny-0.3.1/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     2544 2023-05-12 15:40:04.000000 screeny-0.3.1/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.3.1/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 18:46:54.127216 screeny-0.3.1/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)      195 2023-05-12 15:40:04.000000 screeny-0.3.1/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     4462 2023-05-12 18:44:01.000000 screeny-0.3.1/screeny/image.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 15:40:04.000000 screeny-0.3.1/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 15:40:04.000000 screeny-0.3.1/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 18:46:54.129446 screeny-0.3.1/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 18:46:54.000000 screeny-0.3.1/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-05-12 18:46:54.000000 screeny-0.3.1/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-12 18:46:54.000000 screeny-0.3.1/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-05-12 18:46:54.000000 screeny-0.3.1/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-12 18:46:54.000000 screeny-0.3.1/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-05-12 18:46:54.130507 screeny-0.3.1/setup.cfg
```

### Comparing `screeny-0.3.0/LICENSE` & `screeny-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.3.0/LICENSE-3RD-Party.txt` & `screeny-0.3.1/LICENSE-3RD-Party.txt`

 * *Files identical despite different names*

### Comparing `screeny-0.3.0/PKG-INFO` & `screeny-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `screeny-0.3.0/README.md` & `screeny-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `screeny-0.3.0/screeny/image.py` & `screeny-0.3.1/screeny/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,18 +53,18 @@
 
         self.color_code = "HSV"
         return self
 
     def locate_image(self, image_to_find: Union[str, np.ndarray, "Image"], confidence: float = 0.8) -> Point | bool:
         template = Image(image_to_find).to_grayscale()
 
-        heat_map = cv2.matchTemplate(self.data, template.data(), cv2.TM_CCOEFF_NORMED)
+        heat_map = cv2.matchTemplate(self.data, template.get_data(), cv2.TM_CCOEFF_NORMED)
         min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(heat_map)
         if max_val >= confidence:
-            w, h = template.data().shape
+            w, h = template.get_data().shape
             return Point(max_loc[0] + (w / 2), max_loc[1] + (h / 2))
         else:
             return False
 
     def resize(self, factor: int) -> "Image":
         self.data = cv2.resize(self.data, None, fx=factor, fy=factor, interpolation=cv2.INTER_CUBIC)
         return self
```

### Comparing `screeny-0.3.0/screeny/screeny.py` & `screeny-0.3.1/screeny/screeny.py`

 * *Files identical despite different names*

### Comparing `screeny-0.3.0/screeny.egg-info/PKG-INFO` & `screeny-0.3.1/screeny.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `screeny-0.3.0/setup.cfg` & `screeny-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = screeny
-version = 0.3.0
+version = 0.3.1
 author = Paul Pol
 author_email = mail@paul-pol.de
 description = A simple python library for working with screens and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

