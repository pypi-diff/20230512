# Comparing `tmp/gradiop-0.0.4.tar.gz` & `tmp/gradiop-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gradiop-0.0.4.tar", last modified: Fri May 12 08:37:53 2023, max compression
+gzip compressed data, was "dist\gradiop-0.0.5.tar", last modified: Fri May 12 09:08:21 2023, max compression
```

## Comparing `gradiop-0.0.4.tar` & `gradiop-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/
--rw-rw-rw-   0        0        0       37 2023-05-12 08:27:27.000000 gradiop-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      264 2023-05-12 08:37:53.000000 gradiop-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/
--rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.4/gradiop/__init__.py
--rw-rw-rw-   0        0        0      610 2023-05-12 07:10:44.000000 gradiop-0.0.4/gradiop/plug.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/assets/
--rw-rw-rw-   0        0        0    58332 2023-05-12 08:36:58.000000 gradiop-0.0.4/gradiop/templates/assets/index-7da4454e.js
--rw-rw-rw-   0        0        0   234226 2023-05-12 08:36:58.000000 gradiop-0.0.4/gradiop/templates/assets/index-7da4454e.js.map
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/cdn/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/cdn/ajax/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/cdn/ajax/libs/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/cdn/ajax/libs/iframe-resizer/
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop/templates/cdn/ajax/libs/iframe-resizer/4.3.1/
--rw-rw-rw-   0        0        0    13719 2023-05-12 04:10:04.000000 gradiop-0.0.4/gradiop/templates/cdn/ajax/libs/iframe-resizer/4.3.1/iframeResizer.contentWindow.min.js
--rw-rw-rw-   0        0        0     2025 2023-05-12 08:37:08.000000 gradiop-0.0.4/gradiop/templates/cdn/index.html
--rw-rw-rw-   0        0        0     1176 2023-05-12 08:37:30.000000 gradiop-0.0.4/gradiop/version.py
-drwxrwxrwx   0        0        0        0 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop.egg-info/
--rw-rw-rw-   0        0        0      264 2023-05-12 08:37:52.000000 gradiop-0.0.4/gradiop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-12 08:37:53.000000 gradiop-0.0.4/gradiop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 08:37:52.000000 gradiop-0.0.4/gradiop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-12 08:37:52.000000 gradiop-0.0.4/gradiop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 08:37:52.000000 gradiop-0.0.4/gradiop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 08:37:52.000000 gradiop-0.0.4/gradiop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 08:37:53.000000 gradiop-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-05-12 08:28:20.000000 gradiop-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/
+-rw-rw-rw-   0        0        0       37 2023-05-12 08:27:27.000000 gradiop-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      264 2023-05-12 09:08:21.000000 gradiop-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop/
+-rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.5/gradiop/__init__.py
+-rw-rw-rw-   0        0        0      610 2023-05-12 07:10:44.000000 gradiop-0.0.5/gradiop/plug.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop/templates/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop/templates/cdn/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop/templates/cdn/assets/
+-rw-rw-rw-   0        0        0    13719 2023-05-12 04:10:04.000000 gradiop-0.0.5/gradiop/templates/cdn/assets/iframeResizer.contentWindow.min.js
+-rw-rw-rw-   0        0        0    58332 2023-05-12 08:36:58.000000 gradiop-0.0.5/gradiop/templates/cdn/assets/index-7da4454e.js
+-rw-rw-rw-   0        0        0   234226 2023-05-12 08:36:58.000000 gradiop-0.0.5/gradiop/templates/cdn/assets/index-7da4454e.js.map
+-rw-rw-rw-   0        0        0     2001 2023-05-12 09:07:43.000000 gradiop-0.0.5/gradiop/templates/cdn/index.html
+-rw-rw-rw-   0        0        0     1176 2023-05-12 09:08:08.000000 gradiop-0.0.5/gradiop/version.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 09:08:21.000000 gradiop-0.0.5/gradiop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 09:08:21.000000 gradiop-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-05-12 08:28:20.000000 gradiop-0.0.5/setup.py
```

### Comparing `gradiop-0.0.4/gradiop/plug.py` & `gradiop-0.0.5/gradiop/plug.py`

 * *Files identical despite different names*

### Comparing `gradiop-0.0.4/gradiop/templates/assets/index-7da4454e.js` & `gradiop-0.0.5/gradiop/templates/cdn/assets/index-7da4454e.js`

 * *Files identical despite different names*

### Comparing `gradiop-0.0.4/gradiop/templates/assets/index-7da4454e.js.map` & `gradiop-0.0.5/gradiop/templates/cdn/assets/index-7da4454e.js.map`

 * *Files identical despite different names*

### Comparing `gradiop-0.0.4/gradiop/templates/cdn/ajax/libs/iframe-resizer/4.3.1/iframeResizer.contentWindow.min.js` & `gradiop-0.0.5/gradiop/templates/cdn/assets/iframeResizer.contentWindow.min.js`

 * *Files identical despite different names*

### Comparing `gradiop-0.0.4/gradiop/templates/cdn/index.html` & `gradiop-0.0.5/gradiop/templates/cdn/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 		<link rel="preconnect" href="https://fonts.googleapis.com" />
 		<link
 			rel="preconnect"
 			href="https://fonts.gstatic.com"
 			crossorigin="anonymous"
 		/>
-		<script src="/ajax/libs/iframe-resizer/4.3.1/iframeResizer.contentWindow.min.js"></script>
+		<script src="/assets/iframeResizer.contentWindow.min.js"></script>
 		<script type="module" crossorigin src="/assets/index-7da4454e.js"></script>
 		
 	</head>
 
 	<body
 		style="
 			width: 100%;
```

### Comparing `gradiop-0.0.4/gradiop/version.py` & `gradiop-0.0.5/gradiop/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `gradiop-0.0.4/setup.py` & `gradiop-0.0.5/setup.py`

 * *Files identical despite different names*

