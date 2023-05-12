# Comparing `tmp/harlequin-0.0.6.tar.gz` & `tmp/harlequin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.6.tar", max compression
+gzip compressed data, was "harlequin-0.0.7.tar", max compression
```

## Comparing `harlequin-0.0.6.tar` & `harlequin-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1068 2023-05-09 19:58:18.252669 harlequin-0.0.6/LICENSE
--rw-r--r--   0        0        0     1473 2023-05-09 19:58:18.252669 harlequin-0.0.6/README.md
--rw-r--r--   0        0        0     1438 2023-05-09 19:58:18.260669 harlequin-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/__main__.py
--rw-r--r--   0        0        0      336 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/cli.py
--rw-r--r--   0        0        0       53 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0     2647 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/app.css
--rw-r--r--   0        0        0     8744 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/app.py
--rw-r--r--   0        0        0      812 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/components/__init__.py
--rw-r--r--   0        0        0      913 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/components/code_editor.py
--rw-r--r--   0        0        0     1125 2023-05-09 19:58:18.260669 harlequin-0.0.6/src/harlequin/tui/components/error_modal.py
--rw-r--r--   0        0        0      672 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/components/filename_modal.py
--rw-r--r--   0        0        0     3126 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/components/key_handlers.py
--rw-r--r--   0        0        0     2480 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/components/results_viewer.py
--rw-r--r--   0        0        0     3001 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/components/schema_viewer.py
--rw-r--r--   0        0        0    13674 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/components/textarea.py
--rw-r--r--   0        0        0      661 2023-05-09 19:58:18.264670 harlequin-0.0.6/src/harlequin/tui/utils.py
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 harlequin-0.0.6/setup.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 harlequin-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-12 18:43:06.953114 harlequin-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1473 2023-05-12 18:43:06.953114 harlequin-0.0.7/README.md
+-rw-r--r--   0        0        0     1438 2023-05-12 18:43:06.961115 harlequin-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/__main__.py
+-rw-r--r--   0        0        0      336 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/cli.py
+-rw-r--r--   0        0        0       53 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     8744 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      812 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1125 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0     3126 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/key_handlers.py
+-rw-r--r--   0        0        0     2480 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3001 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0    15911 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/textarea.py
+-rw-r--r--   0        0        0      661 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/utils.py
+-rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 harlequin-0.0.7/setup.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 harlequin-0.0.7/PKG-INFO
```

### Comparing `harlequin-0.0.6/LICENSE` & `harlequin-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/README.md` & `harlequin-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/pyproject.toml` & `harlequin-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
```

### Comparing `harlequin-0.0.6/src/harlequin/tui/app.css` & `harlequin-0.0.7/src/harlequin/tui/app.css`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/app.py` & `harlequin-0.0.7/src/harlequin/tui/app.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/__init__.py` & `harlequin-0.0.7/src/harlequin/tui/components/__init__.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/code_editor.py` & `harlequin-0.0.7/src/harlequin/tui/components/code_editor.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/error_modal.py` & `harlequin-0.0.7/src/harlequin/tui/components/error_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/filename_modal.py` & `harlequin-0.0.7/src/harlequin/tui/components/filename_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/key_handlers.py` & `harlequin-0.0.7/src/harlequin/tui/components/key_handlers.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/results_viewer.py` & `harlequin-0.0.7/src/harlequin/tui/components/results_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/schema_viewer.py` & `harlequin-0.0.7/src/harlequin/tui/components/schema_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/src/harlequin/tui/components/textarea.py` & `harlequin-0.0.7/src/harlequin/tui/components/textarea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Tuple, Union
 
 from rich.console import RenderableType
 from rich.syntax import Syntax
 from sqlfmt.api import Mode, format_string
 from sqlfmt.exception import SqlfmtError
 from textual import events
 from textual.app import ComposeResult
@@ -19,14 +19,15 @@
 
 BRACKETS = {
     "(": ")",
     "[": "]",
     "{": "}",
 }
 CLOSERS = {'"': '"', "'": "'", **BRACKETS}
+TAB_SIZE = 4
 
 
 class TextInput(Static, can_focus=True):
     BINDINGS = [
         ("ctrl+`", "format", "Format Query"),
         Binding("ctrl+@", "format", "Format Query", show=False),
         ("ctrl+s", "save", "Save Query"),
