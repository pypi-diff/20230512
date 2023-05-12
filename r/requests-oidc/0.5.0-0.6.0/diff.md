# Comparing `tmp/requests_oidc-0.5.0.tar.gz` & `tmp/requests_oidc-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oidc-0.5.0.tar", max compression
+gzip compressed data, was "requests_oidc-0.6.0.tar", max compression
```

## Comparing `requests_oidc-0.5.0.tar` & `requests_oidc-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1054 2023-01-12 17:44:30.444663 requests_oidc-0.5.0/LICENSE
--rw-r--r--   0        0        0     3079 2023-01-10 20:21:29.006848 requests_oidc-0.5.0/README.rst
--rw-r--r--   0        0        0      890 2023-05-02 20:31:44.315480 requests_oidc-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      399 2023-05-02 17:03:33.755813 requests_oidc-0.5.0/src/requests_oidc/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 17:34:02.957460 requests_oidc-0.5.0/src/requests_oidc/__main__.py
--rw-r--r--   0        0        0     3292 2023-05-02 20:09:15.339987 requests_oidc-0.5.0/src/requests_oidc/cli.py
--rw-r--r--   0        0        0       41 2023-03-09 21:03:13.808063 requests_oidc-0.5.0/src/requests_oidc/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-02 16:29:21.372377 requests_oidc-0.5.0/src/requests_oidc/flows/__init__.py
--rw-r--r--   0        0        0     3285 2023-05-02 20:05:09.358251 requests_oidc-0.5.0/src/requests_oidc/flows/auth_code.py
--rw-r--r--   0        0        0     1174 2023-05-02 20:03:58.532599 requests_oidc-0.5.0/src/requests_oidc/flows/client_credentials.py
--rw-r--r--   0        0        0     4021 2023-05-02 20:04:50.713816 requests_oidc-0.5.0/src/requests_oidc/flows/device_code.py
--rw-r--r--   0        0        0      558 2023-05-02 20:10:42.870029 requests_oidc-0.5.0/src/requests_oidc/flows/utils.py
--rw-r--r--   0        0        0     1097 2023-05-02 19:25:42.426856 requests_oidc-0.5.0/src/requests_oidc/plugins.py
--rw-r--r--   0        0        0      170 2023-05-02 18:00:22.770816 requests_oidc-0.5.0/src/requests_oidc/types.py
--rw-r--r--   0        0        0      104 2023-03-09 21:21:42.347700 requests_oidc-0.5.0/src/requests_oidc/utils/__init__.py
--rw-r--r--   0        0        0      930 2023-05-02 16:52:14.156034 requests_oidc-0.5.0/src/requests_oidc/utils/catcher.py
--rw-r--r--   0        0        0      637 2023-03-21 20:15:54.236655 requests_oidc-0.5.0/src/requests_oidc/utils/discovery.py
--rw-r--r--   0        0        0      220 2023-03-21 20:15:54.236655 requests_oidc-0.5.0/src/requests_oidc/utils/scope.py
--rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 requests_oidc-0.5.0/setup.py
--rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 requests_oidc-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1054 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3079 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/README.rst
+-rw-r--r--   0        0        0      890 2023-05-12 14:40:39.399026 requests_oidc-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/__main__.py
+-rw-r--r--   0        0        0     3292 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/cli.py
+-rw-r--r--   0        0        0       41 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/__init__.py
+-rw-r--r--   0        0        0     3285 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/auth_code.py
+-rw-r--r--   0        0        0     1174 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/client_credentials.py
+-rw-r--r--   0        0        0     4021 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/device_code.py
+-rw-r--r--   0        0        0     1192 2023-05-12 14:40:01.115653 requests_oidc-0.6.0/src/requests_oidc/flows/token.py
+-rw-r--r--   0        0        0      558 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/flows/utils.py
+-rw-r--r--   0        0        0     1402 2023-05-12 14:39:40.251995 requests_oidc-0.6.0/src/requests_oidc/plugins.py
+-rw-r--r--   0        0        0      170 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/types.py
+-rw-r--r--   0        0        0      104 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/catcher.py
+-rw-r--r--   0        0        0      637 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/discovery.py
+-rw-r--r--   0        0        0      220 2023-05-12 13:41:52.727655 requests_oidc-0.6.0/src/requests_oidc/utils/scope.py
+-rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 requests_oidc-0.6.0/PKG-INFO
```

### Comparing `requests_oidc-0.5.0/LICENSE` & `requests_oidc-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/README.rst` & `requests_oidc-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/pyproject.toml` & `requests_oidc-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests-oidc"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Tristan Sweeney <tsweeney@dustidentity.com>"]
 readme = "README.rst"
 packages = [{include = "requests_oidc", from = "src"}]
 repository = "https://github.com/tsweeney-dust/requests-oidc"
 documentation = "https://requests-oidc.readthedocs.io/en/latest/"
 license = "MIT"
