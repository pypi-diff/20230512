# Comparing `tmp/austin_tui-1.2.2.tar.gz` & `tmp/austin_tui-1.2.3.tar.gz`

## Comparing `austin_tui-1.2.2.tar` & `austin_tui-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 austin_tui-1.2.2/.flake8
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 austin_tui-1.2.2/.travis.yml
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 austin_tui-1.2.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 austin_tui-1.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 austin_tui-1.2.2/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 austin_tui-1.2.2/MANIFEST.in
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 austin_tui-1.2.2/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0   324415 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-flamegraph.gif
--rw-r--r--   0        0        0   153057 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-full-mode.png
--rw-r--r--   0        0        0    69864 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-normal-mode.png
--rw-r--r--   0        0        0   155696 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-save.png
--rw-r--r--   0        0        0    79247 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-threshold.png
--rw-r--r--   0        0        0  1258616 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui-vscode.gif
--rw-r--r--   0        0        0  1291385 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/austin-tui.gif
--rw-r--r--   0        0        0    39254 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/logo.png
--rw-r--r--   0        0        0  1064120 2020-02-02 00:00:00.000000 austin_tui-1.2.2/art/logo.svg
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/__init__.py
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/__main__.py
--rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/adapters.py
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/controller.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/model/__init__.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/model/austin.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/model/system.py
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/view/__init__.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/view/austin.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/view/palette.py
--rw-r--r--   0        0        0    10314 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/view/tui.austinui
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/__init__.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/box.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/catalog.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/command_bar.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/graph.py
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/label.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/markup.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/scroll.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/selector.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/table.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 austin_tui-1.2.2/austin_tui/widgets/window.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 austin_tui-1.2.2/tests/mcurses.py
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 austin_tui-1.2.2/tests/target.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 austin_tui-1.2.2/tests/test_point.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 austin_tui-1.2.2/tests/test_view.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 austin_tui-1.2.2/tests/test_widgets.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 austin_tui-1.2.2/.gitignore
--rw-r--r--   0        0        0    34937 2020-02-02 00:00:00.000000 austin_tui-1.2.2/LICENSE.md
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 austin_tui-1.2.2/README.md
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 austin_tui-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 austin_tui-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 austin_tui-1.2.3/.flake8
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 austin_tui-1.2.3/.travis.yml
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 austin_tui-1.2.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 austin_tui-1.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 austin_tui-1.2.3/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 austin_tui-1.2.3/MANIFEST.in
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 austin_tui-1.2.3/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0   324415 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-flamegraph.gif
+-rw-r--r--   0        0        0   153057 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-full-mode.png
+-rw-r--r--   0        0        0    69864 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-normal-mode.png
+-rw-r--r--   0        0        0   155696 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-save.png
+-rw-r--r--   0        0        0    79247 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-threshold.png
+-rw-r--r--   0        0        0  1258616 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui-vscode.gif
+-rw-r--r--   0        0        0  1291385 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/austin-tui.gif
+-rw-r--r--   0        0        0    39254 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/logo.png
+-rw-r--r--   0        0        0  1064120 2020-02-02 00:00:00.000000 austin_tui-1.2.3/art/logo.svg
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/__init__.py
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/__main__.py
+-rw-r--r--   0        0        0    14456 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/adapters.py
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/controller.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/model/__init__.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/model/austin.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/model/system.py
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/view/__init__.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/view/austin.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/view/palette.py
+-rw-r--r--   0        0        0    10314 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/view/tui.austinui
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/__init__.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/box.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/catalog.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/command_bar.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/graph.py
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/label.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/markup.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/scroll.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/selector.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/table.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 austin_tui-1.2.3/austin_tui/widgets/window.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 austin_tui-1.2.3/tests/mcurses.py
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 austin_tui-1.2.3/tests/target.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 austin_tui-1.2.3/tests/test_point.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 austin_tui-1.2.3/tests/test_view.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 austin_tui-1.2.3/tests/test_widgets.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 austin_tui-1.2.3/.gitignore
+-rw-r--r--   0        0        0    34937 2020-02-02 00:00:00.000000 austin_tui-1.2.3/LICENSE.md
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 austin_tui-1.2.3/README.md
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 austin_tui-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 austin_tui-1.2.3/PKG-INFO
```

### Comparing `austin_tui-1.2.2/.travis.yml` & `austin_tui-1.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/CODE-OF-CONDUCT.md` & `austin_tui-1.2.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/CONTRIBUTING.md` & `austin_tui-1.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/ISSUE_TEMPLATE.md` & `austin_tui-1.2.3/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/PULL_REQUEST_TEMPLATE.md` & `austin_tui-1.2.3/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-flamegraph.gif` & `austin_tui-1.2.3/art/austin-tui-flamegraph.gif`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-full-mode.png` & `austin_tui-1.2.3/art/austin-tui-full-mode.png`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-normal-mode.png` & `austin_tui-1.2.3/art/austin-tui-normal-mode.png`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-save.png` & `austin_tui-1.2.3/art/austin-tui-save.png`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-threshold.png` & `austin_tui-1.2.3/art/austin-tui-threshold.png`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui-vscode.gif` & `austin_tui-1.2.3/art/austin-tui-vscode.gif`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/austin-tui.gif` & `austin_tui-1.2.3/art/austin-tui.gif`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/logo.png` & `austin_tui-1.2.3/art/logo.png`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/art/logo.svg` & `austin_tui-1.2.3/art/logo.svg`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/__init__.py` & `austin_tui-1.2.3/austin_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/__main__.py` & `austin_tui-1.2.3/austin_tui/__main__.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/adapters.py` & `austin_tui-1.2.3/austin_tui/adapters.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/controller.py` & `austin_tui-1.2.3/austin_tui/controller.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/model/__init__.py` & `austin_tui-1.2.3/austin_tui/model/__init__.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/model/austin.py` & `austin_tui-1.2.3/austin_tui/model/austin.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/model/system.py` & `austin_tui-1.2.3/austin_tui/model/system.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/view/__init__.py` & `austin_tui-1.2.3/austin_tui/view/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,18 @@
                     continue
 
                 # Handle user input on the root widget
                 try:
                     event = self.root_widget._win.getkey()
                     if event in self._event_handlers:
                         done, pending = await asyncio.wait(
-                            [_() for _ in self._event_handlers[event]]
+                            [
+                                asyncio.create_task(_())
+                                for _ in self._event_handlers[event]
+                            ]
                         )
                         assert not pending
                         if any(_.result() for _ in done):
                             self.root_widget.refresh()
                 except (KeyError, curses.error):
                     pass
```

