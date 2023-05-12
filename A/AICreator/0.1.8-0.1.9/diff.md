# Comparing `tmp/AICreator-0.1.8.tar.gz` & `tmp/AICreator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.1.8.tar", last modified: Fri May 12 12:57:29 2023, max compression
+gzip compressed data, was "AICreator-0.1.9.tar", last modified: Fri May 12 12:59:17 2023, max compression
```

## Comparing `AICreator-0.1.8.tar` & `AICreator-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:57:29.485458 AICreator-0.1.8/
-drwxrwxrwx   0        0        0        0 2023-05-12 12:57:29.475921 AICreator-0.1.8/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-12 12:57:29.000000 AICreator-0.1.8/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-12 12:57:29.000000 AICreator-0.1.8/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:57:29.000000 AICreator-0.1.8/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-12 12:57:29.000000 AICreator-0.1.8/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-12 12:57:29.000000 AICreator-0.1.8/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-12 12:57:29.478941 AICreator-0.1.8/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.8/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:57:29.481459 AICreator-0.1.8/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      906 2023-05-12 12:57:04.000000 AICreator-0.1.8/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.8/AICreatorPackage/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:57:29.482459 AICreator-0.1.8/AICreatorPackage/functions/ini/
--rw-rw-rw-   0        0        0    52493 2023-05-12 12:14:40.000000 AICreator-0.1.8/AICreatorPackage/functions/ini/ini.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.8/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-12 12:57:29.484459 AICreator-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.8/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.8/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-12 12:57:29.485458 AICreator-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-12 12:57:25.000000 AICreator-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:59:17.067421 AICreator-0.1.9/
+drwxrwxrwx   0        0        0        0 2023-05-12 12:59:17.055117 AICreator-0.1.9/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-12 12:59:16.000000 AICreator-0.1.9/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-05-12 12:59:16.000000 AICreator-0.1.9/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:59:16.000000 AICreator-0.1.9/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 12:59:16.000000 AICreator-0.1.9/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 12:59:16.000000 AICreator-0.1.9/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 12:59:17.058424 AICreator-0.1.9/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.9/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:59:17.061425 AICreator-0.1.9/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      904 2023-05-12 12:58:58.000000 AICreator-0.1.9/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.9/AICreatorPackage/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:59:17.062420 AICreator-0.1.9/AICreatorPackage/functions/co/
+-rw-rw-rw-   0        0        0    52493 2023-05-12 12:14:40.000000 AICreator-0.1.9/AICreatorPackage/functions/co/co.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.9/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-12 12:59:17.064422 AICreator-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.9/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.9/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 12:59:17.067421 AICreator-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-12 12:59:12.000000 AICreator-0.1.9/setup.py
```

### Comparing `AICreator-0.1.8/AICreator.egg-info/PKG-INFO` & `AICreator-0.1.9/AICreator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.1.8
+Version: 0.1.9
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.1.8/AICreatorPackage/functions/AICreatorPackage.py` & `AICreator-0.1.9/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print("[+] AICreator (By Oren) Is Ready!")
 
     cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/discordbot/apiKey/{apiKEY}')
 
     cc1 = cc.json()
 
     try:
-        subprocess.run(["python", f"{os.path.dirname(__file__)}\ini\ini.py"])
+        subprocess.run(["python", f"{os.path.dirname(__file__)}\co\co.py"])
     except Exception as e:
         print(f"error, please contact support. {e}")
 
 
 
 
 def AICreatorWebsiteBot(apiKEY):
```

### Comparing `AICreator-0.1.8/AICreatorPackage/functions/ini/ini.py` & `AICreator-0.1.9/AICreatorPackage/functions/co/co.py`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.8/LICENCE.txt` & `AICreator-0.1.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.8/PKG-INFO` & `AICreator-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AICreator
-Version: 0.1.8
+Version: 0.1.9
 Summary: AI Creator Package By - oren
 Home-page: 
 Author: oren
 Author-email: orennadle@gmail.com
 License: MIT
 Keywords: ai
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `AICreator-0.1.8/setup.py` & `AICreator-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.1.8',
+    version='0.1.9',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

