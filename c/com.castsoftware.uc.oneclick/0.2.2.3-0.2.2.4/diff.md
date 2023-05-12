# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.3.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.3.tar", last modified: Mon Apr 24 15:45:47 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.4.tar", last modified: Tue Apr 25 14:33:52 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.3.tar` & `com.castsoftware.uc.oneclick-0.2.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.988118 com.castsoftware.uc.oneclick-0.2.2.3/
--rw-rw-rw-   0        0        0      517 2023-04-24 15:45:46.978077 com.castsoftware.uc.oneclick-0.2.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.680508 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      517 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 15:45:46.000000 com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.769439 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/
--rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.826132 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3454 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19536 2023-04-24 15:43:03.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:45:46.964703 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9049 2023-04-20 20:31:28.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6803 2023-04-20 20:26:23.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11311 2023-04-24 15:11:15.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.3/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0      737 2023-04-24 15:45:27.000000 com.castsoftware.uc.oneclick-0.2.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 15:45:46.988118 com.castsoftware.uc.oneclick-0.2.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 14:33:52.153600 com.castsoftware.uc.oneclick-0.2.2.4/
+-rw-rw-rw-   0        0        0      517 2023-04-25 14:33:52.141813 com.castsoftware.uc.oneclick-0.2.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 14:33:51.907945 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-25 14:33:51.000000 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-04-25 14:33:51.000000 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:33:51.000000 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-04-25 14:33:51.000000 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 14:33:51.000000 com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 14:33:51.988495 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:33:52.041982 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3454 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19552 2023-04-25 13:49:10.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:33:52.130275 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9049 2023-04-20 20:31:28.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-04-25 14:27:31.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11247 2023-04-25 13:53:33.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.4/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0      737 2023-04-25 14:32:05.000000 com.castsoftware.uc.oneclick-0.2.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 14:33:52.153600 com.castsoftware.uc.oneclick-0.2.2.4/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.3
+Version: 0.2.2.4
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2.3
+Version: 0.2.2.4
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.4/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 
         self.log.info(f'New project: {value}')
         if 'project' not in self._config:
             self._config['project']={}
             self._config['project']['name']=value
             self._config['project']['application']={}
 
-        elif value != self.project_name:
+        elif value.lower() != self.project_name.lower():
             raise ValueError("Can't rename a project")
 
     @property
     def project_name(self):
         return self.project['name']
 
     @property
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/cloc.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/sqlDiscovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def run(cls,config:Config):
         
         apps= config.application
 
         for app in apps:
             cls._log.info(f'Running {cls.__class__.__name__} for {app}')
 
-            app_folder = f'{config.work}\\{app}\\AIP'
+            app_folder = abspath(f'{config.work}\\AIP\\{config.project_name}\\{app}')
             for root, dirs, files in walk(app_folder):
                 for file in files:
                     if file.endswith(".sql") or file.endswith(".dtd") :
                         found = True
                         cls.read_sql_file(root,file)
 
             table_dict={}
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,17 @@
         log.error("Invalid Configuration")
         log.error(ex)
         cfg = ''
         if 'CLOC' in str(ex):
             cfg = '--cloc_version <cloc.exe>'
 
         log.info('To update the default configuraiton file use')
-        log.info(f'     python -m oneclick.main config -b {config.base} {cfg}')
+        log.info(f'     OneClick config {cfg}')
         log.info('To update the application configuraiton file use:')
-        log.info(f'     python -m oneclick.main config -b {config.base} -p {config.project_name} {cfg}')
+        log.info(f'     OneClick config -p {config.project_name} {cfg}')
         exit()
 
 
     # parser.add_argument('-c','--companyName',  default='Company Name', help='Name of the project')
     # parser.add_argument('--JavaHome',  help='Location of the JRE')
     # parser.add_argument('--from-email',  help='Email sending from')
     # parser.add_argument('--from-to',  help='Email sending from')
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.4/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2.3/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2.3' #prod version
+version='0.2.2.4' #prod version
 dependencies = [
     'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
     'com.castsoftware.uc.python.common>=0.1.6',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
```