@@ -81,14 +82,16 @@
         self.cursor_visible = True
         self.blink_timer.reset()
         selection_before = self.selection_anchor
 
         # set selection_anchor if it's unset
         if event.key == "shift+delete":
             pass  # todo: shift+delete should delete the whole line
+        if event.key == "ctrl+underscore":
+            pass  # this comments out a section, which should maintain selection
         elif event.key == "ctrl+a":
             self.selection_anchor = Cursor(0, 0)
         elif selection_before is None and "shift" in event.key:
             self.selection_anchor = self.cursor
         elif selection_before is not None and "shift" not in event.key:
             self.selection_anchor = None
 
@@ -137,27 +140,57 @@
         elif event.key in ("home", "shift+home"):
             event.stop()
             self.cursor = Cursor(self.cursor.lno, 0)
         elif event.key in ("end", "shift+end"):
             event.stop()
             self.cursor = Cursor(self.cursor.lno, len(self.lines[self.cursor.lno]) - 1)
         elif event.key == "ctrl+home":
+            event.stop()
             self.cursor = Cursor(0, 0)
         elif event.key in ("ctrl+end", "ctrl+a"):
+            event.stop()
             self.cursor = Cursor(lno=len(self.lines) - 1, pos=len(self.lines[-1]) - 1)
+        elif event.key == "ctrl+underscore":  # actually ctrl+/
+            event.stop()
+            lines, first, last = self._get_selected_lines(selection_before)
+            stripped_lines = [line.lstrip() for line in lines]
+            indents = [len(line) - len(line.lstrip()) for line in lines]
+            if all([line.startswith("-- ") for line in stripped_lines]):
+                no_comment_lines = [line[3:] for line in stripped_lines]
+                self.lines[first.lno : last.lno + 1] = [
+                    f"{' ' * indent}{stripped_line}"
+                    for indent, stripped_line in zip(indents, no_comment_lines)
+                ]
+            else:
+                self.lines[first.lno : last.lno + 1] = [
+                    f"{' ' * indent}-- {stripped_line}"
+                    for indent, stripped_line in zip(indents, stripped_lines)
+                ]
         elif event.key == "enter":
             event.stop()
-            anchor = selection_before or self.cursor
-            first = min(anchor, self.cursor)
-            last = max(anchor, self.cursor)
-            old_lines = self.lines[first.lno : last.lno + 1]
+            old_lines, first, last = self._get_selected_lines(selection_before)
             head = f"{old_lines[0][:first.pos]} "
             tail = f"{old_lines[-1][last.pos:]}"
-            self.lines[first.lno : last.lno + 1] = [head, tail]
-            self.cursor = Cursor(first.lno + 1, 0)
+            indent = len(old_lines[0]) - len(old_lines[0].lstrip())
+            char_before = self._get_character_before_cursor(first)
+            if char_before in BRACKETS and BRACKETS[
+                char_before
+            ] == self._get_character_at_cursor(last):
+                self.lines[first.lno : last.lno + 1] = [
+                    head,
+                    f"{' ' * (indent+TAB_SIZE)} ",
+                    f"{' ' * indent}{tail.lstrip()}",
+                ]
+                self.cursor = Cursor(first.lno + 1, indent + TAB_SIZE)
+            else:
+                self.lines[first.lno : last.lno + 1] = [
+                    head,
+                    f"{' ' * indent}{tail.lstrip()} ",
+                ]
+                self.cursor = Cursor(first.lno + 1, min(first.pos, indent))
         elif event.key == "delete":
             event.stop()
             if selection_before is None:
                 anchor = self.cursor
                 cursor = handle_arrow("right", self.lines, self.cursor)
             else:
                 anchor = selection_before
@@ -198,15 +231,15 @@
                 (self.cursor.lno + 1, self.cursor.pos),
                 (self.cursor.lno + 1, self.cursor.pos + 1),
             )
         if self.selection_anchor is not None:
             first = min(self.selection_anchor, self.cursor)
             second = max(self.selection_anchor, self.cursor)
             syntax.stylize_range(
-                "on #666666",
+                "on #444444",
                 # rows are 1-indexed
                 (first.lno + 1, first.pos),
                 (second.lno + 1, second.pos),
             )
         return syntax
 
     def _scroll_to_cursor(self) -> None:
