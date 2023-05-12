# Comparing `tmp/jupyterlab_hide_code-3.6.2.tar.gz` & `tmp/jupyterlab_hide_code-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_hide_code-3.6.2.tar", last modified: Mon Mar 20 14:17:11 2023, max compression
+gzip compressed data, was "jupyterlab_hide_code-3.6.3.tar", last modified: Fri May 12 07:23:07 2023, max compression
```

## Comparing `jupyterlab_hide_code-3.6.2.tar` & `jupyterlab_hide_code-3.6.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.531319 jupyterlab_hide_code-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/install.json
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/jest.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.519318 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.523319 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)    21753 2023-03-20 14:17:08.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/build_log.json
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    28459 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-20 14:17:08.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js
--rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.519318 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-20 14:17:11.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-20 14:17:11.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 14:17:11.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 14:17:11.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-20 14:17:11.000000 jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-20 14:17:09.000000 jupyterlab_hide_code-3.6.2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 14:17:11.531319 jupyterlab_hide_code-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/src/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/src/__tests__/jupyterlab_hide_code.spec.ts
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/style/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/style/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/ui-tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/ui-tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/ui-tests/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/ui-tests/playwright.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 14:17:11.527319 jupyterlab_hide_code-3.6.2/ui-tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-20 14:16:05.000000 jupyterlab_hide_code-3.6.2/ui-tests/tests/jupyterlab_hide_code.spec.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jest.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)    21786 2023-05-12 07:23:04.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/build_log.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.131062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    28556 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27376 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-12 07:23:04.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13808 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.127062 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:23:07.000000 jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-12 07:23:05.000000 jupyterlab_hide_code-3.6.3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/src/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/src/__tests__/jupyterlab_hide_code.spec.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.135062 jupyterlab_hide_code-3.6.3/style/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/ui-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/playwright.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 07:23:07.139062 jupyterlab_hide_code-3.6.3/ui-tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 07:21:42.000000 jupyterlab_hide_code-3.6.3/ui-tests/tests/jupyterlab_hide_code.spec.ts
```

### Comparing `jupyterlab_hide_code-3.6.2/LICENSE` & `jupyterlab_hide_code-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/PKG-INFO` & `jupyterlab_hide_code-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_hide_code
-Version: 3.6.2
+Version: 3.6.3
 Summary: A JupyterLab extension to run and hide source code.
 Home-page: https://github.com/osscar-org/jupyterlab-hide-code
 Author: Dou Du
 Author-email: dou.du@epfl.ch
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_hide_code-3.6.2/README.md` & `jupyterlab_hide_code-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/RELEASE.md` & `jupyterlab_hide_code-3.6.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jest.config.js` & `jupyterlab_hide_code-3.6.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/_version.py` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/_version.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/build_log.json` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/build_log.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999107831790125%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^3.6.3'}, '@jupyterlab/application-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^3.6.3'}, "*

 * *      "'@jupyterlab/colla […]*

```diff
@@ -124,435 +124,436 @@
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^0.2.3",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/collaboration": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/collaboration-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^5.6.2",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docprovider": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/docprovider-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/mathjax2-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^4.6.2"
+                            "requiredVersion": "^4.6.3"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^6.6.2",
+                            "requiredVersion": "^6.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/shared-models": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3",
+                            "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^5.6.2",
+                            "requiredVersion": "^5.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^5.6.2"
+                            "requiredVersion": "^5.6.3"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^3.6.2",
+                            "requiredVersion": "^3.6.3",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vdom-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^3.6.2"
+                            "requiredVersion": "^3.6.3"
                         },
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^1.9.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^1.31.3",
+                            "requiredVersion": "^1.31.4",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
                             "requiredVersion": "^1.19.0",
                             "singleton": true
                         },
@@ -594,21 +595,21 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^1.14.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^1.37.1",
+                            "requiredVersion": "^1.37.2",
                             "singleton": true
                         },
                         "jupyterlab-hide-code": {
                             "import": "/home/runner/work/jupyterlab-hide-code/jupyterlab-hide-code/lib/index.js",
                             "singleton": true,
-                            "version": "3.6.1"
+                            "version": "3.6.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^17.0.1",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/package.json` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9568216175359032%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.3', '@jupyterlab/apputils': '3.6.3', "*

 * *                   "'@jupyterlab/docregistry': '3.6.3', '@jupyterlab/notebook': '3.6.3', "*

 * *                   "'@jupyterlab/services': '6.6.3'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.8', '@babel/preset-env': '^7.21.5', "*

 * *                      "'@jupyterlab/builder': '^3.6.3', '@jupyterlab/testutils': '^3.6.3', "*

 * *                      "'@types/jest': '^29.5.1', '@typescript-eslint/eslint-plugin': '^5.59.5',  […]*