```

### Comparing `requests_oidc-0.5.0/src/requests_oidc/cli.py` & `requests_oidc-0.6.0/src/requests_oidc/cli.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/flows/auth_code.py` & `requests_oidc-0.6.0/src/requests_oidc/flows/auth_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/flows/client_credentials.py` & `requests_oidc-0.6.0/src/requests_oidc/flows/client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/flows/device_code.py` & `requests_oidc-0.6.0/src/requests_oidc/flows/device_code.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/flows/utils.py` & `requests_oidc-0.6.0/src/requests_oidc/flows/utils.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/plugins.py` & `requests_oidc-0.6.0/src/requests_oidc/plugins.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,36 +3,45 @@
 import appdirs
 from typing import Optional
 
 
 class PathPlugin:
     """Same as ``make_oidc_session``, but saves/loads token to OS path."""
 
-    def __init__(self, path: Path) -> None:
+    def __init__(self, path: Path, *, noload: bool = False, nostore: bool = False) -> None:
         self.path = path
+        self.noload = noload
+        self.nostore = nostore
 
     def load(self) -> Optional[dict]:
+        if self.noload:
+            return None
+        
         try:
             with self.path.open() as f:
                 return json.load(f)
         except FileNotFoundError:
             return None
 
     def update(self, token: dict) -> None:
+        if self.nostore:
+            return
+        
         with self.path.open("w") as f:
             json.dump(token, f)
 
 
 class OSCachedPlugin(PathPlugin):
     """Same as ``make_oidc_session``, but saves/loads token to the OS-relevant user cache directory (appdata, ~/.cache/..., etc)."""
 
     def __init__(
         self,
         appname: str,
         appauthor: str,
         version: str | None = None,
         filename: str = "token.json",
+        *, noload: bool = False, nostore: bool = False
     ) -> None:
         dirs = appdirs.AppDirs(appname=appname, appauthor=appauthor, version=version)
         dir = Path(dirs.user_cache_dir)
         dir.mkdir(parents=True, exist_ok=True)
