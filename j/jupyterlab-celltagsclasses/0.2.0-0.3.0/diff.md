# Comparing `tmp/jupyterlab_celltagsclasses-0.2.0.tar.gz` & `tmp/jupyterlab_celltagsclasses-0.3.0.tar.gz`

## Comparing `jupyterlab_celltagsclasses-0.2.0.tar` & `jupyterlab_celltagsclasses-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.eslintrc.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.gitattributes
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/install.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/package.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/package.json.version
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/release.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/tsconfig.json
--rw-r--r--   0        0        0   208796 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/yarn.lock
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/examples/test.ipynb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/_version.py
--rw-r--r--   0        0        0    21418 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/build_log.json
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/package.json
--rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js
--rw-r--r--   0        0        0    22193 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js.map
--rw-r--r--   0        0        0     6351 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.e0bf585461963e3d1e28.js.map
--rw-r--r--   0        0        0    26439 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.cc30540db9a44cea877f.js.map
--rw-r--r--   0        0        0    27740 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js
--rw-r--r--   0        0        0    26652 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style.js
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
--rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
--rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/media/screenshot.png
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/index.ts
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/metadata.ts
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath-test.js
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath-test.ts
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath.js
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/src/xpath.ts
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/LICENSE
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/README.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5709 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.eslintrc.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.gitattributes
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/install.json
+-rw-r--r--   0        0        0   164226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package-lock.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package.json.version
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/release-to-pypi.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0   208738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/yarn.lock
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/examples/test.ipynb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/_version.py
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/build_log.json
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/package.json
+-rw-r--r--   0        0        0    25055 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js
+-rw-r--r--   0        0        0    23941 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map
+-rw-r--r--   0        0        0    27701 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js
+-rw-r--r--   0        0        0    26608 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style.js
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
+-rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/media/screenshot.png
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/apply_on_cells.ts
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/index.ts
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/metadata.ts
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath-test.js
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath-test.ts
+-rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath.js
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath.ts
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/PKG-INFO
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/.eslintrc.js` & `jupyterlab_celltagsclasses-0.3.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/RELEASE.md` & `jupyterlab_celltagsclasses-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/package.json` & `jupyterlab_celltagsclasses-0.3.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9650297619047619%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0-rc.1', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0-rc.1', '@jupyterlab/notebook': '^4.0.0-rc.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0-rc.1'}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -3,22 +3,22 @@
         "email": "thierry.parmentelat@inria.fr",
         "name": "Thierry Parmentelat"
     },
     "bugs": {
         "url": "https://github.com/parmentelat/jupyterlab-celltagsclasses/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0-rc.0",
-        "@jupyterlab/apputils": "^4.0.0-rc.0",
-        "@jupyterlab/notebook": "^4.0.0-rc.0",
+        "@jupyterlab/application": "^4.0.0-rc.1",
+        "@jupyterlab/apputils": "^4.0.0-rc.1",
+        "@jupyterlab/notebook": "^4.0.0-rc.1",
         "@lumino/widgets": "^2.0.1"
     },
     "description": "JLAB extension to add classes to cells based on their tags",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-rc.0",
+        "@jupyterlab/builder": "^4.0.0-rc.1",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
@@ -90,9 +90,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/package.json.version` & `jupyterlab_celltagsclasses-0.3.0/package.json.version`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9650297619047619%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0-rc.1', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0-rc.1', '@jupyterlab/notebook': '^4.0.0-rc.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0-rc.1'}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -3,22 +3,22 @@
         "email": "thierry.parmentelat@inria.fr",
         "name": "Thierry Parmentelat"
     },
     "bugs": {
         "url": "https://github.com/parmentelat/jupyterlab-celltagsclasses/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0-rc.0",
-        "@jupyterlab/apputils": "^4.0.0-rc.0",
-        "@jupyterlab/notebook": "^4.0.0-rc.0",
+        "@jupyterlab/application": "^4.0.0-rc.1",
+        "@jupyterlab/apputils": "^4.0.0-rc.1",
+        "@jupyterlab/notebook": "^4.0.0-rc.1",
         "@lumino/widgets": "^2.0.1"
     },
     "description": "JLAB extension to add classes to cells based on their tags",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-rc.0",
+        "@jupyterlab/builder": "^4.0.0-rc.1",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
@@ -90,9 +90,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/release.sh` & `jupyterlab_celltagsclasses-0.3.0/release-to-pypi.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/tsconfig.json` & `jupyterlab_celltagsclasses-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/yarn.lock` & `jupyterlab_celltagsclasses-0.3.0/yarn.lock`

 * *Files 3% similar despite different names*

