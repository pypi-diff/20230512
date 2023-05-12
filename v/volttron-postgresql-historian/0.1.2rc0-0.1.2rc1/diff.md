# Comparing `tmp/volttron_postgresql_historian-0.1.2rc0.tar.gz` & `tmp/volttron_postgresql_historian-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_postgresql_historian-0.1.2rc0.tar", max compression
+gzip compressed data, was "volttron_postgresql_historian-0.1.2rc1.tar", max compression
```

## Comparing `volttron_postgresql_historian-0.1.2rc0.tar` & `volttron_postgresql_historian-0.1.2rc1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11928 2023-05-12 20:43:46.632365 volttron_postgresql_historian-0.1.2rc0/LICENSE
--rwxr-xr-x   0        0        0     9154 2023-05-12 20:44:41.469448 volttron_postgresql_historian-0.1.2rc0/README.md
--rw-r--r--   0        0        0     1400 2023-05-12 20:46:59.159836 volttron_postgresql_historian-0.1.2rc0/pyproject.toml
--rw-r--r--   0        0        0     1082 2023-05-12 20:43:46.632365 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__init__.py
--rw-r--r--   0        0        0      362 2023-05-12 20:44:49.841596 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    16058 2023-05-12 20:44:49.841596 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__pycache__/postgresqlfuncts.cpython-310.pyc
--rw-r--r--   0        0        0    18297 2023-05-12 20:44:41.469448 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/postgresqlfuncts.py
--rw-r--r--   0        0        0     9977 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc0/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/LICENSE
+-rwxr-xr-x   0        0        0     9154 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/README.md
+-rw-r--r--   0        0        0     1374 2023-05-12 20:48:49.686171 volttron_postgresql_historian-0.1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/__init__.py
+-rw-r--r--   0        0        0    18297 2023-05-12 20:47:21.648528 volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/postgresqlfuncts.py
+-rw-r--r--   0        0        0    10470 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc1/setup.py
+-rw-r--r--   0        0        0     9977 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc1/PKG-INFO
```

### Comparing `volttron_postgresql_historian-0.1.2rc0/LICENSE` & `volttron_postgresql_historian-0.1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc0/README.md` & `volttron_postgresql_historian-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc0/pyproject.toml` & `volttron_postgresql_historian-0.1.2rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-postgresql-historian"
-version = "0.1.2rc0"
+version = "0.1.2rc1"
 description = "VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 keywords = []
@@ -26,15 +26,14 @@
 safety = "^1.10.3"
 mypy = "^0.942"
 coverage = "^6.3.2"
 pytest-cov = "^3.0.0"
 Sphinx = "^6.0.0"
 sphinx-rtd-theme = "^1.2.0"
 volttron-testing = "^0.4.0rc3"
-pytest-timeout = "^2.1.0"
 
 [tool.yapfignore]
 ignore_patterns = [
     ".venv/**",
     ".pytest_cache/**",
     "dist/**",
     "docs/**"
```

### Comparing `volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__init__.py` & `volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/postgresqlfuncts.py` & `volttron_postgresql_historian-0.1.2rc1/src/historian/postgresql/postgresqlfuncts.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.2rc0/PKG-INFO` & `volttron_postgresql_historian-0.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-postgresql-historian
-Version: 0.1.2rc0
+Version: 0.1.2rc1
 Summary: VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class.
 Home-page: https://github.com/eclipse-volttron/volttron-postgresql-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

