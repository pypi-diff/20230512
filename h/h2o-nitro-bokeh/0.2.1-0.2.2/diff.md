# Comparing `tmp/h2o_nitro_bokeh-0.2.1-py3-none-any.whl.zip` & `tmp/h2o_nitro_bokeh-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7916 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      645 b- defN 22-Jun-10 00:22 h2o_nitro_bokeh/__init__.py
--rw-rw-r--  2.0 unx     1961 b- defN 22-Jun-10 00:22 h2o_nitro_bokeh/plugin.py
--rw-rw-r--  2.0 unx    11357 b- defN 22-Jun-10 00:54 h2o_nitro_bokeh-0.2.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2471 b- defN 22-Jun-10 00:54 h2o_nitro_bokeh-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Jun-10 00:54 h2o_nitro_bokeh-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 22-Jun-10 00:54 h2o_nitro_bokeh-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      592 b- defN 22-Jun-10 00:54 h2o_nitro_bokeh-0.2.1.dist-info/RECORD
-7 files, 17134 bytes uncompressed, 6860 bytes compressed:  60.0%
+Zip file size: 7955 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx      645 b- defN 23-May-12 17:09 h2o_nitro_bokeh/__init__.py
+-rw-rw-r--  2.0 unx     2080 b- defN 23-May-12 17:07 h2o_nitro_bokeh/plugin.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-May-12 17:11 h2o_nitro_bokeh-0.2.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2385 b- defN 23-May-12 17:11 h2o_nitro_bokeh-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-12 17:11 h2o_nitro_bokeh-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       16 b- defN 23-May-12 17:11 h2o_nitro_bokeh-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      592 b- defN 23-May-12 17:11 h2o_nitro_bokeh-0.2.2.dist-info/RECORD
+7 files, 17167 bytes uncompressed, 6899 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: h2o_nitro_bokeh/__init__.py
 Comment: 
 
 Filename: h2o_nitro_bokeh/plugin.py
 Comment: 
 
-Filename: h2o_nitro_bokeh-0.2.1.dist-info/LICENSE
+Filename: h2o_nitro_bokeh-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: h2o_nitro_bokeh-0.2.1.dist-info/METADATA
+Filename: h2o_nitro_bokeh-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: h2o_nitro_bokeh-0.2.1.dist-info/WHEEL
+Filename: h2o_nitro_bokeh-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_nitro_bokeh-0.2.1.dist-info/top_level.txt
+Filename: h2o_nitro_bokeh-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_nitro_bokeh-0.2.1.dist-info/RECORD
+Filename: h2o_nitro_bokeh-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_nitro_bokeh/__init__.py

```diff
@@ -10,9 +10,9 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .plugin import bokeh_plugin, bokeh_box
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

## h2o_nitro_bokeh/plugin.py

```diff
@@ -9,40 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-from bokeh.util.version import __version__ as bokeh_version
-from bokeh.model import Model
-from bokeh.embed import json_item
+from typing import Optional
 
+from bokeh.embed import json_item
+from bokeh.model import Model
+from bokeh.util.version import __version__ as bokeh_version
 from h2o_nitro import box, Box, Plugin, Script
 
+bokeh_js_cdn_path = f'https://cdnjs.cloudflare.com/ajax/libs/bokeh/{bokeh_version}/bokeh.min.js'
+
 # Javascript function for embedding the Bokeh plot.
 # See: http://docs.bokeh.org/en/latest/docs/user_guide/embed.html#json-items
 # Here, we export one function called embed(), which we can later invoke from our Python box().
 _bokeh_embed_js = '''
 exports.embed = (context, element, data) => {
     Bokeh.embed.embed_item(JSON.parse(data.model), element.id);
 };
 '''
 
 
-def bokeh_plugin():
+def bokeh_plugin(bokeh_js_path: Optional[str] = None):
     """
     Creates a Nitro plugin for the currently installed version of Bokeh.
     :return: A plugin
     """
     return Plugin(
         name='bokeh',
         scripts=[
             # Install the Bokeh library.
-            Script(source=f'https://cdnjs.cloudflare.com/ajax/libs/bokeh/{bokeh_version}/bokeh.min.js'),
+            Script(source=bokeh_js_path or bokeh_js_cdn_path),
             # Install our custom Bokeh-embedding Javascript.
             Script(source=_bokeh_embed_js, type='inline'),
         ],
     )
 
 
 def bokeh_box(model: Model) -> Box:
```

## Comparing `h2o_nitro_bokeh-0.2.1.dist-info/LICENSE` & `h2o_nitro_bokeh-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `h2o_nitro_bokeh-0.2.1.dist-info/METADATA` & `h2o_nitro_bokeh-0.2.2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-nitro-bokeh
-Version: 0.2.1
+Version: 0.2.2
 Summary: Bokeh plugin for H2O Nitro
 Home-page: https://github.com/h2oai/nitro-bokeh
 Author: Prithvi Prabhu
 Author-email: prithvi.prabhu@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/h2oai/nitro-bokeh
 Project-URL: Source, https://github.com/h2oai/nitro-bokeh
@@ -35,53 +35,57 @@
 # Bokeh plugin for H2O Nitro
 
 This plugin lets you use [Bokeh](https://docs.bokeh.org/en/latest/) visualizations in [Nitro](https://github.com/h2oai/nitro)
 apps.
 
 ## Demo
 
-[View source](example).
-
 ![Demo](demo.gif)
 
+[View source](examples/bokeh_basic.py).
+
 ## Install
 
 ```
 pip install h2o-nitro-bokeh
 ```
 
 ## Usage
 
-1. Import `bokeh_plugin` and `bokeh_box` from `h2o_nitro_bokeh`.
-2. Add `bokeh_plugin()` to your Nitro app.
-3. Use `bokeh_box(model)` to render Bokeh models (figures, widgets, and so on).
-
+1. Import the plugin:
 
 ```py 
-from bokeh.plotting import figure, show
-from h2o_nitro import View, web_directory
 from h2o_nitro_bokeh import bokeh_plugin, bokeh_box
+```
 
+2. Register the plugin:
 
-def main(view: View):
-    view(bokeh_box(make_plot()))
+```py 
+nitro = View(main, title='My App', caption='v1.0', plugins=[bokeh_plugin()])
+```
 
+3. Use the plugin:
 
-nitro = View(
-    main,
-    title='Nitro + Bokeh',
-    caption='A minimal example',
-    plugins=[bokeh_plugin()],  # Include the Bokeh plugin
-)
-
-def make_plot():
-    x = [1, 2, 3, 4, 5]
-    y = [6, 7, 2, 4, 5]
-    p = figure(title="Simple line example", x_axis_label="x", y_axis_label="y")
-    p.line(x, y, legend_label="Temp.", line_width=2)
-    return p
+```py 
+# Make a plot
+x = [1, 2, 3, 4, 5]
+y = [6, 7, 2, 4, 5]
+p = figure(title="Simple line example", x_axis_label="x", y_axis_label="y")
+p.line(x, y, legend_label="Temp.", line_width=2)
 
+# Display the plot
+view(bokeh_box(p))
 ```
 
+## Change Log
+
+- v0.2.1 - Jun 09, 2022
+    - Fixed
+        - Don't return value from plots.
+- v0.2.0 - May 39, 2022
+    - Perf
+        - Quicker loading
+- v0.1.0 - May 25, 2022
+    - Initial Version
```