```diff
@@ -29,39 +29,39 @@
     chalk: ^2.0.0
     js-tokens: ^4.0.0
   checksum: 92d8ee61549de5ff5120e945e774728e5ccd57fd3b2ed6eace020ec744823d4a98e242be1453d21764a30a14769ecd62170fba28539b211799bbaf232bbb2789
   languageName: node
   linkType: hard
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1":
-  version: 6.6.0
-  resolution: "@codemirror/autocomplete@npm:6.6.0"
+  version: 6.7.0
+  resolution: "@codemirror/autocomplete@npm:6.7.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.6.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 01d5d81e46d179da2c742020d7cb7c97cceb1af5772ac1fbf81abfe18408d694a78851234137fabadce1ed8f829d598a2e9c4b6fbd9632a813fa72772e458f9d
+  checksum: 7e644dcc43d9d389c1ef6ab0430b42933dc20a8254a993e5202b3b0709a4f1bfd0a879a2e726d80823e7e602abbcade5bca955bca0f484cb55a7e6b0cd2d0d25
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
-  version: 6.2.3
-  resolution: "@codemirror/commands@npm:6.2.3"
+  version: 6.2.4
+  resolution: "@codemirror/commands@npm:6.2.4"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: e6b7d07818d6df4372a272539b84a256e651cfa3416a33f9e1859f2ced0f6e3c944e0c40c2c407dcd5b13ffab2931d4e5ea5952db439837071de336e7a31c722
+  checksum: 468895fa19ff0554181b698c81f850820de5c0289cab92c44392fb127286f09ca72b921d6ea4353b70b616a4fd0c3667d86b6f917202a3ad2e196eb7b581f7b6
   languageName: node
   linkType: hard
 
 "@codemirror/lang-cpp@npm:^6.0.2":
   version: 6.0.2
   resolution: "@codemirror/lang-cpp@npm:6.0.2"
   dependencies:
@@ -270,21 +270,21 @@
   version: 6.2.0
   resolution: "@codemirror/state@npm:6.2.0"
   checksum: fdc99c773dc09c700dd02bf918f06132aa8d3069c262cc4eb6ca5c810ce24ae2d7e90719ae7630a8158fd263018de6d40bd78f312e6bfba754e737b64e6c6b3d
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.2.2, @codemirror/view@npm:^6.6.0, @codemirror/view@npm:^6.9.6":
-  version: 6.10.0
-  resolution: "@codemirror/view@npm:6.10.0"
+  version: 6.11.1
+  resolution: "@codemirror/view@npm:6.11.1"
   dependencies:
     "@codemirror/state": ^6.1.4
     style-mod: ^4.0.0
     w3c-keyname: ^2.2.4
-  checksum: ff6a370319fc62a70af062e187b28c0ae2f9df3edd29fd8096129b3be76b46ccfebb8baa1fef36a7a1b73977e5d54b036e3a4b52bd0b0bc70d82ffb8842541f2
+  checksum: a7e6ebb1f31b3d998018adcd031edb19dcf4018b6524ad82ca4fe1cc65e902626307c1f7c2875fcd4c72c16fa04886c2309c50ef5c9ebfbce3285c514ed53acb
   languageName: node
   linkType: hard
 
 "@csstools/selector-specificity@npm:^2.0.2":
   version: 2.2.0
   resolution: "@csstools/selector-specificity@npm:2.2.0"
   peerDependencies:
@@ -308,41 +308,41 @@
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || >=8.0.0
   checksum: cdfe3ae42b4f572cbfb46d20edafe6f36fc5fb52bf2d90875c58aefe226892b9677fef60820e2832caf864a326fe4fc225714c46e8389ccca04d5f9288aabd22
   languageName: node
   linkType: hard
 
 "@eslint-community/regexpp@npm:^4.4.0":
-  version: 4.5.0
-  resolution: "@eslint-community/regexpp@npm:4.5.0"
-  checksum: 99c01335947dbd7f2129e954413067e217ccaa4e219fe0917b7d2bd96135789384b8fedbfb8eb09584d5130b27a7b876a7150ab7376f51b3a0c377d5ce026a10
+  version: 4.5.1
+  resolution: "@eslint-community/regexpp@npm:4.5.1"
+  checksum: 6d901166d64998d591fab4db1c2f872981ccd5f6fe066a1ad0a93d4e11855ecae6bfb76660869a469563e8882d4307228cebd41142adb409d182f2966771e57e
   languageName: node
   linkType: hard
 
-"@eslint/eslintrc@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "@eslint/eslintrc@npm:2.0.2"
+"@eslint/eslintrc@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "@eslint/eslintrc@npm:2.0.3"
   dependencies:
     ajv: ^6.12.4
     debug: ^4.3.2
-    espree: ^9.5.1
+    espree: ^9.5.2
     globals: ^13.19.0
     ignore: ^5.2.0
     import-fresh: ^3.2.1
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
-  checksum: cfcf5e12c7b2c4476482e7f12434e76eae16fcd163ee627309adb10b761e5caa4a4e52ed7be464423320ff3d11eca5b50de5bf8be3e25834222470835dd5c801
+  checksum: ddc51f25f8524d8231db9c9bf03177e503d941a332e8d5ce3b10b09241be4d5584a378a529a27a527586bfbccf3031ae539eb891352033c340b012b4d0c81d92
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.39.0":
-  version: 8.39.0
-  resolution: "@eslint/js@npm:8.39.0"
-  checksum: 63fe36e2bfb5ff5705d1c1a8ccecd8eb2f81d9af239713489e767b0e398759c0177fcc75ad62581d02942f2776903a8496d5fae48dc2d883dff1b96fcb19e9e2
+"@eslint/js@npm:8.40.0":
+  version: 8.40.0
+  resolution: "@eslint/js@npm:8.40.0"
+  checksum: e84936b8ebd1c8fd90e860182e95d1404006da4cbca722b14950b298aeeca102b080aa9b62c8e69f90824ec54e19f1ba79b239046223624d1414ee82e8e628ac
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
@@ -443,88 +443,88 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: 739f9630940466b3cfcd7b742dd06479f81772ca13f863d057af0bbb5e318829506969066ab72977e7c721644982b5c8f88cf44e1ae81955ed1c27e87632d1f2
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.0-beta.2":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/application@npm:4.0.0-rc.0"
+"@jupyterlab/application@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/application@npm:4.0.0-rc.1"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: a287f484f412c02ba67e1b87364750b5457a73e5c4a547cf197e580ed591c32df1ae58b6012af817e78c223ca3e007009805eccfb1836cf6366c08a51edfc5f3
+  checksum: bd57439f4b7eef3e3f8d535bfe83527c1033166da1430e524849e264237199908b3295a56b2941ada4dbdc49d6091291b5f10140d64fb24e10c6e6df2d2d8e3b
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.0.0-beta.2, @jupyterlab/apputils@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/apputils@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+"@jupyterlab/apputils@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/apputils@npm:4.0.0-rc.1"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/settingregistry": ^4.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
+    "@jupyterlab/statusbar": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: 1236e35b5a52c0de2f3895680e1e885df32704f84a926d8cd221c0da0e44935e57c47de128427f23f76aee4f80658d9b64cd36dc75b11417a1b68f0eaaaef526
+  checksum: 2692b4ebaa5f62b64a9ebf673bd417d1367784455937d174c51a59cec67a2dfb7be54d2d8bd6abc3af96c193a0132bdb708d408bbaf80c0999a501c09eeea3b1
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/attachments@npm:4.0.0-rc.0"
+"@jupyterlab/attachments@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/attachments@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
-  checksum: 8bdd87fcc1b780c3f20f6cf76a312af1dce8e54d4683c56978cb052779a2d255199ffa8559d3f290f0604ab10b2e2dd0cb608dc64954c5db079bc29f8368e1e7
+  checksum: 5faa7f1e3cc6c19c545fe9db2e93b617d385b6120c3a8ed4930d5915335cbd27e11bc6d165568c38de46426c6c21d32f4cb4e5b4ae11aaca961548314c8da65e
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:^4.0.0-beta.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/builder@npm:4.0.0-rc.0"
+"@jupyterlab/builder@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/builder@npm:4.0.0-rc.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/application": ^2.1.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
@@ -551,80 +551,80 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 0f958759b1210cf2d2293d681adf7ab279e63c918ae23ebf891cb1aab15d865446d640ef019f63acd33a917362db36a04e066d1ee57da80e963019925e97dab4
+  checksum: a0b3ec715f7b31d4cc9cbafc8e06d2b4be994008ca4c3d548dd81b1ca65141c4350fb65218394f4d2219b4f17bc064fec1e5001572fa15569a1f144b2060b92b
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/cells@npm:4.0.0-rc.0"
+"@jupyterlab/cells@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/cells@npm:4.0.0-rc.1"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/attachments": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/codemirror": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/filebrowser": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/outputarea": ^4.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/toc": ^6.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/attachments": ^4.0.0-rc.1
+    "@jupyterlab/codeeditor": ^4.0.0-rc.1
+    "@jupyterlab/codemirror": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/documentsearch": ^4.0.0-rc.1
+    "@jupyterlab/filebrowser": ^4.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/outputarea": ^4.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/toc": ^6.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: ee71d6f4763ea6ad44e0662d9f0fc4c0e7a81b5881160c00477b09e3c6094561bb01592286edcb05ac76d1a9756fdda0cf40d5df4554c119265e3bcbaceb196e
+  checksum: 28cb57c0df7e631910abba07189a4b7f2fbd7b6e1eb912e70a40c7a143f8db0bb9989496bef419b9fd3d7313392a4e1c2a44bdb54c690deca30e6ecaed15ac1e
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/codeeditor@npm:4.0.0-rc.0"
+"@jupyterlab/codeeditor@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/codeeditor@npm:4.0.0-rc.1"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/statusbar": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: f6d869bf526a14478576d55f98470ee31d147e52c65843d5dedc8e62cd83ee36084e3cdcbde9363edaf28522a4d92414f0caf19c0482da9cbdcb40267248b79c
+  checksum: d0da0ea4f37ed0535f96f1161c79dfc7cc151edbfc5c262a5e3f658abe9b5adbae30f544fbe79d4383f47893972678f1ac1813f2ddbad0c8264e71c2d3e4690f
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/codemirror@npm:4.0.0-rc.0"
+"@jupyterlab/codemirror@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/codemirror@npm:4.0.0-rc.1"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -639,378 +639,378 @@
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/codeeditor": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/documentsearch": ^4.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     yjs: ^13.5.40
-  checksum: 9ac820eb1b8dd239b47f1cebea86e15342bf75ca14c0a03858ece85876e8ce509acf02d4f9eba4f4149014ec9ef54f093ec7547ab89343e133571382e24fcdd4
+  checksum: f0d4f608a1a8501cffc0fd8c42ec5f84eaa837ac7551c5ffb605f1f49437ac30c0945d965044b09680c86f4a5a0f88bda11d225e64a12232d5c2f042e5f0f56b
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.0.0-rc.0":
-  version: 6.0.0-rc.0
-  resolution: "@jupyterlab/coreutils@npm:6.0.0-rc.0"
+"@jupyterlab/coreutils@npm:^6.0.0-rc.1":
+  version: 6.0.0-rc.1
+  resolution: "@jupyterlab/coreutils@npm:6.0.0-rc.1"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: 5b1e3e19aa2a9aec27ddf8c1997480c46dfbda46719e6cb1e6529b151fc95058554d80cf40e96a0a4328c74e25249cf75819a5fc5f2357f726a51c530a040b41
+  checksum: 8a20d8ac6ae937280757b51cbf240f9de2c6d4896075ce6469c2758562d82d6013b964b2a538f447edbc3f5a2ff18067fe436d87a4d82a5c6e4c35ab9a3ed6f6
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/docmanager@npm:4.0.0-rc.0"
+"@jupyterlab/docmanager@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/docmanager@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/statusbar": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 601c285b79f8a9bfb01a4ff729f65e76c0131593e9f2bc216cd99fd9457552187c3663f31f86109981fb2e7edb8fe074b731795d610f2b4fc173969f017b5a13
+  checksum: 7058083f9d8ca1cec8191d3adce625bd768f0058ffa1c9662a04ffaf300e9d65bc7d87dbeddff11be4736e890b02594b53c8c986c0263109c76d659ed1c641aa
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/docregistry@npm:4.0.0-rc.0"
+"@jupyterlab/docregistry@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/docregistry@npm:4.0.0-rc.1"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/codeeditor": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: d34ad77d8aadc33652f1fed858dc100580425ce005426796a4c9589933ba926c79fca95fe79460c7f04a58887f3e814c3616e45b823689d7d24582a3c5ca4645
+  checksum: 8d9dda5575e98ff2074629c996dbb03f32d8aa2b2a7352c7848673b01205bfa3c42c6caaffa2fcc900ec595d25e3e98a1645c4d03b2427ea1a4aedb6decb7e3c
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/documentsearch@npm:4.0.0-rc.0"
+"@jupyterlab/documentsearch@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/documentsearch@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: c0cf07ff23625e20f67715a5296a4b2918087152991afa541aca60f3bc552be5ebdc9fd216b80e047cf3cedbfc4326d4ede02585e9274c7e21a1fb61b7863c48
+  checksum: 09c2111c69b41e3f5b5fa5e787ac2d136a965828808511f35d58e10299c42eb96eea38820a347858fd1a4729f12ff00b77931cd49dbf9481d3439a7fcb4e6801
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/filebrowser@npm:4.0.0-rc.0"
-  dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docmanager": ^4.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+"@jupyterlab/filebrowser@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/filebrowser@npm:4.0.0-rc.1"
+  dependencies:
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docmanager": ^4.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
+    "@jupyterlab/statusbar": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 9ce98e059792e02984b142d009314ee56331156f2b09bc11787322188ec99412acb8b04ada1f40e815f5b37031da48a8e1fe88b91e42f99052bc005850518ae6
+  checksum: 648a2c2dbd0a5c8925dec399b4dd6462bd8661d5adea0013ff5485f63ebb4d130c9576936915505247975f70958a649bdeb466a11a639f8ea4ae6f2ff51a9618
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/lsp@npm:4.0.0-rc.0"
+"@jupyterlab/lsp@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/lsp@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/codeeditor": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 216fb96098f5b736fb237ee060309a766fee0b378d8bbe45ae2db4858d942fd41a5f58bbad8d26af771e704b0eff09252702e0538fe30086012128a840940b2b
+  checksum: 41aff27dfae3ca88d50e8e159409fb84d9b533c7716b6748d0deafeef34a539e25a85dd4931a0a977d77df3393b8325897ae111f67b1f15562500829baec590a
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/nbformat@npm:4.0.0-rc.0"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/nbformat@npm:4.0.0-rc.1"
   dependencies:
     "@lumino/coreutils": ^2.1.1
-  checksum: b37a04681f7a4364bb87a038298b40468306b8d83799fa0f1fec6c09f330c4f878320e82ebb08945a0c9377fb385fbf65a12e7a2f5895966af25e4db6561d062
+  checksum: 57e224a6913336e8b2261866a4fced1f8b52ab840a09cfb15070d50416325f7183273773553aaf668dd949e902672fcc172f2efd3951d35fd9b6c269348a7c38
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.0.0-beta.2":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/notebook@npm:4.0.0-rc.0"
+"@jupyterlab/notebook@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/notebook@npm:4.0.0-rc.1"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/cells": ^4.0.0-rc.0
-    "@jupyterlab/codeeditor": ^4.0.0-rc.0
-    "@jupyterlab/codemirror": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/documentsearch": ^4.0.0-rc.0
-    "@jupyterlab/lsp": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statusbar": ^4.0.0-rc.0
-    "@jupyterlab/toc": ^6.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/cells": ^4.0.0-rc.1
+    "@jupyterlab/codeeditor": ^4.0.0-rc.1
+    "@jupyterlab/codemirror": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/documentsearch": ^4.0.0-rc.1
+    "@jupyterlab/lsp": ^4.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/settingregistry": ^4.0.0-rc.1
+    "@jupyterlab/statusbar": ^4.0.0-rc.1
+    "@jupyterlab/toc": ^6.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/domutils": ^2.0.0
     "@lumino/dragdrop": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/virtualdom": ^2.0.0
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: a2ea0c8e13827957c70b69a28ee7a8eefc60ff858778d36fbac9040c40af8c36f46ed8311e8c400c40ef904939459f72b437d8376fa8f2bbcc3d16070a1490be
+  checksum: 804bb611c14bfda1ecee132c01d427c2e4ecdc7571af1bcc2b1af268abee32b934cfb74e3cddb6af2f7926a66528c151ba05c2ed13cb4dc57b64b6e7ede9e3d3
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.0.0-rc.0":
-  version: 5.0.0-rc.0
-  resolution: "@jupyterlab/observables@npm:5.0.0-rc.0"
+"@jupyterlab/observables@npm:^5.0.0-rc.1":
+  version: 5.0.0-rc.1
+  resolution: "@jupyterlab/observables@npm:5.0.0-rc.1"
   dependencies:
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: ab5a846b80fec04c16d1021fa15a82de2e7b57ac343c0d13d3893277c07364d1986a7aac7668f0d340de3471a8b922ce6c3a5459c77f5ec3998ffe6d4c8052c9
+  checksum: fa31985a980bb5679c73e332e5d3a2db5ebef6a9325e3a9748603057e5ead13db33e087b2337d3dc4287f473b993dd47f176a56f45b602c45edbcb954caa24fb
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/outputarea@npm:4.0.0-rc.0"
+"@jupyterlab/outputarea@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/outputarea@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: ec9c3ccb3a743f487172cde5e78088cdf5eb0d005d5e52ca688b8005f3e9ebe59a659956d2210a50927610339a194af5efd664c149bebca4ef5fc49919b0bba4
+  checksum: 174ace4352eae70b01bf3481902544833b5956a1875f22fb2eafca4c1b803e4280f2a84f840827d7ecaa1690b701977e7542007fa8f24a019260671f94252c78
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.8.0-rc.0":
-  version: 3.8.0-rc.0
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0-rc.0"
+"@jupyterlab/rendermime-interfaces@npm:^3.8.0-rc.1":
+  version: 3.8.0-rc.1
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.8.0-rc.1"
   dependencies:
     "@lumino/coreutils": ^2.1.1
     "@lumino/widgets": ^2.1.1
-  checksum: 373045bbc1cfb8fee5cc373741419ef11f97fb163ef22f1ad4e69cdaa51c714f369ec07cca8e10a00dc64c510b4aa08b1630419632c61e4f1219678bb35bc904
+  checksum: f2a6ea315b0e18a2a50364b9892438c94ad614cad99427d46497e542a2c10226d6dc249a10f482b8982262f6e91ffffc8a372b57489a89339a027025bcf0a866
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/rendermime@npm:4.0.0-rc.0"
+"@jupyterlab/rendermime@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/rendermime@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     lodash.escape: ^4.0.1
-  checksum: 3605eb77a905ae3767e10b4202de5686d6bff215a23a1dafb59c2c6045a55d208136bf786f26c6db6cce4c1e710eb374a98726b2bbf97aafcffb965094cdf116
+  checksum: 82dd43b14357a2218a42c2747bcefdd4f3ef70dc3f42cb9796deab3b2e7f20e18d0c83f735423219838af9506d1d900f0f7e3304818f423cc61663695fb3ee29
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^7.0.0-rc.0":
-  version: 7.0.0-rc.0
-  resolution: "@jupyterlab/services@npm:7.0.0-rc.0"
+"@jupyterlab/services@npm:^7.0.0-rc.1":
+  version: 7.0.0-rc.1
+  resolution: "@jupyterlab/services@npm:7.0.0-rc.1"
   dependencies:
     "@jupyter/ydoc": ^1.0.2
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/settingregistry": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/settingregistry": ^4.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
     ws: ^8.11.0
-  checksum: 92f6b6944cab467683d8fa535cd8361497cc52d54fb621a2f6fface82f99b57e00b86bff0f31ada6fad9a0833ff3de331eae2585dea0d10f3dc9597127c5d508
+  checksum: 952ab6edf651ae78f5d59e258e99c56008f7916b375750427b963967a91b4bf1fa36701d6b3c535d5b2011a82a59fefe60c6b6339308ce11e5218cc632b868a8
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/settingregistry@npm:4.0.0-rc.0"
+"@jupyterlab/settingregistry@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/settingregistry@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/nbformat": ^4.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/nbformat": ^4.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/signaling": ^2.1.1
     "@rjsf/utils": ^5.1.0
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: c4d7d0b0777f6cc5e614153db51277516c1e665db37b7a42f4de03b449ffd61f2a30b63ce9e0e9e4011dd88f3b0ff57ee7fe10f5044e8bbc5ff41c17f48c2bb5
+  checksum: 976e733243e0f585f435cf1035914de33a6a6c9cc6b0e80a0f2a2084112309026afa592bae4ad5743c412b6f70fac167560966a052dea8fa7d94e9328f13045f
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/statedb@npm:4.0.0-rc.0"
+"@jupyterlab/statedb@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/statedb@npm:4.0.0-rc.1"
   dependencies:
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/properties": ^2.0.0
     "@lumino/signaling": ^2.1.1
-  checksum: cb2ed22b6b66d43e03cf07d3a95c09551fd812770e66d950c4eb7e1c6c4bb59e9cd65ec7522dd61de66af4c92492c8cf49db7ee89d63fc17cfc3e15d8696d7ad
+  checksum: f494b88370e6a966199d0e60ade2fe05412b1e1a6635a3f5259fb16894502341cf9ea2904bbc6dc0c6ef1d6b9beb89b5118118cdec57c89213608fb8283972b9
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/statusbar@npm:4.0.0-rc.0"
+"@jupyterlab/statusbar@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/statusbar@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: df1e481c2a681ec133c1f2cc9e3094dfa1297cbb9bfafc9a1351bf5381952dcee09c07ec3b16f3c73ecbdb16c775dd58c7b6d9e8a8766f47a7f98fe876c55031
+  checksum: e4ce8224885755e683932a4acca1083bc9451dc9a104b69bccee193c342b95123494dc705c0d5e3a2f2809bb282c314bec8339b98a7bd41ab75c0e4a90725633
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.0.0-rc.0":
-  version: 6.0.0-rc.0
-  resolution: "@jupyterlab/toc@npm:6.0.0-rc.0"
+"@jupyterlab/toc@npm:^6.0.0-rc.1":
+  version: 6.0.0-rc.1
+  resolution: "@jupyterlab/toc@npm:6.0.0-rc.1"
   dependencies:
-    "@jupyterlab/apputils": ^4.0.0-rc.0
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/docregistry": ^4.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime": ^4.0.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
-    "@jupyterlab/ui-components": ^4.0.0-rc.0
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/docregistry": ^4.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime": ^4.0.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
+    "@jupyterlab/ui-components": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/signaling": ^2.1.1
     "@lumino/widgets": ^2.1.1
     react: ^18.2.0
-  checksum: 091bb3b0988e63b4a232dca4a2e2ee1b023daad67dbb0cc65883ba08b72c7673d82d506228d5919b9f33dff9815b4f4a6d5ea172fb2af22e5fb87b56d7562197
+  checksum: 8a7c73323a71a1e9b51ac7b3ec3002dcd24f83a0d0843f09fd4cf0580a06f04a2fbfdcca6b5be468a0a84163c1e04aee2e2d8097a2158ef3d93b871115d807fe
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/translation@npm:4.0.0-rc.0"
+"@jupyterlab/translation@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/translation@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/services": ^7.0.0-rc.0
-    "@jupyterlab/statedb": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/services": ^7.0.0-rc.1
+    "@jupyterlab/statedb": ^4.0.0-rc.1
     "@lumino/coreutils": ^2.1.1
-  checksum: f0c2abfd3b7c3e93c3e42b39f1e3fa92ba2d2edb6ba86d7ea0cfff6fb889de9d81fcf4cf3c76bddf0fa79d333009dbd46aed0800a84aee99470eb751e1fdb1f6
+  checksum: 2591566442ce4fd52f5ac1f208eb98875e73f70f6bee6b406cbc012cffb4dcd041f1650b157228bf1cbe6d1b2db5427d444c072c6122319541a379f21b679cb1
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.0-rc.0":
-  version: 4.0.0-rc.0
-  resolution: "@jupyterlab/ui-components@npm:4.0.0-rc.0"
+"@jupyterlab/ui-components@npm:^4.0.0-rc.1":
+  version: 4.0.0-rc.1
+  resolution: "@jupyterlab/ui-components@npm:4.0.0-rc.1"
   dependencies:
-    "@jupyterlab/coreutils": ^6.0.0-rc.0
-    "@jupyterlab/observables": ^5.0.0-rc.0
-    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.0
-    "@jupyterlab/translation": ^4.0.0-rc.0
+    "@jupyterlab/coreutils": ^6.0.0-rc.1
+    "@jupyterlab/observables": ^5.0.0-rc.1
+    "@jupyterlab/rendermime-interfaces": ^3.8.0-rc.1
+    "@jupyterlab/translation": ^4.0.0-rc.1
     "@lumino/algorithm": ^2.0.0
     "@lumino/commands": ^2.1.1
     "@lumino/coreutils": ^2.1.1
     "@lumino/disposable": ^2.1.1
     "@lumino/messaging": ^2.0.0
     "@lumino/polling": ^2.1.1
     "@lumino/properties": ^2.0.0
@@ -1020,15 +1020,15 @@
     "@rjsf/core": ^5.1.0
     "@rjsf/utils": ^5.1.0
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: b6c01808b0e02e4289aca18c62967c0bde1f380954fa4342274cf692d0d4615df371e19e19a63bf3419fa690d23ba87fc92f78ecabedf36a8c19702d6dc14f3f
+  checksum: f48477a98300c5dc3e714f74306e568c446a322ba65715c35bcb3e36762f5f0d023958794a7f18799f17beecee4ebaf52a2d877aeade60307473a2d99bfd8aee
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2":
   version: 1.0.2
   resolution: "@lezer/common@npm:1.0.2"
   checksum: bbcc58e07be02652bf0700d2856042ec089d5be0b95893d628b3e18192ade864fac83b61b19653e10b9f1472261a178b12318d934e9004edd5483a577c0db56b
@@ -1420,17 +1420,17 @@
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 18.16.2
-  resolution: "@types/node@npm:18.16.2"
-  checksum: 7ad66d23b3b93885a9f879bff98e0196790ad35589b47a3d81b52db969ad17ee298082020296df5166c2d72d3cd6a4b9ab34d254483637d967944a4b3e6febdb
+  version: 20.1.3
+  resolution: "@types/node@npm:20.1.3"
+  checksum: abdb593f662a079715b4e9df0c706822e49814dd641fa5a6226ab73fb931cbfc9cfd5df92e09c13dbc90dbc8fce680d29cb735b88899d661481d93e09a8df2be
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
@@ -1448,35 +1448,35 @@
   version: 15.7.5
   resolution: "@types/prop-types@npm:15.7.5"
   checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.0
-  resolution: "@types/react@npm:18.2.0"
+  version: 18.2.6
+  resolution: "@types/react@npm:18.2.6"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: db3d92b423150222a666329f7aa3023e3e942044700557b8a7d161530847e621aec9f56c9e7f71761b06dd164c8a7b17ad52355863efe80963dffa5537e8e5fd
+  checksum: dea9d232d8df7ac357367a69dcb557711ab3d5501807ffa77cebeee73d49ee94d095f298e36853c63ed47cce097eee4c7eae2aaa8c02fac3f0171ec1b523a819
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
   version: 0.16.3
   resolution: "@types/scheduler@npm:0.16.3"
   checksum: 2b0aec39c24268e3ce938c5db2f2e77f5c3dd280e05c262d9c2fe7d890929e4632a6b8e94334017b66b45e4f92a5aa42ba3356640c2a1175fa37bef2f5200767
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.3.12":
-  version: 7.3.13
-  resolution: "@types/semver@npm:7.3.13"
-  checksum: 00c0724d54757c2f4bc60b5032fe91cda6410e48689633d5f35ece8a0a66445e3e57fa1d6e07eb780f792e82ac542948ec4d0b76eb3484297b79bd18b8cf1cb0
+  version: 7.5.0
+  resolution: "@types/semver@npm:7.5.0"
+  checksum: 0a64b9b9c7424d9a467658b18dd70d1d781c2d6f033096a6e05762d20ebbad23c1b69b0083b0484722aabf35640b78ccc3de26368bcae1129c87e9df028a22e2
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
   version: 0.1.2
   resolution: "@types/source-list-map@npm:0.1.2"
   checksum: fda8f37537aca9d3ed860d559289ab1dddb6897e642e6f53e909bbd18a7ac3129a8faa2a7d093847c91346cf09c86ef36e350c715406fba1f2271759b449adf6
@@ -1491,315 +1491,315 @@
     "@types/source-list-map": "*"
     source-map: ^0.6.1
   checksum: bc09c584c7047e8aed29801a3981787dee3898e9e7a99891a362df114fcac3879eea5a00932314866a01b25220391839be09fe1487b16d4970ff4a7afd5b9725
   languageName: node
   linkType: hard
 
 "@typescript-eslint/eslint-plugin@npm:^5.55.0":
-  version: 5.59.1
-  resolution: "@typescript-eslint/eslint-plugin@npm:5.59.1"
+  version: 5.59.5
+  resolution: "@typescript-eslint/eslint-plugin@npm:5.59.5"
   dependencies:
     "@eslint-community/regexpp": ^4.4.0
-    "@typescript-eslint/scope-manager": 5.59.1
-    "@typescript-eslint/type-utils": 5.59.1
-    "@typescript-eslint/utils": 5.59.1
+    "@typescript-eslint/scope-manager": 5.59.5
+    "@typescript-eslint/type-utils": 5.59.5
+    "@typescript-eslint/utils": 5.59.5
     debug: ^4.3.4
     grapheme-splitter: ^1.0.4
     ignore: ^5.2.0
     natural-compare-lite: ^1.4.0
     semver: ^7.3.7
     tsutils: ^3.21.0
   peerDependencies:
     "@typescript-eslint/parser": ^5.0.0
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: 9ada3ae721594ddd8101a6093e6383bc95e4dcb19b3929210dee5480637786473a9eba2e69e61e560fa592965f4fd02aeb98ddfda91b00b448ae01c5d77431d6
+  checksum: cc0e5ad8d70e140f0dada2fd1ad69d7c31d3f3dfe75939286fdc3950ff2e37033889acc7c9d92c074b67de3bbb6e46916d688e848fb98dde63b23c08a8b07884
   languageName: node
   linkType: hard
 
 "@typescript-eslint/parser@npm:^5.55.0":
-  version: 5.59.1
-  resolution: "@typescript-eslint/parser@npm:5.59.1"
+  version: 5.59.5
+  resolution: "@typescript-eslint/parser@npm:5.59.5"
   dependencies:
-    "@typescript-eslint/scope-manager": 5.59.1
-    "@typescript-eslint/types": 5.59.1
-    "@typescript-eslint/typescript-estree": 5.59.1
+    "@typescript-eslint/scope-manager": 5.59.5
+    "@typescript-eslint/types": 5.59.5
+    "@typescript-eslint/typescript-estree": 5.59.5
     debug: ^4.3.4
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: d324d32a69e06ab12aacb72cd3e2a8eb8ade6c2a4d4e6bb013941588a675e818a8ebd973bef1cd818da6a76eb00908bf66d84ef214c3f015dfcb40f8067a335e
+  checksum: ef4122074f2c00be1dabbb3fb5534280f81b45f8de6c1a696092af5175684fea65bc002814546d06f880ea5beff2006589e2633662e92d65035437c8e2d9134c
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/scope-manager@npm:5.59.1"
+"@typescript-eslint/scope-manager@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/scope-manager@npm:5.59.5"
   dependencies:
-    "@typescript-eslint/types": 5.59.1
-    "@typescript-eslint/visitor-keys": 5.59.1
-  checksum: ae7758181d0f18d1ad20abf95164553fa98c20410968d538ac7abd430ec59f69e30d4da16ad968d029feced1ed49abc65daf6685c996eb4529d798e8320204ff
+    "@typescript-eslint/types": 5.59.5
+    "@typescript-eslint/visitor-keys": 5.59.5
+  checksum: b3d8a5b70e741b9bef60d0a297da77e844cb744895f31fb6880fdac4c53f7c58f3e04065a7d644afb6e1dc51591285ec866eca2fbd2ad50de6b376031aaccfbd
   languageName: node
   linkType: hard
 
-"@typescript-eslint/type-utils@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/type-utils@npm:5.59.1"
+"@typescript-eslint/type-utils@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/type-utils@npm:5.59.5"
   dependencies:
-    "@typescript-eslint/typescript-estree": 5.59.1
-    "@typescript-eslint/utils": 5.59.1
+    "@typescript-eslint/typescript-estree": 5.59.5
+    "@typescript-eslint/utils": 5.59.5
     debug: ^4.3.4
     tsutils: ^3.21.0
   peerDependencies:
     eslint: "*"
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: ff46cc049995bb6505a6170550a9e658c42cd5699a95e1976822318fef2963381223505f797051fc727938ace66d4a7dc072a4b4cadbbdf91d2fda1a16c05c98
+  checksum: 9ef2b219c71abe3d2ffa4c791ec3da8d120b6a202e7f9c7722d1e8193f8709d6ebec2abc2862b9fa78dffe6214d033898d21c925fc961feb4488070b66aab9f5
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/types@npm:5.59.1"
-  checksum: 40ea7ccf59c4951797d3761e53c866a5979e07fbdabef9dc07d3a3f625a99d4318d5329ae8e628cdfdc0bb9bb6e6d8dfb740f33c7bf318e63fa0a863b9ae85c7
+"@typescript-eslint/types@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/types@npm:5.59.5"
+  checksum: 98c93d354d6410934f468ba8bd468d2746f20b2910c0ef5b08fc788c0742aa7cb82eb2edc4194c85d3fabac5563c1a91d377e84bf5c25caeb4ac9e871aabd4bb
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/typescript-estree@npm:5.59.1"
+"@typescript-eslint/typescript-estree@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/typescript-estree@npm:5.59.5"
   dependencies:
-    "@typescript-eslint/types": 5.59.1
-    "@typescript-eslint/visitor-keys": 5.59.1
+    "@typescript-eslint/types": 5.59.5
+    "@typescript-eslint/visitor-keys": 5.59.5
     debug: ^4.3.4
     globby: ^11.1.0
     is-glob: ^4.0.3
     semver: ^7.3.7
     tsutils: ^3.21.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: e33081937225f38e717ac2f9e90c4a8c6b71b701923eea3e03be76d8c466f0d3c6a4ec1d65c9fc1da4f1989416d386305353c5b53aa736d3af9503061001e3eb
+  checksum: 10a8c01ad53da115ca698668941dcb18c497035ba07faf08237bfa3ab92185bdfaf1df93562915a936b49e9f72a4cc6b10b1d9296b7cdc8c34ba0ca323c37677
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/utils@npm:5.59.1"
+"@typescript-eslint/utils@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/utils@npm:5.59.5"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@types/json-schema": ^7.0.9
     "@types/semver": ^7.3.12
-    "@typescript-eslint/scope-manager": 5.59.1
-    "@typescript-eslint/types": 5.59.1
-    "@typescript-eslint/typescript-estree": 5.59.1
+    "@typescript-eslint/scope-manager": 5.59.5
+    "@typescript-eslint/types": 5.59.5
+    "@typescript-eslint/typescript-estree": 5.59.5
     eslint-scope: ^5.1.1
     semver: ^7.3.7
   peerDependencies:
     eslint: ^6.0.0 || ^7.0.0 || ^8.0.0
-  checksum: ca32c90efa57e937ebf812221e070c0604ca99f900fbca60578b42d40c923d5a94fd9503cf5918ecd75b687b68a1be562f7c6593a329bc40b880c95036a021c0
+  checksum: 2703972653d3c6eab2423d9a2586908086afa3b89580969ed38e454bc372265d5ca9fadf7967e4ea639d482ad069f763981ef4a03a42d79df28f43f00ee9d43a
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:5.59.1":
-  version: 5.59.1
-  resolution: "@typescript-eslint/visitor-keys@npm:5.59.1"
+"@typescript-eslint/visitor-keys@npm:5.59.5":
+  version: 5.59.5
+  resolution: "@typescript-eslint/visitor-keys@npm:5.59.5"
   dependencies:
-    "@typescript-eslint/types": 5.59.1
+    "@typescript-eslint/types": 5.59.5
     eslint-visitor-keys: ^3.3.0
-  checksum: f98e399147310cad67de718a8a6336f053d46753bade380c89ddac3dd49512555c3f613636b255ce0b5e2b004654d1c167eb5e53fc8085148b637a5afc20cdd8
+  checksum: 94db281ec8ea3a7ede46763aaa0d3349e035b19334fd03e2e560f89c70faebcfa937d51b53d2eaad2506b60a5d901428cc8b5a65ad8e90ca1c12a133dbe977fc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.5, @webassemblyjs/ast@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/ast@npm:1.11.5"
+"@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ast@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/helper-numbers": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-  checksum: 7df16d8d4364d40e2506776330f8114fddc6494e6e18e8d5ec386312a0881a564cef136b0a74cc4a6ba284e2ff6bad890ddc029a0ba6cf45cc15186e638db118
+    "@webassemblyjs/helper-numbers": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+  checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
   languageName: node
   linkType: hard
 
-"@webassemblyjs/floating-point-hex-parser@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.5"
-  checksum: a6f35e3035a1ec4e446fa43da01539f3ed7e0f4b53d152f36ff34be1b63b08d86c4b09b6af375c95472a75f0c37b3b98b07199d157e767b8b3274e7a3962890c
+"@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
+  checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-api-error@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-api-error@npm:1.11.5"
-  checksum: 717a6ffb3283bd24a7b74710c9bd3d71ec331a26c15446441af19fae9f087e36acb8dcf25b900b6897a1d1eff838e463fe678d66281e7eccee9a3ac0e3447372
+"@webassemblyjs/helper-api-error@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
+  checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.5"
-  checksum: 2c0925b1c3c9b115c183b88d9cf1a12e87fa4fc83ef985aa2a65d72cda543eba6b73b378d231b4feb810b17d3aa6cd297bd603199854346f8a50e3458d7ebbc0
+"@webassemblyjs/helper-buffer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
+  checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-numbers@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-numbers@npm:1.11.5"
+"@webassemblyjs/helper-numbers@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/floating-point-hex-parser": 1.11.5
-    "@webassemblyjs/helper-api-error": 1.11.5
+    "@webassemblyjs/floating-point-hex-parser": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: 49c8bbf561d4df38009e38e6357c396f4454773fd31a03579a8e050a2b28053f5c47f675f00a37f79a65082c938c2159fa603049688ac01b1bafdb472c21110c
+  checksum: f4b562fa219f84368528339e0f8d273ad44e047a07641ffcaaec6f93e5b76fd86490a009aa91a294584e1436d74b0a01fa9fde45e333a4c657b58168b04da424
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-bytecode@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.5"
-  checksum: 4e868de92587e131a7f22bc4eb44eee60c178d4c2c3eeabcb973b4eac73ec477f25d5f838394797265dbe4b600e781c6e150c762a45f249b94bf0711e73409a7
+"@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
+  checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.5"
+"@webassemblyjs/helper-wasm-section@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-  checksum: 1752d7e0dbbf236a5cdc2257e1626a3562bfb0a7d2e967dc5e798c73088f18f20a991491565e2ffee61615f08035b4760e7aa080380bb60b86b393b6eb7486ae
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+  checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ieee754@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/ieee754@npm:1.11.5"
+"@webassemblyjs/ieee754@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
     "@xtuc/ieee754": ^1.2.0
-  checksum: 68a855a3e3dd488fff4d2d100e491cb6ac07f728c9432f3216b8e1bb0a374b397b0a5f58fd3b71195e525d49c0c827db15c18897e1c220c629e759b19978e64c
+  checksum: 13574b8e41f6ca39b700e292d7edf102577db5650fe8add7066a320aa4b7a7c09a5056feccac7a74eb68c10dea9546d4461412af351f13f6b24b5f32379b49de
   languageName: node
   linkType: hard
 
-"@webassemblyjs/leb128@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/leb128@npm:1.11.5"
+"@webassemblyjs/leb128@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/leb128@npm:1.11.6"
   dependencies:
     "@xtuc/long": 4.2.2
-  checksum: 555314708b6615c203c31a9dd810141c6de728e0043c2169ca69905ccf4d8603102994cb74ac5d057ac229bfc2be40f69cad2edd134ef2b909ef694eefe7bba6
+  checksum: 7ea942dc9777d4b18a5ebfa3a937b30ae9e1d2ce1fee637583ed7f376334dd1d4274f813d2e250056cca803e0952def4b954913f1a3c9068bcd4ab4ee5143bf0
   languageName: node
   linkType: hard
 
-"@webassemblyjs/utf8@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/utf8@npm:1.11.5"
-  checksum: d8f67a5650d9bf26810da76e72d0547211a44f30f35657953f547e08185facb39ff326920bddec96d35b5cc65e4e66b1f23c6461847e2f93fad2a60b0bb20211
+"@webassemblyjs/utf8@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/utf8@npm:1.11.6"
+  checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
 "@webassemblyjs/wasm-edit@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.5"
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/helper-wasm-section": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-    "@webassemblyjs/wasm-opt": 1.11.5
-    "@webassemblyjs/wasm-parser": 1.11.5
-    "@webassemblyjs/wast-printer": 1.11.5
-  checksum: 790142a1e282848201c7b68860aabc0141ee44a98a62c3f0af05f8de3cc69b439c3af54ae9a06acbbfbf7fd192b30ee97fb31eda3e08973cae373534ad2135c7
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/helper-wasm-section": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-opt": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+    "@webassemblyjs/wast-printer": 1.11.6
+  checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.5"
+"@webassemblyjs/wasm-gen@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/ieee754": 1.11.5
-    "@webassemblyjs/leb128": 1.11.5
-    "@webassemblyjs/utf8": 1.11.5
-  checksum: 0122df4e5ce52d873f19f34b3ebe8237072e9e6a69667cbec42a2d98ba49f85ea2ed3d935195e6a7ad4f64b9dd7da42883f057fe1103d2062bc90f3428b063fe
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.5"
+"@webassemblyjs/wasm-opt@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-buffer": 1.11.5
-    "@webassemblyjs/wasm-gen": 1.11.5
-    "@webassemblyjs/wasm-parser": 1.11.5
-  checksum: f9416b0dece071e308616fb30e560f0c3c53b5bb23cc4409781b8c47d31e935b27e9a248c65aee9dd9136271e37a4c5cb0971b27e5adf623020fbb298423fe55
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-buffer": 1.11.6
+    "@webassemblyjs/wasm-gen": 1.11.6
+    "@webassemblyjs/wasm-parser": 1.11.6
+  checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.5, @webassemblyjs/wasm-parser@npm:^1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.5"
+"@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
-    "@webassemblyjs/helper-api-error": 1.11.5
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.5
-    "@webassemblyjs/ieee754": 1.11.5
-    "@webassemblyjs/leb128": 1.11.5
-    "@webassemblyjs/utf8": 1.11.5
-  checksum: 094b3df07532cd2a1db91710622cbaf3d7467a361f9f73dc564999385a472fcc08497d8ccf9294bd7c8813d5e2056c06a81e032abb60520168899605fde9b12c
+    "@webassemblyjs/ast": 1.11.6
+    "@webassemblyjs/helper-api-error": 1.11.6
+    "@webassemblyjs/helper-wasm-bytecode": 1.11.6
+    "@webassemblyjs/ieee754": 1.11.6
+    "@webassemblyjs/leb128": 1.11.6
+    "@webassemblyjs/utf8": 1.11.6
+  checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.5":
-  version: 1.11.5
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.5"
+"@webassemblyjs/wast-printer@npm:1.11.6":
+  version: 1.11.6
+  resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
   dependencies:
-    "@webassemblyjs/ast": 1.11.5
+    "@webassemblyjs/ast": 1.11.6
     "@xtuc/long": 4.2.2
-  checksum: c2995224c56b403be7fce7afbb3ad6b2ceadce07a47b28bce745eabb0435fa363c0180bca907d28703ece02422d0de219e689253b55de288c79b8f92416c1d71
+  checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
   languageName: node
   linkType: hard
 
-"@webpack-cli/configtest@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "@webpack-cli/configtest@npm:2.0.1"
+"@webpack-cli/configtest@npm:^2.1.0":
+  version: 2.1.0
+  resolution: "@webpack-cli/configtest@npm:2.1.0"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
-  checksum: 15d0ca835f2e16ec99e9f295f07b676435b9e706d7700df0ad088692fea065e34772fc44b96a4f6a86178b9ca8cf1ff941fbce15269587cf0925d70b18928cea
+  checksum: b875fccd8be9a936924e24986725823347703e3eb72ea884e74669ca20f007704e859855a6a05940d5d3805ce2fc08b183a0f1658d5395b5454b3f5f88293081
   languageName: node
   linkType: hard
 
 "@webpack-cli/info@npm:^2.0.1":
   version: 2.0.1
   resolution: "@webpack-cli/info@npm:2.0.1"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   checksum: b8fba49fee10d297c2affb0b064c9a81e9038d75517c6728fb85f9fb254cae634e5d33e696dac5171e6944ae329d85fddac72f781c7d833f7e9dfe43151ce60d
   languageName: node
   linkType: hard
 
-"@webpack-cli/serve@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "@webpack-cli/serve@npm:2.0.2"
+"@webpack-cli/serve@npm:^2.0.4":
+  version: 2.0.4
+  resolution: "@webpack-cli/serve@npm:2.0.4"
   peerDependencies:
     webpack: 5.x.x
     webpack-cli: 5.x.x
   peerDependenciesMeta:
     webpack-dev-server:
       optional: true
-  checksum: f74c8cc7d3e4de58e1261c6d09af0e8b8a23f53ada4ec336140f30fa16d57d9f56de954e87125947c090c06a30b10a243ca1e093c3e4bd60ba3f19c852cb20b7
+  checksum: 561ea2e6eb551415f0b1675393a8480e1201293fe37eae334cbb1fdc466986668cca76ca1ca327ada9b498eae27cbecef0793e3bb5677288f1a5216cad414efe
   languageName: node
   linkType: hard
 
 "@xtuc/ieee754@npm:^1.2.0":
   version: 1.2.0
   resolution: "@xtuc/ieee754@npm:1.2.0"
   checksum: ac56d4ca6e17790f1b1677f978c0c6808b1900a5b138885d3da21732f62e30e8f0d9120fcf8f6edfff5100ca902b46f8dd7c1e3f903728634523981e80e2885a
@@ -2077,17 +2077,17 @@
   version: 5.3.1
   resolution: "camelcase@npm:5.3.1"
   checksum: e6effce26b9404e3c0f301498184f243811c30dfe6d0b9051863bd8e4034d09c8c2923794f280d6827e5aa055f6c434115ff97864a16a963366fb35fd673024b
   languageName: node
   linkType: hard
 
 "caniuse-lite@npm:^1.0.30001449":
-  version: 1.0.30001481
-  resolution: "caniuse-lite@npm:1.0.30001481"
-  checksum: 8200a043c191b4fd4fe0beda37a58fd61869c895ab93f87bdd0420e5927453f48434d716ce9da8552ff6c3ecc4dcd1366354cda3a134f3cc844af741574a7cab
+  version: 1.0.30001486
+  resolution: "caniuse-lite@npm:1.0.30001486"
+  checksum: 5e8c2ba2679e4ad17dea6d2761a6449b814441bfeac81af6cc9d58af187df6af4b79b27befcbfc4a557e720b21c0399a7d1911c8705922e38938dcc0f40b5d4b
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.0.0, chalk@npm:^2.3.0, chalk@npm:^2.4.1":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -2444,17 +2444,17 @@
     lodash: ^4.17.4
     semver: ^5.4.1
   checksum: d77be45cb72d79a429c64d8f8f7603fea681d182fb795459a3d4afa608faad9a923378a7e80c6855f465263e1983140b6fc3682bd0213228b8cd7906ab4b934d
   languageName: node
   linkType: hard
 
 "electron-to-chromium@npm:^1.4.284":
-  version: 1.4.376
-  resolution: "electron-to-chromium@npm:1.4.376"
-  checksum: 881351d25e0e983432c10844540bb664ee4c54f781b81b7247c36d6e617dc85305fd87ffb5de6d9630c6a54f4432afd8e97565a11c62bb77b63051e43cb8a942
+  version: 1.4.392
+  resolution: "electron-to-chromium@npm:1.4.392"
+  checksum: 502784f59ebf5a6ee7a542983dbdf38c3e2b9a270e8f507454b63dcacd8166888a7aa2c48ae9325e489c58b2e9596ce67b61e5c12de0ac6410b8bf3b0ad6476d
   languageName: node
   linkType: hard
 
 "emoji-regex@npm:^8.0.0":
   version: 8.0.0
   resolution: "emoji-regex@npm:8.0.0"
   checksum: d4c5c39d5a9868b5fa152f00cada8a936868fd3367f33f71be515ecee4c803132d11b31a6222b2571b1e5f7e13890156a94880345594d0ce7e3c9895f560f192
@@ -2464,21 +2464,21 @@
 "emojis-list@npm:^3.0.0":
   version: 3.0.0
   resolution: "emojis-list@npm:3.0.0"
   checksum: ddaaa02542e1e9436c03970eeed445f4ed29a5337dfba0fe0c38dfdd2af5da2429c2a0821304e8a8d1cadf27fdd5b22ff793571fa803ae16852a6975c65e8e70
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.13.0":
-  version: 5.13.0
-  resolution: "enhanced-resolve@npm:5.13.0"
+"enhanced-resolve@npm:^5.14.0":
+  version: 5.14.0
+  resolution: "enhanced-resolve@npm:5.14.0"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: 76d6844c4393d76beed5b3ce6cf5a98dee3ad5c84a9887f49ccde1224e3b7af201dfbd5a57ebf2b49f623b74883df262d50ff480d3cc02fc2881fc58b84e1bbe
+  checksum: fff1aaebbf376371e5df4502e111967f6247c37611ad3550e4e7fca657f6dcb29ef7ffe88bf14e5010b78997f1ddd984a8db97af87ee0a5477771398fd326f5b
   languageName: node
   linkType: hard
 
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
@@ -2637,41 +2637,41 @@
   dependencies:
     esrecurse: ^4.3.0
     estraverse: ^5.2.0
   checksum: 64591a2d8b244ade9c690b59ef238a11d5c721a98bcee9e9f445454f442d03d3e04eda88e95a4daec558220a99fa384309d9faae3d459bd40e7a81b4063980ae
   languageName: node
   linkType: hard
 
-"eslint-visitor-keys@npm:^3.3.0, eslint-visitor-keys@npm:^3.4.0":
-  version: 3.4.0
-  resolution: "eslint-visitor-keys@npm:3.4.0"
-  checksum: 33159169462d3989321a1ec1e9aaaf6a24cc403d5d347e9886d1b5bfe18ffa1be73bdc6203143a28a606b142b1af49787f33cff0d6d0813eb5f2e8d2e1a6043c
+"eslint-visitor-keys@npm:^3.3.0, eslint-visitor-keys@npm:^3.4.1":
+  version: 3.4.1
+  resolution: "eslint-visitor-keys@npm:3.4.1"
+  checksum: f05121d868202736b97de7d750847a328fcfa8593b031c95ea89425333db59676ac087fa905eba438d0a3c5769632f828187e0c1a0d271832a2153c1d3661c2c
   languageName: node
   linkType: hard
 
 "eslint@npm:^8.36.0":
-  version: 8.39.0
-  resolution: "eslint@npm:8.39.0"
+  version: 8.40.0
+  resolution: "eslint@npm:8.40.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.4.0
-    "@eslint/eslintrc": ^2.0.2
-    "@eslint/js": 8.39.0
+    "@eslint/eslintrc": ^2.0.3
+    "@eslint/js": 8.40.0
     "@humanwhocodes/config-array": ^0.11.8
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
     ajv: ^6.10.0
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
     debug: ^4.3.2
     doctrine: ^3.0.0
     escape-string-regexp: ^4.0.0
     eslint-scope: ^7.2.0
-    eslint-visitor-keys: ^3.4.0
-    espree: ^9.5.1
+    eslint-visitor-keys: ^3.4.1
+    espree: ^9.5.2
     esquery: ^1.4.2
     esutils: ^2.0.2
     fast-deep-equal: ^3.1.3
     file-entry-cache: ^6.0.1
     find-up: ^5.0.0
     glob-parent: ^6.0.2
     globals: ^13.19.0
@@ -2690,26 +2690,26 @@
     natural-compare: ^1.4.0
     optionator: ^0.9.1
     strip-ansi: ^6.0.1
     strip-json-comments: ^3.1.0
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: d7a074ff326e7ea482500dc0427a7d4b0260460f0f812d19b46b1cca681806b67309f23da9d17cd3de8eb74dd3c14cb549c4d58b05b140564d14cc1a391122a0
+  checksum: b79eba37f52f517a420eec99a80ae9f284d2cbe73afc0d4d3d4d5ed1cce0b06f21badc0374bfb7ac239efd2d49a1fd7c6111d6c3d52888521f377ba33de77e61
   languageName: node
   linkType: hard
 
-"espree@npm:^9.5.1":
-  version: 9.5.1
-  resolution: "espree@npm:9.5.1"
+"espree@npm:^9.5.2":
+  version: 9.5.2
+  resolution: "espree@npm:9.5.2"
   dependencies:
     acorn: ^8.8.0
     acorn-jsx: ^5.3.2
-    eslint-visitor-keys: ^3.4.0
-  checksum: cdf6e43540433d917c4f2ee087c6e987b2063baa85a1d9cdaf51533d78275ebd5910c42154e7baf8e3e89804b386da0a2f7fad2264d8f04420e7506bf87b3b88
+    eslint-visitor-keys: ^3.4.1
+  checksum: 6506289d6eb26471c0b383ee24fee5c8ae9d61ad540be956b3127be5ce3bf687d2ba6538ee5a86769812c7c552a9d8239e8c4d150f9ea056c6d5cbe8399c03c1
   languageName: node
   linkType: hard
 
 "esquery@npm:^1.4.2":
   version: 1.5.0
   resolution: "esquery@npm:1.5.0"
   dependencies:
@@ -3654,18 +3654,18 @@
   languageName: node
   linkType: hard
 
 "jupyterlab-celltagsclasses@workspace:.":
   version: 0.0.0-use.local
   resolution: "jupyterlab-celltagsclasses@workspace:."
   dependencies:
-    "@jupyterlab/application": ^4.0.0-beta.2
-    "@jupyterlab/apputils": ^4.0.0-beta.2
-    "@jupyterlab/builder": ^4.0.0-beta.0
-    "@jupyterlab/notebook": ^4.0.0-beta.2
+    "@jupyterlab/application": ^4.0.0-rc.1
+    "@jupyterlab/apputils": ^4.0.0-rc.1
+    "@jupyterlab/builder": ^4.0.0-rc.1
+    "@jupyterlab/notebook": ^4.0.0-rc.1
     "@lumino/widgets": ^2.0.1
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@typescript-eslint/eslint-plugin": ^5.55.0
     "@typescript-eslint/parser": ^5.55.0
     css-loader: ^6.7.1
     eslint: ^8.36.0
@@ -3848,15 +3848,15 @@
   resolution: "lru-cache@npm:6.0.0"
   dependencies:
     yallist: ^4.0.0
   checksum: f97f499f898f23e4585742138a22f22526254fdba6d75d41a1c2526b3b6cc5747ef59c5612ba7375f42aca4f8461950e925ba08c991ead0651b4918b7c978297
   languageName: node
   linkType: hard
 
-"lru-cache@npm:^9.0.0":
+"lru-cache@npm:^9.1.1":
   version: 9.1.1
   resolution: "lru-cache@npm:9.1.1"
   checksum: 4d703bb9b66216bbee55ead82a9682820a2b6acbdfca491b235390b1ef1056000a032d56dfb373fdf9ad4492f1fa9d04cc9a05a77f25bd7ce6901d21ad9b68b7
   languageName: node
   linkType: hard
 
 "map-obj@npm:^1.0.0":
@@ -4312,20 +4312,20 @@
   version: 1.0.7
   resolution: "path-parse@npm:1.0.7"
   checksum: 49abf3d81115642938a8700ec580da6e830dde670be21893c62f4e10bd7dd4c3742ddc603fe24f898cba7eb0c6bc1777f8d9ac14185d34540c6d4d80cd9cae8a
   languageName: node
   linkType: hard
 
 "path-scurry@npm:^1.6.1":
-  version: 1.7.0
-  resolution: "path-scurry@npm:1.7.0"
+  version: 1.8.0
+  resolution: "path-scurry@npm:1.8.0"
   dependencies:
-    lru-cache: ^9.0.0
+    lru-cache: ^9.1.1
     minipass: ^5.0.0
-  checksum: 4e86df0fa6848cef1ba672d4a332b8dbd0297c42d5123bcc419d714c34b25ee6775b0d2e66dd5e698a38e9bcd808f8fc47333e3a3357307cada98e16bfae8b98
+  checksum: 53974a328e379aa3e22b18bbc97f135522d329597faa924bc99bc95959a21ae07c1aa7747a00c21c3579a5d25af4596ea1ed7f135cafd12ec949e35969a39e3e
   languageName: node
   linkType: hard
 
 "path-type@npm:^3.0.0":
   version: 3.0.0
   resolution: "path-type@npm:3.0.0"
   dependencies:
@@ -4444,20 +4444,20 @@
   peerDependencies:
     postcss: ^8.3.3
   checksum: 06c733eaad83a3954367e7ee02ddfe3796e7a44d4299ccf9239f40964a4daac153c7d77613f32964b5a86c0c6c2f6167738f31d578b73b17cb69d0c4446f0ebe
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.11, postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.11
-  resolution: "postcss-selector-parser@npm:6.0.11"
+  version: 6.0.12
+  resolution: "postcss-selector-parser@npm:6.0.12"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: 0b01aa9c2d2c8dbeb51e9b204796b678284be9823abc8d6d40a8b16d4149514e922c264a8ed4deb4d6dbced564b9be390f5942c058582d8656351516d6c49cde
+  checksum: f166ed4350511f6fb4a7e82aaaa6dfd81a1e648d4567ca15a3ca87b7ea2e55a8c136fb0ae9456b7b88a390c160f05d06bd1c69f47d7e331b53b70941e06e90fe
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
@@ -5316,46 +5316,46 @@
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
 "terser-webpack-plugin@npm:^5.3.7":
-  version: 5.3.7
-  resolution: "terser-webpack-plugin@npm:5.3.7"
+  version: 5.3.8
+  resolution: "terser-webpack-plugin@npm:5.3.8"
   dependencies:
     "@jridgewell/trace-mapping": ^0.3.17
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
-    terser: ^5.16.5
+    terser: ^5.16.8
   peerDependencies:
     webpack: ^5.1.0
   peerDependenciesMeta:
     "@swc/core":
       optional: true
     esbuild:
       optional: true
     uglify-js:
       optional: true
-  checksum: 095e699fdeeb553cdf2c6f75f983949271b396d9c201d7ae9fc633c45c1c1ad14c7257ef9d51ccc62213dd3e97f875870ba31550f6d4f1b6674f2615562da7f7
+  checksum: 0ffc2a1949b1fd60ef9c815c4629b9817656db612bb58c5db96e3b04204c86afd142b115392e48733364edc7bf95131f54c10174c05f046ba8f2adead6b06c3c
   languageName: node
   linkType: hard
 
-"terser@npm:^5.16.5":
-  version: 5.17.1
-  resolution: "terser@npm:5.17.1"
+"terser@npm:^5.16.8":
+  version: 5.17.3
+  resolution: "terser@npm:5.17.3"
   dependencies:
     "@jridgewell/source-map": ^0.3.2
     acorn: ^8.5.0
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 69b0e80e3c4084db2819de4d6ae8a2ba79f2fcd7ed6df40fe4b602ec7bfd8e889cc63c7d5268f30990ffecbf6eeda18f857adad9386fe2c2331b398d58ed855c
+  checksum: 6b5a859bf9707f34be6e4c567437bc4e47e9364eec37a48b0ae3bff46bb510ef43caf543a23a89b8f43eca47c90a6759105add171fdb0d768dd639deb4545ac9
   languageName: node
   linkType: hard
 
 "text-table@npm:^0.2.0":
   version: 0.2.0
   resolution: "text-table@npm:0.2.0"
   checksum: b6937a38c80c7f84d9c11dd75e49d5c44f71d95e810a3250bd1f1797fc7117c57698204adf676b71497acc205d769d65c16ae8fa10afad832ae1322630aef10a
@@ -5660,21 +5660,21 @@
   version: 6.1.0
   resolution: "webidl-conversions@npm:6.1.0"
   checksum: 1f526507aa491f972a0c1409d07f8444e1d28778dfa269a9971f2e157182f3d496dc33296e4ed45b157fdb3bf535bb90c90bf10c50dcf1dd6caacb2a34cc84fb
   languageName: node
   linkType: hard
 
 "webpack-cli@npm:^5.0.1":
-  version: 5.0.2
-  resolution: "webpack-cli@npm:5.0.2"
+  version: 5.1.1
+  resolution: "webpack-cli@npm:5.1.1"
   dependencies:
     "@discoveryjs/json-ext": ^0.5.0
-    "@webpack-cli/configtest": ^2.0.1
+    "@webpack-cli/configtest": ^2.1.0
     "@webpack-cli/info": ^2.0.1
-    "@webpack-cli/serve": ^2.0.2
+    "@webpack-cli/serve": ^2.0.4
     colorette: ^2.0.14
     commander: ^10.0.1
     cross-spawn: ^7.0.3
     envinfo: ^7.7.3
     fastest-levenshtein: ^1.0.12
     import-local: ^3.0.2
     interpret: ^3.1.1
@@ -5687,15 +5687,15 @@
       optional: true
     webpack-bundle-analyzer:
       optional: true
     webpack-dev-server:
       optional: true
   bin:
     webpack-cli: bin/cli.js
-  checksum: 98816d84c51487b90e1008ddbcda8827dcb7ae9ab7892f4d742f0d7b93f90a4a18a6ec2671b380e5a7ee4b0917cf0c43921119419d8ba9e1b14ea060115684fd
+  checksum: 7738e6a84a0098886e1e0c0fd0dab44b7dedfbb0580afbb5ef734c5109dcaee80140bebb5d9f4b40f425029563bb09bcbda8b08d904fa14e60ff632e6dcc8a17
   languageName: node
   linkType: hard
 
 "webpack-merge@npm:^5.7.3, webpack-merge@npm:^5.8.0":
   version: 5.8.0
   resolution: "webpack-merge@npm:5.8.0"
   dependencies:
@@ -5719,27 +5719,27 @@
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
 "webpack@npm:^5.76.1":
-  version: 5.81.0
-  resolution: "webpack@npm:5.81.0"
+  version: 5.82.1
+  resolution: "webpack@npm:5.82.1"
   dependencies:
     "@types/eslint-scope": ^3.7.3
     "@types/estree": ^1.0.0
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
     acorn-import-assertions: ^1.7.6
     browserslist: ^4.14.5
     chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.13.0
+    enhanced-resolve: ^5.14.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.2.9
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
@@ -5751,15 +5751,15 @@
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 1a6eecaffac3226d80f4e8f330b32e0ff117d9dafd8700166d230afbc171d68ea1ff55a9939fa789307f7b9d11881889ccb8e6cd79d4ccbaeef916788ce73fdb
+  checksum: 747ee7ebd238c15249c2652060e3c6ca6d62cc66dcf7e4e2824ecd4875b7ea5e01fce8f4179080a3e84dfdb3c8d0992700444c7c5a05ef47b38c0623d3ac76de
   languageName: node
   linkType: hard
 
 "whatwg-mimetype@npm:^2.3.0":
   version: 2.3.0
   resolution: "whatwg-mimetype@npm:2.3.0"
   checksum: 23eb885940bcbcca4ff841c40a78e9cbb893ec42743993a42bf7aed16085b048b44b06f3402018931687153550f9a32d259dfa524e4f03577ab898b6965e5383
@@ -5911,19 +5911,19 @@
   version: 20.2.9
   resolution: "yargs-parser@npm:20.2.9"
   checksum: 8bb69015f2b0ff9e17b2c8e6bfe224ab463dd00ca211eece72a4cd8a906224d2703fb8a326d36fdd0e68701e201b2a60ed7cf81ce0fd9b3799f9fe7745977ae3
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.6.0
-  resolution: "yjs@npm:13.6.0"
+  version: 13.6.1
+  resolution: "yjs@npm:13.6.1"
   dependencies:
     lib0: ^0.2.74
-  checksum: 54bd3b0c8a8dc5724044356c8015210f9840b7ac46c8d87d66a0cc5f5bf669298d45324942681ad01ea22c7a4de6a29aa22180d63596e18734bc90335ced982f
+  checksum: bf18ed3f53b4baed61363461b2567cf841f27c326ae107736bb46239fb7273d9d0ef71ea83ae792e96e406d074218d6666f2909a680214b940ada39b58545336
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/examples/test.ipynb` & `jupyterlab_celltagsclasses-0.3.0/examples/test.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985119047619048%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.10'}}"}*

```diff
@@ -117,15 +117,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.10"
         },
         "toc": {
             "base_numbering": 1
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/build_log.json` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/build_log.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999211907776723%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^4.0.0-rc.1'}, '@jupyterlab/application-extension': {'requiredVersion': '^4.0.0-rc.1'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^4.0.0-rc.1'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^4.0.0-rc.1'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^4.0.0-rc.1'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^4.0.0-rc.1' […]*

```diff
@@ -136,415 +136,415 @@
                         "@jupyter/ydoc": {
                             "import": false,
                             "requiredVersion": "^1.0.2",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/celltags": {
                             "import": false,
                             "requiredVersion": "^4.0.0-alpha.20"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-beta.2",
+                            "requiredVersion": "^6.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.0.0-beta.2"
+                            "requiredVersion": "^5.0.0-rc.1"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.8.0-beta.2",
+                            "requiredVersion": "^3.8.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.0.0-beta.2",
+                            "requiredVersion": "^7.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-beta.2",
+                            "requiredVersion": "^6.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.0.0-beta.2"
+                            "requiredVersion": "^6.0.0-rc.1"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2",
+                            "requiredVersion": "^4.0.0-rc.1",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.0-beta.2"
+                            "requiredVersion": "^4.0.0-rc.1"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -626,15 +626,15 @@
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "jupyterlab-celltagsclasses": {
                             "import": "/Users/tparment/git/jupyterlab-celltagsclasses/lib/index.js",
                             "singleton": true,
-                            "version": "0.2.0"
+                            "version": "0.3.0"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/package.json` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9643353174603174%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0-rc.1', '@jupyterlab/apputils': "*

 * *                   "'^4.0.0-rc.1', '@jupyterlab/notebook': '^4.0.0-rc.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0-rc.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.8de4dac15b9641f8640c.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -3,22 +3,22 @@
         "email": "thierry.parmentelat@inria.fr",
         "name": "Thierry Parmentelat"
     },
     "bugs": {
         "url": "https://github.com/parmentelat/jupyterlab-celltagsclasses/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^4.0.0-rc.0",
-        "@jupyterlab/apputils": "^4.0.0-rc.0",
-        "@jupyterlab/notebook": "^4.0.0-rc.0",
+        "@jupyterlab/application": "^4.0.0-rc.1",
+        "@jupyterlab/apputils": "^4.0.0-rc.1",
+        "@jupyterlab/notebook": "^4.0.0-rc.1",
         "@lumino/widgets": "^2.0.1"
     },
     "description": "JLAB extension to add classes to cells based on their tags",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.0-rc.0",
+        "@jupyterlab/builder": "^4.0.0-rc.1",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@typescript-eslint/eslint-plugin": "^5.55.0",
         "@typescript-eslint/parser": "^5.55.0",
         "css-loader": "^6.7.1",
         "eslint": "^8.36.0",
         "eslint-config-prettier": "^8.7.0",
@@ -41,15 +41,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/parmentelat/jupyterlab-celltagsclasses",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e8bcb578ed91b775bd99.js",
+            "load": "static/remoteEntry.8de4dac15b9641f8640c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_celltagsclasses/labextension"
     },
     "keywords": [
         "jupyter",
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,90 @@
 "use strict";
 (self["webpackChunkjupyterlab_celltagsclasses"] = self["webpackChunkjupyterlab_celltagsclasses"] || []).push([
     ["lib_index_js"], {
 
         /***/
+        "./lib/apply_on_cells.js":
+            /*!*******************************!*\
+              !*** ./lib/apply_on_cells.js ***!
+              \*******************************/
+            /***/
+            ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
+
+                __webpack_require__.r(__webpack_exports__);
+                /* harmony export */
+                __webpack_require__.d(__webpack_exports__, {
+                    /* harmony export */
+                    "Scope": () => ( /* binding */ Scope),
+                    /* harmony export */
+                    "apply_on_cells": () => ( /* binding */ apply_on_cells)
+                    /* harmony export */
+                });
+                /*
+                 * the logic of applying a function on a set of cells
+                 */
+                var Scope;
+                (function(Scope) {
+                    Scope[Scope["All"] = 0] = "All";
+                    Scope[Scope["Active"] = 1] = "Active";
+                    Scope[Scope["Multiple"] = 2] = "Multiple";
+                })(Scope || (Scope = {}));
+                const apply_on_cells = (notebookTracker, scope, to_apply) => {
+                    var _a;
+                    const notebook = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content;
+                    if (notebook === undefined) {
+                        return;
+                    }
+                    let actionCells;
+                    if (scope === Scope.All) {
+                        actionCells = notebook.widgets.slice();
+                    } else {
+                        const activeCell = notebook.activeCell;
+                        if (activeCell === null) {
+                            return;
+                        }
+                        if (scope === Scope.Active) {
+                            actionCells = [activeCell];
+                        } else {
+                            const {
+                                anchor,
+                                head
+                            } = notebook.getContiguousSelection();
+                            // when only one cell is selected/active, both are null
+                            if (anchor === null || head === null) {
+                                actionCells = [activeCell];
+                            } else {
+                                actionCells = notebook.widgets.slice(anchor, head + 1);
+                            }
+                        }
+                    }
+                    // console.log(`apply_on_cells with scope=${scope} on ${actionCells.length} cells`)
+                    actionCells.forEach(to_apply);
+                };
+
+
+                /***/
+            }),
+
+        /***/
         "./lib/index.js":
             /*!**********************!*\
               !*** ./lib/index.js ***!
               \**********************/
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
+                    "Scope": () => ( /* reexport safe */ _apply_on_cells__WEBPACK_IMPORTED_MODULE_2__.Scope),
+                    /* harmony export */
+                    "apply_on_cells": () => ( /* reexport safe */ _apply_on_cells__WEBPACK_IMPORTED_MODULE_2__.apply_on_cells),
+                    /* harmony export */
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__),
                     /* harmony export */
                     "md_clean": () => ( /* reexport safe */ _metadata__WEBPACK_IMPORTED_MODULE_1__.md_clean),
                     /* harmony export */
                     "md_get": () => ( /* reexport safe */ _metadata__WEBPACK_IMPORTED_MODULE_1__.md_get),
                     /* harmony export */
                     "md_has": () => ( /* reexport safe */ _metadata__WEBPACK_IMPORTED_MODULE_1__.md_has),
@@ -35,14 +102,16 @@
                 });
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__( /*! @jupyterlab/notebook */ "webpack/sharing/consume/default/@jupyterlab/notebook");
                 /* harmony import */
                 var _jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_notebook__WEBPACK_IMPORTED_MODULE_0__);
                 /* harmony import */
                 var _metadata__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__( /*! ./metadata */ "./lib/metadata.js");
+                /* harmony import */
+                var _apply_on_cells__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__( /*! ./apply_on_cells */ "./lib/apply_on_cells.js");
                 /*
                  * for attaching keybindings later on, see
                  * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d
                  */
 
                 /**
                  * Initialization data for the jupyterlab-celltagsclasses extension.
@@ -64,36 +133,36 @@
                                     return;
                                 }
                                 change.newValues.forEach(cellModel => {
                                     var _a, _b;
                                     // compute widgets attached to cellModel
                                     const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => cell.model.id === cellModel.id);
                                     if (cellWidgets === undefined || (cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0) {
-                                        console.warn('could not find cell widget for cell model', cellModel);
+                                        // console.warn('could not find cell widget for cell model', cellModel)
                                         return;
                                     }
-                                    console.debug(`found ${cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length} cell widgets`, cellWidgets[0]);
+                                    // console.debug( `found ${cellWidgets?.length} cell widgets`, cellWidgets[0] )
                                     // add classes for pre-existing tags
                                     (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {
-                                        console.debug(`adding initial class for tag ${class_for_tag(tag)}`);
+                                        // console.debug( `adding initial class for tag ${class_for_tag(tag)}` )
                                         cellWidget.addClass(class_for_tag(tag));
                                     }));
                                     // react to changes in tags
                                     cellModel.metadataChanged.connect((sender, change) => {
-                                        console.debug('metadata changed', sender, change);
+                                        // console.debug('metadata changed', sender, change)
                                         if (change.key !== 'tags') {
                                             // console.debug("ignoring non-tags metadata change")
                                             return;
                                         }
                                         // does not seem useful to recompute this
                                         // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(
                                         //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)
                                         // )
                                         if (change.type === 'change') {
-                                            console.debug('change', change, change.newValue);
+                                            // console.debug('change', change, change.newValue)
                                             // compute difference between old and new tags
                                             const oldTags = change.oldValue;
                                             const newTags = change.newValue;
                                             const addedTags = newTags.filter(tag => !oldTags.includes(tag));
                                             const removedTags = oldTags.filter(tag => !newTags.includes(tag));
                                             // console.debug('addedTags', addedTags)
                                             // console.debug('removedTags', removedTags)
@@ -107,23 +176,23 @@
                                                     cellWidget.removeClass(class_for_tag(tag));
                                                 });
                                             });
                                         } else if (change.type === 'add') {
                                             console.log('add', change, change.newValue);
                                             cellWidgets.forEach(cellWidget => {
                                                 for (const tag of change.newValue) {
-                                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);
+                                                    // console.debug(`adding class for tag ${class_for_tag(tag)}`)
                                                     cellWidget.addClass(class_for_tag(tag));
                                                 }
                                             });
                                         } else if (change.type === 'remove') {
                                             console.log('remove', change, change.newValue);
                                             cellWidgets.forEach(cellWidget => {
                                                 for (const tag of change.newValue) {
-                                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);
+                                                    // console.debug(`removing class for tag ${class_for_tag(tag)}`)
                                                     cellWidget.removeClass(class_for_tag(tag));
                                                 }
                                             });
                                         }
                                     });
                                 });
                             });
@@ -132,14 +201,15 @@
                 };
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (plugin);
                 // re-export metadata helper functions
 
 
 
+
                 /***/
             }),
 
         /***/
         "./lib/metadata.js":
             /*!*************************!*\
               !*** ./lib/metadata.js ***!
@@ -574,8 +644,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.cddacca2ba0e6c761c6d.js.map
+//# sourceMappingURL=lib_index_js.8b68da7de22fb270ee0f.js.map
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.cddacca2ba0e6c761c6d.js.map` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7964285714285715%*

 * *Differences: {"'file'": "'lib_index_js.8b68da7de22fb270ee0f.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;AAAA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA,CAAC,sBAAsB;AAChB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,eAAe;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gDAAgD,OAAO,KAAK,oBAAoB;AAChF;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACxCA;AACA;AACA;AACA;AACwD;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA; […]*

```diff
@@ -1,17 +1,19 @@
 {
-    "file": "lib_index_js.cddacca2ba0e6c761c6d.js",
-    "mappings": ";;;;;;;;;;;;;;;;;;;;;;;;AAAA;AACA;AACA;AACA;AACwD;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,2CAA2C,8EAA8E;AACzH;AACA;AACA,sEAAsE,mBAAmB;AACzF;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,iCAAiC;AACjC;AACA,4EAA4E,mBAAmB;AAC/F;AACA,iCAAiC;AACjC,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA;AACA,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,4EAA4E,mBAAmB;AAC/F;AACA;AACA,6BAA6B;AAC7B;AACA,qBAAqB;AACrB,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;AACtB;AACyG;;;;;;;;;;;;;;;;;;;;;;;;;AC/FzG;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACyC;AACuE;AAChH;AACO;AACP,wBAAwB,mDAAI;AAC5B;AACA;AACA,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,iDAAS;AACxB;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,iDAAS;AAC5B;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,mDAAW;AAClC;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA,iBAAiB,iDAAS;AAC1B;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,oDAAY;AACnC;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,oDAAY;AACnC;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,mDAAW;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0BAA0B,mDAAW;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;AC9LA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,wBAAwB;AAClB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4DAA4D,MAAM;AAClE;AACA;AACA;AACA;AACA;AACA,YAAY,mCAAmC;AAC/C;AACA,gDAAgD,MAAM;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qEAAqE,OAAO,SAAS,WAAW;AAChG;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACA;AACA;AACA;AACA;AACA",
+    "file": "lib_index_js.8b68da7de22fb270ee0f.js",
+    "mappings": ";;;;;;;;;;;;;;AAAA;AACA;AACA;AACO;AACP;AACA;AACA;AACA;AACA,CAAC,sBAAsB;AAChB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,oBAAoB,eAAe;AACnC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,gDAAgD,OAAO,KAAK,oBAAoB;AAChF;AACA;;;;;;;;;;;;;;;;;;;;;;;;;;;;;ACxCA;AACA;AACA;AACA;AACwD;AACxD;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,kEAAgB;AAC/B;AACA;AACA,mDAAmD,IAAI;AACvD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,+CAA+C,qBAAqB;AACpE;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,qBAAqB;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0EAA0E,mBAAmB;AAC7F;AACA,iCAAiC;AACjC;AACA,4EAA4E,mBAAmB;AAC/F;AACA,iCAAiC;AACjC,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,6EAA6E,mBAAmB;AAChG;AACA;AACA,6BAA6B;AAC7B;AACA;AACA;AACA;AACA;AACA,+EAA+E,mBAAmB;AAClG;AACA;AACA,6BAA6B;AAC7B;AACA,qBAAqB;AACrB,iBAAiB;AACjB,aAAa;AACb,SAAS;AACT;AACA;AACA,iEAAe,MAAM,EAAC;AACtB;AACyG;AAChD;;;;;;;;;;;;;;;;;;;;;;;;;AChGzD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACyC;AACuE;AAChH;AACO;AACP,wBAAwB,mDAAI;AAC5B;AACA;AACA,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA,eAAe,iDAAS;AACxB;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA,mBAAmB,iDAAS;AAC5B;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,mDAAW;AAClC;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA,iBAAiB,iDAAS;AAC1B;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,oDAAY;AACnC;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,uBAAuB,oDAAY;AACnC;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACP,YAAY,iDAAS;AACrB;AACA;AACA;AACA;AACA;AACA;AACA,8BAA8B,mDAAW;AACzC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,0BAA0B,mDAAW;AACrC;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;;;;;;;;;;;;;;;;;;;;AC9LA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,CAAC,wBAAwB;AAClB;AACP;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,4DAA4D,MAAM;AAClE;AACA;AACA;AACA;AACA;AACA,YAAY,mCAAmC;AAC/C;AACA,gDAAgD,MAAM;AACtD;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,qEAAqE,OAAO,SAAS,WAAW;AAChG;AACA;AACA;AACA;AACA;AACA;AACA;AACO;AACA;AACA;AACA;AACA;AACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
+        "webpack://jupyterlab-celltagsclasses/./lib/apply_on_cells.js",
         "webpack://jupyterlab-celltagsclasses/./lib/index.js",
         "webpack://jupyterlab-celltagsclasses/./lib/metadata.js",
         "webpack://jupyterlab-celltagsclasses/./lib/xpath.js"
     ],
     "sourcesContent": [
-        "/*\n * for attaching keybindings later on, see\n * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d\n */\nimport { INotebookTracker } from '@jupyterlab/notebook';\n/**\n * Initialization data for the jupyterlab-celltagsclasses extension.\n */\nconst plugin = {\n    id: 'jupyterlab-celltagsclasses:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    activate: (app, notebookTracker) => {\n        console.log('extension jupyterlab-celltagsclasses is activating');\n        const class_for_tag = (tag) => `cell-tag-${tag}`;\n        notebookTracker.widgetAdded.connect((_, panel) => {\n            const notebookModel = panel.content.model;\n            if (notebookModel === null) {\n                return;\n            }\n            notebookModel.cells.changed.connect((cellList, change) => {\n                if (change.type !== 'add') {\n                    return;\n                }\n                change.newValues.forEach(cellModel => {\n                    var _a, _b;\n                    // compute widgets attached to cellModel\n                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => cell.model.id === cellModel.id);\n                    if (cellWidgets === undefined || (cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0) {\n                        console.warn('could not find cell widget for cell model', cellModel);\n                        return;\n                    }\n                    console.debug(`found ${cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length} cell widgets`, cellWidgets[0]);\n                    // add classes for pre-existing tags\n                    (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {\n                        console.debug(`adding initial class for tag ${class_for_tag(tag)}`);\n                        cellWidget.addClass(class_for_tag(tag));\n                    }));\n                    // react to changes in tags\n                    cellModel.metadataChanged.connect((sender, change) => {\n                        console.debug('metadata changed', sender, change);\n                        if (change.key !== 'tags') {\n                            // console.debug(\"ignoring non-tags metadata change\")\n                            return;\n                        }\n                        // does not seem useful to recompute this\n                        // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(\n                        //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)\n                        // )\n                        if (change.type === 'change') {\n                            console.debug('change', change, change.newValue);\n                            // compute difference between old and new tags\n                            const oldTags = change.oldValue;\n                            const newTags = change.newValue;\n                            const addedTags = newTags.filter(tag => !oldTags.includes(tag));\n                            const removedTags = oldTags.filter(tag => !newTags.includes(tag));\n                            // console.debug('addedTags', addedTags)\n                            // console.debug('removedTags', removedTags)\n                            cellWidgets.forEach(cellWidget => {\n                                addedTags.forEach(tag => {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                });\n                                removedTags.forEach(tag => {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                });\n                            });\n                        }\n                        else if (change.type === 'add') {\n                            console.log('add', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                        else if (change.type === 'remove') {\n                            console.log('remove', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                    });\n                });\n            });\n        });\n    }\n};\nexport default plugin;\n// re-export metadata helper functions\nexport { md_get, md_set, md_unset, md_has, md_insert, md_remove, md_toggle, md_clean } from './metadata';\n",
+        "/*\n * the logic of applying a function on a set of cells\n */\nexport var Scope;\n(function (Scope) {\n    Scope[Scope[\"All\"] = 0] = \"All\";\n    Scope[Scope[\"Active\"] = 1] = \"Active\";\n    Scope[Scope[\"Multiple\"] = 2] = \"Multiple\";\n})(Scope || (Scope = {}));\nexport const apply_on_cells = (notebookTracker, scope, to_apply) => {\n    var _a;\n    const notebook = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content;\n    if (notebook === undefined) {\n        return;\n    }\n    let actionCells;\n    if (scope === Scope.All) {\n        actionCells = notebook.widgets.slice();\n    }\n    else {\n        const activeCell = notebook.activeCell;\n        if (activeCell === null) {\n            return;\n        }\n        if (scope === Scope.Active) {\n            actionCells = [activeCell];\n        }\n        else {\n            const { anchor, head } = notebook.getContiguousSelection();\n            // when only one cell is selected/active, both are null\n            if (anchor === null || head === null) {\n                actionCells = [activeCell];\n            }\n            else {\n                actionCells = notebook.widgets.slice(anchor, head + 1);\n            }\n        }\n    }\n    // console.log(`apply_on_cells with scope=${scope} on ${actionCells.length} cells`)\n    actionCells.forEach(to_apply);\n};\n",
+        "/*\n * for attaching keybindings later on, see\n * https://towardsdatascience.com/how-to-customize-jupyterlab-keyboard-shortcuts-72321f73753d\n */\nimport { INotebookTracker } from '@jupyterlab/notebook';\n/**\n * Initialization data for the jupyterlab-celltagsclasses extension.\n */\nconst plugin = {\n    id: 'jupyterlab-celltagsclasses:plugin',\n    autoStart: true,\n    requires: [INotebookTracker],\n    activate: (app, notebookTracker) => {\n        console.log('extension jupyterlab-celltagsclasses is activating');\n        const class_for_tag = (tag) => `cell-tag-${tag}`;\n        notebookTracker.widgetAdded.connect((_, panel) => {\n            const notebookModel = panel.content.model;\n            if (notebookModel === null) {\n                return;\n            }\n            notebookModel.cells.changed.connect((cellList, change) => {\n                if (change.type !== 'add') {\n                    return;\n                }\n                change.newValues.forEach(cellModel => {\n                    var _a, _b;\n                    // compute widgets attached to cellModel\n                    const cellWidgets = (_a = notebookTracker.currentWidget) === null || _a === void 0 ? void 0 : _a.content.widgets.filter((cell, index) => cell.model.id === cellModel.id);\n                    if (cellWidgets === undefined || (cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.length) === 0) {\n                        // console.warn('could not find cell widget for cell model', cellModel)\n                        return;\n                    }\n                    // console.debug( `found ${cellWidgets?.length} cell widgets`, cellWidgets[0] )\n                    // add classes for pre-existing tags\n                    (_b = cellModel.getMetadata('tags')) === null || _b === void 0 ? void 0 : _b.forEach((tag) => cellWidgets === null || cellWidgets === void 0 ? void 0 : cellWidgets.forEach(cellWidget => {\n                        // console.debug( `adding initial class for tag ${class_for_tag(tag)}` )\n                        cellWidget.addClass(class_for_tag(tag));\n                    }));\n                    // react to changes in tags\n                    cellModel.metadataChanged.connect((sender, change) => {\n                        // console.debug('metadata changed', sender, change)\n                        if (change.key !== 'tags') {\n                            // console.debug(\"ignoring non-tags metadata change\")\n                            return;\n                        }\n                        // does not seem useful to recompute this\n                        // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(\n                        //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)\n                        // )\n                        if (change.type === 'change') {\n                            // console.debug('change', change, change.newValue)\n                            // compute difference between old and new tags\n                            const oldTags = change.oldValue;\n                            const newTags = change.newValue;\n                            const addedTags = newTags.filter(tag => !oldTags.includes(tag));\n                            const removedTags = oldTags.filter(tag => !newTags.includes(tag));\n                            // console.debug('addedTags', addedTags)\n                            // console.debug('removedTags', removedTags)\n                            cellWidgets.forEach(cellWidget => {\n                                addedTags.forEach(tag => {\n                                    console.debug(`adding class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.addClass(class_for_tag(tag));\n                                });\n                                removedTags.forEach(tag => {\n                                    console.debug(`removing class for tag ${class_for_tag(tag)}`);\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                });\n                            });\n                        }\n                        else if (change.type === 'add') {\n                            console.log('add', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    // console.debug(`adding class for tag ${class_for_tag(tag)}`)\n                                    cellWidget.addClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                        else if (change.type === 'remove') {\n                            console.log('remove', change, change.newValue);\n                            cellWidgets.forEach(cellWidget => {\n                                for (const tag of change.newValue) {\n                                    // console.debug(`removing class for tag ${class_for_tag(tag)}`)\n                                    cellWidget.removeClass(class_for_tag(tag));\n                                }\n                            });\n                        }\n                    });\n                });\n            });\n        });\n    }\n};\nexport default plugin;\n// re-export metadata helper functions\nexport { md_get, md_set, md_unset, md_has, md_insert, md_remove, md_toggle, md_clean } from './metadata';\nexport { Scope, apply_on_cells } from './apply_on_cells';\n",
         "/* eslint-disable prettier/prettier */\n//\n// Metadata helper tools\n// a xpath can be either a dot-separated string, or an array of strings\n//\n//  single valued metadata:\n//\n// (*) md_get: get a metadata value\n//         e.g. md_get(cell, \"some.path.in.the.metadata\")\n//           or md_get(cell, \"some.path.in.the.metadata\", \"default value\")\n//           or md_get(cell, [\"some\", \"path\", \"in\", \"the\", \"metadata\"])\n// (*) md_set: set a metadata value\n//         e.g. md_set(cell, \"some.path.in.the.metadata\", \"new value\")\n// (*) md_unset: unset a metadata value\n//         e.g. md_unset(cell, \"some.path.in.the.metadata\")\n//\n//  list valued metadata (typically xpath = 'tags')\n//\n// (*) md_has: check if a value is present in a metadata list\n//         e.g. md_has(cell, \"path.to.tags\", \"tag-to-check\")\n// (*) md_insert: insert a value in a metadata list\n//         e.g. md_insert(cell, \"path.to.tags\", \"added-tag\")\n// (*) md_remove: remove a value from a metadata list\n//         e.g. md_remove(cell, \"path.to.tags\", \"removed-tag\")\n// (*) md_toggle: toggle a value in a metadata list\n//         e.g. md_toggle(cell, \"path.to.tags\", \"toggled-tag\")\n//\n// clean up\n// (*) md_clean: remove empty metadata elements\n//         e.g. md_clean(cell, \"path.to.subtree\")\n//         or more typically\n//              md_clean(cell, \"\")\n//          will alter the cell's metadata so as to remove empty lists or empty keys\nimport { Cell } from '@jupyterlab/cells';\nimport { normalize, xpath_get, xpath_set, xpath_unset, xpath_insert, xpath_remove, xpath_clean } from './xpath';\n// atomic values\nexport const md_get = (cell, xpath, if_missing) => {\n    if (cell instanceof Cell) {\n        cell = cell.model;\n    }\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.getMetadata(first);\n    if (start === undefined) {\n        return if_missing;\n    }\n    else {\n        return xpath_get(start, tail);\n    }\n};\nexport const md_set = (cell, xpath, value) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.model.getMetadata(first);\n    if (tail.length === 0) {\n        cell.model.setMetadata(first, value);\n        return value;\n    }\n    const subtree = start || {};\n    const retcod = xpath_set(subtree, tail, value);\n    cell.model.setMetadata(first, subtree);\n    return retcod;\n};\nexport const md_unset = (cell, xpath) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.model.getMetadata(first);\n    if (start === undefined) {\n        return false;\n    }\n    if (tail.length === 0) {\n        cell.model.deleteMetadata(first);\n        return true;\n    }\n    else {\n        const retcod = xpath_unset(start, tail);\n        cell.model.setMetadata(first, start);\n        return retcod;\n    }\n};\n// lists (e.g. tags)\nexport const md_has = (cell, xpath, key) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.model.getMetadata(first);\n    if (start === undefined) {\n        return false;\n    }\n    const list = xpath_get(start, tail);\n    if (list === undefined) {\n        return false;\n    }\n    return list.indexOf(key) >= 0;\n};\nexport const md_insert = (cell, xpath, key) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.model.getMetadata(first);\n    if (tail.length === 0) {\n        let sublist;\n        if (start !== undefined) {\n            sublist = start;\n            // use another object as otherwise .setMetadata() does not seem to propagate\n            sublist = sublist.slice();\n        }\n        else {\n            sublist = [];\n        }\n        if (sublist.indexOf(key) < 0) {\n            sublist.push(key);\n            cell.model.setMetadata(first, sublist);\n            return key;\n        }\n        else {\n            return undefined;\n        }\n    }\n    else {\n        const subtree = start || {};\n        const retcod = xpath_insert(subtree, tail, key);\n        cell.model.setMetadata(first, subtree);\n        return retcod;\n    }\n};\nexport const md_remove = (cell, xpath, key) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    const start = cell.model.getMetadata(first);\n    if (start === undefined) {\n        return undefined;\n    }\n    if (tail.length === 0) {\n        const sublist = start;\n        if (!(sublist instanceof Array)) {\n            return undefined;\n        }\n        // use another object as otherwise .set() does not seem to propagate\n        const copy = sublist.slice();\n        const index = copy.indexOf(key);\n        if (index < 0) {\n            return undefined;\n        }\n        // const as_array = sublist as Array<string>\n        copy.splice(index, 1);\n        cell.model.setMetadata(first, copy);\n        return key;\n    }\n    else {\n        const subtree = start;\n        const retcod = xpath_remove(subtree, tail, key);\n        cell.model.setMetadata(first, subtree);\n        return retcod;\n    }\n};\nexport const md_toggle = (cell, xpath, key) => {\n    xpath = normalize(xpath);\n    if (!md_has(cell, xpath, key)) {\n        return md_insert(cell, xpath, key);\n    }\n    else {\n        return md_remove(cell, xpath, key);\n    }\n};\nexport const md_clean = (cell, xpath) => {\n    xpath = normalize(xpath);\n    const [first, ...tail] = xpath;\n    if (first === undefined) {\n        console.log(cell.model.metadata);\n        // no xpath, clean the whole metadata\n        for (const key of Object.entries(cell.model.metadata)) {\n            const xpath = key;\n            const new_value = xpath_clean(md_get(cell, xpath), \"\");\n            if ((new_value === undefined) || (new_value.length === 0)) {\n                md_unset(cell, xpath);\n            }\n            else {\n                md_set(cell, xpath, new_value);\n            }\n        }\n    }\n    else {\n        const subtree = md_get(cell, first);\n        const new_value = xpath_clean(subtree, tail);\n        if ((new_value === undefined) || (new_value.length === 0)) {\n            md_unset(cell, first);\n        }\n        else {\n            md_set(cell, first, new_value);\n        }\n    }\n};\n",
         "/* eslint-disable no-case-declarations */\n/* eslint-disable prettier/prettier */\n// helpers to manage a JS object\n//\n// in this module we are only concerned about doing side effects\n// in a JavaScript object\n// what to do on the passed object\nvar Action;\n(function (Action) {\n    Action[Action[\"Get\"] = 0] = \"Get\";\n    Action[Action[\"Set\"] = 1] = \"Set\";\n    Action[Action[\"Unset\"] = 2] = \"Unset\";\n    Action[Action[\"Insert\"] = 3] = \"Insert\";\n    Action[Action[\"Remove\"] = 4] = \"Remove\";\n})(Action || (Action = {}));\nexport const normalize = (xpath) => {\n    if (typeof xpath === 'string') {\n        const string = xpath;\n        if (string.length === 0) {\n            return [];\n        }\n        return string.split('.');\n    }\n    else if (xpath instanceof Array) {\n        return xpath;\n    }\n    else {\n        console.error(`xpath must be string or array, got ${xpath}`);\n        return [];\n    }\n};\nconst _manage_metadata = (data, // intended to be cell.metadata\naction, xpath, value) => {\n    const { Get, Set, Unset, Insert, Remove, } = Action;\n    const recurse = (scanner, action, xpath, value) => {\n        // console.log(`in recurse with xpath=${xpath}`)\n        if (xpath.length === 0) {\n            switch (action) {\n                case Get:\n                    return scanner;\n                default:\n                    return undefined;\n            }\n        }\n        else if (xpath.length === 1) {\n            const [step] = xpath;\n            //\n            switch (action) {\n                case Get:\n                    return scanner[step];\n                case Set:\n                    scanner[step] = value;\n                    return value;\n                case Unset:\n                    if (step in scanner) {\n                        delete scanner[step];\n                        return true;\n                    }\n                    else {\n                        return false;\n                    }\n                case Insert:\n                    // create list if needed\n                    if (!(step in scanner)) {\n                        scanner[step] = [];\n                    }\n                    if (!(scanner[step] instanceof Array)) {\n                        return undefined;\n                    }\n                    // insert if not already present\n                    {\n                        const list = scanner[step];\n                        if (list.indexOf(value) < 0) {\n                            list.push(value);\n                            return value;\n                        }\n                        else {\n                            return undefined;\n                        }\n                    }\n                case Remove:\n                    if (!(scanner[step] instanceof Array)) {\n                        return undefined;\n                    }\n                    const list = (scanner[step]);\n                    // list.pop(value) is not accepted by ts ?!?\n                    const index = list.indexOf(value);\n                    if (index >= 0) {\n                        list.splice(index, 1);\n                    }\n                    return value;\n            }\n        }\n        else {\n            const [first, ...rest] = xpath;\n            if (first in scanner) {\n                if (!(scanner[first] instanceof Object)) {\n                    return undefined;\n                }\n                else {\n                    const next = scanner[first];\n                    return recurse(next, action, rest, value);\n                }\n            }\n            else {\n                switch (action) {\n                    case Get:\n                        return undefined;\n                    case Set:\n                        scanner[first] = {};\n                        const next = scanner[first];\n                        return recurse(next, action, rest, value);\n                    case Unset:\n                        return undefined;\n                    case Insert:\n                        if (rest.length === 0) {\n                            scanner[first] = [];\n                            return recurse(scanner[first], action, rest, value);\n                        }\n                        else {\n                            scanner[first] = {};\n                            return recurse(scanner[first], action, rest, value);\n                        }\n                    case Remove:\n                        return undefined;\n                }\n            }\n        }\n    };\n    const xpath_list = normalize(xpath);\n    return recurse(data, action, xpath_list, value);\n};\nconst _clean_metadata = (data, xpath) => {\n    const not_empty = (x) => {\n        if (x instanceof Array) {\n            return x.length !== 0;\n        }\n        else if (x instanceof Object) {\n            return Object.keys(x).length !== 0;\n        }\n        else if ((typeof x) === 'string') {\n            return x.length !== 0;\n        }\n        else {\n            return true;\n        }\n    };\n    const clean_array = (data) => {\n        return data.map(clean).filter(not_empty);\n    };\n    const clean_object = (data) => {\n        const result = {};\n        for (const key in data) {\n            const value = data[key];\n            const cleaned = clean(value);\n            if (not_empty(cleaned)) {\n                result[key] = cleaned;\n            }\n        }\n        return result;\n    };\n    const clean = (data) => {\n        if (data instanceof Array) {\n            return clean_array(data);\n        }\n        else if (data instanceof Object) {\n            return clean_object(data);\n        }\n        else {\n            return data;\n        }\n    };\n    const xpath_list = normalize(xpath);\n    if (xpath_list.length === 0) {\n        return clean(data);\n    }\n    else {\n        const start = xpath_get(data, xpath_list);\n        if (start === undefined) {\n            // nothing serious here, just a debug message\n            //console.debug(`DBG: xpath_clean: nothing to clean at ${xpath} - from ${xpath_list}`)\n            return data;\n        }\n        else {\n            return xpath_set(data, xpath_list, clean(start));\n        }\n    }\n};\nexport const xpath_get = (metadata, xpath) => _manage_metadata(metadata, Action.Get, xpath, undefined);\nexport const xpath_set = (metadata, xpath, value) => _manage_metadata(metadata, Action.Set, xpath, value);\nexport const xpath_unset = (metadata, xpath) => _manage_metadata(metadata, Action.Unset, xpath, undefined);\nexport const xpath_insert = (metadata, xpath, key) => _manage_metadata(metadata, Action.Insert, xpath, key);\nexport const xpath_remove = (metadata, xpath, key) => _manage_metadata(metadata, Action.Remove, xpath, key);\nexport const xpath_clean = (metadata, xpath) => _clean_metadata(metadata, xpath);\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.cc30540db9a44cea877f.js.map` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8311688311688312%*

 * *Differences: {"'file'": "'remoteEntry.8de4dac15b9641f8640c.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.cc30540db9a44cea877f.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.8de4dac15b9641f8640c.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,8EAA8E;WAC5G;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC5KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-celltagsclasses/webpack/container-entry",
         "webpack://jupyterlab-celltagsclasses/webpack/bootstrap",
         "webpack://jupyterlab-celltagsclasses/webpack/runtime/compat get default export",
         "webpack://jupyterlab-celltagsclasses/webpack/runtime/define property getters",
@@ -25,23 +25,23 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId](module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"e0bf585461963e3d1e28\",\"style_index_js\":\"4784725fff15b54ffe3d\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"8b68da7de22fb270ee0f\",\"style_index_js\":\"4784725fff15b54ffe3d\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-celltagsclasses:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.2.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab-celltagsclasses\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-celltagsclasses\", \"0.3.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"beta\",2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
-        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-celltagsclasses\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_celltagsclasses\"] = self[\"webpackChunkjupyterlab_celltagsclasses\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/notebook\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/notebook\", [1,4,0,0,,\"rc\",1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/cells\": () => (loadVersionCheck(\"default\", \"@jupyterlab/cells\", [1,4,0,0,,\"rc\",1]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/notebook\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/cells\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab-celltagsclasses\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_celltagsclasses\"] = self[\"webpackChunkjupyterlab_celltagsclasses\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab-celltagsclasses\");\n",
         ""
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.e8bcb578ed91b775bd99.js` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "cddacca2ba0e6c761c6d",
+                "lib_index_js": "8b68da7de22fb270ee0f",
                 "style_index_js": "4784725fff15b54ffe3d"
             } [chunkId] + ".js";
             /******/
         };
         /******/
     })();
     /******/
@@ -426,15 +426,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab-celltagsclasses", "0.2.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab-celltagsclasses", "0.3.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -827,17 +827,17 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "beta", 2])),
+            "webpack/sharing/consume/default/@jupyterlab/notebook": () => (loadSingletonVersionCheck("default", "@jupyterlab/notebook", [1, 4, 0, 0, , "rc", 1])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 4, 0, 0, , "beta", 2]))
+            "webpack/sharing/consume/default/@jupyterlab/cells": () => (loadVersionCheck("default", "@jupyterlab/cells", [1, 4, 0, 0, , "rc", 1]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -982,15 +982,15 @@
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
@@ -1075,8 +1075,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-celltagsclasses");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-celltagsclasses"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.e8bcb578ed91b775bd99.js.map
+//# sourceMappingURL=remoteEntry.8de4dac15b9641f8640c.js.map
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map` & `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/media/screenshot.png` & `jupyterlab_celltagsclasses-0.3.0/media/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/index.ts` & `jupyterlab_celltagsclasses-0.3.0/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -36,45 +36,40 @@
         change.newValues.forEach(cellModel => {
           // compute widgets attached to cellModel
           const cellWidgets =
             notebookTracker.currentWidget?.content.widgets.filter(
               (cell: Cell, index: number) => cell.model.id === cellModel.id
             )
           if (cellWidgets === undefined || cellWidgets?.length === 0) {
-            console.warn('could not find cell widget for cell model', cellModel)
+            // console.warn('could not find cell widget for cell model', cellModel)
             return
           }
-          console.debug(
-            `found ${cellWidgets?.length} cell widgets`,
-            cellWidgets[0]
-          )
+          // console.debug( `found ${cellWidgets?.length} cell widgets`, cellWidgets[0] )
 
           // add classes for pre-existing tags
           cellModel.getMetadata('tags')?.forEach((tag: string) =>
             cellWidgets?.forEach(cellWidget => {
-              console.debug(
-                `adding initial class for tag ${class_for_tag(tag)}`
-              )
+              // console.debug( `adding initial class for tag ${class_for_tag(tag)}` )
               cellWidget.addClass(class_for_tag(tag))
             })
           )
 
           // react to changes in tags
           cellModel.metadataChanged.connect((sender: ICellModel, change) => {
-            console.debug('metadata changed', sender, change)
+            // console.debug('metadata changed', sender, change)
             if (change.key !== 'tags') {
               // console.debug("ignoring non-tags metadata change")
               return
             }
             // does not seem useful to recompute this
             // const cellWidgets = notebookTracker.currentWidget?.content.widgets.filter(
             //   (cell: Cell, index: number) => (cell.model.id === cellModel.id)
             // )
             if (change.type === 'change') {
-              console.debug('change', change, change.newValue)
+              // console.debug('change', change, change.newValue)
               // compute difference between old and new tags
               const oldTags = change.oldValue as string[]
               const newTags = change.newValue as string[]
               const addedTags = newTags.filter(tag => !oldTags.includes(tag))
               const removedTags = oldTags.filter(tag => !newTags.includes(tag))
               // console.debug('addedTags', addedTags)
               // console.debug('removedTags', removedTags)
@@ -88,23 +83,23 @@
                   cellWidget.removeClass(class_for_tag(tag))
                 })
               })
             } else if (change.type === 'add') {
               console.log('add', change, change.newValue)
               cellWidgets.forEach(cellWidget => {
                 for (const tag of change.newValue) {
-                  console.debug(`adding class for tag ${class_for_tag(tag)}`)
+                  // console.debug(`adding class for tag ${class_for_tag(tag)}`)
                   cellWidget.addClass(class_for_tag(tag))
                 }
               })
             } else if (change.type === 'remove') {
               console.log('remove', change, change.newValue)
               cellWidgets.forEach(cellWidget => {
                 for (const tag of change.newValue) {
-                  console.debug(`removing class for tag ${class_for_tag(tag)}`)
+                  // console.debug(`removing class for tag ${class_for_tag(tag)}`)
                   cellWidget.removeClass(class_for_tag(tag))
                 }
               })
             }
           })
         })
       })
@@ -112,7 +107,9 @@
   }
 }
 
 export default plugin
 
 // re-export metadata helper functions
 export { md_get, md_set, md_unset, md_has, md_insert, md_remove, md_toggle, md_clean } from './metadata'
+
+export { Scope, apply_on_cells } from './apply_on_cells'
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/metadata.ts` & `jupyterlab_celltagsclasses-0.3.0/src/metadata.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/xpath-test.js` & `jupyterlab_celltagsclasses-0.3.0/src/xpath-test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/xpath-test.ts` & `jupyterlab_celltagsclasses-0.3.0/src/xpath-test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/xpath.js` & `jupyterlab_celltagsclasses-0.3.0/src/xpath.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/src/xpath.ts` & `jupyterlab_celltagsclasses-0.3.0/src/xpath.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/style/base.css` & `jupyterlab_celltagsclasses-0.3.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/.gitignore` & `jupyterlab_celltagsclasses-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/LICENSE` & `jupyterlab_celltagsclasses-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/README.md` & `jupyterlab_celltagsclasses-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,19 +34,30 @@
 specifically the DOM elements that are decorated have the `.jpCell` class set by jlab, like so, where we have set tag `celltagsclasses-test1`
 
 ![](media/screenshot.png)
 
 ### metadata management helper functions
 
 it also exports utilities to manage a cell's metadata, specifically for
+
 * getting, setting or unsetting a key/value pair
 * adding, removing items in a list inside the metadata (e.g. tags)
 * cleaning the metadata for empty/useless items
 
-to that effect, see the `md_get` and similar functions
+to that effect, see the `md_get` and similar functions in `metadata.ts` (that can be imported right from the module)
+
+### helper: apply function on cells
+
+the `apply_on_cells` function allows you to write a function that works on an individual cell, and then call it on either
+
+* the active cell only
+* all the selected cells if relevant, otherwise the active cell
+* all the cells in the notebook
+
+for that you can pass it a `Scope` value that can be either `Active`, `Multiple`, or `All`
 
 ## Development
 
 See the documentation on Jlab extensions for more details; the gist of it is
 
 ### Development install
```

### Comparing `jupyterlab_celltagsclasses-0.2.0/pyproject.toml` & `jupyterlab_celltagsclasses-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.2.0/PKG-INFO` & `jupyterlab_celltagsclasses-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_celltagsclasses
-Version: 0.2.0
+Version: 0.3.0
 Summary: JLAB extension to add classes to cells based on their tags
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-celltagsclasses
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-celltagsclasses/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-celltagsclasses.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
         
@@ -87,19 +87,30 @@
 specifically the DOM elements that are decorated have the `.jpCell` class set by jlab, like so, where we have set tag `celltagsclasses-test1`
 
 ![](media/screenshot.png)
 
 ### metadata management helper functions
 
 it also exports utilities to manage a cell's metadata, specifically for
+
 * getting, setting or unsetting a key/value pair
 * adding, removing items in a list inside the metadata (e.g. tags)
 * cleaning the metadata for empty/useless items
 
-to that effect, see the `md_get` and similar functions
+to that effect, see the `md_get` and similar functions in `metadata.ts` (that can be imported right from the module)
+
+### helper: apply function on cells
+
+the `apply_on_cells` function allows you to write a function that works on an individual cell, and then call it on either
+
+* the active cell only
+* all the selected cells if relevant, otherwise the active cell
+* all the cells in the notebook
+
+for that you can pass it a `Scope` value that can be either `Active`, `Multiple`, or `All`
 
 ## Development
 
 See the documentation on Jlab extensions for more details; the gist of it is
 
 ### Development install
```

