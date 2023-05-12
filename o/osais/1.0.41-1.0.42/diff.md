# Comparing `tmp/osais-1.0.41.tar.gz` & `tmp/osais-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-5ex_q5v2\osais-1.0.41.tar", last modified: Fri May 12 12:26:40 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-pyu0zaem\osais-1.0.42.tar", last modified: Fri May 12 12:48:18 2023, max compression
```

## Comparing `osais-1.0.41.tar` & `osais-1.0.42.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 12:26:40.164061 osais-1.0.41/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.41/LICENSE
--rw-rw-rw-   0        0        0     1172 2023-05-12 12:26:40.164061 osais-1.0.41/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 12:26:40.158549 osais-1.0.41/osais/
--rw-rw-rw-   0        0        0      777 2023-05-12 12:25:52.000000 osais-1.0.41/osais/__init__.py
--rw-rw-rw-   0        0        0    51610 2023-05-12 12:24:02.000000 osais-1.0.41/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-05-12 12:26:40.163064 osais-1.0.41/osais.egg-info/
--rw-rw-rw-   0        0        0     1172 2023-05-12 12:26:40.000000 osais-1.0.41/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-12 12:26:40.000000 osais-1.0.41/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 12:26:40.000000 osais-1.0.41/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-05-12 12:26:40.000000 osais-1.0.41/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-12 12:26:40.000000 osais-1.0.41/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.41/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 12:26:40.164061 osais-1.0.41/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-05-12 12:26:10.000000 osais-1.0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.149699 osais-1.0.42/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.42/LICENSE
+-rw-rw-rw-   0        0        0     1172 2023-05-12 12:48:18.149699 osais-1.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-12 12:25:24.000000 osais-1.0.42/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.143175 osais-1.0.42/osais/
+-rw-rw-rw-   0        0        0      777 2023-05-12 12:47:53.000000 osais-1.0.42/osais/__init__.py
+-rw-rw-rw-   0        0        0    51840 2023-05-12 12:47:43.000000 osais-1.0.42/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:48:18.148689 osais-1.0.42/osais.egg-info/
+-rw-rw-rw-   0        0        0     1172 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-12 12:48:18.000000 osais-1.0.42/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.42/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 12:48:18.149699 osais-1.0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-05-12 12:47:59.000000 osais-1.0.42/setup.py
```

### Comparing `osais-1.0.41/LICENSE` & `osais-1.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.41/PKG-INFO` & `osais-1.0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.41
+Version: 1.0.42
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.41/osais/__init__.py` & `osais-1.0.42/osais/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.41"
+__version__="1.0.42"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
```

### Comparing `osais-1.0.41/osais/osais.py` & `osais-1.0.42/osais/osais.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.41"
+__version__="1.0.42"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -339,15 +339,15 @@
         try:
             # Filename - File to upload
             # Bucket - Bucket to upload to (the top level directory under AWS S3)
             # Key - S3 object name (can contain subdirectories). If not specified then file_name is used
             gS3.meta.client.upload_file(Filename=_filename, Bucket=gS3Bucket, Key=_dirS3+os.path.basename(_filename))
             return True
         except Exception as err:
-            consoleLog(err)
+            consoleLog({"msg":"Could not upload file to S3"})
             raise err
         
     return False
 
 ## ========================================================================
 ## 
 ##                      OSAIS starts here 
@@ -743,26 +743,26 @@
     try:
         response = requests.post(f"{gOriginGateway}api/v1/public/ai/config", headers=headers, data=json.dumps(objParam))
         objRes=response.json()["data"]
         if objRes is None:
             raise ValueError("CRITICAL: could not notify Gateway")
 
     except Exception as err:
-        consoleLog(err)
+        consoleLog({"msg":"CRITICAL: could not notify Gateway"})
         raise err
     return True
 
 ## PUBLIC - Reset connection to local gateway
 def osais_resetGateway(_localGateway):
     global gOriginGateway
     gOriginGateway=_localGateway
     try:
         _notifyGateway()
     except Exception as err:
-        consoleLog(err)
+        consoleLog({"msg":"Could not reset connection to Gateway"})
         raise err
     
     print("=> This AI is reset to talk to Gateway "+_localGateway)
     return True
 
 ## ------------------------------------------------------------------------
 #       authenticate into OSAIS as virtual AI
@@ -803,30 +803,30 @@
                 gSecret=objRes["secret"]
             else :
                 gTokenLocal=objRes["token"]
                 gSecretLocal=objRes["secret"]
 
             print("We are REGISTERED with OSAIS Prod")
         except Exception as err:
