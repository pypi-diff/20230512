# Comparing `tmp/fastramqpi-1.4.0.tar.gz` & `tmp/fastramqpi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.4.0.tar", max compression
+gzip compressed data, was "fastramqpi-1.4.1.tar", max compression
```

## Comparing `fastramqpi-1.4.0.tar` & `fastramqpi-1.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0        0        0        0 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/LICENSES/
--rw-r--r--   0        0        0    15177 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     2932 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/README.md
--rw-r--r--   0        0        0       85 2023-04-20 11:30:25.500164 fastramqpi-1.4.0/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/config.py
--rw-r--r--   0        0        0     1144 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/context.py
--rw-r--r--   0        0        0     7100 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1577 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     3930 2023-04-20 11:30:25.501164 fastramqpi-1.4.0/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-04-20 11:30:25.552171 fastramqpi-1.4.0/fastramqpi/py.typed
--rw-r--r--   0        0        0     1390 2023-04-20 11:30:38.503015 fastramqpi-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 fastramqpi-1.4.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-05-12 08:30:32.722341 fastramqpi-1.4.1/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-05-12 08:30:32.722341 fastramqpi-1.4.1/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     2932 2023-05-12 08:30:32.722341 fastramqpi-1.4.1/README.md
+-rw-r--r--   0        0        0       85 2023-05-12 08:30:32.723341 fastramqpi-1.4.1/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-05-12 08:30:32.723341 fastramqpi-1.4.1/fastramqpi/config.py
+-rw-r--r--   0        0        0     1144 2023-05-12 08:30:32.723341 fastramqpi-1.4.1/fastramqpi/context.py
+-rw-r--r--   0        0        0     7100 2023-05-12 08:30:32.723341 fastramqpi-1.4.1/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-05-12 08:30:32.724341 fastramqpi-1.4.1/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     3930 2023-05-12 08:30:32.724341 fastramqpi-1.4.1/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:30:32.826351 fastramqpi-1.4.1/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1390 2023-05-12 08:30:51.902102 fastramqpi-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 fastramqpi-1.4.1/PKG-INFO
```

### Comparing `fastramqpi-1.4.0/LICENSES/MPL-2.0.txt` & `fastramqpi-1.4.1/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/README.md` & `fastramqpi-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/fastramqpi/config.py` & `fastramqpi-1.4.1/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/fastramqpi/context.py` & `fastramqpi-1.4.1/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/fastramqpi/fastapi.py` & `fastramqpi-1.4.1/fastramqpi/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/fastramqpi/healthcheck.py` & `fastramqpi-1.4.1/fastramqpi/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/fastramqpi/main.py` & `fastramqpi-1.4.1/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.0/pyproject.toml` & `fastramqpi-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.4.0"
+version = "1.4.1"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
 packages = [ { include = "fastramqpi" } ]
 include = ["fastramqpi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-structlog = "^22.3.0"
-ramqp = "^8.2.0"
+structlog = "^23.1.0"
+ramqp = "^8.3.0"
 pydantic = "^1.10.5"
 raclients = "^3.0.5"
 gql = "^3.4.0"
 more-itertools = "^9.1.0"
 ra-utils = "^1.12.2"
 prometheus-fastapi-instrumentator = ">=5.9.1,<7.0.0"
 fastapi = ">=0.93, <1.0"
```

### Comparing `fastramqpi-1.4.0/PKG-INFO` & `fastramqpi-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.4.0
+Version: 1.4.1
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -15,16 +15,16 @@
 Requires-Dist: fastapi (>=0.93,<1.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<7.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: ra-utils (>=1.12.2,<2.0.0)
 Requires-Dist: raclients (>=3.0.5,<4.0.0)
-Requires-Dist: ramqp (>=8.2.0,<9.0.0)
-Requires-Dist: structlog (>=22.3.0,<23.0.0)
+Requires-Dist: ramqp (>=8.3.0,<9.0.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/FastRAMQPI
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2021 Magenta ApS <https://magenta.dk>
 SPDX-License-Identifier: MPL-2.0
 -->
```