### Comparing `austin_tui-1.2.2/austin_tui/view/austin.py` & `austin_tui-1.2.3/austin_tui/view/austin.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/view/palette.py` & `austin_tui-1.2.3/austin_tui/view/palette.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/view/tui.austinui` & `austin_tui-1.2.3/austin_tui/view/tui.austinui`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/__init__.py` & `austin_tui-1.2.3/austin_tui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/box.py` & `austin_tui-1.2.3/austin_tui/widgets/box.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/catalog.py` & `austin_tui-1.2.3/austin_tui/widgets/catalog.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/command_bar.py` & `austin_tui-1.2.3/austin_tui/widgets/command_bar.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/graph.py` & `austin_tui-1.2.3/austin_tui/widgets/graph.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/label.py` & `austin_tui-1.2.3/austin_tui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/markup.py` & `austin_tui-1.2.3/austin_tui/widgets/markup.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/scroll.py` & `austin_tui-1.2.3/austin_tui/widgets/scroll.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/selector.py` & `austin_tui-1.2.3/austin_tui/widgets/selector.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/table.py` & `austin_tui-1.2.3/austin_tui/widgets/table.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/austin_tui/widgets/window.py` & `austin_tui-1.2.3/austin_tui/widgets/window.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/tests/test_point.py` & `austin_tui-1.2.3/tests/test_point.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/tests/test_view.py` & `austin_tui-1.2.3/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/tests/test_widgets.py` & `austin_tui-1.2.3/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/.gitignore` & `austin_tui-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/LICENSE.md` & `austin_tui-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/README.md` & `austin_tui-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/pyproject.toml` & `austin_tui-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `austin_tui-1.2.2/PKG-INFO` & `austin_tui-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: austin-tui
-Version: 1.2.2
+Version: 1.2.3
 Summary: The top-like text-based user interface for Austin
 Project-URL: documentation, https://austin-tui.readthedocs.io
 Project-URL: homepage, https://github.com/P403n1x87/austin-tui
 Project-URL: issues, https://github.com/P403n1x87/austin-tui/issues
 Project-URL: repository, https://github.com/P403n1x87/austin-tui
 Author-email: "Gabriele N. Tornetta" <phoenix1987@gmail.com>
+License-Expression: GPL-3.0-or-later
 License-File: LICENSE.md
 Keywords: development,performance,profiling,testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: austin-tui Version: 1.2.2 Summary: The top-like
+Metadata-Version: 2.1 Name: austin-tui Version: 1.2.3 Summary: The top-like
 text-based user interface for Austin Project-URL: documentation, https://
 austin-tui.readthedocs.io Project-URL: homepage, https://github.com/P403n1x87/
 austin-tui Project-URL: issues, https://github.com/P403n1x87/austin-tui/issues
 Project-URL: repository, https://github.com/P403n1x87/austin-tui Author-email:
 "Gabriele N. Tornetta"
-gmail.com> License-File: LICENSE.md Keywords:
-development,performance,profiling,testing Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >=3.7 Requires-Dist: austin-
-python~=1.1 Requires-Dist: importlib-resources~=5.10 Requires-Dist: lxml~=4.8
-Requires-Dist: windows-curses~=2.1; sys_platform == 'win32' Description-
-Content-Type: text/markdown
+gmail.com> License-Expression: GPL-3.0-or-later License-File: LICENSE.md
+Keywords: development,performance,profiling,testing Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later
+(GPLv3+) Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Requires-Dist:
+austin-python~=1.1 Requires-Dist: importlib-resources~=5.10 Requires-Dist:
+lxml~=4.8 Requires-Dist: windows-curses~=2.1; sys_platform == 'win32'
+Description-Content-Type: text/markdown
 
                                  [Austin TUI]
                    **** A Top-like Interface for Austin ****
                            [GitHub_Actions:_Tests]
  [PyPI] [PyPI_Downloads]   [https://anaconda.org/conda-forge/austin-tui/badges/
 version.svg] [https://anaconda.org/conda-forge/austin-tui/badges/downloads.svg]
```