-        super().__init__(dir / filename)
+        super().__init__(dir / filename, noload=noload, nostore=nostore)
```

### Comparing `requests_oidc-0.5.0/src/requests_oidc/utils/catcher.py` & `requests_oidc-0.6.0/src/requests_oidc/utils/catcher.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/src/requests_oidc/utils/discovery.py` & `requests_oidc-0.6.0/src/requests_oidc/utils/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oidc-0.5.0/setup.py` & `requests_oidc-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-package_dir = \
-{'': 'src'}
-
-packages = \
-['requests_oidc', 'requests_oidc.flows', 'requests_oidc.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['appdirs>=1.4.4,<2.0.0',
- 'qrcode>=7.4.2,<8.0.0',
- 'requests-oauthlib>=1.3.1,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'typer>=0.9.0,<0.10.0']
-
-entry_points = \
-{'console_scripts': ['requests-oidc-cli = requests_oidc.cli:app']}
-
-setup_kwargs = {
-    'name': 'requests-oidc',
-    'version': '0.5.0',
-    'description': '',
-    'long_description': 'Requests-OIDC\n=================\n\n.. inclusion-marker-do-not-remove\n\nImplements a simple single-function API for creating a requests ``Session`` that\nmanages your OIDC-discovered OAuth2 session for you.\n\n::\n\n   pip install requests-oidc\n\n\n.. list-table::\n\n   * - Package\n     - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|\n   * - build\n     - |checks| |rtd build| |coverage|\n   * - Git\n     - |last commit| |commit activity| |commits since| |issues| |prs|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI\n   \n.. |downloads| image:: https://img.shields.io/pypi/dm/requests-oidc\n   :target: https://pypistats.org/packages/requests-oidc\n   :alt: PyPI - Downloads\n\n.. |formats| image:: https://img.shields.io/pypi/format/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Format\n\n.. |py status| image:: https://img.shields.io/pypi/status/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Status\n\n.. |py impls| image:: https://img.shields.io/pypi/implementation/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Implementation\n\n.. |python| image:: https://img.shields.io/pypi/pyversions/requests-oidc\n   :target: https://pypi.org/project/requests-oidc/\n   :alt: PyPI - Python Version\n\n.. |license| image:: https://img.shields.io/github/license/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub\n\n.. |checks| image:: https://img.shields.io/github/checks-status/tsweeney-dust/requests-oidc/main?logo=github\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub branch checks state\n\n.. |rtd build| image:: https://img.shields.io/readthedocs/requests-oidc\n   :target: https://requests-oidc.readthedocs.io/en/latest/?badge=latest\n   :alt: Read the Docs\n\n.. |coverage| image:: https://coveralls.io/repos/github/tsweeney-dust/requests-oidc/badge.svg?branch=main\n   :target: https://coveralls.io/github/tsweeney-dust/requests-oidc?branch=main\n   :alt: Coverage\n\n.. |last commit| image:: https://img.shields.io/github/last-commit/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub last commit\n\n.. |commit activity| image:: https://img.shields.io/github/commit-activity/m/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commit activity\n\n.. |commits since| image:: https://img.shields.io/github/commits-since/tsweeney-dust/requests-oidc/latest\n   :target: https://github.com/tsweeney-dust/requests-oidc\n   :alt: GitHub commits since latest release (by SemVer)\n\n.. |issues| image:: https://img.shields.io/github/issues/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/issues\n   :alt: GitHub issues\n\n.. |prs| image:: https://img.shields.io/github/issues-pr/tsweeney-dust/requests-oidc\n   :target: https://github.com/tsweeney-dust/requests-oidc/pulls\n   :alt: GitHub pull requests',
-    'author': 'Tristan Sweeney',
-    'author_email': 'tsweeney@dustidentity.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tsweeney-dust/requests-oidc',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: requests-oidc
+Version: 0.6.0
+Summary: 
+Home-page: https://github.com/tsweeney-dust/requests-oidc
+License: MIT
+Author: Tristan Sweeney
+Author-email: tsweeney@dustidentity.com
+Requires-Python: >=3.7,<4
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: qrcode (>=7.4.2,<8.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests-oauthlib (>=1.3.1,<2.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Project-URL: Documentation, https://requests-oidc.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/tsweeney-dust/requests-oidc
+Description-Content-Type: text/x-rst
+
+Requests-OIDC
+=================
+
+.. inclusion-marker-do-not-remove
+
+Implements a simple single-function API for creating a requests ``Session`` that
+manages your OIDC-discovered OAuth2 session for you.
+
+::
+
+   pip install requests-oidc
+
+
+.. list-table::
+
+   * - Package
+     - |pypi| |license| |py status| |formats| |python| |py impls| |downloads|
+   * - build
+     - |checks| |rtd build| |coverage|
+   * - Git
+     - |last commit| |commit activity| |commits since| |issues| |prs|
+
+.. |pypi| image:: https://img.shields.io/pypi/v/requests-oidc
+   :target: https://pypi.org/project/requests-oidc/
+   :alt: PyPI
+   
+.. |downloads| image:: https://img.shields.io/pypi/dm/requests-oidc
+   :target: https://pypistats.org/packages/requests-oidc
+   :alt: PyPI - Downloads
+
+.. |formats| image:: https://img.shields.io/pypi/format/requests-oidc
+   :target: https://pypi.org/project/requests-oidc/
+   :alt: PyPI - Format
+
+.. |py status| image:: https://img.shields.io/pypi/status/requests-oidc
+   :target: https://pypi.org/project/requests-oidc/
+   :alt: PyPI - Status
+
+.. |py impls| image:: https://img.shields.io/pypi/implementation/requests-oidc
+   :target: https://pypi.org/project/requests-oidc/
+   :alt: PyPI - Implementation
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/requests-oidc
+   :target: https://pypi.org/project/requests-oidc/
+   :alt: PyPI - Python Version
+
+.. |license| image:: https://img.shields.io/github/license/tsweeney-dust/requests-oidc
+   :target: https://github.com/tsweeney-dust/requests-oidc
+   :alt: GitHub
+
+.. |checks| image:: https://img.shields.io/github/checks-status/tsweeney-dust/requests-oidc/main?logo=github
+   :target: https://github.com/tsweeney-dust/requests-oidc
+   :alt: GitHub branch checks state
+
+.. |rtd build| image:: https://img.shields.io/readthedocs/requests-oidc
+   :target: https://requests-oidc.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs
+
+.. |coverage| image:: https://coveralls.io/repos/github/tsweeney-dust/requests-oidc/badge.svg?branch=main
+   :target: https://coveralls.io/github/tsweeney-dust/requests-oidc?branch=main
+   :alt: Coverage
+
+.. |last commit| image:: https://img.shields.io/github/last-commit/tsweeney-dust/requests-oidc
+   :target: https://github.com/tsweeney-dust/requests-oidc
+   :alt: GitHub last commit
+
+.. |commit activity| image:: https://img.shields.io/github/commit-activity/m/tsweeney-dust/requests-oidc
+   :target: https://github.com/tsweeney-dust/requests-oidc
+   :alt: GitHub commit activity
+
+.. |commits since| image:: https://img.shields.io/github/commits-since/tsweeney-dust/requests-oidc/latest
+   :target: https://github.com/tsweeney-dust/requests-oidc
+   :alt: GitHub commits since latest release (by SemVer)
+
+.. |issues| image:: https://img.shields.io/github/issues/tsweeney-dust/requests-oidc
+   :target: https://github.com/tsweeney-dust/requests-oidc/issues
+   :alt: GitHub issues
+
+.. |prs| image:: https://img.shields.io/github/issues-pr/tsweeney-dust/requests-oidc
+   :target: https://github.com/tsweeney-dust/requests-oidc/pulls
+   :alt: GitHub pull requests
```

