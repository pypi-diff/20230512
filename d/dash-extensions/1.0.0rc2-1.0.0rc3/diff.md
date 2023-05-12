# Comparing `tmp/dash_extensions-1.0.0rc2.tar.gz` & `tmp/dash_extensions-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_extensions-1.0.0rc2.tar", max compression
+gzip compressed data, was "dash_extensions-1.0.0rc3.tar", max compression
```

## Comparing `dash_extensions-1.0.0rc2.tar` & `dash_extensions-1.0.0rc3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1077 2021-08-09 04:16:22.416456 dash_extensions-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     1877 2023-05-04 16:58:08.556489 dash_extensions-1.0.0rc2/README.md
--rw-r--r--   0        0        0     2243 2023-05-04 16:04:18.984049 dash_extensions-1.0.0rc2/dash_extensions/BeforeAfter.py
--rw-r--r--   0        0        0     2925 2022-03-23 18:35:09.530478 dash_extensions-1.0.0rc2/dash_extensions/Burger.py
--rw-r--r--   0        0        0     1505 2022-05-01 05:16:38.479837 dash_extensions-1.0.0rc2/dash_extensions/CircleBreaker.py
--rw-r--r--   0        0        0     1388 2023-05-04 16:04:18.984995 dash_extensions-1.0.0rc2/dash_extensions/CycleBreaker.py
--rw-r--r--   0        0        0     1282 2023-05-04 16:04:18.985393 dash_extensions-1.0.0rc2/dash_extensions/DeferScript.py
--rw-r--r--   0        0        0     1801 2022-02-20 12:21:16.871666 dash_extensions-1.0.0rc2/dash_extensions/Download.py
--rw-r--r--   0        0        0     2596 2023-05-04 16:04:18.986055 dash_extensions-1.0.0rc2/dash_extensions/EventListener.py
--rw-r--r--   0        0        0     2043 2023-05-04 16:04:18.986630 dash_extensions-1.0.0rc2/dash_extensions/EventSource.py
--rw-r--r--   0        0        0     2906 2022-04-01 17:51:33.939514 dash_extensions-1.0.0rc2/dash_extensions/Keyboard.py
--rw-r--r--   0        0        0     1849 2022-04-01 17:51:33.940312 dash_extensions-1.0.0rc2/dash_extensions/ListOperator.py
--rw-r--r--   0        0        0     2272 2022-03-09 11:37:59.341906 dash_extensions-1.0.0rc2/dash_extensions/ListStore.py
--rw-r--r--   0        0        0     2665 2023-05-04 16:04:18.987307 dash_extensions-1.0.0rc2/dash_extensions/Lottie.py
--rw-r--r--   0        0        0     1542 2023-05-04 16:04:18.987849 dash_extensions-1.0.0rc2/dash_extensions/Mermaid.py
--rw-r--r--   0        0        0     2134 2022-02-20 12:21:16.904136 dash_extensions-1.0.0rc2/dash_extensions/Monitor.py
--rw-r--r--   0        0        0     1701 2022-03-09 11:05:05.197301 dash_extensions-1.0.0rc2/dash_extensions/PropOperator.py
--rw-r--r--   0        0        0     1377 2023-05-04 16:04:18.988254 dash_extensions-1.0.0rc2/dash_extensions/Purify.py
--rw-r--r--   0        0        0     1809 2023-05-04 16:04:18.988789 dash_extensions-1.0.0rc2/dash_extensions/Ticker.py
--rw-r--r--   0        0        0     1885 2023-05-04 16:04:18.989393 dash_extensions-1.0.0rc2/dash_extensions/WebSocket.py
--rw-r--r--   0        0        0     2492 2022-07-18 07:36:13.443588 dash_extensions-1.0.0rc2/dash_extensions/__init__.py
--rw-r--r--   0        0        0      519 2023-05-04 16:04:18.990459 dash_extensions-1.0.0rc2/dash_extensions/_imports_.py
--rw-r--r--   0        0        0   114292 2022-02-16 10:00:42.958352 dash_extensions-1.0.0rc2/dash_extensions/async-burger.js
--rw-r--r--   0        0        0   517537 2022-02-16 10:00:42.959968 dash_extensions-1.0.0rc2/dash_extensions/async-burger.js.map
--rw-r--r--   0        0        0   292596 2022-05-02 16:25:25.006211 dash_extensions-1.0.0rc2/dash_extensions/async-lottie.js
--rw-r--r--   0        0        0  1063846 2022-12-05 09:25:25.233867 dash_extensions-1.0.0rc2/dash_extensions/async-lottie.js.map
--rw-r--r--   0        0        0   838722 2023-04-21 09:01:21.928275 dash_extensions-1.0.0rc2/dash_extensions/async-mermaid.js
--rw-r--r--   0        0        0      108 2023-04-21 09:01:21.928044 dash_extensions-1.0.0rc2/dash_extensions/async-mermaid.js.LICENSE.txt
--rw-r--r--   0        0        0  2940311 2023-04-21 09:01:21.928514 dash_extensions-1.0.0rc2/dash_extensions/async-mermaid.js.map
--rw-r--r--   0        0        0   125717 2023-05-04 16:04:17.457022 dash_extensions-1.0.0rc2/dash_extensions/dash_extensions.min.js
--rw-r--r--   0        0        0      342 2023-04-21 09:01:21.932190 dash_extensions-1.0.0rc2/dash_extensions/dash_extensions.min.js.LICENSE.txt
--rw-r--r--   0        0        0   429997 2023-05-04 16:04:17.457130 dash_extensions-1.0.0rc2/dash_extensions/dash_extensions.min.js.map
--rw-r--r--   0        0        0     2232 2022-04-22 10:52:51.916624 dash_extensions-1.0.0rc2/dash_extensions/dataiku.py
--rw-r--r--   0        0        0    45252 2023-05-04 15:59:45.538221 dash_extensions-1.0.0rc2/dash_extensions/enrich.py
--rw-r--r--   0        0        0     1520 2022-02-20 12:21:16.962416 dash_extensions-1.0.0rc2/dash_extensions/javascript.py
--rw-r--r--   0        0        0    20497 2023-05-04 16:04:18.990389 dash_extensions-1.0.0rc2/dash_extensions/metadata.json
--rw-r--r--   0        0        0     2360 2023-05-04 16:04:18.448009 dash_extensions-1.0.0rc2/dash_extensions/package-info.json
--rw-r--r--   0        0        0     3468 2023-04-21 08:59:04.250798 dash_extensions-1.0.0rc2/dash_extensions/snippets.py
--rw-r--r--   0        0        0      960 2023-05-04 16:05:33.374455 dash_extensions-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 dash_extensions-1.0.0rc2/setup.py
--rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 dash_extensions-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-08-09 04:16:22.416456 dash_extensions-1.0.0rc3/LICENSE
+-rw-r--r--   0        0        0     1877 2023-05-11 12:16:12.110694 dash_extensions-1.0.0rc3/README.md
+-rw-r--r--   0        0        0     2243 2023-05-11 12:18:35.538831 dash_extensions-1.0.0rc3/dash_extensions/BeforeAfter.py
+-rw-r--r--   0        0        0     2925 2022-03-23 18:35:09.530478 dash_extensions-1.0.0rc3/dash_extensions/Burger.py
+-rw-r--r--   0        0        0     1505 2022-05-01 05:16:38.479837 dash_extensions-1.0.0rc3/dash_extensions/CircleBreaker.py
+-rw-r--r--   0        0        0     1388 2023-05-11 12:18:35.539553 dash_extensions-1.0.0rc3/dash_extensions/CycleBreaker.py
+-rw-r--r--   0        0        0     1282 2023-05-11 12:18:35.539917 dash_extensions-1.0.0rc3/dash_extensions/DeferScript.py
+-rw-r--r--   0        0        0     1801 2022-02-20 12:21:16.871666 dash_extensions-1.0.0rc3/dash_extensions/Download.py
+-rw-r--r--   0        0        0     2596 2023-05-11 12:18:35.540539 dash_extensions-1.0.0rc3/dash_extensions/EventListener.py
+-rw-r--r--   0        0        0     2043 2023-05-11 12:18:35.541109 dash_extensions-1.0.0rc3/dash_extensions/EventSource.py
+-rw-r--r--   0        0        0     2906 2022-04-01 17:51:33.939514 dash_extensions-1.0.0rc3/dash_extensions/Keyboard.py
+-rw-r--r--   0        0        0     1849 2022-04-01 17:51:33.940312 dash_extensions-1.0.0rc3/dash_extensions/ListOperator.py
+-rw-r--r--   0        0        0     2272 2022-03-09 11:37:59.341906 dash_extensions-1.0.0rc3/dash_extensions/ListStore.py
+-rw-r--r--   0        0        0     2665 2023-05-11 12:18:35.541759 dash_extensions-1.0.0rc3/dash_extensions/Lottie.py
+-rw-r--r--   0        0        0     1542 2023-05-11 12:18:35.542255 dash_extensions-1.0.0rc3/dash_extensions/Mermaid.py
+-rw-r--r--   0        0        0     2134 2022-02-20 12:21:16.904136 dash_extensions-1.0.0rc3/dash_extensions/Monitor.py
+-rw-r--r--   0        0        0     1701 2022-03-09 11:05:05.197301 dash_extensions-1.0.0rc3/dash_extensions/PropOperator.py
+-rw-r--r--   0        0        0     1377 2023-05-11 12:18:35.542651 dash_extensions-1.0.0rc3/dash_extensions/Purify.py
+-rw-r--r--   0        0        0     1809 2023-05-11 12:18:35.543181 dash_extensions-1.0.0rc3/dash_extensions/Ticker.py
+-rw-r--r--   0        0        0     1885 2023-05-11 12:18:35.543757 dash_extensions-1.0.0rc3/dash_extensions/WebSocket.py
+-rw-r--r--   0        0        0     2492 2022-07-18 07:36:13.443588 dash_extensions-1.0.0rc3/dash_extensions/__init__.py
+-rw-r--r--   0        0        0      519 2023-05-11 12:18:35.544838 dash_extensions-1.0.0rc3/dash_extensions/_imports_.py
+-rw-r--r--   0        0        0   114292 2022-02-16 10:00:42.958352 dash_extensions-1.0.0rc3/dash_extensions/async-burger.js
+-rw-r--r--   0        0        0   517537 2022-02-16 10:00:42.959968 dash_extensions-1.0.0rc3/dash_extensions/async-burger.js.map
+-rw-r--r--   0        0        0   292596 2022-05-02 16:25:25.006211 dash_extensions-1.0.0rc3/dash_extensions/async-lottie.js
+-rw-r--r--   0        0        0  1063846 2022-12-05 09:25:25.233867 dash_extensions-1.0.0rc3/dash_extensions/async-lottie.js.map
+-rw-r--r--   0        0        0   838722 2023-04-21 09:01:21.928275 dash_extensions-1.0.0rc3/dash_extensions/async-mermaid.js
+-rw-r--r--   0        0        0      108 2023-04-21 09:01:21.928044 dash_extensions-1.0.0rc3/dash_extensions/async-mermaid.js.LICENSE.txt
+-rw-r--r--   0        0        0  2940311 2023-04-21 09:01:21.928514 dash_extensions-1.0.0rc3/dash_extensions/async-mermaid.js.map
+-rw-r--r--   0        0        0   125717 2023-05-11 12:18:34.253374 dash_extensions-1.0.0rc3/dash_extensions/dash_extensions.min.js
+-rw-r--r--   0        0        0      342 2023-04-21 09:01:21.932190 dash_extensions-1.0.0rc3/dash_extensions/dash_extensions.min.js.LICENSE.txt
+-rw-r--r--   0        0        0   429997 2023-05-11 12:18:34.253617 dash_extensions-1.0.0rc3/dash_extensions/dash_extensions.min.js.map
+-rw-r--r--   0        0        0     2232 2022-04-22 10:52:51.916624 dash_extensions-1.0.0rc3/dash_extensions/dataiku.py
+-rw-r--r--   0        0        0    45252 2023-05-11 12:16:12.111184 dash_extensions-1.0.0rc3/dash_extensions/enrich.py
+-rw-r--r--   0        0        0     1520 2022-02-20 12:21:16.962416 dash_extensions-1.0.0rc3/dash_extensions/javascript.py
+-rw-r--r--   0        0        0    20497 2023-05-11 12:18:35.544763 dash_extensions-1.0.0rc3/dash_extensions/metadata.json
+-rw-r--r--   0        0        0     2360 2023-05-11 12:18:35.015106 dash_extensions-1.0.0rc3/dash_extensions/package-info.json
+-rw-r--r--   0        0        0     3468 2023-04-21 08:59:04.250798 dash_extensions-1.0.0rc3/dash_extensions/snippets.py
+-rw-r--r--   0        0        0      960 2023-05-11 12:18:10.104124 dash_extensions-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     2747 1970-01-01 00:00:00.000000 dash_extensions-1.0.0rc3/setup.py
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 dash_extensions-1.0.0rc3/PKG-INFO
```

### Comparing `dash_extensions-1.0.0rc2/LICENSE` & `dash_extensions-1.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/README.md` & `dash_extensions-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/BeforeAfter.py` & `dash_extensions-1.0.0rc3/dash_extensions/BeforeAfter.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Burger.py` & `dash_extensions-1.0.0rc3/dash_extensions/Burger.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/CircleBreaker.py` & `dash_extensions-1.0.0rc3/dash_extensions/CircleBreaker.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/CycleBreaker.py` & `dash_extensions-1.0.0rc3/dash_extensions/CycleBreaker.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/DeferScript.py` & `dash_extensions-1.0.0rc3/dash_extensions/DeferScript.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Download.py` & `dash_extensions-1.0.0rc3/dash_extensions/Download.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/EventListener.py` & `dash_extensions-1.0.0rc3/dash_extensions/EventListener.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/EventSource.py` & `dash_extensions-1.0.0rc3/dash_extensions/EventSource.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Keyboard.py` & `dash_extensions-1.0.0rc3/dash_extensions/Keyboard.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/ListOperator.py` & `dash_extensions-1.0.0rc3/dash_extensions/ListOperator.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/ListStore.py` & `dash_extensions-1.0.0rc3/dash_extensions/ListStore.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Lottie.py` & `dash_extensions-1.0.0rc3/dash_extensions/Lottie.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Mermaid.py` & `dash_extensions-1.0.0rc3/dash_extensions/Mermaid.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Monitor.py` & `dash_extensions-1.0.0rc3/dash_extensions/Monitor.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/PropOperator.py` & `dash_extensions-1.0.0rc3/dash_extensions/PropOperator.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Purify.py` & `dash_extensions-1.0.0rc3/dash_extensions/Purify.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/Ticker.py` & `dash_extensions-1.0.0rc3/dash_extensions/Ticker.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/WebSocket.py` & `dash_extensions-1.0.0rc3/dash_extensions/WebSocket.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/__init__.py` & `dash_extensions-1.0.0rc3/dash_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/_imports_.py` & `dash_extensions-1.0.0rc3/dash_extensions/_imports_.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-burger.js` & `dash_extensions-1.0.0rc3/dash_extensions/async-burger.js`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-burger.js.map` & `dash_extensions-1.0.0rc3/dash_extensions/async-burger.js.map`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-lottie.js` & `dash_extensions-1.0.0rc3/dash_extensions/async-lottie.js`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-lottie.js.map` & `dash_extensions-1.0.0rc3/dash_extensions/async-lottie.js.map`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-mermaid.js` & `dash_extensions-1.0.0rc3/dash_extensions/async-mermaid.js`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/async-mermaid.js.map` & `dash_extensions-1.0.0rc3/dash_extensions/async-mermaid.js.map`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/dash_extensions.min.js` & `dash_extensions-1.0.0rc3/dash_extensions/dash_extensions.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3389,15 +3389,15 @@
         var c = jsonpScriptSrc;
         jsonpScriptSrc = function(t) {
             var e, r = (e = a(), /\/_dash-component-suites\//.test(e.src)),
                 n = c(t);
             if (!r) return n;
             var o = n.split("/"),
                 i = o.slice(-1)[0].split(".");
-            return i.splice(1, 0, "v1_0_0rc1m1683216244"), o.splice(-1, 1, i.join(".")), o.join("/")
+            return i.splice(1, 0, "v1_0_0rc3m1683807503"), o.splice(-1, 1, i.join(".")), o.join("/")
         }
     }(() => {
         var t = {
             179: 0
         };
         o.f.j = (e, r) => {
             var n = o.o(t, e) ? t[e] : void 0;
```

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/dash_extensions.min.js.map` & `dash_extensions-1.0.0rc3/dash_extensions/dash_extensions.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979879275653923%*

 * *Differences: {"'sourcesContent'": "{insert: [(58, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc […]*

```diff
@@ -1486,15 +1486,15 @@
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + {\"34\":\"async-mermaid\",\"597\":\"async-lottie\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.nmd = (module) => {\n\tmodule.paths = [];\n\tif (!module.children) module.children = [];\n\treturn module;\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v1_0_0rc1m1683216244\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v1_0_0rc3m1683807503\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t179: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t} else installedChunks[chunkId] = 0;\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_extensions\"] = self[\"webpackChunkdash_extensions\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "import React from 'react';\nimport { bool, func, node, number, object, oneOfType, string } from 'prop-types';\n\nvar debounce = function debounce(fn, time) {\n  var timeout = void 0;\n\n  return function () {\n    var _this = this,\n        _arguments = arguments;\n\n    var functionCall = function functionCall() {\n      return fn.apply(_this, _arguments);\n    };\n\n    clearTimeout(timeout);\n    timeout = setTimeout(functionCall, time);\n  };\n};\n\n// https://stackoverflow.com/questions/6860853/generate-random-string-for-div-id#6860916\n\nvar guidGenerator = (function () {\n  var S4 = function S4() {\n    return ((1 + Math.random()) * 0x10000 | 0).toString(16).substring(1);\n  };\n  return S4() + S4() + '-' + S4() + '-' + S4() + '-' + S4() + '-' + S4() + S4() + S4();\n});\n\nfunction getHighest(elements) {\n  var highest = 0;\n  elements.forEach(function (el) {\n    if (el.rect && el.rect.height > highest) {\n      highest = el.rect.height;\n    }\n  });\n  return highest;\n}\n\nfunction nextTriggerOnMount(_ref) {\n  var rect = _ref.rect,\n      mode = _ref.mode,\n      prevOffset = _ref.prevOffset,\n      position = _ref.position,\n      direction = _ref.direction,\n      width = _ref.width;\n\n  if (mode !== 'chain') return false;\n  switch (direction) {\n    case 'toRight':\n      return position.from > 0;\n    case 'toLeft':\n    default:\n      return rect.width + position.from <= width;\n  }\n}\n\nfunction getFromOffset(_ref) {\n  var rect = _ref.rect,\n      offset = _ref.offset,\n      direction = _ref.direction;\n\n  switch (direction) {\n    case 'toRight':\n      return offset - rect.width;\n    case 'toLeft':\n    default:\n      return offset;\n  }\n}\n\nfunction getFrom(_ref2) {\n  var index = _ref2.index,\n      rect = _ref2.rect,\n      offset = _ref2.offset,\n      width = _ref2.width,\n      direction = _ref2.direction;\n\n  if (index === 0) return offset;\n\n  if (typeof offset === 'number') {\n    return getFromOffset({ rect: rect, offset: offset, direction: direction });\n  }\n\n  switch (direction) {\n    case 'toRight':\n      return -rect.width;\n    case 'toLeft':\n    default:\n      return width;\n  }\n}\n\nfunction getTo(_ref3) {\n  var rect = _ref3.rect,\n      width = _ref3.width,\n      direction = _ref3.direction;\n\n  switch (direction) {\n    case 'toRight':\n      return width;\n    case 'toLeft':\n    default:\n      return -rect.width;\n  }\n}\n\nfunction getNext(_ref4) {\n  var mode = _ref4.mode,\n      from = _ref4.from,\n      direction = _ref4.direction,\n      rect = _ref4.rect,\n      width = _ref4.width;\n\n  var start = from || 0;\n\n  switch (mode) {\n    case 'await':\n      switch (direction) {\n        case 'toRight':\n          return width;\n        case 'toLeft':\n        default:\n          return -rect.width;\n      }\n    case 'smooth':\n      switch (direction) {\n        case 'toRight':\n          return rect.width > width ? 0 : width - rect.width;\n        case 'toLeft':\n        default:\n          return rect.width > width ? width - rect.width : 0;\n      }\n    case 'chain':\n    default:\n      switch (direction) {\n        case 'toRight':\n          return 0;\n        case 'toLeft':\n        default:\n          return rect.width + start > width ? width - rect.width : width - rect.left - rect.width;\n      }\n  }\n}\n\nvar getPosition = (function (_ref5) {\n  var mode = _ref5.mode,\n      index = _ref5.index,\n      rect = _ref5.rect,\n      offset = _ref5.offset,\n      width = _ref5.width,\n      direction = _ref5.direction;\n\n  var from = getFrom({ index: index, rect: rect, offset: offset, width: width, direction: direction });\n  var to = getTo({ rect: rect, width: width, direction: direction });\n  return {\n    from: from,\n    to: to,\n    next: getNext({ mode: mode, from: from, direction: direction, rect: rect, width: width })\n  };\n});\n\nfunction getNextOffset(_ref) {\n  var from = _ref.from,\n      rect = _ref.rect,\n      direction = _ref.direction;\n\n  switch (direction) {\n    case 'toRight':\n      {\n        return from;\n      }\n    case 'toLeft':\n    default:\n      {\n        return from + rect.width;\n      }\n  }\n}\n\nfunction getStartOffset(_ref) {\n  var offset = _ref.offset,\n      rect = _ref.rect,\n      direction = _ref.direction,\n      width = _ref.width;\n\n  if (offset === 'run-in') {\n    switch (direction) {\n      case 'toRight':\n        return -rect.width;\n      case 'toLeft':\n      default:\n        return width;\n    }\n  }\n  if (typeof offset === 'string') {\n    var offsetRelative = Number(offset.replace('%', ''));\n    if (offsetRelative) return width / 100 * offsetRelative;\n  }\n  return offset;\n}\n\nvar classCallCheck = function (instance, Constructor) {\n  if (!(instance instanceof Constructor)) {\n    throw new TypeError(\"Cannot call a class as a function\");\n  }\n};\n\nvar createClass = function () {\n  function defineProperties(target, props) {\n    for (var i = 0; i < props.length; i++) {\n      var descriptor = props[i];\n      descriptor.enumerable = descriptor.enumerable || false;\n      descriptor.configurable = true;\n      if (\"value\" in descriptor) descriptor.writable = true;\n      Object.defineProperty(target, descriptor.key, descriptor);\n    }\n  }\n\n  return function (Constructor, protoProps, staticProps) {\n    if (protoProps) defineProperties(Constructor.prototype, protoProps);\n    if (staticProps) defineProperties(Constructor, staticProps);\n    return Constructor;\n  };\n}();\n\nvar _extends = Object.assign || function (target) {\n  for (var i = 1; i < arguments.length; i++) {\n    var source = arguments[i];\n\n    for (var key in source) {\n      if (Object.prototype.hasOwnProperty.call(source, key)) {\n        target[key] = source[key];\n      }\n    }\n  }\n\n  return target;\n};\n\nvar inherits = function (subClass, superClass) {\n  if (typeof superClass !== \"function\" && superClass !== null) {\n    throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass);\n  }\n\n  subClass.prototype = Object.create(superClass && superClass.prototype, {\n    constructor: {\n      value: subClass,\n      enumerable: false,\n      writable: true,\n      configurable: true\n    }\n  });\n  if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass;\n};\n\nvar possibleConstructorReturn = function (self, call) {\n  if (!self) {\n    throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\");\n  }\n\n  return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self;\n};\n\nvar toConsumableArray = function (arr) {\n  if (Array.isArray(arr)) {\n    for (var i = 0, arr2 = Array(arr.length); i < arr.length; i++) arr2[i] = arr[i];\n\n    return arr2;\n  } else {\n    return Array.from(arr);\n  }\n};\n\nvar TickerElement = function (_React$Component) {\n  inherits(TickerElement, _React$Component);\n\n  function TickerElement() {\n    var _ref;\n\n    var _temp, _this, _ret;\n\n    classCallCheck(this, TickerElement);\n\n    for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {\n      args[_key] = arguments[_key];\n    }\n\n    return _ret = (_temp = (_this = possibleConstructorReturn(this, (_ref = TickerElement.__proto__ || Object.getPrototypeOf(TickerElement)).call.apply(_ref, [this].concat(args))), _this), _this.state = {\n      children: _this.props.children({\n        index: _this.props.index\n      }),\n      move: _this.props.move,\n      position: { from: undefined, to: undefined, next: undefined },\n      offset: _this.props.offset,\n      rect: null\n    }, _this.x = 0, _this.isMoving = false, _this.nextTriggered = false, _this.elementRef = React.createRef(), _this.raf = null, _this.componentDidMount = function () {\n      _this.setPosition(true);\n      _this.observer = new MutationObserver(_this.onMutation);\n      _this.observer.observe(_this.elementRef.current, { characterData: true, childList: true, subtree: true });\n    }, _this.componentWillUnmount = function () {\n      _this.observer.disconnect();\n    }, _this.onMutation = function () {\n      _this.setPosition();\n    }, _this.componentDidUpdate = function (prevProps, prevState) {\n      if (!_this.x && prevState.position.from !== _this.state.position.from) {\n        _this.x = _this.state.position.from;\n        _this.elementRef.current.style.transform = 'translate3d(' + _this.x + 'px, 0, 0)';\n      }\n      if (_this.x !== _this.state.position.from && prevProps.prevRect && _this.props.prevRect && prevProps.prevRect.width !== _this.props.prevRect.width) {\n        if (_this.props.offset) {\n          _this.x = _this.x + (_this.props.offset - prevProps.offset);\n        } else {\n          _this.x = _this.x + (_this.props.prevRect.width - prevProps.prevRect.width);\n        }\n        _this.elementRef.current.style.transform = 'translate3d(' + _this.x + 'px, 0, 0)';\n      }\n      if (_this.props.move && !prevProps.start && _this.props.start) {\n        _this.animate();\n      }\n      if (_this.props.start && !prevProps.move && _this.props.move) {\n        _this.animate();\n      }\n      if (prevProps.move && !_this.props.move) {\n        _this.isMoving = false;\n        window.cancelAnimationFrame(_this.raf);\n      }\n    }, _this.setPosition = function (isMount) {\n      var _this$props = _this.props,\n          mode = _this$props.mode,\n          width = _this$props.width,\n          id = _this$props.id,\n          onNext = _this$props.onNext,\n          direction = _this$props.direction,\n          index = _this$props.index,\n          setRect = _this$props.setRect;\n\n\n      var rect = _this.elementRef.current.getBoundingClientRect();\n      if (rect.width === 0) return;\n\n      var offset = _this.props.index === 0 ? getStartOffset({ offset: _this.props.offset, rect: rect, direction: direction, width: width }) : _this.props.offset;\n\n      var position = getPosition({ mode: mode, rect: rect, index: index, offset: offset, width: width, direction: direction });\n\n      setRect({\n        index: _this.props.index,\n        rect: rect,\n        offset: offset,\n        nextOffset: getNextOffset({ from: position.from, rect: rect, direction: direction })\n      });\n\n      if (isMount) {\n        var nextTriggerOnMount$$1 = nextTriggerOnMount({ mode: mode, rect: rect, position: position, offset: offset, direction: direction, width: width });\n        if (nextTriggerOnMount$$1) {\n          onNext({\n            id: id,\n            index: index,\n            rect: rect,\n            nextOffset: getNextOffset({ from: position.from, rect: rect, direction: direction })\n          });\n        }\n        if (!nextTriggerOnMount$$1 && (offset || index === 0)) {\n          onNext({ id: id, index: index, rect: rect });\n        }\n        _this.nextTriggered = nextTriggerOnMount$$1;\n      }\n\n      _this.setState({\n        rect: rect,\n        offset: offset,\n        position: position\n      });\n    }, _this.shouldTriggerNext = function () {\n      if (_this.nextTriggered) return false;\n      return _this.props.direction === 'toLeft' ? _this.x <= _this.state.position.next : _this.x >= _this.state.position.next;\n    }, _this.triggerNext = function () {\n      if (_this.shouldTriggerNext()) {\n        // if (this.props.index === 5) console.log(this.x)\n        _this.nextTriggered = true;\n        _this.props.onNext({\n          id: _this.props.id,\n          index: _this.props.index,\n          rect: _this.state.rect\n        });\n      }\n    }, _this.shouldFinish = function () {\n      switch (_this.props.direction) {\n        case 'toRight':\n          return _this.x >= _this.state.position.to;\n        case 'toLeft':\n        default:\n          return _this.x <= _this.state.position.to;\n      }\n    }, _this.animate = function () {\n      if (_this.isMoving) return;\n      _this.isMoving = true;\n\n      var prevTimestamp = null;\n\n      var step = function step(timestamp) {\n        if (!_this.isMoving) return;\n        if (!_this.elementRef.current) return;\n\n        var progress = prevTimestamp ? timestamp - prevTimestamp : 0;\n\n        _this.x = _this.props.direction === 'toLeft' ? _this.x - progress / 100 * _this.props.speed : _this.x + progress / 100 * _this.props.speed;\n        _this.elementRef.current.style.transform = 'translate3d(' + _this.x + 'px, 0, 0)';\n        _this.triggerNext();\n\n        if (_this.shouldFinish()) {\n          _this.isMoving = false;\n          prevTimestamp = null;\n          _this.props.onFinish(_this.props.id);\n        } else {\n          prevTimestamp = timestamp;\n          _this.raf = window.requestAnimationFrame(step);\n        }\n      };\n      _this.raf = window.requestAnimationFrame(step);\n    }, _this.render = function () {\n      return React.createElement(\n        'div',\n        {\n          className: 'ticker__element',\n          style: {\n            willChange: 'transform',\n            position: 'absolute',\n            left: 0,\n            top: 0,\n            transform: 'translate3d(' + _this.x + 'px, 0, 0)'\n          },\n          ref: _this.elementRef\n        },\n        _this.state.children\n      );\n    }, _temp), possibleConstructorReturn(_this, _ret);\n  }\n\n  return TickerElement;\n}(React.Component);\n\nTickerElement.propTypes = {\n  children: oneOfType([node, func]).isRequired,\n  direction: string.isRequired,\n  speed: number.isRequired,\n  id: string.isRequired,\n  index: number.isRequired,\n  mode: string.isRequired,\n  move: bool.isRequired,\n  onNext: func.isRequired,\n  onFinish: func.isRequired,\n  setRect: func.isRequired,\n  start: bool.isRequired,\n\n  offset: oneOfType([number, string]),\n  prevRect: object,\n  width: number\n};\nTickerElement.defaultProps = {\n  offset: undefined,\n  width: undefined,\n  prevRect: null\n};\n\nvar getDefaultState = function getDefaultState(offset, width) {\n  return {\n    elements: [{\n      id: guidGenerator(),\n      index: 0,\n      height: 0,\n      start: false,\n      offset: offset,\n      rect: null,\n      prevRect: null\n    }],\n    width: width,\n    height: 0\n  };\n};\n\nvar Ticker = function (_React$Component) {\n  inherits(Ticker, _React$Component);\n\n  function Ticker() {\n    var _ref;\n\n    var _temp, _this, _ret;\n\n    classCallCheck(this, Ticker);\n\n    for (var _len = arguments.length, args = Array(_len), _key = 0; _key < _len; _key++) {\n      args[_key] = arguments[_key];\n    }\n\n    return _ret = (_temp = (_this = possibleConstructorReturn(this, (_ref = Ticker.__proto__ || Object.getPrototypeOf(Ticker)).call.apply(_ref, [this].concat(args))), _this), _this.next = null, _this.state = getDefaultState(_this.props.offset), _this.tickerRef = React.createRef(), _this.dOnResize = debounce(function () {\n      return _this.onResize();\n    }, 150), _this.componentDidMount = function () {\n      _this.setState({\n        width: _this.tickerRef.current.offsetWidth,\n        height: _this.props.height\n      });\n      window.addEventListener('resize', _this.dOnResize);\n    }, _this.componentWillUnmount = function () {\n      window.removeEventListener('resize', _this.dOnResize);\n    }, _this.setRect = function (_ref2) {\n      var index = _ref2.index,\n          rect = _ref2.rect,\n          offset = _ref2.offset,\n          nextOffset = _ref2.nextOffset;\n\n      _this.setState(function (prevState) {\n        var elements = prevState.elements.map(function (el) {\n          var newEl = el;\n          if (el.index === index) newEl.rect = rect;\n          // next element\n          if (el.index === index + 1) {\n            newEl.prevRect = rect;\n            if (newEl.offset) {\n              newEl.offset = nextOffset;\n            }\n          }\n          return newEl;\n        });\n        return {\n          elements: elements,\n          height: _this.props.height ? prevState.height : getHighest(elements)\n        };\n      });\n    }, _this.onResize = function () {\n      if (!_this.tickerRef.current || _this.tickerRef.current.offsetWidth === _this.state.width) return;\n      _this.setState(_extends({}, getDefaultState(_this.props.offset, _this.tickerRef.current.offsetWidth), {\n        height: _this.props.height\n      }));\n    }, _this.onFinish = function (id) {\n      _this.props.onFinish();\n      _this.setState(function (prevState) {\n        return {\n          elements: prevState.elements.filter(function (el) {\n            return el.id !== id;\n          })\n        };\n      });\n    }, _this.onNext = function (_ref3) {\n      var id = _ref3.id,\n          index = _ref3.index,\n          rect = _ref3.rect,\n          nextOffset = _ref3.nextOffset;\n\n      _this.props.onNext(index);\n\n      _this.setState(function (prevState) {\n        return {\n          elements: [].concat(toConsumableArray(prevState.elements.map(function (el) {\n            var newEl = el;\n            if (el.index === index) newEl.rect = rect;\n            if (el.index === 0 || el.offset || newEl.index === index + 1) {\n              newEl.start = true;\n            }\n            return newEl;\n            // create new element\n          })), [{\n            id: guidGenerator(),\n            index: prevState.elements[prevState.elements.length - 1].index + 1,\n            height: 0,\n            start: false,\n            offset: nextOffset,\n            rect: null,\n            prevRect: rect\n          }])\n        };\n      });\n    }, _temp), possibleConstructorReturn(_this, _ret);\n  }\n\n  createClass(Ticker, [{\n    key: 'render',\n    value: function render() {\n      var _this2 = this;\n\n      return React.createElement(\n        'div',\n        {\n          className: 'ticker',\n          ref: this.tickerRef,\n          style: {\n            position: 'relative',\n            overflow: 'hidden',\n            height: this.state.height && this.state.height + 'px'\n          }\n        },\n        this.state.width && this.state.elements.map(function (el) {\n          return React.createElement(\n            TickerElement,\n            {\n              key: el.id,\n              id: el.id,\n              index: el.index,\n              start: el.start,\n              offset: el.offset,\n              prevRect: el.prevRect,\n\n              direction: _this2.props.direction,\n              mode: _this2.props.mode,\n              move: _this2.props.move,\n              speed: _this2.props.speed,\n\n              onFinish: _this2.onFinish,\n              onNext: _this2.onNext,\n              setRect: _this2.setRect,\n              width: _this2.state.width\n            },\n            _this2.props.children\n          );\n        })\n      );\n    }\n  }]);\n  return Ticker;\n}(React.Component);\n\nTicker.propTypes = {\n  children: oneOfType([node, func]).isRequired,\n\n  direction: string,\n  mode: string,\n  move: bool,\n  offset: oneOfType([number, string]),\n  speed: number,\n  height: oneOfType([number, string]),\n  onNext: func,\n  onFinish: func\n};\nTicker.defaultProps = {\n  offset: 0,\n  speed: 5,\n  direction: 'toLeft',\n  mode: 'chain',\n  move: true,\n  height: undefined,\n  onNext: function onNext() {},\n  onFinish: function onFinish() {}\n};\n\nexport default Ticker;\n//# sourceMappingURL=index.es.js.map\n",
         "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\nimport ReactTicker from 'react-ticker';\n\n/**\n * A light wrapper of ReactTicker.\n */\nexport default class Ticker extends Component {\n\n    render() {\n        return (\n            <ReactTicker {...this.props}>\n                {({index}) => (\n                    <>\n                        {this.props.children}\n                    </>\n                )}\n            </ReactTicker>\n        );\n    }\n\n}\n\nTicker.propTypes = {\n\n    direction: PropTypes.oneOf([\"toRight\", \"toLeft\"]),\n\n    mode: PropTypes.oneOf([\"chain\", \"await\", \"smooth\"]),\n\n    move: PropTypes.bool,\n\n    offset: PropTypes.oneOfType([PropTypes.number, PropTypes.string]),\n\n    speed: PropTypes.number,\n\n    height: PropTypes.oneOfType([PropTypes.number, PropTypes.string]),\n\n    // Dash props.\n\n    /**\n     * The ID used to identify this component in Dash callbacks\n     */\n    id: PropTypes.string,\n\n    /**\n     * The children of this component\n     */\n    children: PropTypes.node,\n\n    /**\n     * The class of the component\n     */\n    className: PropTypes.string,\n\n};",
         "import {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * A simple interface to\n */\nexport default class DashWebSocket extends Component {\n\n    _init_client() {\n        // Create a new client.\n        let {url} = this.props;\n        const {protocols} = this.props;\n        url = url? url : \"ws://\" + location.host + location.pathname + \"ws\";\n        this.client = new WebSocket(url, protocols);\n        // Listen for events.\n        this.client.onopen = (e) => {\n            // TODO: Add more properties here?\n            this.props.setProps({\n                state: {\n                    // Mandatory props.\n                    readyState: WebSocket.OPEN,\n                    isTrusted: e.isTrusted,\n                    timeStamp: e.timeStamp,\n                    // Extra props.\n                    origin: e.origin,\n                }\n            })\n        }\n        this.client.onmessage = (e) => {\n            // TODO: Add more properties here?\n            this.props.setProps({\n                message: {\n                    data: e.data,\n                    isTrusted: e.isTrusted,\n                    origin: e.origin,\n                    timeStamp: e.timeStamp\n                }\n            })\n        }\n        this.client.onerror = (e) => {\n            // TODO: Implement error handling.\n            this.props.setProps({error: JSON.stringify(e)})\n        }\n        this.client.onclose = (e) => {\n            // TODO: Add more properties here?\n            this.props.setProps({\n                state: {\n                    // Mandatory props.\n                    readyState: WebSocket.CLOSED,\n                    isTrusted: e.isTrusted,\n                    timeStamp: e.timeStamp,\n                    // Extra props.\n                    code: e.code,\n                    reason: e.reason,\n                    wasClean: e.wasClean,\n                }\n            })\n        }\n    }\n\n    componentDidMount() {\n        this._init_client()\n    }\n\n    componentDidUpdate(prevProps) {\n        const {send} = this.props;\n        // Send messages.\n        if (send && send !== prevProps.send) {\n            if (this.props.state.readyState === WebSocket.OPEN) {\n                this.client.send(send)\n            }\n        }\n        // TODO: Maybe add support for changing the url?\n    }\n\n    componentWillUnmount() {\n        // Clean up (close the connection).\n        this.client.onopen = null;\n        this.client.onclose = null;\n        this.client.onerror = null;\n        this.client.onmessage = null;\n        this.client.close();\n    }\n\n    render() {\n        return (null);\n    }\n\n}\n\nDashWebSocket.defaultProps = {\n    state: {readyState: WebSocket.CONNECTING}\n}\n\nDashWebSocket.propTypes = {\n\n    /**\n     * This websocket state (in the readyState prop) and associated information.\n     */\n    state: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\n\n    /**\n     * When messages are received, this property is updated with the message content.\n     */\n    message: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\n\n    /**\n     * This property is set with the content of the onerror event.\n     */\n    error: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\n\n    /**\n     * When this property is set, a message is sent with its content.\n     */\n    send: PropTypes.oneOfType([PropTypes.object, PropTypes.string]),\n\n    /**\n     * The websocket endpoint (e.g. wss://echo.websocket.org).\n     */\n    url: PropTypes.string,\n\n    /**\n     * Supported websocket protocols (optional).\n     */\n    protocols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n\n}",
         "import React from 'react';\nimport PropTypes from 'prop-types';\nimport {ImgComparisonSlider} from '@img-comparison-slider/react';\n\n/**\n * Before After Image Slider based on https://github.com/sneas/img-comparison-slider\n */\nconst BeforeAfter = props => {\n    const {\n        id,\n        before,\n        after,\n        width,\n        height,\n        hover,\n        value,\n        direction,\n        keyboard,\n    } = props;\n\n    return (\n        <div id={id}>\n            <ImgComparisonSlider\n                hover={hover}\n                value={value}\n                direction={direction}\n                keyboard={keyboard}\n            >\n                <img\n                    slot=\"first\"\n                    width={width}\n                    height={height}\n                    {...before}\n                />\n                <img\n                    slot=\"second\"\n                    width={width}\n                    height={height}\n                    {...after}\n                />\n            </ImgComparisonSlider>\n        </div>\n    );\n};\n\n\nBeforeAfter.defaultProps = {\n    width: '100%',\n    height: 'auto',\n    hover: true,\n    value: 50,\n    direction: 'horizontal',\n    keyboard: 'enabled',\n};\n\nBeforeAfter.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks\n     */\n    id: PropTypes.string,\n\n    /**\n     *  Image height - default \"auto\" for responsive images\n     */\n    height: PropTypes.string,\n\n    /**\n     * Image width - default \"100%\" for responsive images\n     */\n    width: PropTypes.string,\n\n    /**\n     * Automatic slide on mouse over\n     */\n    hover: PropTypes.bool,\n\n    /**\n     * The divider position can be specified as a percentage, i.e. 0 to 100\n     */\n    value: PropTypes.number,\n\n    /**\n     * Set slider direction\n     */\n    direction: PropTypes.oneOf(['horizontal', 'vertical']),\n\n    /**\n     * Enable/disable slider position control with the keyboard\n     */\n    keyboard: PropTypes.oneOf(['enabled', 'disabled']),\n\n    /**\n     * Props for the `before` Img component. eg {\"src\": \"/assets/lena_bw.png\"}\n     */\n    before: PropTypes.object,\n\n    /**\n     *  Props for the `after` Img component. eg {\"src\": \"/assets/lena_color.png\"}\n     */\n    after: PropTypes.object,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func,\n};\n\nexport default BeforeAfter;\n",
         "import React from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Used to delay import of js resources until after React had been loaded. Typically used to apply js to dynamic\n * content. Based on https://github.com/Grasia/grasia-dash-components/blob/master/src/components/Import.react.js\n */\nexport default class DeferScript extends React.Component {\n\n  componentDidMount () {\n    if (this.props.src) {\n      const {src} = this.props;\n      const script = document.createElement('script');\n\n      script.src = src;\n      script.defer = true;\n\n      document.body.appendChild(script);\n      }\n    }\n\n  render() {\n    return null;\n  }\n}\n\nDeferScript.propTypes = {\n\n  /**\n  * The ID used to identify this component in Dash callbacks\n  */\n  id: PropTypes.string,\n\n  /**\n  * Local or external source of the javascript to import\n  */\n  src: PropTypes.string\n\n};",
         "import DOMPurify from \"dompurify\";\nimport React from \"react\";\nimport PropTypes from \"prop-types\";\n\n/**\n * The Html component makes it possible to render html sanitized via DOMPurify.\n */\nconst Purify = ({html, config, className}) => {\n    const html_safe = DOMPurify.sanitize(html, config);\n    return <div className={className} dangerouslySetInnerHTML={{__html: html_safe}}/>;\n}\n\nPurify.propTypes = {\n\n    /**\n     * Html string\n     */\n    html: PropTypes.string,\n\n    /**\n     * Configuration (optional) of DOMPurify, see the docs https://github.com/cure53/DOMPurify\n     */\n    config: PropTypes.object,\n\n\n    // Dash props.\n\n    /**\n     * The ID used to identify this component in Dash callbacks\n     */\n    id: PropTypes.string,\n\n    /**\n     * The class of the component\n     */\n    className: PropTypes.string,\n\n};\n\n\nexport default Purify\n",
```

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/dataiku.py` & `dash_extensions-1.0.0rc3/dash_extensions/dataiku.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/enrich.py` & `dash_extensions-1.0.0rc3/dash_extensions/enrich.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/javascript.py` & `dash_extensions-1.0.0rc3/dash_extensions/javascript.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/metadata.json` & `dash_extensions-1.0.0rc3/dash_extensions/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/package-info.json` & `dash_extensions-1.0.0rc3/dash_extensions/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'1.0.0rc3'"}*

```diff
@@ -58,9 +58,9 @@
         "build:py_and_r": "dash-generate-components ./src/lib/components dash_extensions -p package-info.json --r-prefix ''",
         "build:py_and_r-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build_no_r": "npm run build:js && npm run build:py",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "1.0.0rc1"
+    "version": "1.0.0rc3"
 }
```

### Comparing `dash_extensions-1.0.0rc2/dash_extensions/snippets.py` & `dash_extensions-1.0.0rc3/dash_extensions/snippets.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.0rc2/pyproject.toml` & `dash_extensions-1.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dash-extensions"
-version = "1.0.0rc2"
+version = "1.0.0rc3"
 description = "Extensions for Plotly Dash."
 authors = ["emher <emil.h.eriksen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://dash-extensions.com"
 repository = "https://github.com/thedirtyfew/dash-extensions"
```

### Comparing `dash_extensions-1.0.0rc2/setup.py` & `dash_extensions-1.0.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'more-itertools>=9.0.0,<10.0.0']
 
 extras_require = \
 {'mantine': ['dash-mantine-components>=0.11.1,<0.12.0']}
 
 setup_kwargs = {
     'name': 'dash-extensions',
-    'version': '1.0.0rc2',
+    'version': '1.0.0rc3',
     'description': 'Extensions for Plotly Dash.',
     'long_description': '[![PyPI Latest Release](https://img.shields.io/pypi/v/dash-extensions.svg)](https://pypi.org/project/dash-extensions/)\n[![codecov](https://img.shields.io/codecov/c/github/thedirtyfew/dash-extensions?logo=codecov)](https://codecov.io/gh/thedirtyfew/dash-extensions)\n[![Testing](https://github.com/thedirtyfew/dash-extensions/actions/workflows/python-test.yml/badge.svg)](https://github.com/thedirtyfew/dash-extensions/actions/workflows/python-test.yml)\n[![CodeQL](https://github.com/thedirtyfew/dash-extensions/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/thedirtyfew/dash-extensions/actions/workflows/codeql-analysis.yml)\n\nThe `dash-extensions` package is a collection of utility functions, syntax extensions, and Dash components that aim to improve the Dash development experience. It can be divided in four main pillars,\n\n* The `enrich` module, which contains various enriched versions of Dash components\n* A number of custom components, e.g. the `Websocket` component, which enables real-time communication and push notifications\n* The `javascript` module, which contains functionality to ease the interplay between Dash and JavaScript\n* The `snippets` module, which contains a collection of utility functions (documentation limited to source code comments)\n\nThe `enrich` module enables a number of _transforms_ that add functionality and/or syntactic sugar to Dash. Examples include\n\n* Making it possible to avoid invoking a callback _if it is already running_ via the `BlockingCallbackTransform`\n* Enabling logging from within Dash callbacks via the `LogTransform`\n* Improving app performance via the `ServersideOutputTransform`\n\nto name a few. To enable interactivity, the documentation has been moved to a [separate page](http://dash-extensions.com).\n\nNB: The 1.0.0 version introduces a number of breaking changes, see documentation for details.\n',
     'author': 'emher',
     'author_email': 'emil.h.eriksen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dash-extensions.com',
```

### Comparing `dash_extensions-1.0.0rc2/PKG-INFO` & `dash_extensions-1.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-extensions
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Extensions for Plotly Dash.
 Home-page: https://dash-extensions.com
 License: MIT
 Author: emher
 Author-email: emil.h.eriksen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
```

