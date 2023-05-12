# Comparing `tmp/gradiop-0.0.1.tar.gz` & `tmp/gradiop-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gradiop-0.0.1.tar", last modified: Fri May 12 06:49:40 2023, max compression
+gzip compressed data, was "dist\gradiop-0.0.2.tar", last modified: Fri May 12 07:22:26 2023, max compression
```

## Comparing `gradiop-0.0.1.tar` & `gradiop-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 06:49:40.000000 gradiop-0.0.1/
--rw-rw-rw-   0        0        0      264 2023-05-12 06:49:40.000000 gradiop-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-12 06:49:40.000000 gradiop-0.0.1/gradiop/
--rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.1/gradiop/__init__.py
--rw-rw-rw-   0        0        0      556 2023-05-12 06:40:42.000000 gradiop-0.0.1/gradiop/plug.py
--rw-rw-rw-   0        0        0     1176 2023-05-12 04:15:37.000000 gradiop-0.0.1/gradiop/version.py
-drwxrwxrwx   0        0        0        0 2023-05-12 06:49:40.000000 gradiop-0.0.1/gradiop.egg-info/
--rw-rw-rw-   0        0        0      264 2023-05-12 06:49:39.000000 gradiop-0.0.1/gradiop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-12 06:49:40.000000 gradiop-0.0.1/gradiop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 06:49:39.000000 gradiop-0.0.1/gradiop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-12 06:49:40.000000 gradiop-0.0.1/gradiop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 06:49:40.000000 gradiop-0.0.1/gradiop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 06:49:40.000000 gradiop-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-05-12 06:40:42.000000 gradiop-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/
+-rw-rw-rw-   0        0        0      264 2023-05-12 07:22:26.000000 gradiop-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop/
+-rw-rw-rw-   0        0        0      194 2023-05-12 06:40:29.000000 gradiop-0.0.2/gradiop/__init__.py
+-rw-rw-rw-   0        0        0      610 2023-05-12 07:10:44.000000 gradiop-0.0.2/gradiop/plug.py
+-rw-rw-rw-   0        0        0     1176 2023-05-12 07:16:45.000000 gradiop-0.0.2/gradiop/version.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/
+-rw-rw-rw-   0        0        0      264 2023-05-12 07:22:25.000000 gradiop-0.0.2/gradiop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:22:25.000000 gradiop-0.0.2/gradiop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 07:22:26.000000 gradiop-0.0.2/gradiop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 07:22:26.000000 gradiop-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-05-12 07:15:05.000000 gradiop-0.0.2/setup.py
```

### Comparing `gradiop-0.0.1/gradiop/plug.py` & `gradiop-0.0.2/gradiop/plug.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,11 @@
     html_file_path = pkg_resources.resource_filename('gradiop', 'templates')  
     gradio_path = pkg_resources.resource_filename('gradio','templates') 
 
     print("gradio_path:",gradio_path)
     print("html_file_path:",html_file_path)
     
     # 复制文件到gradio的安装位置
-    shutil.copytree(html_file_path, gradio_path, dirs_exist_ok=True)
+    shutil.copytree(html_file_path, gradio_path, dirs_exist_ok=True)
+    
+if __name__ == '__main__':
+    print("start")
```

### Comparing `gradiop-0.0.1/gradiop/version.py` & `gradiop-0.0.2/gradiop/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 def parse_version_info(version_str: str, length: int = 4) -> tuple:
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `gradiop-0.0.1/setup.py` & `gradiop-0.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,25 +11,28 @@
 
 def get_version(): 
     version_file = name + '/version.py'
     with open(version_file, 'r', encoding='utf-8') as f:
         exec(compile(f.read(), version_file, 'exec'))
     return locals()['__version__']
     '''
-    return '0.0.1'
+    return '0.0.2'
     '''  
 
 setup(
     name=name,
     version=get_version(),
     description="gradio 本地部署 插件",
     author='zhys513',#作者
     packages=find_packages(),
     author_email="254851907@qq.com",
     url="https://gitee.com/zhys513/gradio_plug",
     python_requires='>=3.6', 
     install_requires=['gradio'],
     # 任何包如果包含 *.txt or *.rst 文件都加进去，可以处理多层package目录结构 
     package_data={'': ['*.js','*.css','*.map'],},
+    entry_points={
+        'console_scripts': ['gradiop=gradiop.plug:install']
+    },
  
 )
```

