# Comparing `tmp/mkdocs_exporter-1.1.0.tar.gz` & `tmp/mkdocs_exporter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-1.1.0.tar", max compression
+gzip compressed data, was "mkdocs_exporter-1.2.0.tar", max compression
```

## Comparing `mkdocs_exporter-1.1.0.tar` & `mkdocs_exporter-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.1.0/LICENSE
--rw-r--r--   0        0        0     3084 2023-05-09 09:12:35.847118 mkdocs_exporter-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.1.0/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1899 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.1.0/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.1.0/mkdocs_exporter/page.py
--rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.1.0/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      977 2023-05-09 09:27:33.387117 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0      812 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      731 2023-05-09 09:13:25.647118 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1088 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4793 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2330 2023-05-09 11:31:09.967140 mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4073 2023-05-09 17:07:37.227188 mkdocs_exporter-1.1.0/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.1.0/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0     1298 2023-05-09 17:08:04.297189 mkdocs_exporter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4479 1970-01-01 00:00:00.000000 mkdocs_exporter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3066 2023-05-11 19:49:17.381184 mkdocs_exporter-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-1.2.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1899 2023-05-09 17:07:37.227188 mkdocs_exporter-1.2.0/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-1.2.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      440 2023-05-08 15:32:49.823552 mkdocs_exporter-1.2.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0      705 2023-05-08 15:33:10.113552 mkdocs_exporter-1.2.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      977 2023-05-09 09:27:33.387117 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0      812 2023-05-09 17:07:37.227188 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      731 2023-05-09 09:13:25.647118 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1120 2023-05-11 19:49:17.381184 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4456 2023-05-11 19:49:17.381184 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2330 2023-05-09 11:31:09.967140 mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     4080 2023-05-09 18:59:51.747207 mkdocs_exporter-1.2.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-1.2.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-1.2.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-1.2.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   499714 2023-05-08 14:10:56.413538 mkdocs_exporter-1.2.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0     1525 2023-05-11 21:30:55.690459 mkdocs_exporter-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 mkdocs_exporter-1.2.0/PKG-INFO
```

### Comparing `mkdocs_exporter-1.1.0/LICENSE` & `mkdocs_exporter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/README.md` & `mkdocs_exporter-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # MkDocs Exporter
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs) that exports your pages to PDF files.
 
 ## Features
 
