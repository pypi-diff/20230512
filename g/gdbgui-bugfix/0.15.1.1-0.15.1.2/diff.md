# Comparing `tmp/gdbgui-bugfix-0.15.1.1.tar.gz` & `tmp/gdbgui-bugfix-0.15.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdbgui-bugfix-0.15.1.1.tar", last modified: Mon Jan 30 17:26:17 2023, max compression
+gzip compressed data, was "gdbgui-bugfix-0.15.1.2.tar", last modified: Fri May 12 21:47:47 2023, max compression
```

## Comparing `gdbgui-bugfix-0.15.1.1.tar` & `gdbgui-bugfix-0.15.1.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.133605 gdbgui-bugfix-0.15.1.1/
--rw-rw-r--   0 greg      (1000) greg      (1000)    35184 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/LICENSE
--rw-rw-r--   0 greg      (1000) greg      (1000)      864 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/MANIFEST.in
--rw-rw-r--   0 greg      (1000) greg      (1000)     1650 2023-01-30 17:26:17.133605 gdbgui-bugfix-0.15.1.1/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)      656 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/README.md
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.041606 gdbgui-bugfix-0.15.1.1/gdbgui/
--rw-rw-r--   0 greg      (1000) greg      (1000)     3253 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/SSLify.py
--rw-rw-r--   0 greg      (1000) greg      (1000)        9 2023-01-30 17:24:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/VERSION.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      339 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/__init__.py
--rw-rw-r--   0 greg      (1000) greg      (1000)       30 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/__main__.py
--rwxrwxr-x   0 greg      (1000) greg      (1000)     9205 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/cli.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     1363 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/htmllistformatter.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      158 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/py.typed
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.041606 gdbgui-bugfix-0.15.1.1/gdbgui/server/
--rw-rw-r--   0 greg      (1000) greg      (1000)        0 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/__init__.py
--rw-rw-r--   0 greg      (1000) greg      (1000)    11141 2023-01-24 17:03:02.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/app.py
--rw-rw-r--   0 greg      (1000) greg      (1000)      913 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/constants.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     7464 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/http_routes.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     2519 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/http_util.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     2689 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/ptylib.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     3203 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/server.py
--rw-rw-r--   0 greg      (1000) greg      (1000)     6230 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/server/sessionmanager.py
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.041606 gdbgui-bugfix-0.15.1.1/gdbgui/static/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.041606 gdbgui-bugfix-0.15.1.1/gdbgui/static/css/
--rw-rw-r--   0 greg      (1000) greg      (1000)     8638 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/css/gdbgui.css
--rw-rw-r--   0 greg      (1000) greg      (1000)     1083 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/css/splitjs-gdbgui.css
--rw-rw-r--   0 greg      (1000) greg      (1000)      258 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/css/tailwind.css
--rw-rw-r--   0 greg      (1000) greg      (1000)    13950 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/favicon.ico
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.041606 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/
--rw-rw-r--   0 greg      (1000) greg      (1000)    14680 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/github.jpg
--rw-rw-r--   0 greg      (1000) greg      (1000)     4945 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/paypal.svg
--rw-rw-r--   0 greg      (1000) greg      (1000)      563 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/ploticon.png
--rw-rw-r--   0 greg      (1000) greg      (1000)    19584 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/ploticon_orig.png
--rw-rw-r--   0 greg      (1000) greg      (1000)     3291 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/images/twitter.png
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.093605 gdbgui-bugfix-0.15.1.1/gdbgui/static/js/
--rw-rw-r--   0 greg      (1000) greg      (1000)  3550339 2023-01-24 17:07:09.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/js/dashboard.js
--rw-rw-r--   0 greg      (1000) greg      (1000)  4412025 2023-01-24 17:07:09.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/js/dashboard.js.map
--rw-rw-r--   0 greg      (1000) greg      (1000)  4538000 2023-01-24 17:14:26.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/js/main.js
--rw-rw-r--   0 greg      (1000) greg      (1000)  5522133 2023-01-24 17:14:26.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/js/main.js.map
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.037606 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.121605 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/
--rw-rw-r--   0 greg      (1000) greg      (1000)    23848 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/animate.css
--rw-rw-r--   0 greg      (1000) greg      (1000)   121260 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/bootstrap.min.css
--rw-rw-r--   0 greg      (1000) greg      (1000)     2169 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/gdbgui_awesomeplete.css
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.121605 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/
--rw-rw-r--   0 greg      (1000) greg      (1000)     4059 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/emacs.css
--rw-rw-r--   0 greg      (1000) greg      (1000)     4828 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/light.css
--rw-rw-r--   0 greg      (1000) greg      (1000)     4848 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/monokai.css
--rw-rw-r--   0 greg      (1000) greg      (1000)     4009 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/vim.css
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.121605 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/fonts/
--rw-rw-r--   0 greg      (1000) greg      (1000)    18028 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.037606 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/images/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.037606 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/images/splitjs/
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.121605 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/images/splitjs/grips/
--rw-rw-r--   0 greg      (1000) greg      (1000)      104 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/images/splitjs/grips/horizontal.png
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.129605 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/
--rw-rw-r--   0 greg      (1000) greg      (1000)     5692 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/awesomeplete.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    36868 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/bootstrap.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    36669 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/jquery.flot-0.8.3.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    85578 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/jquery.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    71753 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/lodash.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    61318 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/moment.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)    61212 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/socket.io-2.0.3.min.js
--rw-rw-r--   0 greg      (1000) greg      (1000)   402868 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/socket.io.js.map
--rw-rw-r--   0 greg      (1000) greg      (1000)     5261 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/splitjs.min-1.2.0.js
--rw-rw-r--   0 greg      (1000) greg      (1000)   663624 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/vis-4.20.1.min.js
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.133605 gdbgui-bugfix-0.15.1.1/gdbgui/templates/
--rw-rw-r--   0 greg      (1000) greg      (1000)      730 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/templates/dashboard.html
--rw-rw-r--   0 greg      (1000) greg      (1000)     1755 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/gdbgui/templates/gdbgui.html
-drwxrwxr-x   0 greg      (1000) greg      (1000)        0 2023-01-30 17:26:17.133605 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/
--rw-rw-r--   0 greg      (1000) greg      (1000)     1650 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/PKG-INFO
--rw-rw-r--   0 greg      (1000) greg      (1000)     1976 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/SOURCES.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/dependency_links.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)       43 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/entry_points.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        1 2023-01-30 17:26:16.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/not-zip-safe
--rw-rw-r--   0 greg      (1000) greg      (1000)      311 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/requires.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)        7 2023-01-30 17:26:17.000000 gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/top_level.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)      870 2023-01-24 16:33:28.000000 gdbgui-bugfix-0.15.1.1/requirements.txt
--rw-rw-r--   0 greg      (1000) greg      (1000)       38 2023-01-30 17:26:17.133605 gdbgui-bugfix-0.15.1.1/setup.cfg
--rw-rw-r--   0 greg      (1000) greg      (1000)     2318 2023-01-30 17:23:55.000000 gdbgui-bugfix-0.15.1.1/setup.py
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.985797 gdbgui-bugfix-0.15.1.2/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    35184 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/LICENSE
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      864 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/MANIFEST.in
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1752 2023-05-12 21:47:47.985797 gdbgui-bugfix-0.15.1.2/PKG-INFO
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      656 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/README.md
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.925796 gdbgui-bugfix-0.15.1.2/gdbgui/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     3253 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/SSLify.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)        9 2023-05-12 21:44:51.000000 gdbgui-bugfix-0.15.1.2/gdbgui/VERSION.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      339 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/__init__.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)       30 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/__main__.py
+-rwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)     9205 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/cli.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1363 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/htmllistformatter.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      158 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/py.typed
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.929796 gdbgui-bugfix-0.15.1.2/gdbgui/server/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/__init__.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    11141 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/app.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      913 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/constants.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     7464 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/http_routes.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     2519 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/http_util.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     2689 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/ptylib.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     3203 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/server.py
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     6230 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/server/sessionmanager.py
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.929796 gdbgui-bugfix-0.15.1.2/gdbgui/static/
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.929796 gdbgui-bugfix-0.15.1.2/gdbgui/static/css/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     8638 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/css/gdbgui.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1083 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/css/splitjs-gdbgui.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      258 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/css/tailwind.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    13950 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/favicon.ico
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.929796 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    14680 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/github.jpg
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     4945 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/paypal.svg
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      563 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/ploticon.png
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    19584 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/ploticon_orig.png
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     3291 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/images/twitter.png
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.961797 gdbgui-bugfix-0.15.1.2/gdbgui/static/js/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)  3550339 2023-05-12 21:42:19.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/js/dashboard.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)  4412025 2023-05-12 21:42:19.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/js/dashboard.js.map
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)  4538000 2023-05-12 21:42:19.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/js/main.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)  5522133 2023-05-12 21:42:19.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/js/main.js.map
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.921796 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.977797 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    23848 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/animate.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)   121260 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/bootstrap.min.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     2169 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/gdbgui_awesomeplete.css
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.977797 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     4059 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/emacs.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     4828 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/light.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     4848 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/monokai.css
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     4009 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/vim.css
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.977797 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/fonts/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    18028 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.921796 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/images/
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.921796 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/images/splitjs/
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.977797 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/images/splitjs/grips/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      104 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/images/splitjs/grips/horizontal.png
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.981797 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     5692 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/awesomeplete.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    36868 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/bootstrap.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    36669 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/jquery.flot-0.8.3.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    85578 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/jquery.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    71753 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/lodash.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    61318 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/moment.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)    61212 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/socket.io-2.0.3.min.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)   402868 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/socket.io.js.map
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     5261 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/splitjs.min-1.2.0.js
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)   663624 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/vis-4.20.1.min.js
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.985797 gdbgui-bugfix-0.15.1.2/gdbgui/templates/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      730 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/templates/dashboard.html
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1755 2023-05-12 21:33:13.000000 gdbgui-bugfix-0.15.1.2/gdbgui/templates/gdbgui.html
+drwxrwxr-x   0 ggbaker   (1000) ggbaker   (1000)        0 2023-05-12 21:47:47.985797 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1752 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/PKG-INFO
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     1976 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/SOURCES.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)        1 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/dependency_links.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)       43 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/entry_points.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)        1 2023-05-12 21:47:30.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/not-zip-safe
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      326 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/requires.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)        7 2023-05-12 21:47:47.000000 gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/top_level.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)      936 2023-05-12 21:42:00.000000 gdbgui-bugfix-0.15.1.2/requirements.txt
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)       38 2023-05-12 21:47:47.985797 gdbgui-bugfix-0.15.1.2/setup.cfg
+-rw-rw-r--   0 ggbaker   (1000) ggbaker   (1000)     2418 2023-05-12 21:46:55.000000 gdbgui-bugfix-0.15.1.2/setup.py
```

### Comparing `gdbgui-bugfix-0.15.1.1/LICENSE` & `gdbgui-bugfix-0.15.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/MANIFEST.in` & `gdbgui-bugfix-0.15.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/PKG-INFO` & `gdbgui-bugfix-0.15.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdbgui-bugfix
-Version: 0.15.1.1
+Version: 0.15.1.2
 Summary: Browser-based frontend to gdb. Debug C, C++, Go, or Rust.
 Home-page: https://github.com/cs01/gdbgui
 Author: Chad Smith
 Author-email: chadsmith.software@gmail.com
 License: License :: GNU GPLv3
 Project-URL: Documentation, https://cs01.github.io/gdbgui/
 Project-URL: Source Code, https://github.com/cs01/gdbgui