@@ -217,14 +250,31 @@
         assert isinstance(parent, TextContainer)
         return parent.window_region.height
 
     def _toggle_cursor(self) -> None:
         self.cursor_visible = not self.cursor_visible
         self.update(self._content)
 
+    def _get_selected_lines(
+        self,
+        maybe_anchor: Union[Cursor, None],
+        maybe_cursor: Union[Cursor, None] = None,
+    ) -> Tuple[List[str], Cursor, Cursor]:
+        """
+        Returns a tuple of:
+         - the lines between (inclusive) the optional selection anchor and the cursor,
+         - the first of either the cursor or anchor
+         - the last of either the cursor or anchor
+        """
+        cursor = maybe_cursor or self.cursor
+        anchor = maybe_anchor or cursor
+        first = min(anchor, cursor)
+        last = max(anchor, cursor)
+        return self.lines[first.lno : last.lno + 1], first, last
+
     def _insert_character_at_cursor(self, character: str, cursor: Cursor) -> None:
         line = self.lines[cursor.lno]
         new_line = f"{line[:cursor.pos]}{character}{line[cursor.pos:]}"
         self.lines[cursor.lno] = new_line
 
     def _insert_characters_around_selection(
         self, character: str, anchor: Cursor, cursor: Cursor
@@ -251,17 +301,15 @@
                 character in CLOSERS
                 and self.cursor.pos == len(self.lines[self.cursor.lno]) - 1
                 and (prev is None or prev == " " or character in BRACKETS)
             ):
                 self._insert_character_at_cursor(CLOSERS[character], self.cursor)
 
     def _delete_selection(self, anchor: Cursor, cursor: Cursor) -> None:
-        first = min(anchor, cursor)
-        last = max(anchor, cursor)
-        old_lines = self.lines[first.lno : last.lno + 1]
+        old_lines, first, last = self._get_selected_lines(anchor, maybe_cursor=cursor)
         head = f"{old_lines[0][:first.pos]}"
         tail = f"{old_lines[-1][last.pos:]}"
         self.lines[first.lno : last.lno + 1] = [f"{head}{tail}"]
         self.cursor = Cursor(first.lno, first.pos)
 
     def _get_character_at_cursor(self, cursor: Cursor) -> str:
         return self.lines[cursor.lno][cursor.pos]
```

### Comparing `harlequin-0.0.6/src/harlequin/tui/utils.py` & `harlequin-0.0.7/src/harlequin/tui/utils.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.6/setup.py` & `harlequin-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'textual>=0.22.3,<0.25.0']
 
 entry_points = \
 {'console_scripts': ['harlequin = harlequin.cli:harlequin']}
 
 setup_kwargs = {
     'name': 'harlequin',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'A Text User Interface for DuckDB',
     'long_description': '# harlequin\nA Terminal-based SQL IDE for DuckDB.\n\n![harlequin TUI](harlequinv004.gif)\n\n(A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)\n\n![harlequin duck](harlequin.jpg)\n\n## Installing Harlequin\n\nUse `pip` or `pipx`:\n\n```bash\npipx install harlequin\n```\n\n> **Tip:**\n>\n> You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:\n> - `pipx run harlequin --help`\n> - `pipx run harlequin ./my.duckdb`\n\n## Using Harlequin\n\nTo open a DuckDB database file:\n\n```bash\nharlequin "path/to/duck.db"\n```\n\nTo open an in-memory DuckDB session, run Harlequin with no arguments:\n\n```bash\nharlequin\n```\n\nWhen Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.\n\nTo run a query, enter your code in the main textarea, then press Ctrl+Enter. You should see the data appear in the pane below.\n\nYou can press Tab or use your mouse to change the focus between the panes.\n\nWhen the focus is on the data pane, you can use your arrow keys or mouse to select different cells.\n\nPress Ctrl+c to quit and return to your shell.\n\n### Running Harlequin in a Container\n\nWithout a database file:\n\n```bash\ndocker run ghcr.io/tconbeer/harlequin:latest\n```\n\nMounting a database file `./foo.db` into the container\'s working directory, `/data`:\n\n```bash\ndocker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db\n```\n',
     'author': 'Ted Conbeer',
     'author_email': 'tconbeer@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `harlequin-0.0.6/PKG-INFO` & `harlequin-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