```diff
@@ -3,42 +3,42 @@
         "email": "dou.du@epfl.ch",
         "name": "Dou Du"
     },
     "bugs": {
         "url": "https://github.com/osscar-org/jupyterlab-hide-code/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.2",
-        "@jupyterlab/apputils": "3.6.2",
-        "@jupyterlab/docregistry": "3.6.2",
-        "@jupyterlab/notebook": "3.6.2",
-        "@jupyterlab/services": "6.6.2"
+        "@jupyterlab/application": "^3.6.3",
+        "@jupyterlab/apputils": "3.6.3",
+        "@jupyterlab/docregistry": "3.6.3",
+        "@jupyterlab/notebook": "3.6.3",
+        "@jupyterlab/services": "6.6.3"
     },
     "description": "A JupyterLab extension to run and hide source code.",
     "devDependencies": {
-        "@babel/core": "^7.21.3",
-        "@babel/preset-env": "^7.20.2",
-        "@jupyterlab/builder": "^3.6.2",
-        "@jupyterlab/testutils": "^3.6.2",
-        "@types/jest": "^29.5.0",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
-        "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
+        "@babel/core": "^7.21.8",
+        "@babel/preset-env": "^7.21.5",
+        "@jupyterlab/builder": "^3.6.3",
+        "@jupyterlab/testutils": "^3.6.3",
+        "@types/jest": "^29.5.1",
+        "@typescript-eslint/eslint-plugin": "^5.59.5",
+        "@typescript-eslint/parser": "^5.59.5",
+        "eslint": "^8.40.0",
+        "eslint-config-prettier": "^8.8.0",
         "eslint-plugin-prettier": "^4.2.1",
         "jest": "^29.5.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.5",
-        "rimraf": "^4.4.0",
+        "prettier": "^2.8.8",
+        "rimraf": "^5.0.0",
         "stylelint": "^14.16.1",
         "stylelint-config-prettier": "^9.0.5",
         "stylelint-config-recommended": "^9.0.0",
         "stylelint-config-standard": "~29.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^29.0.5",
+        "ts-jest": "^29.1.0",
         "typescript": "4.3.5"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/osscar-org/jupyterlab-hide-code",
@@ -52,15 +52,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8ea1efdce447437d2cdc.js",
+            "load": "static/remoteEntry.10c1996eae06db73781b.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_hide_code/labextension"
     },
     "keywords": [
         "jupyter",
@@ -106,9 +106,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.6.1"
+    "version": "3.6.2"
 }
```

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -375,15 +375,19 @@
             /******/ // creates a new share scope if needed
             /******/
             if (!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};
             /******/ // runs all init snippets from all modules reachable
             /******/
             var scope = __webpack_require__.S[name];
             /******/
-            var warn = (msg) => (typeof console !== "undefined" && console.warn && console.warn(msg));
+            var warn = (msg) => {
+                /******/
+                if (typeof console !== "undefined" && console.warn) console.warn(msg);
+                /******/
+            };
             /******/
             var uniqueName = "jupyterlab-hide-code";
             /******/
             var register = (name, version, factory, eager) => {
                 /******/
                 var versions = scope[name] = scope[name] || {};
                 /******/
@@ -423,15 +427,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-hide-code", "3.6.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-hide-code", "3.6.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -460,15 +464,21 @@
                 /******/
                 scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
-                if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
+                if (scripts.length) {
+                    /******/
+                    var i = scripts.length - 1;
+                    /******/
+                    while (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;
+                    /******/
+                }
                 /******/
             }
             /******/
         }
         /******/ // When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration
         /******/ // or pass an empty string ("") and set the __webpack_public_path__ variable from your code to use your own logic.
         /******/
