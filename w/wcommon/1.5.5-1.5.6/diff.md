# Comparing `tmp/wcommon-1.5.5.tar.gz` & `tmp/wcommon-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.5.5.tar", last modified: Tue Apr 25 09:31:20 2023, max compression
+gzip compressed data, was "wcommon-1.5.6.tar", last modified: Fri May 12 07:52:50 2023, max compression
```

## Comparing `wcommon-1.5.5.tar` & `wcommon-1.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.076849 wcommon-1.5.5/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-25 09:31:20.076590 wcommon-1.5.5/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.5/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-04-25 09:31:20.076955 wcommon-1.5.5/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-04-25 09:31:05.000000 wcommon-1.5.5/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.073238 wcommon-1.5.5/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    24477 2023-04-25 09:22:06.000000 wcommon-1.5.5/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-25 09:31:20.076191 wcommon-1.5.5/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-04-25 09:31:19.000000 wcommon-1.5.5/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.389356 wcommon-1.5.6/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-05-12 07:52:50.388942 wcommon-1.5.6/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.6/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-05-12 07:52:50.389530 wcommon-1.5.6/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-05-12 07:51:53.000000 wcommon-1.5.6/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.384383 wcommon-1.5.6/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    25863 2023-05-12 07:24:30.000000 wcommon-1.5.6/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-05-12 07:52:50.388380 wcommon-1.5.6/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-05-12 07:52:50.000000 wcommon-1.5.6/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.5.5/PKG-INFO` & `wcommon-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.5
+Version: 1.5.6
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wcommon-1.5.5/README.md` & `wcommon-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `wcommon-1.5.5/setup.py` & `wcommon-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.5.5",
+    version="1.5.6",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.5.5/wcommon/__init__.py` & `wcommon-1.5.6/wcommon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -207,16 +207,14 @@
 def query(database, sql, argumentTuple=(), timestamp2str=True):
     import pymysql
     cursor = database.cursor()
     logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
-        if type(argumentTuple) == list:
-            argumentTuple = tuple(argumentTuple)
         cursor.execute(sql, argumentTuple)
     rows = []
 
     if timestamp2str:
         timestamp_field_array = []
         date_field_array = []
         for tp in cursor.description:
@@ -290,16 +288,14 @@
 
 def execute(database, sql, argumentTuple=()):
     cursor = database.cursor()
     logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
-        if type(argumentTuple) == list:
-            argumentTuple = tuple(argumentTuple)
         cursor.execute(sql, argumentTuple)
 
 
 def delete(database, sql, commit=True):
     cursor = database.cursor()
     logger.debug("delete sql:\t" + sql)
     if commit:
@@ -308,17 +304,15 @@
 
 
 def mysql_execute(database, sql, argumentTuple, commit=True):
     cursor = database.cursor()
     if argumentTuple:
         cursor.execute(sql, argumentTuple)
     else:
-        if type(argumentTuple) == list:
-            argumentTuple = tuple(argumentTuple)
-        cursor.execute(sql, argumentTuple)
+        cursor.execute(sql)
     if commit:
         database.commit()
 
 
 # 获取文件的创建时间
 def getFileCreateTime(filePath):
     # filePath = unicode(filePath,'utf8')
@@ -587,16 +581,14 @@
     @pingmysql
     def query(self, sql, argumentTuple=(), timestamp2str=True):
         cursor = self.database.cursor()
         logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
         if len(argumentTuple) == 0:
             cursor.execute(sql)
         else:
-            if type(argumentTuple) == list:
-                argumentTuple = tuple(argumentTuple)
             cursor.execute(sql, argumentTuple)
         rows = []
 
         if timestamp2str:
             timestamp_field_array = []
             date_field_array = []
             for tp in cursor.description:
@@ -684,16 +676,14 @@
     @pingmysql
     def execute(self, sql, argumentTuple=(), commit=True):
         cursor = self.database.cursor()
         logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
         if len(argumentTuple) == 0:
             cursor.execute(sql)
         else:
-            if type(argumentTuple) == list:
-                argumentTuple = tuple(argumentTuple)
             cursor.execute(sql, argumentTuple)
         if commit:
             self.database.commit()
 
     @pingmysql
     def delete(self, sql, commit=True):
         cursor = self.database.cursor()
@@ -743,7 +733,64 @@
             values_array.append(tmp_ar)
         logger.debug(values_array)
         cursor = self.database.cursor()
         for start in range(0, len(values_array), batch_size):
             logger.debug(values_array[start:start + batch_size])
             cursor.executemany(ql, values_array[start:start + batch_size])
             self.database.commit()
+
+
+class ElasticSearch():
+    """
+    通过requests来访问ElasticSearch
+    """
+
+    def __init__(self, host, port=9200, username=None, password=None):
+        self.host = host
+        self.port = port
+        self.username = username
+        self.password = password
+        self.urlPrefix = "http://{}:{}".format(host, port)
+
+    headers = {
+        'content-type': 'application/json'
+    }
+
+    def _transfer_data(self, data=None):
+        if data is not None:
+            if type(data) == str:
+                return data
+            elif type(data) == dict:
+                return json.dumps(data)
+        return None
+
+    def search(self, action, data=None):
+        data1 = self._transfer_data(data)
+        return requests.get(url="{}{}".format(self.urlPrefix, action), auth=(self.username, self.password),
+                            headers=self.headers, data=data1).json()
+
+    def delete_by_query(self, index, data):
+        """
+        :param action: /sym/_delete_by_query
+        :return:
+        """
+        data1 = self._transfer_data(data)
+        return requests.post(url="{}/{}/_delete_by_query".format(self.urlPrefix, index),
+                             auth=(self.username, self.password), headers=self.headers, data=data1)
+
+    def delete(self, index, doc_id):
+        return requests.delete(url="{}/{}/_doc/{}".format(self.urlPrefix, index, doc_id),
+                               auth=(self.username, self.password))
+
+    def put(self, action, data=None):
+        """
+
+        :param action:
+        :param data:
+        :return:
+        """
+        return self.post(action, data)
+
+    def post(self, action, data=None):
+        data1 = self._transfer_data(data)
+        return requests.post(url="{}{}".format(self.urlPrefix, action), auth=(self.username, self.password),
+                             headers=self.headers, data=data1)
```

### Comparing `wcommon-1.5.5/wcommon.egg-info/PKG-INFO` & `wcommon-1.5.6/wcommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.5.5
+Version: 1.5.6
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

