# Comparing `tmp/serviceboot-2.1.3.tar.gz` & `tmp/serviceboot-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/serviceboot-2.1.3.tar", last modified: Tue May  9 02:58:37 2023, max compression
+gzip compressed data, was "dist/serviceboot-2.1.4.tar", last modified: Fri May 12 01:55:21 2023, max compression
```

## Comparing `serviceboot-2.1.3.tar` & `serviceboot-2.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-09 02:58:37.000000 serviceboot-2.1.3/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 02:58:34.000000 serviceboot-2.1.3/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.3/serviceboot/build_docker.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.3/serviceboot/build_zip.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/command.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/compile_python.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/config_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/consul_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/oauth_client.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/onboarding.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/request_info.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    23475 2023-05-09 02:56:33.000000 serviceboot-2.1.3/serviceboot/serviceboot.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.3/serviceboot/token_service.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-09 02:58:37.000000 serviceboot-2.1.3/serviceboot.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-09 02:58:37.000000 serviceboot-2.1.3/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-09 02:56:33.000000 serviceboot-2.1.3/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-12 01:55:21.000000 serviceboot-2.1.4/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1526 2023-05-09 04:02:39.000000 serviceboot-2.1.4/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2764 2023-04-04 03:17:10.000000 serviceboot-2.1.4/serviceboot/build_docker.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4167 2023-04-03 13:17:50.000000 serviceboot-2.1.4/serviceboot/build_zip.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1376 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/command.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     4143 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/compile_python.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      417 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/config_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3010 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/consul_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3171 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/oauth_client.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2790 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/onboarding.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      178 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/request_info.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    23524 2023-05-12 01:54:19.000000 serviceboot-2.1.4/serviceboot/serviceboot.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1144 2022-11-15 06:17:47.000000 serviceboot-2.1.4/serviceboot/token_service.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2726 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      556 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       83 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       93 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       12 2023-05-12 01:55:21.000000 serviceboot-2.1.4/serviceboot.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2023-05-12 01:55:21.000000 serviceboot-2.1.4/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2438 2023-05-12 01:55:19.000000 serviceboot-2.1.4/setup.py
```

### Comparing `serviceboot-2.1.3/PKG-INFO` & `serviceboot-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.3
+Version: 2.1.4
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.3/README.md` & `serviceboot-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/build_docker.py` & `serviceboot-2.1.4/serviceboot/build_docker.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/build_zip.py` & `serviceboot-2.1.4/serviceboot/build_zip.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/command.py` & `serviceboot-2.1.4/serviceboot/command.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/compile_python.py` & `serviceboot-2.1.4/serviceboot/compile_python.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/consul_client.py` & `serviceboot-2.1.4/serviceboot/consul_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/oauth_client.py` & `serviceboot-2.1.4/serviceboot/oauth_client.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/onboarding.py` & `serviceboot-2.1.4/serviceboot/onboarding.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot/serviceboot.py` & `serviceboot-2.1.4/serviceboot/serviceboot.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
         logging.critical(f'    Python frontend started ...')
         logging.critical(f'    Web access: http://{get_local_ip()}:{g.python_frontend_port}/')
         logging.critical('##################################################')
         thread = threading.Thread(target=python_frontend_thread, args=(asyncio.get_event_loop(), python_frontend))
         thread.setDaemon(True)
         thread.start()
     except Exception as e:
-        pass
+        logging.error('Python前端启动失败：' + str(e))
 
 
 def python_frontend_thread(event_loop, python_frontend):
     asyncio.set_event_loop(event_loop)
     kwargs = {
         'server_name': '0.0.0.0',
         'server_port': g.python_frontend_port,
```

### Comparing `serviceboot-2.1.3/serviceboot/token_service.py` & `serviceboot-2.1.4/serviceboot/token_service.py`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/serviceboot.egg-info/PKG-INFO` & `serviceboot-2.1.4/serviceboot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serviceboot
-Version: 2.1.3
+Version: 2.1.4
 Summary: ServiceBoot云原生微服务引擎
 Home-page: https://openi.pcl.ac.cn/cubepy/serviceboot
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # ServiceBoot云原生微服务引擎
```

### Comparing `serviceboot-2.1.3/serviceboot.egg-info/SOURCES.txt` & `serviceboot-2.1.4/serviceboot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serviceboot-2.1.3/setup.py` & `serviceboot-2.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='serviceboot',
-    version='2.1.3',
+    version='2.1.4',
     author='cubeai',
     author_email='cubeai@163.com',
     description='ServiceBoot云原生微服务引擎',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