-- :rocket: **Fast** - PDF documents are generated concurrently!
-- :star: **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
+- 🚀 **Fast** - PDF documents are generated concurrently!
+- ⭐ **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
   - [*Paged.js*](https://github.com/pagedjs/pagedjs) polyfills are included by default ([Paged Media](https://www.w3.org/TR/css-page-3/) and [Generated Content](https://www.w3.org/TR/css-gcpm-3/) CSS modules)
   - [*Sass*](https://sass-lang.com/) support (via [`libsass`](https://github.com/sass/libsass-python)) for your stylesheets
-- :paintbrush: **Customizable** - full control over the resulting documents
+- 🎨 **Customizable** - full control over the resulting documents
   - Built for and compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
   - Cover pages with templating support (for instance, with the [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
   - Define custom scripts and stylesheets to customize your PDF documents
   - Define "buttons" at the top of your documentation pages
 
 ## Prerequisites
 
@@ -67,8 +67,8 @@
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
 Feel free to request additional features by submitting an issue or by contributing through a pull request.
 
 ## License
 
-This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE.md).
+This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/browser.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugin.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,81 @@
 import os
 import types
 import asyncio
 
-from weasyprint import urls
-from typing import Optional
 from mkdocs.plugins import BasePlugin
 from mkdocs_exporter.page import Page
 from mkdocs.plugins import event_priority
 from mkdocs_exporter.logging import logger
 from mkdocs.livereload import LiveReloadServer
+from typing import Optional, Coroutine, Sequence
 from mkdocs_exporter.plugins.pdf.config import Config
 from mkdocs_exporter.plugins.pdf.renderer import Renderer
 
 
 class Plugin(BasePlugin[Config]):
   """The plugin."""
 
 
   def __init__(self):
     """The constructor."""
 
+    self.watch: list[str] = []
     self.renderer: Optional[Renderer] = None
     self.tasks: list[types.CoroutineType] = []
-    self.loop: Optional[asyncio.AbstractEventLoop] = None
 
 
   def on_config(self, config: dict) -> None:
     """Invoked when the configuration has been validated."""
 
-    def resolve(path: str) -> str:
-      if path is None:
-        return None
-      if urls.url_is_absolute(path):
-        return path
-
-      return os.path.join(os.path.dirname(config['config_file_path']), path)
-
-    self.config.covers.front = resolve(self.config.covers.front)
-    self.config.covers.back = resolve(self.config.covers.back)
-    self.config.scripts = [resolve(path) for path in self.config.scripts]
-    self.config.stylesheets = [resolve(path) for path in self.config.stylesheets]
+    self.watch = []
 
 
   def on_serve(self, server: LiveReloadServer, **kwargs) -> LiveReloadServer:
     """Invoked when the website is being served."""
 
     if not self._enabled():
       return
     for path in [*self.config.stylesheets, *self.config.scripts]:
       server.watch(path)
-    for cover in self.config.covers:
-      if self.config.covers[cover]:
-        server.watch(self.config.covers[cover])
+    for path in set(os.path.normpath(path) for path in self.watch):
+      server.watch(path)
 
     return server
 
 
-  def on_page_markdown(self, markdown: str, page: Page, **kwargs) -> str:
+  def on_page_markdown(self, markdown: str, page: Page, config: Config, **kwargs) -> str:
     """Invoked when the page's markdown has been loaded."""
 
-    if not self._enabled(page) or 'cover' in page.meta.get('hide', []):
+    if not self._enabled(page) and 'covers' not in page.meta.get('hide', []):
       return
 
     content = markdown
+    covers = {**self.config.covers, **{k: os.path.join(os.path.dirname(config['config_file_path']), v) for k, v in page.meta.get('covers', {}).items()}}
 
-    if self.config.covers.front:
-      with open(self.config.covers.front, 'r') as file:
+    if covers.get('front'):
+      with open(covers['front'], 'r') as file:
         content = self.renderer.cover(file.read()) + content
-    if self.config.covers.back:
-      with open(self.config.covers.back, 'r') as file:
+    if covers.get('back'):
+      with open(covers['back'], 'r') as file:
         content = content + self.renderer.cover(file.read())
 
+    for path in [path for path in covers.values() if path is not None]:
+      self.watch.append(path)
+
     return content
 
 
   def on_pre_build(self, **kwargs) -> None:
     """Invoked before the build process starts."""
 
+    self.tasks.clear()
+
     if not self._enabled():
       return
-    if self.loop and self.loop.is_running():
-      self.loop.close()
-
-    self.tasks.clear()
 
     self.renderer = Renderer()
 
     for stylesheet in self.config.stylesheets:
       self.renderer.add_stylesheet(stylesheet)
     for script in self.config.scripts:
       self.renderer.add_script(script)
@@ -134,37 +123,32 @@
 
   def on_post_build(self, **kwargs) -> None:
     """Invoked after the build process."""
 
     if not self._enabled():
       return
 
-    self.loop = asyncio.new_event_loop()
+    def concurrently(coroutines: Sequence[Coroutine], concurrency: int) -> Sequence[Coroutine]:
+      semaphore = asyncio.Semaphore(concurrency)
+
+      async def limit(coroutine: Coroutine) -> Coroutine:
+        async with semaphore:
+          return await asyncio.create_task(coroutine)
 
-    def partition(list, n):
-      for i in range(0, len(list), n):
-        yield [self.loop.create_task(task) for task in list[i:i + n]]
+      return [limit(coroutine) for coroutine in coroutines]
 
-    for tasks in partition(self.tasks, self.config.concurrency or 1):
-      self.loop.run_until_complete(asyncio.gather(*tasks))
+    loop = asyncio.get_event_loop()
 
+    loop.run_until_complete(asyncio.gather(*concurrently(self.tasks, max(1, self.config.concurrency or 1))))
     self.tasks.clear()
-    self.loop.run_until_complete(self.renderer.dispose())
-    self.loop.close()
+    loop.run_until_complete(self.renderer.dispose())
 
     self.renderer = None
 
 
-  def on_shutdown(self) -> None:
-    """Invoked on shutdown..."""
-
-    if self.loop and self.loop.is_running():
-      self.loop.stop()
-
-
   def _enabled(self, page: Page = None) -> bool:
     """Is the plugin enabled for this page?"""
 
     if not self.config.enabled:
       return False
     if page and not page.meta.get('pdf', not self.config.explicit):
       return False
```

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-1.2.0/mkdocs_exporter/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import os
 import sass
 
-from weasyprint import urls
+from urllib.parse import urlparse
 from bs4 import BeautifulSoup, Tag
 from typing import Any, Callable, Union
 from mkdocs_exporter.logging import logger
 
 
 class Preprocessor():
   """The HTML preprocessor."""
@@ -143,13 +143,13 @@
 
     return result
 
 
   def _resolve_link(self, url: str, base: str, root: str = None) -> str:
     """Resolves a link to its new base location."""
 
-    if urls.url_is_absolute(url):
+    if bool(urlparse(url).netloc):
       return url
     if root is not None and os.path.isabs(url):
       return 'file://' + os.path.abspath(os.path.join(root, url.strip('/')))
 
     return 'file://' + os.path.abspath(os.path.join(base, url.strip('/')))
```

### Comparing `mkdocs_exporter-1.1.0/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-1.2.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-1.1.0/pyproject.toml` & `mkdocs_exporter-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "1.1.0"
+version = "1.2.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
@@ -20,15 +20,14 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 mkdocs = ">=1.4"
 playwright = ">=1.33"
 beautifulsoup4 = ">=4.12.2"
-weasyprint = ">=50.0"
 lxml = ">=4.9"
 libsass = ">=0.22.0"
 importlib-resources = ">=5.0"
 importlib-metadata = "<5.0"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 "mkdocs/exporter" = "mkdocs_exporter.plugin:Plugin"
@@ -36,7 +35,14 @@
 "mkdocs/exporter/extras" = "mkdocs_exporter.plugins.extras.plugin:Plugin"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/adrienbrignon/mkdocs-exporter/issues"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "<4"
+mkdocs-material = "^9.1.11"
+mkdocs-git-revision-date-localized-plugin = "^1.2.0"
+mkdocs-git-authors-plugin = "^0.7.0"
+mkdocs-awesome-pages-plugin = "^2.9.1"
+mkdocs-macros-plugin = "^0.7.0"
+mkdocs-minify-plugin = "^0.6.4"
+mkdocs-redirects = "^1.2.0"
```

### Comparing `mkdocs_exporter-1.1.0/PKG-INFO` & `mkdocs_exporter-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 1.1.0
+Version: 1.2.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -22,30 +22,29 @@
 Requires-Dist: beautifulsoup4 (>=4.12.2)
 Requires-Dist: importlib-metadata (<5.0)
 Requires-Dist: importlib-resources (>=5.0)
 Requires-Dist: libsass (>=0.22.0)
 Requires-Dist: lxml (>=4.9)
 Requires-Dist: mkdocs (>=1.4)
 Requires-Dist: playwright (>=1.33)
-Requires-Dist: weasyprint (>=50.0)
 Project-URL: Bug Tracker, https://github.com/adrienbrignon/mkdocs-exporter/issues
 Project-URL: Repository, https://github.com/adrienbrignon/mkdocs-exporter
 Description-Content-Type: text/markdown
 
 # MkDocs Exporter
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs) that exports your pages to PDF files.
 
 ## Features
 
-- :rocket: **Fast** - PDF documents are generated concurrently!
-- :star: **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
+- 🚀 **Fast** - PDF documents are generated concurrently!
+- ⭐ **Powerful** - it uses a headless browser and some awesome libraries under the hood to generate PDF files
   - [*Paged.js*](https://github.com/pagedjs/pagedjs) polyfills are included by default ([Paged Media](https://www.w3.org/TR/css-page-3/) and [Generated Content](https://www.w3.org/TR/css-gcpm-3/) CSS modules)
   - [*Sass*](https://sass-lang.com/) support (via [`libsass`](https://github.com/sass/libsass-python)) for your stylesheets
-- :paintbrush: **Customizable** - full control over the resulting documents
+- 🎨 **Customizable** - full control over the resulting documents
   - Built for and compatible with [`mkdocs-material`](https://github.com/squidfunk/mkdocs-material)
   - Cover pages with templating support (for instance, with the [`macros`](https://github.com/fralau/mkdocs_macros_plugin) plugin)
   - Define custom scripts and stylesheets to customize your PDF documents
   - Define "buttons" at the top of your documentation pages
 
 ## Prerequisites
 
@@ -100,9 +99,9 @@
 - Ensure full compatibility with other themes than `mkdocs-material`
 - Combine all pages as one PDF
 
 Feel free to request additional features by submitting an issue or by contributing through a pull request.
 
 ## License
 
-This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE.md).
+This project is licensed under the `MIT License (MIT)`, which you can read [here](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

