# Comparing `tmp/algospace-0.4.5.tar.gz` & `tmp/algospace-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algospace-0.4.5.tar", last modified: Wed May 10 08:47:40 2023, max compression
+gzip compressed data, was "algospace-0.4.6.tar", last modified: Fri May 12 09:46:12 2023, max compression
```

## Comparing `algospace-0.4.5.tar` & `algospace-0.4.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.723793 algospace-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 08:47:25.000000 algospace-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 08:47:25.000000 algospace-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 08:47:40.723793 algospace-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 08:47:25.000000 algospace-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/customer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/docker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/enroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/algospace-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.723793 algospace-0.4.5/algospace/provider/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:47:40.723793 algospace-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 08:47:25.000000 algospace-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.420284 algospace-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-12 09:46:03.000000 algospace-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-12 09:46:03.000000 algospace-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-12 09:46:12.420284 algospace-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-12 09:46:03.000000 algospace-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.412284 algospace-0.4.6/algospace/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/customer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/customer/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/docker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/enroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.416284 algospace-0.4.6/algospace/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/algospace-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.420284 algospace-0.4.6/algospace/provider/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-docker-stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/provider/templates/docker/algospace-dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 09:46:03.000000 algospace-0.4.6/algospace/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 09:46:12.412284 algospace-0.4.6/algospace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 09:46:12.000000 algospace-0.4.6/algospace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 09:46:12.420284 algospace-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-12 09:46:03.000000 algospace-0.4.6/setup.py
```

### Comparing `algospace-0.4.5/PKG-INFO` & `algospace-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.5
+Version: 0.4.6
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.5/README.md` & `algospace-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/__init__.py` & `algospace-0.4.6/algospace/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/__main__.py` & `algospace-0.4.6/algospace/__main__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/customer/fn.py` & `algospace-0.4.6/algospace/customer/fn.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/customer/service.py` & `algospace-0.4.6/algospace/customer/service.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/exceptions/__init__.py` & `algospace-0.4.6/algospace/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/logger.py` & `algospace-0.4.6/algospace/logger.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/login.py` & `algospace-0.4.6/algospace/login.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/cloud.py` & `algospace-0.4.6/algospace/provider/cloud.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/config.py` & `algospace-0.4.6/algospace/provider/config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/config_generator.py` & `algospace-0.4.6/algospace/provider/config_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/config_loader.py` & `algospace-0.4.6/algospace/provider/config_loader.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/docker_generator.py` & `algospace-0.4.6/algospace/provider/docker_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/enroll.py` & `algospace-0.4.6/algospace/provider/enroll.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/service.py` & `algospace-0.4.6/algospace/provider/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 算法提供者核心服务
 @Author: Kermit
 @Date: 2022-11-05 16:46:46
 @LastEditors: Kermit
-@LastEditTime: 2023-04-14 12:52:52
+@LastEditTime: 2023-05-12 17:10:35
 '''
 
 from typing import Any, Callable, Optional, List, Tuple, Union
 from algospace.logger import Logger, algospace_logger
 from algospace.util import create_timestamp_filename
 from . import config
 from .config import Algoinfo
@@ -830,87 +830,91 @@
                                                            fn_req_queue_list,
                                                            fn_res_queue_list,
                                                            gradio_port_con1),
                                                      daemon=True)
             gradio_process.start()
             return gradio_process
 
-        def check_process_alive(process: multiprocessing.Process):
-            is_alive = process.is_alive()
-            if not is_alive:
-                process.kill()
-            return is_alive
-
         fn_process = create_fn_process()
         service_process = create_service_process()
         gradio_process = create_gradio_process()
+        process_exit_code = None
 
         self.algo_logger.info(f'Waiting for service launched...')
 
-        # 开启事件循环
-        async def alive_task():
-            nonlocal fn_process
-            nonlocal service_process
-            nonlocal gradio_process
-            while True:
-                await asyncio.sleep(1)
-                if not check_process_alive(fn_process):
-                    raise Exception('Fn process is not alive. Please check error log above.')
-                if not check_process_alive(service_process):
-                    raise Exception('Service process is not alive')
-                if not check_process_alive(gradio_process):
-                    raise Exception('Gradio process is not alive')
+        async def join_task(process: multiprocessing.Process):
+            nonlocal process_exit_code
+            try:
+                await asyncio.get_event_loop().run_in_executor(None, process.join)
+                process_exit_code = process.exitcode
+            except:
+                if process.is_alive():
+                    process.kill()
 
         async def heartbeat_task():
             times = 0
             while True:
                 try:
                     await asyncio.sleep(1)
                     if times % 10 == 0:
                         # 每 10 秒发送心跳
-                        await asyncio.get_running_loop().run_in_executor(None, self.send_heartbeat)
+                        await asyncio.get_event_loop().run_in_executor(None, self.send_heartbeat)
                         times = 0
                     times += 1
+                except concurrent.futures._base.CancelledError:
+                    break
+                except asyncio.CancelledError:
+                    break
                 except Exception as e:
                     times = 1
                     traceback.print_exc()
                     self.algo_logger.error(f'Heartbeat error: {str(e)}')
 
         async def subprocess_stdio_task():
             queue_stdio_exec = QueueStdIOExec(stdio_queue)
             stdio_exec = queue_stdio_exec.exec
             stdio_exec_all = queue_stdio_exec.exec_all
             is_execed = True
             while True:
                 try:
                     if not is_execed:
                         await asyncio.sleep(0.1)
-                    is_execed = await asyncio.get_running_loop().run_in_executor(None, stdio_exec)
+                    is_execed = await asyncio.get_event_loop().run_in_executor(None, stdio_exec)
                 except concurrent.futures._base.CancelledError:
                     stdio_exec_all()
-                    raise
+                    break
                 except asyncio.CancelledError:
                     stdio_exec_all()
-                    raise
+                    break
                 except Exception as e:
                     traceback.print_exc()
                     self.algo_logger.error(f'Handle subprocess stdio error: {str(e)}')
 
         # 当有任务抛出异常时，停止所有任务
-        tasks = [alive_task(), heartbeat_task(), subprocess_stdio_task()]
-        done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_EXCEPTION)
+        tasks = [join_task(fn_process),
+                 join_task(service_process),
+                 join_task(gradio_process),
+                 heartbeat_task(),
+                 subprocess_stdio_task()]
+        done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
         for task in pending:
             task.cancel()
         for task in done:
             task.result()
+        return process_exit_code
 
 
 def run_service(config_path: str, fetch_mode: str = 'listen') -> None:
     loop = asyncio.get_event_loop()
+    service_coroutine = None
+    exit_code = None
     try:
         algospace_logger.info('Init.')
         service = Service(config_path, fetch_mode)
-        loop.run_until_complete(service.start())
+        service_coroutine = service.start()
+        exit_code = loop.run_until_complete(service_coroutine)
     except:
         traceback.print_exc()
+        exit_code = 1
     finally:
         algospace_logger.info('Exit.')
+    exit(exit_code or 0)
```

### Comparing `algospace-0.4.5/algospace/provider/stdio.py` & `algospace-0.4.6/algospace/provider/stdio.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace/provider/templates/algospace-config.py` & `algospace-0.4.6/algospace/provider/templates/algospace-config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/algospace.egg-info/PKG-INFO` & `algospace-0.4.6/algospace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.5
+Version: 0.4.6
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.5/algospace.egg-info/SOURCES.txt` & `algospace-0.4.6/algospace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algospace-0.4.5/setup.py` & `algospace-0.4.6/setup.py`

 * *Files identical despite different names*

