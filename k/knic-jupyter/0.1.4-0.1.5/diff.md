# Comparing `tmp/knic_jupyter-0.1.4.tar.gz` & `tmp/knic_jupyter-0.1.5.tar.gz`

## Comparing `knic_jupyter-0.1.4.tar` & `knic_jupyter-0.1.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.eslintrc.js
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/Dockerfile
--rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/GEO-R-6a.ipynb
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/RELEASE.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/Untitled.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/babel.config.js
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/docker-compose.yaml
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/environment.yaml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/install.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/jest.config.js
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/package.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/requirements.txt
--rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/run-jupyter-lab.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/setup.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/tsconfig.json
--rw-r--r--   0        0        0   388358 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/yarn.lock
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/build_log.json
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/package.json
--rw-r--r--   0        0        0    20010 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js
--rw-r--r--   0        0        0    21213 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js.map
--rw-r--r--   0        0        0    29216 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js
--rw-r--r--   0        0        0    27936 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js.map
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/style.js
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map
--rw-r--r--   0        0        0   135674 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js
--rw-r--r--   0        0        0   117914 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map
--rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map
--rw-r--r--   0        0        0   195842 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js
--rw-r--r--   0        0        0   230605 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map
--rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/src/index.ts
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/src/__tests__/KNICS_Jupyter_frontend.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/style/index.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/ui-tests/tests/KNICS_Jupyter_frontend.spec.ts
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/LICENSE
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/README.md
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 knic_jupyter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.eslintrc.js
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/Dockerfile
+-rw-r--r--   0        0        0     6067 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/GEO-R-6a.ipynb
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/MANIFEST.in
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/babel.config.js
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/config.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/docker-compose.yaml
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/environment.yaml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/install.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/jest.config.js
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/package.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/requirements.txt
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/run-jupyter-lab.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/setup.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/tsconfig.json
+-rw-r--r--   0        0        0   388358 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/yarn.lock
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/build_log.json
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/package.json
+-rw-r--r--   0        0        0    20010 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js
+-rw-r--r--   0        0        0    21213 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js.map
+-rw-r--r--   0        0        0    29216 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js
+-rw-r--r--   0        0        0    27936 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js.map
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/style.js
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map
+-rw-r--r--   0        0        0   135674 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js
+-rw-r--r--   0        0        0   117914 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map
+-rw-r--r--   0        0        0    12054 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map
+-rw-r--r--   0        0        0   195842 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js
+-rw-r--r--   0        0        0   230605 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/src/index.ts
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/src/__tests__/KNICS_Jupyter_frontend.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/style/index.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/ui-tests/tests/KNICS_Jupyter_frontend.spec.ts
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/README.md
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 knic_jupyter-0.1.5/PKG-INFO
```

### Comparing `knic_jupyter-0.1.4/.eslintrc.js` & `knic_jupyter-0.1.5/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/GEO-R-6a.ipynb` & `knic_jupyter-0.1.5/GEO-R-6a.ipynb`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/RELEASE.md` & `knic_jupyter-0.1.5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/environment.yaml` & `knic_jupyter-0.1.5/environment.yaml`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/jest.config.js` & `knic_jupyter-0.1.5/jest.config.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/package.json` & `knic_jupyter-0.1.5/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.1.5'"}*

```diff
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.1.5"
 }
```

### Comparing `knic_jupyter-0.1.4/requirements.txt` & `knic_jupyter-0.1.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/tsconfig.json` & `knic_jupyter-0.1.5/tsconfig.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/yarn.lock` & `knic_jupyter-0.1.5/yarn.lock`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/build_log.json` & `knic_jupyter-0.1.5/knic-jupyter/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/package.json` & `knic_jupyter-0.1.5/knic-jupyter/labextension/package.json`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/lib_index_js.f8b97348b0adbe8ebbfc.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/remoteEntry.8e11d4bedb2c1c09fb7d.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/style_index_js.f52bc77755c454c42949.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_axios_index_js.1ca6784f009c20db95e8.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.a0ffbb03a81b5fb1c68c.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map` & `knic_jupyter-0.1.5/knic-jupyter/labextension/static/vendors-node_modules_dexie_dist_modern_dexie_mjs.0aea58707561a10ac2f5.js.map`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/src/index.ts` & `knic_jupyter-0.1.5/src/index.ts`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/ui-tests/README.md` & `knic_jupyter-0.1.5/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/ui-tests/jupyter_server_test_config.py` & `knic_jupyter-0.1.5/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/.gitignore` & `knic_jupyter-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/LICENSE` & `knic_jupyter-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/README.md` & `knic_jupyter-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/pyproject.toml` & `knic_jupyter-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `knic_jupyter-0.1.4/PKG-INFO` & `knic_jupyter-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knic-jupyter
-Version: 0.1.4
+Version: 0.1.5
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/usc-isi-i2/knic-jupyter
 Project-URL: Bug Tracker, https://github.com/usc-isi-i2/knic-jupyter/issues
 Project-URL: Repository, https://github.com/usc-isi-i2/knic-jupyter.git
 License: MIT License
         
         Copyright (c) 2017 University of Southern California
```