-            consoleLog("Exception raised while trying to register to PROD")
+            consoleLog({"msg":"Exception raised while trying to register to PROD"})
             raise err
 
     ## our AI is local, reg with Local OSAIS (debug)
     else:
         try:
             response = requests.post(f"{gOriginLocalOSAIS}api/v1/public/virtualai/register", headers=headers, data=json.dumps(objParam))
             objRes=response.json()["data"]
             if objRes is None:
                 print("COULD NOT REGISTER with debug")
 
             gTokenLocal=objRes["token"]
             gSecretLocal=objRes["secret"]
             print("We are REGISTERED with OSAIS Local (debug)")
         except Exception as err:
-            consoleLog("Exception raised while trying to register to DEBUG")
+            consoleLog({"msg":"Exception raised while trying to register to DEBUG"})
             raise err
 
     return True
 
 # Authenticate into OSAIS
 def _loginVAI(_originOSAIS):
     global gToken
@@ -850,15 +850,15 @@
             objRes=response.json()["data"]
             if objRes is None:
                 print("COULD NOT LOGIN, stopping it here")
                 sys.exit()
             print("We got an authentication token into OSAIS")
             gAuthToken=objRes["authToken"]    
         except Exception as err:
-            consoleLog("Exception raised while trying to login to PROD")
+            consoleLog({"msg":"Exception raised while trying to login to PROD"})
             raise err
 
     if gTokenLocal!= None:
         if _originOSAIS==None:
             _originOSAIS=gOriginLocalOSAIS
         try:
             response = requests.post(f"{_originOSAIS}api/v1/public/virtualai/login", headers=headers, data=json.dumps({
@@ -886,15 +886,15 @@
     
     resp={"data": None}
     if gIsVirtualAI:
         try:
             resp= _registerVAI(_originOSAIS)
             resp=_loginVAI(_originOSAIS)
         except Exception as err:
-            consoleLog("Exception raised while trying to authenticate to OSAIS")
+            consoleLog({"msg":"Exception raised while trying to authenticate to OSAIS"})
             raise err
         
         # Run the scheduler
         if gIsScheduled==False:
             gIsScheduled=True
             schedule.every().day.at("10:30").do(_loginVAI)
 
@@ -988,15 +988,15 @@
             authToken=gClientAuthToken
             resp={"data": {
                 "token": objRes["token"],
                 "authToken": gClientAuthToken,
             }}
 
         except Exception as err:
-            consoleLog("Exception raised while trying to login as CLIENT to PROD")
+            consoleLog({"msg":"Exception raised while trying to login as CLIENT to PROD"})
             gClientAuthToken=None
 
     dataClient=getClientInfo(authToken)
     resp["data"]["user"]=dataClient["data"]["user"]
     return resp 
 
 ## ------------------------------------------------------------------------
@@ -1113,15 +1113,15 @@
                 aArgForparserAI.append(_input)
             else:
                 ## min requirements
                 print("no image to process")
                 return "input required"
         except Exception as err:
             gIsBusy=False
-            consoleLog(err)
+            consoleLog({"msg":"Could not download image"})
             raise err
     
     ## Init OSAIS Params (from all args, keep only those for OSAIS)
     aArgForParserOSAIS=_getArgs(_args)
     args_ExclusiveOSAIS.append('-odir')
     args_ExclusiveOSAIS.append('-idir')
     aArgForParserOSAIS=_argsFromFilter(aArgForParserOSAIS, args_ExclusiveOSAIS, True)
@@ -1162,15 +1162,15 @@
         else:
             if len(args)==3:
                 response=fn_run(aArgForparserAI, args[2])
             else:
                 response=fn_run(aArgForparserAI, args[2], args[3])
     except Exception as err:
         gIsBusy=False
-        consoleLog(err)
+        consoleLog({"msg": "Error processing args in RUN command"})
         raise err
 
     ## calculate cost
     gIsBusy=False
     end_date = datetime.utcnow()
     delta=end_date - beg_date
     cost = int(delta.total_seconds()* 1000 + delta.microseconds / 1000)
@@ -1469,9 +1469,7 @@
 # Multithreading for observers
 watch_directory=start_observer_thread(_getOutputDir(), osais_onNotifyFileCreated, None)     
 
 #cleaning dir every 10min
 schedule.every(10).minutes.do(_clearDir)
 
 print("\r\nPython OSAIS Lib is loaded...")
-
-
```

### Comparing `osais-1.0.41/osais.egg-info/PKG-INFO` & `osais-1.0.42/osais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.41
+Version: 1.0.42
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.41/setup.py` & `osais-1.0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.41',
+    version='1.0.42',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

