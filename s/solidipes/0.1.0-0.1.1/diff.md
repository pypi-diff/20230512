# Comparing `tmp/solidipes-0.1.0.tar.gz` & `tmp/solidipes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipes-0.1.0.tar", max compression
+gzip compressed data, was "solidipes-0.1.1.tar", max compression
```

## Comparing `solidipes-0.1.0.tar` & `solidipes-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1063 2023-04-26 08:20:35.882224 solidipes-0.1.0/README.md
--rw-r--r--   0        0        0     1933 2023-04-26 10:58:20.785076 solidipes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-04-26 10:58:20.785076 solidipes-0.1.0/solidipes/__init__.py
--rw-r--r--   0        0        0      505 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/config.py
--rw-r--r--   0        0        0      446 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/__init__.py
--rw-r--r--   0        0        0      559 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/binary.py
--rw-r--r--   0        0        0      384 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/code_snippet.py
--rw-r--r--   0        0        0     4220 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/data_container.py
--rw-r--r--   0        0        0     2419 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/file.py
--rw-r--r--   0        0        0      386 2023-04-26 08:42:13.550032 solidipes-0.1.0/solidipes/loaders/geof_mesh.py
--rw-r--r--   0        0        0      427 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/image.py
--rw-r--r--   0        0        0      337 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/meshio.py
--rw-r--r--   0        0        0    75141 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/mime_types.py
--rw-r--r--   0        0        0     6583 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/parse_inp.py
--rw-r--r--   0        0        0     5175 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/pyvista_mesh.py
--rw-r--r--   0        0        0     1660 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/table.py
--rw-r--r--   0        0        0      791 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/loaders/text.py
--rw-r--r--   0        0        0        0 2023-04-26 10:58:10.988837 solidipes-0.1.0/solidipes/reports/__init__.py
--rw-r--r--   0        0        0     2559 2023-04-26 09:27:37.848878 solidipes-0.1.0/solidipes/reports/curation.py
--rw-r--r--   0        0        0     6516 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/reports/jtcam.py
--rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.0/solidipes/reports/jtcam_small_logo.png
--rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/reports/jupyter_logo.png
--rw-r--r--   0        0        0    28462 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/reports/web_report.py
--rw-r--r--   0        0        0     2314 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scanners/scanner.py
--rw-r--r--   0        0        0        0 2023-04-26 10:58:10.988837 solidipes-0.1.0/solidipes/scripts/__init__.py
--rw-r--r--   0        0        0     2655 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/download.py
--rw-r--r--   0        0        0     1275 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/generate_report.py
--rw-r--r--   0        0        0     3145 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/init.py
--rw-r--r--   0        0        0      990 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/main.py
--rw-r--r--   0        0        0      817 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/quick_view.py
--rw-r--r--   0        0        0     8574 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/scripts/upload.py
--rw-r--r--   0        0        0     4858 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/utils.py
--rw-r--r--   0        0        0     1528 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewer_backends.py
--rw-r--r--   0        0        0      355 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/__init__.py
--rw-r--r--   0        0        0     1256 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/binary.py
--rw-r--r--   0        0        0      916 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/code_snippet.py
--rw-r--r--   0        0        0      830 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/image.py
--rw-r--r--   0        0        0     3819 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/pyvista_plotter.py
--rw-r--r--   0        0        0     3090 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/table.py
--rw-r--r--   0        0        0     1670 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/text.py
--rw-r--r--   0        0        0     2223 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/viewers/viewer.py
--rw-r--r--   0        0        0     7510 2023-04-26 08:20:35.890224 solidipes-0.1.0/solidipes/zenodo_utils.py
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 solidipes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1165 2023-04-26 11:46:24.627178 solidipes-0.1.1/README.md
+-rw-r--r--   0        0        0     2126 2023-05-12 13:22:06.748835 solidipes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-12 13:22:06.748835 solidipes-0.1.1/solidipes/__init__.py
+-rw-r--r--   0        0        0      505 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/config.py
+-rw-r--r--   0        0        0      446 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/__init__.py
+-rw-r--r--   0        0        0      559 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/binary.py
+-rw-r--r--   0        0        0      384 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/code_snippet.py
+-rw-r--r--   0        0        0     4220 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/data_container.py
+-rw-r--r--   0        0        0     2419 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/file.py
+-rw-r--r--   0        0        0      386 2023-04-26 08:42:13.550032 solidipes-0.1.1/solidipes/loaders/geof_mesh.py
+-rw-r--r--   0        0        0      829 2023-04-28 15:23:01.795502 solidipes-0.1.1/solidipes/loaders/image.py
+-rw-r--r--   0        0        0      337 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/meshio.py
+-rw-r--r--   0        0        0    75141 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/mime_types.py
+-rw-r--r--   0        0        0     6583 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/parse_inp.py
+-rw-r--r--   0        0        0     5175 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/pyvista_mesh.py
+-rw-r--r--   0        0        0     1660 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/table.py
+-rw-r--r--   0        0        0      791 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/loaders/text.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:21:56.464581 solidipes-0.1.1/solidipes/reports/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-26 09:27:37.848878 solidipes-0.1.1/solidipes/reports/curation.py
+-rw-r--r--   0        0        0     6516 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/reports/jtcam.py
+-rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.1/solidipes/reports/jtcam_small_logo.png
+-rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/reports/jupyter_logo.png
+-rw-r--r--   0        0        0    29716 2023-05-08 14:15:43.996185 solidipes-0.1.1/solidipes/reports/web_report.py
+-rw-r--r--   0        0        0     2529 2023-05-08 14:15:43.996185 solidipes-0.1.1/solidipes/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:21:56.464581 solidipes-0.1.1/solidipes/scripts/__init__.py
+-rw-r--r--   0        0        0     2736 2023-05-04 13:43:57.392612 solidipes-0.1.1/solidipes/scripts/download.py
+-rw-r--r--   0        0        0     1275 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/generate_report.py
+-rw-r--r--   0        0        0     3145 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/init.py
+-rw-r--r--   0        0        0      990 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/scripts/main.py
+-rw-r--r--   0        0        0      817 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/scripts/quick_view.py
+-rw-r--r--   0        0        0     8659 2023-05-04 13:43:57.396612 solidipes-0.1.1/solidipes/scripts/upload.py
+-rw-r--r--   0        0        0     4858 2023-05-12 09:53:39.243433 solidipes-0.1.1/solidipes/utils.py
+-rw-r--r--   0        0        0     1532 2023-04-28 10:53:18.883696 solidipes-0.1.1/solidipes/viewer_backends.py
+-rw-r--r--   0        0        0      355 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/__init__.py
+-rw-r--r--   0        0        0     1256 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/binary.py
+-rw-r--r--   0        0        0      916 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/code_snippet.py
+-rw-r--r--   0        0        0      830 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/image.py
+-rw-r--r--   0        0        0     3819 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/pyvista_plotter.py
+-rw-r--r--   0        0        0     3090 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/table.py
+-rw-r--r--   0        0        0     1670 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/text.py
+-rw-r--r--   0        0        0     2223 2023-04-26 08:20:35.890224 solidipes-0.1.1/solidipes/viewers/viewer.py
+-rw-r--r--   0        0        0     7545 2023-05-04 13:43:57.396612 solidipes-0.1.1/solidipes/zenodo_utils.py
+-rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 solidipes-0.1.1/PKG-INFO
```

### Comparing `solidipes-0.1.0/README.md` & `solidipes-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Solidipes 🍄
 
 
+# Solidipes
+
 _Python package for the DCSM project_
 
 [![](https://readthedocs.org/projects/solidipes/badge/?version=latest)](http://solidipes.readthedocs.io/)
 
 See the package's documentation on [Read the Docs](http://solidipes.readthedocs.io/).
 
+<img src="https://gitlab.com/dcsm/solidipes/-/raw/dev/logos/solidipes.jpg" width="200px" height="200px">
+
 
 # Installation
 
 ## As regular user
 
 ```
 pip install solidipes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `solidipes-0.1.0/pyproject.toml` & `solidipes-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidipes"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package for the DCSM project"
 authors = [
 	"Son Pham-Ba <son.phamba@epfl.ch>",
 	"Guillaume Anciaux <guillaume.anciaux@epfl.ch>"
 ]
 license = ""
 readme = "README.md"
@@ -12,36 +12,39 @@
 homepage = "https://gitlab.com/groups/dcsm"
 repository = "https://gitlab.com/dcsm/solidipes"
 documentation = "https://solidipes.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12,!=3.9.7"
 filetype = "^1.2.0"
-pandas = "^1.5.3"
+pandas = ">=1.5.3"
 openpyxl = "^3.1.1"
 meshio = {extras = ["all"], version = "^5.3.4"}
 pyvista = "^0.38.1"
 trame = "^2.2.6"
 streamlit = "^1.17.0"
 stpyvista = "^0.0.6"
 datasize = "^1.0.0"
 ipydatawidgets = "4.3.2"
 streamlit-tree-select = "^0.0.5"
 streamlit-js-eval = "^0.1.5"
-scipy = "^1.10.1"
-sympy = "^1.11.1"
+scipy = ">=1.10.1"
+sympy = ">=1.11.1"
 requests = "^2.28.2"
 pyyaml = "^6.0"
 tqdm = "^4.65.0"
 streamlit-option-menu = "^0.3.2"
 requests-toolbelt = "^0.10.1"
 argcomplete = "^3.0.5"
 streamlit-ace = "^0.1.1"
 markdown = "^3.4.3"
 python-gitlab = "^3.14.0"
+matplotlib = ">=3.7.1"
+svglib = "^1.5.1"
+reportlab = "^3.6.13"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.4"
 build = "^0.10.0"
 pytest = "^7.2.1"
 jupyter = "^1.0.0"
 jupyterlab = "^3.6.1"
@@ -49,20 +52,25 @@
 itkwidgets = "^0.32.5"
 sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.2.0"
 myst-parser = "^0.18.1"
 coverage = "^7.2.1"
 pillow = "^9.4.0"
 pixelmatch = "^0.3.0"
+seleniumbase = "^4.14.2"
+requests-mock = "^1.10.0"
+git-changelog = "^1.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pillow = "^9.5.0"
 pixelmatch = "^0.3.0"
+seleniumbase = "^4.14.2"
+requests-mock = "^1.10.0"
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
```

### Comparing `solidipes-0.1.0/solidipes/loaders/binary.py` & `solidipes-0.1.1/solidipes/loaders/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/data_container.py` & `solidipes-0.1.1/solidipes/loaders/data_container.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/file.py` & `solidipes-0.1.1/solidipes/loaders/file.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/mime_types.py` & `solidipes-0.1.1/solidipes/loaders/mime_types.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/parse_inp.py` & `solidipes-0.1.1/solidipes/loaders/parse_inp.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/pyvista_mesh.py` & `solidipes-0.1.1/solidipes/loaders/pyvista_mesh.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/table.py` & `solidipes-0.1.1/solidipes/loaders/table.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/loaders/text.py` & `solidipes-0.1.1/solidipes/loaders/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/reports/curation.py` & `solidipes-0.1.1/solidipes/reports/curation.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/reports/jtcam.py` & `solidipes-0.1.1/solidipes/reports/jtcam.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/reports/jtcam_small_logo.png` & `solidipes-0.1.1/solidipes/reports/jtcam_small_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/reports/jupyter_logo.png` & `solidipes-0.1.1/solidipes/reports/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/reports/web_report.py` & `solidipes-0.1.1/solidipes/reports/web_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 import fnmatch
 import os
 
 import streamlit as st
 import streamlit.components.v1 as components
 
 ################################################################
-from git import Repo
+from git import InvalidGitRepositoryError, Repo
 from streamlit_ace import st_ace
 from streamlit_tree_select import tree_select
 
+# Must import explicitely from "solidipes" to work in Streamlit
 from solidipes.loaders.file import File
+from solidipes.loaders.mime_types import extension2mime_type, is_valid_extension, mime_types2extensions
 from solidipes.scanners.scanner import Scanner, for_each_file
 from solidipes.utils import (
     get_git_repository,
     get_git_root,
     get_mimes,
+    get_solidipes_directory,
     get_study_metadata,
     set_mimes,
     set_study_metadata,
 )
 
-from ..loaders.mime_types import extension2mime_type, is_valid_extension, mime_types2extensions
-
 ################################################################
 command = "report"
 command_help = "generate report from directory"
 ################################################################
 jupyter_icon_filename = os.path.join(os.path.dirname(__file__), "jupyter_logo.png")
 _jupyter_icon = base64.b64encode(open(jupyter_icon_filename, "rb").read()).decode("utf-8")
 
@@ -106,28 +107,36 @@
 ################################################################
 
 
 class Report:
     def __init__(self):
         self.file_wildcard = "*"
         self.file_error_checkbox = None
+
         self.git_origin = None
-        self.git_root = get_git_root()
-        self.git_repository = get_git_repository()
-        self._set_gitlab_uri()
+        self.git_root = None
+        self.git_repository = None
+        try:
+            self.git_root = get_git_root()
+            self.git_repository = get_git_repository()
+            self._set_gitlab_uri()
+        except InvalidGitRepositoryError:
+            pass
+
         self.scanner = Scanner()
         st.set_page_config(layout="wide")
         self.createLayouts()
 
     def createLayouts(self):
         self.progress_layout = st.sidebar.empty()
         self.update_buttons = st.sidebar.container()
         self.file_selector = st.sidebar.container()
         self.path_selector = st.sidebar.container()
-        self.git_control = st.sidebar.container()
+        if self.git_repository is not None:
+            self.git_control = st.sidebar.container()
         self.jupyter_control = st.sidebar.container()
         self.env_layout = st.sidebar.container()
         self.options = st.sidebar.expander("Options")
 
         self.main_layout = st.container()
         self.logs = self.main_layout.container()
         self.global_message = self.main_layout.container()
@@ -140,15 +149,18 @@
     def scan_files(self, paths):
         found = self.scanner.scan_dirs(paths, recursive=False)
         return found
 
     def _set_gitlab_uri(self):
         dir_path = os.getcwd()
         self.git_repository = Repo(dir_path, search_parent_directories=True)
-        git_origin = [e for e in self.git_repository.remotes.origin.urls][0]
+        remotes = self.git_repository.remotes
+        if "origin" not in remotes:
+            return
+        git_origin = [e for e in remotes.origin.urls][0]
         if git_origin.startswith("git@"):
             git_origin = git_origin.replace("git@", "")
             _split = git_origin.split(":")
             git_origin = "https://" + _split[0] + "/gitlab/" + _split[1]
         self.git_origin = git_origin.replace(".git", "")
 
     def alternative_parser(self, e):
@@ -290,16 +302,17 @@
             col1.download_button(
                 f"Download {os.path.basename(e.file_info.path)}",
                 data=open(e.file_info.path, "rb"),
                 file_name=os.path.basename(e.file_info.path),
                 key="download_" + e.file_info.path,
             )
 
-            url = self.get_file_edit_link(e)
-            col3.markdown(f"[Edit on Gitlab]({url})", unsafe_allow_html=True)
+            if self.git_origin is not None:
+                url = self.get_file_edit_link(e)
+                col3.markdown(f"[Edit on Gitlab]({url})", unsafe_allow_html=True)
 
             self.mime_type_information(e, col4, details_layout)
             with details_layout:
                 e.view()
 
     def scan_directories(self, dir_path):
         paths_to_explore = []
@@ -339,16 +352,18 @@
     def main(self, dir_path):
         show_logs = self.options.checkbox("Show logs (development)", value=False)
         show_zenodo_publish_button = self.options.checkbox("Show zenodo publish (advanced)", value=False)
 
         self._zenodo_info()
         self._zenodo_publish(show_zenodo_publish_button)
         self._environment_info()
-        self._git_info()
-        self._gitlab_issues()
+        if self.git_repository is not None:
+            self._git_info()
+        if self.git_origin is not None:
+            self._gitlab_issues()
 
         st.markdown(
             """
         <style>
         .css-fxzapv {
           justify-content: left;
         }
@@ -498,15 +513,23 @@
                     self.zenodo_upload(token, existing_identifier, sandbox=dry_run)
                 except Exception as e:
                     self.global_message.error(e)
 
     def zenodo_upload(self, access_token, existing_identifier, sandbox=True, new_deposition=False):
         import solidipes.scripts.upload as upload
 
-        _dir = self.git_root
+        if self.git_root is not None:
+            _dir = self.git_root
+        else:
+            try:
+                _dir = get_solidipes_directory()
+            except FileNotFoundError as e:
+                self.global_message.error(e)
+                return
+
         metadata = upload.load_and_check_metadata(_dir)
         archive_path, temp_dir = upload.create_archive(_dir)
         deposition_url, bucket_url, web_url = upload.get_cleaned_deposition_infos(
             new_deposition, existing_identifier, access_token, sandbox
         )
 
         class WebProgressBar:
@@ -618,31 +641,42 @@
                 set_study_metadata(yaml.safe_load(content))
                 self.logger("Rewrote zenodo_content", content)
                 st.experimental_rerun()
 
     def _gitlab_issues(self):
         import gitlab
 
+        # self.git_origin has the form "repo_uri/user_name/project_name"
+        # repo_uri contains multiple "/"
         if "PROJECT_NAME" not in os.environ:
-            repo_uri = "https://renkulab.io/gitlab"
-            project_name = self.git_origin.split(repo_uri + "/guillaume.anciaux/")[1]
-            os.environ["PROJECT_NAME"] = project_name
+            split = self.git_origin.split("/")
+            project_name = split[-1]
+            user_name = split[-2]
+            repo_uri = self.git_origin.split(user_name + "/" + project_name)[0]
             os.environ["REPO_URI"] = repo_uri
+            os.environ["USER_NAME"] = user_name
+            os.environ["PROJECT_NAME"] = project_name
         else:
             project_name = os.environ["PROJECT_NAME"]
-            repo_uri = self.git_origin.split("guillaume.anciaux/" + project_name)[0]
+            repo_uri_and_user_name = self.git_origin.split("/" + project_name)[0]
+            user_name = repo_uri_and_user_name.split("/")[-1]
+            repo_uri = repo_uri_and_user_name.split("/" + user_name)[0]
+            os.environ["USER_NAME"] = user_name
             os.environ["REPO_URI"] = repo_uri
 
         project_name = os.environ["PROJECT_NAME"]
         repo_uri = os.environ["REPO_URI"]
         # self.gitlab_issues.write(project_name)
         # self.gitlab_issues.write(repo_uri)
 
         gl = gitlab.Gitlab(repo_uri)
-        project = gl.projects.get("guillaume.anciaux/" + project_name)
+        try:
+            project = gl.projects.get(user_name + "/" + project_name)
+        except gitlab.GitlabGetError:
+            return
         issues = project.issues.list(get_all=True)
 
         opened_issues = 0
         for issue in issues:
             if issue.state == "open":
                 opened_issues
             if len(issues) == 0:
```

### Comparing `solidipes-0.1.0/solidipes/scanners/scanner.py` & `solidipes-0.1.1/solidipes/scanners/scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from pathlib import Path
 
+from ..config import default_ignore_patterns
 from ..utils import get_ignore, load_file
 
 
 def split_all_path(path):
     head, tail = os.path.split(path)
     _split = [tail]
     path = head
@@ -13,15 +14,19 @@
         _split.insert(0, tail)
         path = head
     return _split
 
 
 class Scanner:
     def __init__(self):
-        self.excluded_patterns = get_ignore()
+        try:
+            # Get ignored patterns from .solidipes
+            self.excluded_patterns = get_ignore()
+        except FileNotFoundError:
+            self.excluded_patterns = default_ignore_patterns.copy()
 
     def scan_dirs(self, paths, recursive=True):
         res = {}
         for p in paths:
             split_p = split_all_path(p)
             _res = res
             for _dir in split_p:
```

### Comparing `solidipes-0.1.0/solidipes/scripts/download.py` & `solidipes-0.1.1/solidipes/scripts/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import os
 
-from ..zenodo_utils import check_response, download_files, get_host_and_id
+from ..zenodo_utils import ZenodoException, check_response, download_files, get_host_and_id
 
 command = "download"
 command_help = "download study from Zenodo"
 
 
 def main(args):
     """Download content from Zenodo"""
@@ -43,14 +43,17 @@
 
         if args.only_metadata:
             return
 
         download_files(record, destination=args.destination, progressbar=True)
 
     except Exception as e:
+        if type(e) is not ZenodoException:
+            raise e
+
         print(e)
         return
 
 
 def process_metadata(metadata):
     """Process metadata to make dataset uploadable again"""
```

### Comparing `solidipes-0.1.0/solidipes/scripts/generate_report.py` & `solidipes-0.1.1/solidipes/scripts/generate_report.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/scripts/init.py` & `solidipes-0.1.1/solidipes/scripts/init.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/scripts/main.py` & `solidipes-0.1.1/solidipes/scripts/main.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/scripts/quick_view.py` & `solidipes-0.1.1/solidipes/scripts/quick_view.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/scripts/upload.py` & `solidipes-0.1.1/solidipes/scripts/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import os
 
 from ..config import study_medatada_mandatory_fields as mandatory_fields
 from ..config import study_metadata_filename, zenodo_infos_filename
 from ..zenodo_utils import (
+    ZenodoException,
     clean_deposition,
     create_deposition,
     get_access_token,
     get_existing_deposition_identifier,
     get_existing_deposition_infos,
     save_deposition_identifier,
     update_deposition_metadata,
@@ -77,14 +78,17 @@
         print("Upload complete.")
         print("Please review your deposition and publish it when ready.")
 
         # Remove temporary file
         temp_dir.cleanup()
 
     except Exception as e:
+        if type(e) is not ZenodoException:
+            raise e
+
         print(e)
 
         if "has been deleted" in str(e) or "does not exist" in str(e):
             print(
                 'Run the command with the "--new-deposition" option to create'
                 ' a new entry, or the "--existing-deposition" option to use'
                 " another existing entry."
```

### Comparing `solidipes-0.1.0/solidipes/utils.py` & `solidipes-0.1.1/solidipes/utils.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewer_backends.py` & `solidipes-0.1.1/solidipes/viewer_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     if backend not in bakends:
         raise TypeError(f'Backend "{backend}" not supported.Choose from {bakends}')
 
     if backend == "python":
         pv.set_jupyter_backend(None)
     elif backend == "jupyter notebook":
         pv.set_jupyter_backend("trame")
-        pv.global_theme.trame.server_proxy_enabled = True
         import os
 
         if "SESSION_URL" in os.environ:
+            pv.global_theme.trame.server_proxy_enabled = True
             session = os.environ["SESSION_URL"]
             session = session.lstrip("https://")
             s = session.split("/")
             s = "/" + "/".join(s[1:] + ["proxy/"])
             pv.global_theme.trame.server_proxy_prefix = s
 
     elif backend == "streamlit":
```

### Comparing `solidipes-0.1.0/solidipes/viewers/binary.py` & `solidipes-0.1.1/solidipes/viewers/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/code_snippet.py` & `solidipes-0.1.1/solidipes/viewers/code_snippet.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/image.py` & `solidipes-0.1.1/solidipes/viewers/image.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/pyvista_plotter.py` & `solidipes-0.1.1/solidipes/viewers/pyvista_plotter.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/table.py` & `solidipes-0.1.1/solidipes/viewers/table.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/text.py` & `solidipes-0.1.1/solidipes/viewers/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/viewers/viewer.py` & `solidipes-0.1.1/solidipes/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.0/solidipes/zenodo_utils.py` & `solidipes-0.1.1/solidipes/zenodo_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 download_chunk_size = 1024
 
 
+class ZenodoException(ValueError):
+    pass
+
+
 def get_host_and_id(identifier):
     """Extract Zenodo host and study ID from string identifier
 
     URL has one of the following forms:
     - https://zenodo.org/record/1234567#xxx
     - https://zenodo.org/deposit/1234567#xxx
     - https://sandbox.zenodo.org/record/1234567#xxx
@@ -56,26 +60,28 @@
         if match:
             return scheme["host"], match.group(1)
 
     raise ValueError(f"Invalid identifier: {identifier}")
 
 
 def check_response(response, expected_status_code, task_description):
-    if response.status_code != expected_status_code:
-        error_message = f"Error {task_description}: {response.status_code}"
-        data = response.json()
-
-        if "message" in data:
-            error_message += f" {data['message']}"
-
-        if "errors" in data:
-            for sub_data in data["errors"]:
-                error_message += f"\n- {sub_data['field']}: {sub_data['message']}"
+    if response.status_code == expected_status_code:
+        return
+
+    error_message = f"Error {task_description}: {response.status_code}"
+    data = response.json()
+
+    if "message" in data:
+        error_message += f" {data['message']}"
+
+    if "errors" in data:
+        for sub_data in data["errors"]:
+            error_message += f"\n- {sub_data['field']}: {sub_data['message']}"
 
-        raise ValueError(error_message)
+    raise ZenodoException(error_message)
 
 
 # Upload methods ##############################################################
 
 
 def get_access_token():
     from getpass import getpass
```

### Comparing `solidipes-0.1.0/PKG-INFO` & `solidipes-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for the DCSM project
 Home-page: https://gitlab.com/groups/dcsm
 Author: Son Pham-Ba
 Author-email: son.phamba@epfl.ch
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,45 +12,51 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argcomplete (>=3.0.5,<4.0.0)
 Requires-Dist: datasize (>=1.0.0,<2.0.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ipydatawidgets (==4.3.2)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: meshio[all] (>=5.3.4,<6.0.0)
 Requires-Dist: openpyxl (>=3.1.1,<4.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
 Requires-Dist: pyvista (>=0.38.1,<0.39.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: reportlab (>=3.6.13,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: stpyvista (>=0.0.6,<0.0.7)
 Requires-Dist: streamlit (>=1.17.0,<2.0.0)
 Requires-Dist: streamlit-ace (>=0.1.1,<0.2.0)
 Requires-Dist: streamlit-js-eval (>=0.1.5,<0.2.0)
 Requires-Dist: streamlit-option-menu (>=0.3.2,<0.4.0)
 Requires-Dist: streamlit-tree-select (>=0.0.5,<0.0.6)
-Requires-Dist: sympy (>=1.11.1,<2.0.0)
+Requires-Dist: svglib (>=1.5.1,<2.0.0)
+Requires-Dist: sympy (>=1.11.1)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: trame (>=2.2.6,<3.0.0)
 Project-URL: Documentation, https://solidipes.readthedocs.io/en/latest/
 Project-URL: Repository, https://gitlab.com/dcsm/solidipes
 Description-Content-Type: text/markdown
 
-# Solidipes 🍄
 
 
+# Solidipes
+
 _Python package for the DCSM project_
 
 [![](https://readthedocs.org/projects/solidipes/badge/?version=latest)](http://solidipes.readthedocs.io/)
 
 See the package's documentation on [Read the Docs](http://solidipes.readthedocs.io/).
 
+<img src="https://gitlab.com/dcsm/solidipes/-/raw/dev/logos/solidipes.jpg" width="200px" height="200px">
+
 
 # Installation
 
 ## As regular user
 
 ```
 pip install solidipes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

