# Comparing `tmp/kmaps-0.0.8.tar.gz` & `tmp/kmaps-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmaps-0.0.8.tar", last modified: Mon May  1 00:14:45 2023, max compression
+gzip compressed data, was "kmaps-0.0.9.tar", last modified: Mon May  1 00:23:48 2023, max compression
```

## Comparing `kmaps-0.0.8.tar` & `kmaps-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 00:14:29.000000 kmaps-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 00:14:29.000000 kmaps-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:14:45.091000 kmaps-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 00:14:29.000000 kmaps-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/kmaps/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/folmaps.py
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-05-01 00:14:29.000000 kmaps-0.0.8/kmaps/kmaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:14:45.091000 kmaps-0.0.8/kmaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 00:14:45.000000 kmaps-0.0.8/kmaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 00:14:29.000000 kmaps-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 00:14:45.091000 kmaps-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 00:14:29.000000 kmaps-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:23:48.425807 kmaps-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-01 00:23:33.000000 kmaps-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 00:23:33.000000 kmaps-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:23:48.425807 kmaps-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-01 00:23:33.000000 kmaps-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:23:48.421807 kmaps-0.0.9/kmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 00:23:33.000000 kmaps-0.0.9/kmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-01 00:23:33.000000 kmaps-0.0.9/kmaps/folmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17287 2023-05-01 00:23:33.000000 kmaps-0.0.9/kmaps/kmaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:23:48.425807 kmaps-0.0.9/kmaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-01 00:23:48.000000 kmaps-0.0.9/kmaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 00:23:33.000000 kmaps-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 00:23:48.425807 kmaps-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 00:23:33.000000 kmaps-0.0.9/setup.py
```

### Comparing `kmaps-0.0.8/LICENSE` & `kmaps-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.8/PKG-INFO` & `kmaps-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.8
+Version: 0.0.9
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.8/README.md` & `kmaps-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.8/kmaps/folmaps.py` & `kmaps-0.0.9/kmaps/folmaps.py`

 * *Files identical despite different names*

### Comparing `kmaps-0.0.8/kmaps/kmaps.py` & `kmaps-0.0.9/kmaps/kmaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -307,14 +307,15 @@
 
         widget = widgets.HTML(value = f'<img src="{url}" width = "{width}" height = "{height}">')
         control = WidgetControl(widget = widget, position = position)
         self.add(control)
 
 
 
+
     def to_streamlit(self, width=None, height=600, scrolling=False, **kwargs):
         ####### just copied from leafmap
         """Renders map figure in a Streamlit app.
         Args:
             width (int, optional): Width of the map. Defaults to None.
             height (int, optional): Height of the map. Defaults to 600.
             responsive (bool, optional): Whether to make the map responsive. Defaults to True.
@@ -335,14 +336,88 @@
             #     st.markdown(make_map_responsive, unsafe_allow_html=True)
             return components.html(
                 self.to_html(), width=width, height=height, scrolling=scrolling
             )
 
         except Exception as e:
             raise Exception(e)
+
+    def to_html(
+        self,
+        outfile=None,
+        title="My Map",
+        width="100%",
+        height="880px",
+        add_layer_control=True,
+        **kwargs,
+    ):
+        ####### just copied from leafmap
+        """Saves the map as an HTML file.
+        Args:
+            outfile (str, optional): The output file path to the HTML file.
+            title (str, optional): The title of the HTML file. Defaults to 'My Map'.
+            width (str, optional): The width of the map in pixels or percentage. Defaults to '100%'.
+            height (str, optional): The height of the map in pixels. Defaults to '880px'.
+            add_layer_control (bool, optional): Whether to add the LayersControl. Defaults to True.
+        """
+        try:
+            save = True
+            if outfile is not None:
+                if not outfile.endswith(".html"):
+                    raise ValueError("The output file extension must be html.")
+                outfile = os.path.abspath(outfile)
+                out_dir = os.path.dirname(outfile)
+                if not os.path.exists(out_dir):
+                    os.makedirs(out_dir)
+            else:
+                outfile = os.path.abspath(random_string() + ".html")
+                save = False
+
+            if add_layer_control and self.layer_control is None:
+                layer_control = ipyleaflet.LayersControl(position="topright")
+                self.layer_control = layer_control
+                self.add(layer_control)
+
+            before_width = self.layout.width
+            before_height = self.layout.height
+
+            if not isinstance(width, str):
+                print("width must be a string.")
+                return
+            elif width.endswith("px") or width.endswith("%"):
+                pass
+            else:
+                print("width must end with px or %")
+                return
+
+            if not isinstance(height, str):
+                print("height must be a string.")
+                return
+            elif not height.endswith("px"):
+                print("height must end with px")
+                return
+
+            self.layout.width = width
+            self.layout.height = height
+
+            self.save(outfile, title=title, **kwargs)
+
+            self.layout.width = before_width
+            self.layout.height = before_height
+
+            if not save:
+                out_html = ""
+                with open(outfile) as f:
+                    lines = f.readlines()
+                    out_html = "".join(lines)
+                os.remove(outfile)
+                return out_html
+
+        except Exception as e:
+            raise Exception(e)
     
 
 
 def generate_random_string(length, upper = False, digit = False, punc = False):
     """Generates a random string of a given length.
 
     Args:
```

### Comparing `kmaps-0.0.8/kmaps.egg-info/PKG-INFO` & `kmaps-0.0.9/kmaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kmaps
-Version: 0.0.8
+Version: 0.0.9
 Summary: TBA
 Home-page: https://github.com/ChangwhaOh/kmaps
 Author: Changwha Oh
 Author-email: coh4@vols.utk.edu
 License: MIT license
 Keywords: kmaps
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kmaps-0.0.8/setup.py` & `kmaps-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='kmaps',
     name='kmaps',
     packages=find_packages(include=['kmaps', 'kmaps.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChangwhaOh/kmaps',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

