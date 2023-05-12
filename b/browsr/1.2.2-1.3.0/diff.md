# Comparing `tmp/browsr-1.2.2.tar.gz` & `tmp/browsr-1.3.0.tar.gz`

## Comparing `browsr-1.2.2.tar` & `browsr-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.2.2/.releaserc.js
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.2.2/mkdocs.yaml
--rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/package-lock.json
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/package.json
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/semantic_release/release_notes.hbs
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/flake8.json
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/mypy.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.2.2/.github/workflows/matchers/python.json
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/__main__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/_base.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/_version.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/code_browser.css
--rw-r--r--   0        0        0    11980 2020-02-02 00:00:00.000000 browsr-1.2.2/browsr/code_browser.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/api_documentation.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/cli.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/contributing.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.2.2/docs/index.md
--rw-r--r--   0        0        0   115617 2020-02-02 00:00:00.000000 browsr-1.2.2/requirements/requirements-dev.txt
--rw-r--r--   0        0        0    79931 2020-02-02 00:00:00.000000 browsr-1.2.2/requirements/requirements-prod.txt
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.2.2/tests/conftest.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 browsr-1.2.2/tests/test_cli.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.2.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.2.2/README.md
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 browsr-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 browsr-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 browsr-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 browsr-1.3.0/.releaserc.js
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 browsr-1.3.0/mkdocs.yaml
+-rw-r--r--   0        0        0   507141 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/package-lock.json
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/package.json
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/semantic_release/release_notes.hbs
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/flake8.json
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/mypy.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 browsr-1.3.0/.github/workflows/matchers/python.json
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/__init__.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/__main__.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_base.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_config.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_utils.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/_version.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/browsr.css
+-rw-r--r--   0        0        0    10712 2020-02-02 00:00:00.000000 browsr-1.3.0/browsr/browsr.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/api_documentation.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/cli.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/contributing.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 browsr-1.3.0/docs/index.md
+-rw-r--r--   0        0        0   118212 2020-02-02 00:00:00.000000 browsr-1.3.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0    82526 2020-02-02 00:00:00.000000 browsr-1.3.0/requirements/requirements-prod.txt
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 browsr-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 browsr-1.3.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 browsr-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 browsr-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 browsr-1.3.0/README.md
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 browsr-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 browsr-1.3.0/PKG-INFO
```

### Comparing `browsr-1.2.2/.pre-commit-config.yaml` & `browsr-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.releaserc.js` & `browsr-1.3.0/.releaserc.js`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/mkdocs.yaml` & `browsr-1.3.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/semantic_release/package-lock.json` & `browsr-1.3.0/.github/semantic_release/package-lock.json`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/semantic_release/release_notes.hbs` & `browsr-1.3.0/.github/semantic_release/release_notes.hbs`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/workflows/lint.yaml` & `browsr-1.3.0/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/workflows/publish.yaml` & `browsr-1.3.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/workflows/release.yaml` & `browsr-1.3.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/.github/workflows/tests.yaml` & `browsr-1.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/browsr/_base.py` & `browsr-1.3.0/browsr/_base.py`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/browsr/code_browser.py` & `browsr-1.3.0/browsr/browsr.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,85 +3,52 @@
 
 This module contains the code browser app for the browsr package.
 This app was inspired by the CodeBrowser example from textual
 """
 
 import json
 import pathlib
-from os import getenv
-from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 import click
 import pandas as pd
 import rich_click
-import rich_pixels
 import upath
 from art import text2art  # type: ignore[import]
-from PIL import Image
 from rich import traceback
 from rich.markdown import Markdown
 from rich.syntax import Syntax
 from rich.traceback import Traceback
+from rich_pixels import Pixels
 from textual.containers import Container, VerticalScroll
 from textual.reactive import var
 from textual.widget import Widget
 from textual.widgets import DataTable, DirectoryTree, Footer, Header, Static
 from upath.implementations.cloud import CloudPath
 
 from browsr._base import (
     BrowsrClickContext,
     BrowsrTextualApp,
     FileSizeError,
     TextualAppContext,
     UniversalDirectoryTree,
     debug_option,
 )
-
-rich_click.rich_click.MAX_WIDTH = 100
-rich_click.rich_click.STYLE_OPTION = "bold green"
-rich_click.rich_click.STYLE_SWITCH = "bold blue"
-rich_click.rich_click.STYLE_METAVAR = "bold red"
-rich_click.rich_click.STYLE_HELPTEXT_FIRST_LINE = "bold blue"
-rich_click.rich_click.STYLE_HELPTEXT = ""
-rich_click.rich_click.STYLE_HEADER_TEXT = "bold green"
-rich_click.rich_click.STYLE_OPTION_DEFAULT = "bold yellow"
-rich_click.rich_click.STYLE_OPTION_HELP = ""
-rich_click.rich_click.STYLE_ERRORS_SUGGESTION = "bold red"
-rich_click.rich_click.STYLE_OPTIONS_TABLE_BOX = "SIMPLE_HEAVY"
-rich_click.rich_click.STYLE_COMMANDS_TABLE_BOX = "SIMPLE_HEAVY"
-
-favorite_themes: List[str] = [
-    "monokai",
-    "material",
-    "dracula",
-    "solarized-light",
-    "one-dark",
-    "solarized-dark",
-    "emacs",
-    "vim",
-    "github-dark",
-    "native",
-    "paraiso-dark",
-]
-
-rich_default_theme = getenv("RICH_THEME", None)
-if rich_default_theme in favorite_themes:
-    assert isinstance(rich_default_theme, str)
-    favorite_themes.remove(rich_default_theme)
-if rich_default_theme is not None:
-    assert isinstance(rich_default_theme, str)
-    favorite_themes.insert(0, rich_default_theme)
+from browsr._config import favorite_themes, image_file_extensions
+from browsr._utils import open_image
+from browsr._version import __application__, __version__
 
 
 class CodeBrowser(BrowsrTextualApp):
     """
     Textual code browser app.
     """
 
-    CSS_PATH = "code_browser.css"
+    TITLE = __application__
+    CSS_PATH = "browsr.css"
     BINDINGS = [
         ("q", "quit", "Quit"),
         ("f", "toggle_files", "Toggle Files"),
         ("t", "theme", "Toggle Theme"),
         ("n", "linenos", "Toggle Line Numbers"),
         ("d", "toggle_dark", "Toggle dark mode"),
     ]
@@ -127,57 +94,51 @@
         yield self.container
         self.footer = Footer()
         yield self.footer
 
     def render_document(
         self,
         document: pathlib.Path,
-    ) -> Union[Syntax, Markdown, DataTable[str]]:
+    ) -> Union[Syntax, Markdown, DataTable[str], Pixels]:
         """
         Render a Code Doc Given Its Extension
 
         Parameters
         ----------
         document: pathlib.Path
             File Path to Render
 
         Returns
         -------
