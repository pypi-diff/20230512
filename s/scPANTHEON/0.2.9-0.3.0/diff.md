# Comparing `tmp/scPANTHEON-0.2.9.tar.gz` & `tmp/scPANTHEON-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\scPANTHEON-0.2.9.tar", last modified: Fri May 12 03:05:50 2023, max compression
+gzip compressed data, was "scPANTHEON-0.3.0.tar", last modified: Fri May 12 03:09:44 2023, max compression
```

## Comparing `scPANTHEON-0.2.9.tar` & `scPANTHEON-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/
--rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0      314 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scpantheon/
--rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.2.9/scpantheon/bokeh_qt.py
--rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.2.9/scpantheon/data_qt.py
--rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.2.9/scpantheon/main.py
--rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.2.9/scpantheon/qt.py
--rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.2.9/scpantheon/run.py
--rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.2.9/scpantheon/save_qt.py
--rw-rw-rw-   0        0        0    59950 2023-05-12 02:56:06.000000 scPANTHEON-0.2.9/scpantheon/source.py
--rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.2.9/scpantheon/transform.py
--rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.2.9/scpantheon/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      314 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/requires.txt
--rw-rw-rw-   0        0        0      425 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/scPANTHEON.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 03:05:50.000000 scPANTHEON-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-05-12 03:05:27.000000 scPANTHEON-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.184852 scPANTHEON-0.3.0/
+-rw-rw-rw-   0        0        0       26 2023-02-09 07:28:41.000000 scPANTHEON-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      261 2023-05-12 03:09:44.183846 scPANTHEON-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-02-09 07:28:41.000000 scPANTHEON-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.169514 scPANTHEON-0.3.0/scPANTHEON.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-05-12 03:09:44.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-12 03:09:43.000000 scPANTHEON-0.3.0/scPANTHEON.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 03:09:44.181840 scPANTHEON-0.3.0/scpantheon/
+-rw-rw-rw-   0        0        0        0 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-05-08 07:38:57.000000 scPANTHEON-0.3.0/scpantheon/bokeh_qt.py
+-rw-rw-rw-   0        0        0     4162 2023-05-08 07:39:20.000000 scPANTHEON-0.3.0/scpantheon/data_qt.py
+-rw-rw-rw-   0        0        0     1162 2023-05-08 06:41:40.000000 scPANTHEON-0.3.0/scpantheon/main.py
+-rw-rw-rw-   0        0        0     5627 2023-05-08 06:44:29.000000 scPANTHEON-0.3.0/scpantheon/qt.py
+-rw-rw-rw-   0        0        0      401 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/run.py
+-rw-rw-rw-   0        0        0     3270 2023-05-12 02:45:41.000000 scPANTHEON-0.3.0/scpantheon/save_qt.py
+-rw-rw-rw-   0        0        0    59950 2023-05-12 02:56:06.000000 scPANTHEON-0.3.0/scpantheon/source.py
+-rw-rw-rw-   0        0        0      634 2023-02-09 07:28:42.000000 scPANTHEON-0.3.0/scpantheon/transform.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 03:09:44.184926 scPANTHEON-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-05-12 03:09:29.000000 scPANTHEON-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scPANTHEON-0.2.9/scpantheon/bokeh_qt.py` & `scPANTHEON-0.3.0/scpantheon/bokeh_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/data_qt.py` & `scPANTHEON-0.3.0/scpantheon/data_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/main.py` & `scPANTHEON-0.3.0/scpantheon/main.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/qt.py` & `scPANTHEON-0.3.0/scpantheon/qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/save_qt.py` & `scPANTHEON-0.3.0/scpantheon/save_qt.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/source.py` & `scPANTHEON-0.3.0/scpantheon/source.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/scpantheon/transform.py` & `scPANTHEON-0.3.0/scpantheon/transform.py`

 * *Files identical despite different names*

### Comparing `scPANTHEON-0.2.9/setup.py` & `scPANTHEON-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 # python setup.py sdist bdist_wheel
 # python -m twine upload dist/*
 
 setup(
     name='scPANTHEON',# 需要打包的名字,即本模块要发布的名字
-    version='0.2.9',#版本
+    version='0.3.0',#版本
     description='A graphical interface for single cell analysis.', # 简要描述
     packages=['scpantheon'],   #  需要打包的模块
     author='xinzhu', # 作者名
     author_email='xinzhu.jiang@sjtu.edu.cn',   # 作者邮件
     url='https://github.com/xinzhu-email/Pantheon', # 项目地址,一般是代码托管的网站
     install_requires=['bokeh==2.4.3','pandas','anndata','colorcet','scanpy','numpy','PyQt5','PyQtWebEngine',
                         'appdirs==1.4.4'], # 依赖包,如果没有,可以不要
```