@@ -633,15 +643,15 @@
             /******/
         };
         /******/
         var getSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
             var version = findSingletonVersionKey(scope, key);
             /******/
-            if (!satisfy(requiredVersion, version)) typeof console !== "undefined" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
+            if (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));
             /******/
             return get(scope[key][version]);
             /******/
         };
         /******/
         var getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
@@ -689,17 +699,23 @@
             /******/
             if (entry) return get(entry);
             /******/
             throw new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
+        var warn = (msg) => {
+            /******/
+            if (typeof console !== "undefined" && console.warn) console.warn(msg);
+            /******/
+        };
+        /******/
         var warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {
             /******/
-            typeof console !== "undefined" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
+            warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));
             /******/
         };
         /******/
         var get = (entry) => {
             /******/
             entry.loaded = 1;
             /******/
@@ -814,17 +830,17 @@
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
             "webpack/sharing/consume/default/@lumino/disposable": () => (loadSingletonVersionCheck("default", "@lumino/disposable", [1, 1, 10, 0])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 2])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 3, 6, 3])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 2]))
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 3, 6, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -971,15 +987,15 @@
                                 /******/
                             }
                             /******/
                         };
                         /******/
                         __webpack_require__.l(url, loadingEnded, "chunk-" + chunkId, chunkId);
                         /******/
-                    } else installedChunks[chunkId] = 0;
+                    }
                     /******/
                 }
                 /******/
             }
             /******/
         };
         /******/
@@ -1064,8 +1080,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-hide-code");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-hide-code"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.8ea1efdce447437d2cdc.js.map
+//# sourceMappingURL=remoteEntry.10c1996eae06db73781b.js.map
```

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js.map` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8311688311688312%*

 * *Differences: {"'file'": "'remoteEntry.10c1996eae06db73781b.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.8ea1efdce447437d2cdc.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC3CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC3KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.10c1996eae06db73781b.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,4MAA4M;WAC1O;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC9KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-hide-code/webpack/container-entry",
         "webpack://jupyterlab-hide-code/webpack/bootstrap",
         "webpack://jupyterlab-hide-code/webpack/runtime/compat get default export",
         "webpack://jupyterlab-hide-code/webpack/runtime/define property getters",
@@ -30,18 +30,18 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"b56891ccedf3d2237715\",\"lib_index_js\":\"d1df23bd25080bd06288\",\"style_index_js\":\"b7522e42ae3acc6f5e3c\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-hide-code:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-hide-code\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-hide-code\", \"3.6.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
-        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,2])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-hide-code\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_hide_code\"] = self[\"webpackChunkjupyterlab_hide_code\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-hide-code\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-hide-code\", \"3.6.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,3])),\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,3,6,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-hide-code\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_hide_code\"] = self[\"webpackChunkjupyterlab_hide_code\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-hide-code\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/PKG-INFO` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-hide-code
-Version: 3.6.2
+Version: 3.6.3
 Summary: A JupyterLab extension to run and hide source code.
 Home-page: https://github.com/osscar-org/jupyterlab-hide-code
 Author: Dou Du
 Author-email: dou.du@epfl.ch
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `jupyterlab_hide_code-3.6.2/jupyterlab_hide_code.egg-info/SOURCES.txt` & `jupyterlab_hide_code-3.6.3/jupyterlab_hide_code.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 jupyterlab_hide_code.egg-info/dependency_links.txt
 jupyterlab_hide_code.egg-info/not-zip-safe
 jupyterlab_hide_code.egg-info/top_level.txt
 jupyterlab_hide_code/labextension/build_log.json
 jupyterlab_hide_code/labextension/package.json
 jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js
 jupyterlab_hide_code/labextension/static/lib_index_js.d1df23bd25080bd06288.js.map
-jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js
-jupyterlab_hide_code/labextension/static/remoteEntry.8ea1efdce447437d2cdc.js.map
+jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js
+jupyterlab_hide_code/labextension/static/remoteEntry.10c1996eae06db73781b.js.map
 jupyterlab_hide_code/labextension/static/style.js
 jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js
 jupyterlab_hide_code/labextension/static/style_index_js.b7522e42ae3acc6f5e3c.js.map
 jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js
 jupyterlab_hide_code/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.b56891ccedf3d2237715.js.map
 src/index.ts
 src/__tests__/jupyterlab_hide_code.spec.ts
```