-        Union[Syntax, Markdown, DataTable[str]]
+        Union[Syntax, Markdown, DataTable[str], Pixels]
         """
         if document.suffix == ".md":
             return Markdown(
                 document.read_text(encoding="utf-8"),
                 code_theme=self.rich_themes[self.theme_index],
                 hyperlinks=True,
             )
         elif ".csv" in document.suffixes:
             df = pd.read_csv(document, nrows=500)
             return self.df_to_table(pandas_dataframe=df, table=self.table_view)
         elif document.suffix == ".parquet":
             df = pd.read_parquet(document)[:500]
             return self.df_to_table(pandas_dataframe=df, table=self.table_view)
-        elif document.suffix.lower() in [".png", ".jpg", ".jpeg"]:
+        elif document.suffix.lower() in image_file_extensions:
             screen_width = self.app.size.width / 4
-            with document.open("rb") as buf:
-                image = Image.open(buf)
-                image_width = image.width
-                image_height = image.height
-                size_ratio = image_width / screen_width
-                new_width = min(int(image_width / size_ratio), image_width)
-                new_height = min(int(image_height / size_ratio), image_height)
-                resized = image.resize((new_width, new_height))
-                content = rich_pixels.Pixels.from_image(resized)
+            content = open_image(document=document, screen_width=screen_width)
             return content
         elif document.suffix.lower() in [".json"]:
             code_str = document.read_text()
             code_obj = json.loads(code_str)
             code_lines = json.dumps(code_obj, indent=2).splitlines()
         else:
-            code_lines = document.read_text().splitlines()
+            code_lines = document.read_text(
+                encoding="utf-8", errors="replace"
+            ).splitlines()
         code = "\n".join(code_lines[:1000])
         lexer = Syntax.guess_lexer(str(document), code=code)
         return Syntax(
             code=code,
             lexer=lexer,
             line_numbers=self.linenos,
             word_wrap=False,
@@ -272,15 +233,17 @@
         On Application Mount - See If a File Should be Displayed
         """
         if self.selected_file_path is not None:
             self.show_tree = self.force_show_tree
             self.render_code_page(file_path=self.selected_file_path)
         else:
             self.show_tree = True