@@ -14,14 +14,16 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <a href="http://gdbgui.com"><img src="https://github.com/cs01/gdbgui/raw/master/images/gdbgui_banner.png"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: gdbgui-bugfix Version: 0.15.1.1 Summary: Browser-
+Metadata-Version: 2.1 Name: gdbgui-bugfix Version: 0.15.1.2 Summary: Browser-
 based frontend to gdb. Debug C, C++, Go, or Rust. Home-page: https://
 github.com/cs01/gdbgui Author: Chad Smith Author-email:
 chadsmith.software@gmail.com License: License :: GNU GPLv3 Project-URL:
 Documentation, https://cs01.github.io/gdbgui/ Project-URL: Source Code, https:/
 /github.com/cs01/gdbgui Project-URL: Bug Tracker, https://github.com/cs01/
 gdbgui/issues Keywords: gdb,debug,c,c++,go,rust,python,machine-
 interface,parse,frontend,flask,browser,gui Classifier: Intended Audience ::
 Developers Classifier: Operating System :: MacOS Classifier: Operating System
 :: Unix Classifier: Operating System :: POSIX Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
      [https://github.com/cs01/gdbgui/raw/master/images/gdbgui_banner.png]
            **** A browser-based frontend to gdb (gnu debugger) ****
                         [image] [PyPI_version] [image]
 --- **Documentation**: https://gdbgui.com **Source Code**: https://github.com/
 cs01/gdbgui/
```

### Comparing `gdbgui-bugfix-0.15.1.1/README.md` & `gdbgui-bugfix-0.15.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/SSLify.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/SSLify.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/cli.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/cli.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/htmllistformatter.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/htmllistformatter.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/app.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/app.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/constants.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/constants.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/http_routes.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/http_routes.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/http_util.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/http_util.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/ptylib.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/ptylib.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/server.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/server.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/server/sessionmanager.py` & `gdbgui-bugfix-0.15.1.2/gdbgui/server/sessionmanager.py`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/css/gdbgui.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/css/gdbgui.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/css/splitjs-gdbgui.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/css/splitjs-gdbgui.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/favicon.ico` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/images/github.jpg` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/images/github.jpg`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/images/paypal.svg` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/images/paypal.svg`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/images/ploticon.png` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/images/ploticon.png`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/images/ploticon_orig.png` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/images/ploticon_orig.png`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/images/twitter.png` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/images/twitter.png`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/js/dashboard.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/js/dashboard.js.map` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/js/dashboard.js.map`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/js/main.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/js/main.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/js/main.js.map` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/js/main.js.map`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/animate.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/animate.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/bootstrap.min.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/gdbgui_awesomeplete.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/gdbgui_awesomeplete.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/emacs.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/emacs.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/light.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/light.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/monokai.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/monokai.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/css/pygments/vim.css` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/css/pygments/vim.css`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/fonts/glyphicons-halflings-regular.woff2` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/awesomeplete.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/awesomeplete.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/bootstrap.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/jquery.flot-0.8.3.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/jquery.flot-0.8.3.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/jquery.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/lodash.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/lodash.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/moment.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/moment.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/socket.io-2.0.3.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/socket.io-2.0.3.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/socket.io.js.map` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/socket.io.js.map`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/splitjs.min-1.2.0.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/splitjs.min-1.2.0.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/static/vendor/js/vis-4.20.1.min.js` & `gdbgui-bugfix-0.15.1.2/gdbgui/static/vendor/js/vis-4.20.1.min.js`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/templates/dashboard.html` & `gdbgui-bugfix-0.15.1.2/gdbgui/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui/templates/gdbgui.html` & `gdbgui-bugfix-0.15.1.2/gdbgui/templates/gdbgui.html`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/PKG-INFO` & `gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdbgui-bugfix
-Version: 0.15.1.1
+Version: 0.15.1.2
 Summary: Browser-based frontend to gdb. Debug C, C++, Go, or Rust.
 Home-page: https://github.com/cs01/gdbgui
 Author: Chad Smith
 Author-email: chadsmith.software@gmail.com
 License: License :: GNU GPLv3
 Project-URL: Documentation, https://cs01.github.io/gdbgui/
 Project-URL: Source Code, https://github.com/cs01/gdbgui
@@ -14,14 +14,16 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <a href="http://gdbgui.com"><img src="https://github.com/cs01/gdbgui/raw/master/images/gdbgui_banner.png"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: gdbgui-bugfix Version: 0.15.1.1 Summary: Browser-
+Metadata-Version: 2.1 Name: gdbgui-bugfix Version: 0.15.1.2 Summary: Browser-
 based frontend to gdb. Debug C, C++, Go, or Rust. Home-page: https://
 github.com/cs01/gdbgui Author: Chad Smith Author-email:
 chadsmith.software@gmail.com License: License :: GNU GPLv3 Project-URL:
 Documentation, https://cs01.github.io/gdbgui/ Project-URL: Source Code, https:/
 /github.com/cs01/gdbgui Project-URL: Bug Tracker, https://github.com/cs01/
 gdbgui/issues Keywords: gdb,debug,c,c++,go,rust,python,machine-
 interface,parse,frontend,flask,browser,gui Classifier: Intended Audience ::
 Developers Classifier: Operating System :: MacOS Classifier: Operating System
 :: Unix Classifier: Operating System :: POSIX Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
      [https://github.com/cs01/gdbgui/raw/master/images/gdbgui_banner.png]
            **** A browser-based frontend to gdb (gnu debugger) ****
                         [image] [PyPI_version] [image]
 --- **Documentation**: https://gdbgui.com **Source Code**: https://github.com/
 cs01/gdbgui/
```

### Comparing `gdbgui-bugfix-0.15.1.1/gdbgui_bugfix.egg-info/SOURCES.txt` & `gdbgui-bugfix-0.15.1.2/gdbgui_bugfix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdbgui-bugfix-0.15.1.1/requirements.txt` & `gdbgui-bugfix-0.15.1.2/requirements.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 #
-# This file is autogenerated by pip-compile with python 3.10
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
 #
 #    pip-compile requirements.in
 #
-bidict==0.21.2
+bidict==0.22.1
     # via python-socketio
+blinker==1.6.2
+    # via flask
 brotli==1.0.9
     # via flask-compress
-click==8.0.1
+click==8.1.3
     # via flask
-dnspython==2.2.1
+dnspython==2.3.0
     # via eventlet
-eventlet==0.33.0
+eventlet==0.33.3
     # via -r requirements.in
-flask==2.0.1
+flask==2.3.2
     # via
     #   flask-compress
     #   flask-socketio
 flask-compress==1.10.1
     # via -r requirements.in
-flask-socketio==5.1.1
+flask-socketio==5.1.2
     # via -r requirements.in
-greenlet==1.1.2
+greenlet==2.0.2
     # via eventlet
-itsdangerous==2.0.1
+itsdangerous==2.1.2
     # via flask
-jinja2==3.0.1
+jinja2==3.1.2
     # via flask
-markupsafe==2.0.1
-    # via jinja2
-pygdbmi==0.10.0.1
+markupsafe==2.1.2
+    # via
+    #   jinja2
+    #   werkzeug
+pygdbmi==0.10.0.2
     # via -r requirements.in
-pygments==2.10.0
+pygments==2.15.1
     # via -r requirements.in
-python-engineio==4.2.1
+python-engineio==4.4.1
     # via python-socketio
-python-socketio==5.4.0
+python-socketio==5.8.0
     # via flask-socketio
 six==1.16.0
     # via eventlet
-werkzeug==2.0.1
+werkzeug==2.3.4
     # via flask
```

### Comparing `gdbgui-bugfix-0.15.1.1/setup.py` & `gdbgui-bugfix-0.15.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Operating System :: POSIX",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.6",
     project_urls={
         "Documentation": "https://cs01.github.io/gdbgui/",
         "Source Code": "https://github.com/cs01/gdbgui",
         "Bug Tracker": "https://github.com/cs01/gdbgui/issues",
     },
```

