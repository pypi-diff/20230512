# Comparing `tmp/gradiop-0.0.2.tar.gz` & `tmp/gradiop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gradiop-0.0.2.tar", last modified: Fri May 12 07:22:26 2023, max compression
+gzip compressed data, was "dist\gradiop-0.0.3.tar", last modified: Fri May 12 08:29:34 2023, max compression
```

## Comparing `gradiop-0.0.2.tar` & `gradiop-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/
--rw-rw-rw-   0        0        0      264 2023-05-12 07:22:26.000000 gradiop-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop/
--rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.2/gradiop/__init__.py
--rw-rw-rw-   0        0        0      610 2023-05-12 07:10:44.000000 gradiop-0.0.2/gradiop/plug.py
--rw-rw-rw-   0        0        0     1176 2023-05-12 07:16:45.000000 gradiop-0.0.2/gradiop/version.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/
--rw-rw-rw-   0        0        0      264 2023-05-12 07:22:25.000000 gradiop-0.0.2/gradiop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:22:25.000000 gradiop-0.0.2/gradiop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 07:22:26.000000 gradiop-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-05-12 07:15:05.000000 gradiop-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/
+-rw-rw-rw-   0        0        0       37 2023-05-12 08:27:27.000000 gradiop-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      264 2023-05-12 08:29:34.000000 gradiop-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/
+-rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.3/gradiop/__init__.py
+-rw-rw-rw-   0        0        0      610 2023-05-12 07:10:44.000000 gradiop-0.0.3/gradiop/plug.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/cdn/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/cdn/ajax/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/cdn/ajax/libs/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/cdn/ajax/libs/iframe-resizer/
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop/templates/cdn/ajax/libs/iframe-resizer/4.3.1/
+-rw-rw-rw-   0        0        0    13719 2023-05-12 04:10:04.000000 gradiop-0.0.3/gradiop/templates/cdn/ajax/libs/iframe-resizer/4.3.1/iframeResizer.contentWindow.min.js
+-rw-rw-rw-   0        0        0     2101 2023-05-12 06:24:53.000000 gradiop-0.0.3/gradiop/templates/cdn/index.html
+-rw-rw-rw-   0        0        0     1176 2023-05-12 07:30:52.000000 gradiop-0.0.3/gradiop/version.py
+drwxrwxrwx   0        0        0        0 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-05-12 08:29:33.000000 gradiop-0.0.3/gradiop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-12 08:29:34.000000 gradiop-0.0.3/gradiop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 08:29:33.000000 gradiop-0.0.3/gradiop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 08:29:33.000000 gradiop-0.0.3/gradiop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-12 08:29:33.000000 gradiop-0.0.3/gradiop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 08:29:33.000000 gradiop-0.0.3/gradiop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 08:29:34.000000 gradiop-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-05-12 08:28:20.000000 gradiop-0.0.3/setup.py
```

### Comparing `gradiop-0.0.2/gradiop/plug.py` & `gradiop-0.0.3/gradiop/plug.py`

 * *Files identical despite different names*

### Comparing `gradiop-0.0.2/gradiop/version.py` & `gradiop-0.0.3/gradiop/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `gradiop-0.0.2/setup.py` & `gradiop-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,23 @@
     '''  
 
 setup(
     name=name,
     version=get_version(),
     description="gradio 本地部署 插件",
     author='zhys513',#作者
-    packages=find_packages(),
+    packages=find_packages(), 
     author_email="254851907@qq.com",
     url="https://gitee.com/zhys513/gradio_plug",
     python_requires='>=3.6', 
     install_requires=['gradio'],
     # 任何包如果包含 *.txt or *.rst 文件都加进去，可以处理多层package目录结构 
-    package_data={'': ['*.js','*.css','*.map'],},
+    package_data={
+        'gradiop': ['templates/*.js', 'templates/*.css', 'templates/*.map'],
+    },
+    include_package_data=True,
     entry_points={
         'console_scripts': ['gradiop=gradiop.plug:install']
     },
  
 )
```