-            self.render_code_page(file_path=pathlib.Path.cwd(), content="BROWSR")
+            self.render_code_page(
+                file_path=pathlib.Path.cwd(), content=__application__.upper()
+            )
 
     def on_directory_tree_file_selected(
         self, event: DirectoryTree.FileSelected
     ) -> None:
         """
         Called when the user click a file in the directory tree.
         """
@@ -311,19 +274,20 @@
         """
         if self.selected_file_path is None:
             return
         self.linenos = not self.linenos
         self.render_code_page(file_path=self.selected_file_path, scroll_home=False)
 
 
-@click.command(name="browse", cls=rich_click.rich_command.RichCommand)
+@click.command(name="browsr", cls=rich_click.rich_command.RichCommand)
 @click.argument("path", default=None, required=False, metavar="PATH")
+@click.version_option(version=__version__, prog_name=__application__)
 @click.pass_obj
 @debug_option
-def browse(
+def browsr(
     context: Optional[BrowsrClickContext], path: Optional[str], debug: bool
 ) -> None:
     """
     Start the TUI File Browser
 
     This utility displays a TUI (textual user interface) application. The application
     allows you to visually browse through a repository and display the contents of its
@@ -335,8 +299,8 @@
         context.debug = debug
     config = TextualAppContext(file_path=path, debug=context.debug)
     app = CodeBrowser(config_object=config)
     app.run()
 
 
 if __name__ == "__main__":
-    browse()
+    browsr()
```

### Comparing `browsr-1.2.2/docs/contributing.md` & `browsr-1.3.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/docs/index.md` & `browsr-1.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/requirements/requirements-dev.txt` & `browsr-1.3.0/requirements/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1160,14 +1160,46 @@
     #   msal
 pymdown-extensions==9.11 \
     --hash=sha256:a499191d8d869f30339de86fcf072a787e86c42b6f16f280f5c2cf174182b7f3 \
     --hash=sha256:f7e86c1d3981f23d9dc43294488ecb54abadd05b0be4bf8f0e15efc90f7853ff
     # via
     #   mkdocs-material
     #   mkdocstrings