### Comparing `jupyterlab_hide_code-3.6.2/package.json` & `jupyterlab_hide_code-3.6.3/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9574829931972789%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.3', '@jupyterlab/apputils': '3.6.3', "*

 * *                   "'@jupyterlab/docregistry': '3.6.3', '@jupyterlab/notebook': '3.6.3', "*

 * *                   "'@jupyterlab/services': '6.6.3'}",*

 * * "'devDependencies'": "{'@babel/core': '^7.21.8', '@babel/preset-env': '^7.21.5', "*

 * *                      "'@jupyterlab/builder': '^3.6.3', '@jupyterlab/testutils': '^3.6.3', "*

 * *                      "'@types/jest': '^29.5.1', '@typescript-eslint/eslint-plugin': '^5.59.5',  […]*

```diff
@@ -3,42 +3,42 @@
         "email": "dou.du@epfl.ch",
         "name": "Dou Du"
     },
     "bugs": {
         "url": "https://github.com/osscar-org/jupyterlab-hide-code/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.2",
-        "@jupyterlab/apputils": "3.6.2",
-        "@jupyterlab/docregistry": "3.6.2",
-        "@jupyterlab/notebook": "3.6.2",
-        "@jupyterlab/services": "6.6.2"
+        "@jupyterlab/application": "^3.6.3",
+        "@jupyterlab/apputils": "3.6.3",
+        "@jupyterlab/docregistry": "3.6.3",
+        "@jupyterlab/notebook": "3.6.3",
+        "@jupyterlab/services": "6.6.3"
     },
     "description": "A JupyterLab extension to run and hide source code.",
     "devDependencies": {
-        "@babel/core": "^7.21.3",
-        "@babel/preset-env": "^7.20.2",
-        "@jupyterlab/builder": "^3.6.2",
-        "@jupyterlab/testutils": "^3.6.2",
-        "@types/jest": "^29.5.0",
-        "@typescript-eslint/eslint-plugin": "^5.55.0",
-        "@typescript-eslint/parser": "^5.55.0",
-        "eslint": "^8.36.0",
-        "eslint-config-prettier": "^8.7.0",
+        "@babel/core": "^7.21.8",
+        "@babel/preset-env": "^7.21.5",
+        "@jupyterlab/builder": "^3.6.3",
+        "@jupyterlab/testutils": "^3.6.3",
+        "@types/jest": "^29.5.1",
+        "@typescript-eslint/eslint-plugin": "^5.59.5",
+        "@typescript-eslint/parser": "^5.59.5",
+        "eslint": "^8.40.0",
+        "eslint-config-prettier": "^8.8.0",
         "eslint-plugin-prettier": "^4.2.1",
         "jest": "^29.5.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.8.5",
-        "rimraf": "^4.4.0",
+        "prettier": "^2.8.8",
+        "rimraf": "^5.0.0",
         "stylelint": "^14.16.1",
         "stylelint-config-prettier": "^9.0.5",
         "stylelint-config-recommended": "^9.0.0",
         "stylelint-config-standard": "~29.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^29.0.5",
+        "ts-jest": "^29.1.0",
         "typescript": "4.3.5"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/osscar-org/jupyterlab-hide-code",
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.6.2"
+    "version": "3.6.3"
 }
```

### Comparing `jupyterlab_hide_code-3.6.2/pyproject.toml` & `jupyterlab_hide_code-3.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/setup.py` & `jupyterlab_hide_code-3.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/src/index.ts` & `jupyterlab_hide_code-3.6.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/tsconfig.json` & `jupyterlab_hide_code-3.6.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/ui-tests/README.md` & `jupyterlab_hide_code-3.6.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/ui-tests/jupyter_server_test_config.py` & `jupyterlab_hide_code-3.6.3/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_hide_code-3.6.2/ui-tests/tests/jupyterlab_hide_code.spec.ts` & `jupyterlab_hide_code-3.6.3/ui-tests/tests/jupyterlab_hide_code.spec.ts`

 * *Files identical despite different names*

