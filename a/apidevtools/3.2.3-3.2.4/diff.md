# Comparing `tmp/apidevtools-3.2.3.tar.gz` & `tmp/apidevtools-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.2.3.tar", last modified: Fri May 12 02:04:18 2023, max compression
+gzip compressed data, was "apidevtools-3.2.4.tar", last modified: Fri May 12 15:39:47 2023, max compression
```

## Comparing `apidevtools-3.2.3.tar` & `apidevtools-3.2.4.tar`

### file list

```diff
@@ -1,69 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.706202 apidevtools-3.2.3/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-05-12 02:04:18.705201 apidevtools-3.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.3/README.md
--rw-rw-rw-   0        0        0     1795 2023-05-12 01:54:56.000000 apidevtools-3.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 02:04:18.706202 apidevtools-3.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.645202 apidevtools-3.2.3/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.3/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.649221 apidevtools-3.2.3/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.3/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.2.3/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.668237 apidevtools-3.2.3/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.2.3/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.3/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     4114 2023-05-12 01:53:42.000000 apidevtools-3.2.3/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.3/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.672203 apidevtools-3.2.3/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.3/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.3/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.675202 apidevtools-3.2.3/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.681202 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-05-01 17:19:11.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3392 2023-05-08 01:29:46.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6745 2023-05-08 01:31:17.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2087 2023-05-03 02:07:38.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.684203 apidevtools-3.2.3/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.3/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.687210 apidevtools-3.2.3/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.640202 apidevtools-3.2.3/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.689206 apidevtools-3.2.3/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.690203 apidevtools-3.2.3/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.693201 apidevtools-3.2.3/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.698212 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.702215 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.704213 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.2.3/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1155 2023-04-16 14:10:32.000000 apidevtools-3.2.3/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-12 02:04:18.664202 apidevtools-3.2.3/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-12 02:04:18.000000 apidevtools-3.2.3/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.288866 apidevtools-3.2.4/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-05-12 15:39:47.288334 apidevtools-3.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.2.4/README.md
+-rw-rw-rw-   0        0        0     1772 2023-05-12 15:39:18.000000 apidevtools-3.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-12 15:39:47.288866 apidevtools-3.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.193706 apidevtools-3.2.4/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.2.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.197711 apidevtools-3.2.4/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.2.4/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0     1743 2023-05-12 15:36:52.000000 apidevtools-3.2.4/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.234542 apidevtools-3.2.4/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.2.4/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.2.4/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-05-12 15:12:51.000000 apidevtools-3.2.4/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.2.4/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.237187 apidevtools-3.2.4/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.2.4/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.2.4/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.2.4/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.240371 apidevtools-3.2.4/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.257374 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4797 2023-05-12 15:05:27.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4450 2023-05-12 15:05:27.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3396 2023-05-12 15:06:13.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6748 2023-05-12 15:03:15.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.286637 apidevtools-3.2.4/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.2.4/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.2.4/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 15:39:47.215792 apidevtools-3.2.4/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-05-12 15:39:47.000000 apidevtools-3.2.4/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1012 2023-05-12 15:39:47.000000 apidevtools-3.2.4/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 15:39:47.000000 apidevtools-3.2.4/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-12 15:39:47.000000 apidevtools-3.2.4/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.2.3/LICENSE.txt` & `apidevtools-3.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/PKG-INFO` & `apidevtools-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.3
+Version: 3.2.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.2.3/README.md` & `apidevtools-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/pyproject.toml` & `apidevtools-3.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.2.3"
+version = "3.2.4"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
@@ -33,16 +33,16 @@
 
     "Operating System :: OS Independent",
 
     "License :: OSI Approved :: MIT License"
 ]
 dependencies=[
 #simpleorm
-    "pydantic~=1.10.4",
-    "loguru~=0.6.0",
+#    "pydantic~=1.10.4",
+#    "loguru~=0.6.0",
 #    "asyncpg~=0.27.0",
 #    "aiomysql~=0.1.1",
 #    "aioredis~=2.0.1",
 #    "aiosqlite~=0.18.0",
 
 #imgproc
 #    "Pillow~=9.4.0",
@@ -57,14 +57,14 @@
 #    "ujson~=5.7.0",
 #    "aiodns~=3.0.0",
 #    "cchardet~=2.1.7",
 #    "uvloop~=0.17.0"
 ]
 
 [tool.setuptools.package-data]
-apidevtools = ["template/template.zip", "media/ARIALNB.TTF"]
+apidevtools = ["media/ARIALNB.TTF"]
 
 [project.urls]
 "Homepage" = "https://github.com/cxllmerichie/apidevtools"
 "Bug Tracker" = "https://github.com/cxllmerichie/apidevtools/issues"
 "Repository" = "https://github.com/cxllmerichie/apidevtools"
 "Documentation" = "https://github.com/cxllmerichie/apidevtools/README.md"