+pymupdf==1.22.3 \
+    --hash=sha256:01daa4e3c2c1b93d357ba0d747d713ad40e0123b9bdca2395bf166f62dd8f703 \
+    --hash=sha256:07d171255964f5a382e280a95a3148c08fc4ec20bf7907e040cf423cf29afe30 \
+    --hash=sha256:0a2040351a1279fafa1db82e5af50a785eb01dc4e1adb3c98e0abfd6e0a4995f \
+    --hash=sha256:0aff7ba35eb2cc285efea87500dd5ee0aaf94f4bb23a79187f0a74101aba7964 \
+    --hash=sha256:13e90a5301990dafc5bba6bfa32aafca1f35809497c274c9d4af4f4bac2d8870 \
+    --hash=sha256:1f00097e8d2bc46dacdb776aeb810b1c760949f6353abdf6d12e8aefdc95dd35 \
+    --hash=sha256:201c7aecf9530c3a5aa33cd3d6b68e36492ff9ac48cb270d8f18e66654744419 \
+    --hash=sha256:46c7fab408ae4d55c4181f95a76bc4f365f5ead3291f67274d6fe90f1b90c479 \
+    --hash=sha256:48ece127e202470209dc63ad8fa85f3e19ce302f5af02d38c7fc0b5798b9bfa6 \
+    --hash=sha256:4c037d5752efd562ac72e74295dfcc8d8dd406c0f6849054b29d2cbc32237ae0 \
+    --hash=sha256:4d2422dffdb4f1c2c8128e6d151f4de5e722388df276ac165572ad5290ad228a \
+    --hash=sha256:4e0904c9bffdfbb527f4fe293986d74477780f0c98f59fa5b42a95e3e441e1f4 \
+    --hash=sha256:5932564a713bd7d576418070c3dd926cb5800edb4411f48813f7694af7386d3e \
+    --hash=sha256:5ecd928e96e63092571020973aa145b57b75707f3a3df97c742e563112615891 \
+    --hash=sha256:60db199553fc9c88cb9f2afba35f9cd54c042e7a6ea2b151ddcc542e6e75ac61 \
+    --hash=sha256:6eddb0975ddd0bcf39812616b5675c26d740f83b12a39c3b5c4425f02c3da754 \
+    --hash=sha256:90950b328603a83b26c2eb2af0cf5498582fbbab84e86074bbb0ae44d745e2a3 \
+    --hash=sha256:932747941ed4973410244376ba77693253e4387e8e09cf2458bc9133348fc16e \
+    --hash=sha256:9aaf3352d9c443ad7622e70b0ff9124079b09c16a1a1aa3f3dde9ba0e19f32a2 \
+    --hash=sha256:9d9bccfb29cbe3962a858c200376d54e7ba64d6f64c0b972ed5b68ff20157b06 \
+    --hash=sha256:a58af441ce454f33f75a4c93a5f76e4659f2c7c849036180f24ab4b84d9e512f \
+    --hash=sha256:a67f2b12120ce9fe5c3f7cb192643134af2c4e28773a2cd5d56cbe1cae66d1b9 \
+    --hash=sha256:be0803be2709285f17c932ee11d4b7f6d11d3e74e1888094e6310c55e9543673 \
+    --hash=sha256:bf275e5dbf332554f98b469899e5a0928b91cb574a5319aeecf1b7e8075cf4b7 \
+    --hash=sha256:d4ea7b016c4561004b48143b8879e1d888e5ba3a1440e6558ea9a47f0d2e6f65 \
+    --hash=sha256:d4f38ecb9518ba2dc12f5f35f33c64ec5466faf20b833f4ac21a2a4190ffef93 \
+    --hash=sha256:dbffc6cabb0cb20033870bde954bbed1436cf9fce33a14682e283bc893767250 \
+    --hash=sha256:e344632215882b49fd2e28ffb848f55b1b34db6b5389917e4865b4d779cbdb4a \
+    --hash=sha256:ed4a624ffc9bebe5c67fc80e16798300d404089585bcdac14448034bd38c5072 \
+    --hash=sha256:fa934c1a02f1f3bb04e447b95ef5b19d03cb2575fee76d23cb7a6d0c526444e2
+    # via -r requirements.in
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via build
 pytest==7.3.1 \
     --hash=sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362 \
     --hash=sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3
```

### Comparing `browsr-1.2.2/requirements/requirements-prod.txt` & `browsr-1.3.0/requirements/requirements-prod.txt`

 * *Files 1% similar despite different names*

```diff
@@ -868,14 +868,46 @@
     # via rich
 pyjwt[crypto]==2.6.0 \
     --hash=sha256:69285c7e31fc44f68a1feb309e948e0df53259d579295e6cfe2b1792329f05fd \
     --hash=sha256:d83c3d892a77bbb74d3e1a2cfa90afaadb60945205d1095d9221f04466f64c14
     # via
     #   adal
     #   msal
+pymupdf==1.22.3 \
+    --hash=sha256:01daa4e3c2c1b93d357ba0d747d713ad40e0123b9bdca2395bf166f62dd8f703 \
+    --hash=sha256:07d171255964f5a382e280a95a3148c08fc4ec20bf7907e040cf423cf29afe30 \
+    --hash=sha256:0a2040351a1279fafa1db82e5af50a785eb01dc4e1adb3c98e0abfd6e0a4995f \
+    --hash=sha256:0aff7ba35eb2cc285efea87500dd5ee0aaf94f4bb23a79187f0a74101aba7964 \
+    --hash=sha256:13e90a5301990dafc5bba6bfa32aafca1f35809497c274c9d4af4f4bac2d8870 \
+    --hash=sha256:1f00097e8d2bc46dacdb776aeb810b1c760949f6353abdf6d12e8aefdc95dd35 \
+    --hash=sha256:201c7aecf9530c3a5aa33cd3d6b68e36492ff9ac48cb270d8f18e66654744419 \
+    --hash=sha256:46c7fab408ae4d55c4181f95a76bc4f365f5ead3291f67274d6fe90f1b90c479 \
+    --hash=sha256:48ece127e202470209dc63ad8fa85f3e19ce302f5af02d38c7fc0b5798b9bfa6 \
+    --hash=sha256:4c037d5752efd562ac72e74295dfcc8d8dd406c0f6849054b29d2cbc32237ae0 \
+    --hash=sha256:4d2422dffdb4f1c2c8128e6d151f4de5e722388df276ac165572ad5290ad228a \
+    --hash=sha256:4e0904c9bffdfbb527f4fe293986d74477780f0c98f59fa5b42a95e3e441e1f4 \
+    --hash=sha256:5932564a713bd7d576418070c3dd926cb5800edb4411f48813f7694af7386d3e \
+    --hash=sha256:5ecd928e96e63092571020973aa145b57b75707f3a3df97c742e563112615891 \
+    --hash=sha256:60db199553fc9c88cb9f2afba35f9cd54c042e7a6ea2b151ddcc542e6e75ac61 \
+    --hash=sha256:6eddb0975ddd0bcf39812616b5675c26d740f83b12a39c3b5c4425f02c3da754 \
+    --hash=sha256:90950b328603a83b26c2eb2af0cf5498582fbbab84e86074bbb0ae44d745e2a3 \
+    --hash=sha256:932747941ed4973410244376ba77693253e4387e8e09cf2458bc9133348fc16e \
+    --hash=sha256:9aaf3352d9c443ad7622e70b0ff9124079b09c16a1a1aa3f3dde9ba0e19f32a2 \
+    --hash=sha256:9d9bccfb29cbe3962a858c200376d54e7ba64d6f64c0b972ed5b68ff20157b06 \
+    --hash=sha256:a58af441ce454f33f75a4c93a5f76e4659f2c7c849036180f24ab4b84d9e512f \
+    --hash=sha256:a67f2b12120ce9fe5c3f7cb192643134af2c4e28773a2cd5d56cbe1cae66d1b9 \
+    --hash=sha256:be0803be2709285f17c932ee11d4b7f6d11d3e74e1888094e6310c55e9543673 \
+    --hash=sha256:bf275e5dbf332554f98b469899e5a0928b91cb574a5319aeecf1b7e8075cf4b7 \
+    --hash=sha256:d4ea7b016c4561004b48143b8879e1d888e5ba3a1440e6558ea9a47f0d2e6f65 \
+    --hash=sha256:d4f38ecb9518ba2dc12f5f35f33c64ec5466faf20b833f4ac21a2a4190ffef93 \
+    --hash=sha256:dbffc6cabb0cb20033870bde954bbed1436cf9fce33a14682e283bc893767250 \
+    --hash=sha256:e344632215882b49fd2e28ffb848f55b1b34db6b5389917e4865b4d779cbdb4a \
+    --hash=sha256:ed4a624ffc9bebe5c67fc80e16798300d404089585bcdac14448034bd38c5072 \
+    --hash=sha256:fa934c1a02f1f3bb04e447b95ef5b19d03cb2575fee76d23cb7a6d0c526444e2
+    # via -r requirements.in
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
     # via
     #   adal
     #   botocore
     #   pandas
```

### Comparing `browsr-1.2.2/.gitignore` & `browsr-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/LICENSE.txt` & `browsr-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/README.md` & `browsr-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `browsr-1.2.2/pyproject.toml` & `browsr-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
   "fsspec~=2023.1.0",
   "pandas~=1.5.2",
   "rich~=13.3.5",
   "rich-click~=1.5.2",
   "rich-pixels~=2.1.1",
   "textual~=0.22.3",
   "universal-pathlib~=0.0.21",
-  "Pillow>=9.1.0"
+  "Pillow>=9.1.0",
+  "PyMuPDF~=1.22.3"
 ]
 description = "TUI File Browser App"
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "browsr"
 readme = "README.md"
@@ -50,15 +51,15 @@
   "requests~=2.28.2",
   "gcsfs~=2023.1.0",
   "adlfs~=2023.1.0",
   "aiohttp~=3.8.3"
 ]
 
 [project.scripts]
-browsr = "browsr.__main__:browse"
+browsr = "browsr.__main__:browsr"
 
 [project.urls]
 Documentation = "https://github.com/juftin/browsr#readme"
 Issues = "https://github.com/juftin/browsr/issues"
 Source = "https://github.com/juftin/browsr"
 
 [tool.coverage.report]
```