```

### Comparing `apidevtools-3.2.3/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.2.4/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/media/telegraph.py` & `apidevtools-3.2.4/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/security/encryptor.py` & `apidevtools-3.2.4/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/security/hasher.py` & `apidevtools-3.2.4/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import aiomysql as _aiomysql
-from loguru._logger import Logger
 from typing import Any, MutableMapping
-import loguru
 
 from ..types import Relation
 from ._connector import Connector
+from ...logman import LoggerManager, Logger
 
 
 class MySQL(Connector):
     def __init__(self, database: str,
                  host: str = 'localhost', port: int | str = 3306,
                  user: str = 'root', password: str | None = None,
-                 logger: Logger = loguru.logger):
+                 logger: Logger = LoggerManager.logger()):
         self.database: str = database
         self.host: str = host
         self.port: str | int = port
         self.user: str = user
         self.password: str | None = password
 
         self.logger: Logger = logger
```

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import asyncpg as _asyncpg
-from loguru._logger import Logger
 from typing import Any, MutableMapping
-import loguru
 
 from ..types import Relation
 from ._connector import Connector
+from ...logman import LoggerManager, Logger
 
 
 class PostgreSQL(Connector):
     def __init__(self, database: str,
                  host: str = 'localhost', port: int | str = 5432,
                  user: str = 'postgres', password: str | None = None,
-                 logger: Logger = loguru.logger):
+                 logger: Logger = LoggerManager.logger()):
         self.database: str = database
         self.host: str = host
         self.port: str | int = port
         self.user: str = user
         self.password: str | None = password
 
         self.logger: Logger = logger
```

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import aiosqlite as _aiosqlite
-from loguru._logger import Logger
 from typing import Any, MutableMapping
-import loguru
 
 from ..types import Relation
 from ._connector import Connector
+from ...logman import LoggerManager, Logger
 
 
 class SQLite(Connector):
     __memory = ':memory:'
 
     def __init__(self, database: str = __memory,
-                 logger: Logger = loguru.logger):
+                 logger: Logger = LoggerManager.logger()):
         self.database: str = database if database.endswith(('.sqlite', '.db')) or database == self.__memory else f'{database}.sqlite'
 
         self.logger: Logger = logger
         self.pool: _aiosqlite.Connection | None = None
 
         super().__init__(placeholder='?', constraint_wrapper='"', value_wrapper="'")
```

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from loguru._logger import Logger
 from typing import Any
-import loguru
 import inspect as _inspect
 
 from ..utils import INF, is_dict as _is_dict
 from .types import RecordType, Record, Schema, Records, Relation, Instance
 from .connectors._connector import Connector
+from ..logman import LoggerManager, Logger
 
 
 class ORM:
-    def __init__(self, connector: Connector, logger: Logger = loguru.logger):
+    def __init__(self, connector: Connector, logger: Logger = LoggerManager.logger()):
         self.connector: Connector = connector
         self.logger: Logger = logger
 
     async def create_pool(self) -> bool:
         try:
             is_created = await self.connector.create_pool()
             self.logger.info(f'`ORM.connector: {self.connector.__class__.__name__}` pool created')
```

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import aioredis as _aioredis
-import loguru
-from loguru._logger import Logger
 from typing import Any
 
 from ..utils import evaluate as _evaluate
+from ..logman import LoggerManager, Logger
 
 
 class Redis:
     def __init__(self, database: int = 0,
                  host: str = 'localhost', port: int | str = 6379,
                  user: str | None = None, password: str | None = None,
-                 logger: Logger = loguru.logger):
+                 logger: Logger = LoggerManager.logger()):
         self.database: int = database
         self.host: str = host
         self.port: str | int = port
         self.user: str | None = user
         self.password: str | None = password
 
         self.logger: Logger = logger
```

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.2.4/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.2.3/src/apidevtools/utils.py` & `apidevtools-3.2.4/src/apidevtools/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         return _ast.literal_eval(f'\'{value.decode()}\'')
     except SyntaxError:
         return value.decode()
     except AttributeError:
         return None
 
 
-def is_dict(subscripted_dict_type: type[dict]) -> bool:
+def is_dict(dict_t: type[dict[Any, Any]]) -> bool:
     """
     compares `dict[Any, Any]` with `dict`, normally done using `is`, but does not work for subscripted types
-    :param subscripted_dict_type:
+    :param dict_t:
     :return:
     """
-    return subscripted_dict_type.__name__ == 'dict'
+    return dict_t.__name__ == 'dict'
```

### Comparing `apidevtools-3.2.3/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.2.4/src/apidevtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.2.3
+Version: 3.2.4
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