### Comparing `browsr-1.2.2/PKG-INFO` & `browsr-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browsr
-Version: 1.2.2
+Version: 1.3.0
 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme
 Project-URL: Issues, https://github.com/juftin/browsr/issues
 Project-URL: Source, https://github.com/juftin/browsr
 Author-email: Justin Flannery <justin.flannery@juftin.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4.0,>=3.8
 Requires-Dist: art~=5.7
 Requires-Dist: click~=8.1.3
 Requires-Dist: fsspec~=2023.1.0
 Requires-Dist: pandas~=1.5.2
 Requires-Dist: pillow>=9.1.0
+Requires-Dist: pymupdf~=1.22.3
 Requires-Dist: rich-click~=1.5.2
 Requires-Dist: rich-pixels~=2.1.1
 Requires-Dist: rich~=13.3.5
 Requires-Dist: textual~=0.22.3
 Requires-Dist: universal-pathlib~=0.0.21
 Provides-Extra: all
 Requires-Dist: adlfs~=2023.1.0; extra == 'all'
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: browsr Version: 1.2.2 Summary: TUI File Browser App
+Metadata-Version: 2.1 Name: browsr Version: 1.3.0 Summary: TUI File Browser App
 Project-URL: Documentation, https://github.com/juftin/browsr#readme Project-
 URL: Issues, https://github.com/juftin/browsr/issues Project-URL: Source,
 https://github.com/juftin/browsr Author-email: Justin Flannery
 flannery@juftin.com> License-Expression: MIT License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: <4.0,>=3.8 Requires-Dist: art~=5.7 Requires-Dist: click~=8.1.3
 Requires-Dist: fsspec~=2023.1.0 Requires-Dist: pandas~=1.5.2 Requires-Dist:
-pillow>=9.1.0 Requires-Dist: rich-click~=1.5.2 Requires-Dist: rich-
-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist: textual~=0.22.3
-Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all Requires-Dist:
-adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3; extra == 'all'
-Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist: pyarrow~=10.0.0;
-extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all' Requires-Dist:
-s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-Dist:
-pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
+pillow>=9.1.0 Requires-Dist: pymupdf~=1.22.3 Requires-Dist: rich-click~=1.5.2
+Requires-Dist: rich-pixels~=2.1.1 Requires-Dist: rich~=13.3.5 Requires-Dist:
+textual~=0.22.3 Requires-Dist: universal-pathlib~=0.0.21 Provides-Extra: all
+Requires-Dist: adlfs~=2023.1.0; extra == 'all' Requires-Dist: aiohttp~=3.8.3;
+extra == 'all' Requires-Dist: gcsfs~=2023.1.0; extra == 'all' Requires-Dist:
+pyarrow~=10.0.0; extra == 'all' Requires-Dist: requests~=2.28.2; extra == 'all'
+Requires-Dist: s3fs~=2023.1.0; extra == 'all' Provides-Extra: parquet Requires-
+Dist: pyarrow~=10.0.0; extra == 'parquet' Provides-Extra: remote Requires-Dist:
 adlfs~=2023.1.0; extra == 'remote' Requires-Dist: aiohttp~=3.8.3; extra ==
 'remote' Requires-Dist: gcsfs~=2023.1.0; extra == 'remote' Requires-Dist:
 requests~=2.28.2; extra == 'remote' Requires-Dist: s3fs~=2023.1.0; extra ==
 'remote' Description-Content-Type: text/markdown # browsr
                                    [browsr]
 [![browsr Version](https://img.shields.io/pypi/v/
 browsr?color=blue&label=browsr)](https://github.com/juftin/browsr) [![PyPI]
```

