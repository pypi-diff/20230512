# Comparing `tmp/volttron_sqlite_historian-0.2.0rc0.tar.gz` & `tmp/volttron_sqlite_historian-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_sqlite_historian-0.2.0rc0.tar", max compression
+gzip compressed data, was "volttron_sqlite_historian-0.2.1rc0.tar", max compression
```

## Comparing `volttron_sqlite_historian-0.2.0rc0.tar` & `volttron_sqlite_historian-0.2.1rc0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11928 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/LICENSE
--rw-r--r--   0        0        0     3435 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/README.md
--rw-r--r--   0        0        0     1581 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1078 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/__init__.py
--rw-r--r--   0        0        0    30419 2022-11-29 22:09:10.366783 volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/sqlitefuncts.py
--rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.2.0rc0/setup.py
--rw-r--r--   0        0        0     4184 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 17:00:15.513400 volttron_sqlite_historian-0.2.1rc0/LICENSE
+-rw-r--r--   0        0        0     3803 2023-05-12 17:01:14.717322 volttron_sqlite_historian-0.2.1rc0/README.md
+-rw-r--r--   0        0        0     1566 2023-05-12 17:03:26.930048 volttron_sqlite_historian-0.2.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     1078 2023-05-12 17:00:15.513400 volttron_sqlite_historian-0.2.1rc0/src/historian/sqlite/__init__.py
+-rw-r--r--   0        0        0    30419 2023-05-12 17:00:15.513400 volttron_sqlite_historian-0.2.1rc0/src/historian/sqlite/sqlitefuncts.py
+-rw-r--r--   0        0        0     4502 1970-01-01 00:00:00.000000 volttron_sqlite_historian-0.2.1rc0/PKG-INFO
```

### Comparing `volttron_sqlite_historian-0.2.0rc0/LICENSE` & `volttron_sqlite_historian-0.2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.2.0rc0/README.md` & `volttron_sqlite_historian-0.2.1rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 [![Run Pytests](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml)
 [![pypi version](https://img.shields.io/pypi/v/volttron-sqlite-historian.svg)](https://pypi.org/project/volttron-sqlite-historian/)
+![Passing?](https://github.com/VOLTTRON/volttron-sqlite-historian/actions/workflows/run-tests.yml/badge.svg)
 
 VOLTTRON historian agent that stores data into a SQLite database
 
 
 ## Requirements
 
- - Python >= 3.8
+ - Python >= 3.10
 
 ## Installation
 
 1. Create and activate a virtual environment.
 
    ```shell
     python -m venv env
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/__init__.py` & `volttron_sqlite_historian-0.2.1rc0/src/historian/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.2.0rc0/src/historian/sqlite/sqlitefuncts.py` & `volttron_sqlite_historian-0.2.1rc0/src/historian/sqlite/sqlitefuncts.py`

 * *Files identical despite different names*

### Comparing `volttron_sqlite_historian-0.2.0rc0/setup.py` & `volttron_sqlite_historian-0.2.1rc0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volttron-sqlite-historian
+Version: 0.2.1rc0
+Summary: VOLTTRON historian that store data in sqlite3 database
+Home-page: https://github.com/VOLTTRON/volttron-sqlite-historian
+License: Apache-2.0
+Author: VOLTTRON Team
+Author-email: volttron@pnnl.gov
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: volttron-lib-sql-historian (>=0.1.1a8,<0.2.0)
+Project-URL: Repository, https://github.com/VOLTTRON/volttron-sqlite-historian
+Description-Content-Type: text/markdown
+
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Run Pytests](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-sqlite-historian.svg)](https://pypi.org/project/volttron-sqlite-historian/)
+![Passing?](https://github.com/VOLTTRON/volttron-sqlite-historian/actions/workflows/run-tests.yml/badge.svg)
+
+VOLTTRON historian agent that stores data into a SQLite database
+
+
+## Requirements
+
+ - Python >= 3.10
+
+## Installation
+
+1. Create and activate a virtual environment.
+
+   ```shell
+    python -m venv env
+    source env/bin/activate
+    ```
+
+2. Installing volttron-sqlite-historian requires a running volttron instance.
+
+    ```shell
+    pip install volttron
+    
+    # Start platform with output going to volttron.log
+    volttron -vv -l volttron.log &
+    ```
+
+3. Create a agent configuration file 
+   SQLite historian supports two parameters
+    
+    - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. sqlite) and params 
+                    containing the path the database file.
+    
+    - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.
+    
+    The configuration can be in a json or yaml formatted file.
+
+    Yaml Format:
+
+    ```yaml
+    connection:
+      # type should be sqlite
+      type: sqlite
+      params:
+        # Relative to the agents data directory
+        database: "data/historian.sqlite"
+    
+      tables_def:
+        # prefix for data, topics, and (in version < 4.0.0 metadata tables)
+        # default is ""
+        table_prefix: ""
+        # table name for time series data. default "data"
+        data_table: data
+        # table name for list of topics. default "topics"
+        topics_table: topics
+    ```
+    
+4. Install and start the volttron-sqlite-historian.
+
+    ```shell
+    vctl install volttron-sqlite-historian --agent-config <path to configuration> --start
+    ```
+
+5. View the status of the installed agent
+
+    ```shell
+    vctl status
+    ```
+
+## Development
+
+Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
+
+Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
+
+# Disclaimer Notice
+
+This material was prepared as an account of work sponsored by an agency of the
+United States Government.  Neither the United States Government nor the United
+States Department of Energy, nor Battelle, nor any of their employees, nor any
+jurisdiction or organization that has cooperated in the development of these
+materials, makes any warranty, express or implied, or assumes any legal
+liability or responsibility for the accuracy, completeness, or usefulness or any
+information, apparatus, product, software, or process disclosed, or represents
+that its use would not infringe privately owned rights.
+
+Reference herein to any specific commercial product, process, or service by
+trade name, trademark, manufacturer, or otherwise does not necessarily
+constitute or imply its endorsement, recommendation, or favoring by the United
+States Government or any agency thereof, or Battelle Memorial Institute. The
+views and opinions of authors expressed herein do not necessarily state or
+reflect those of the United States Government or any agency thereof.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['historian', 'historian.sqlite']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['volttron-lib-sql-historian>=0.2.0rc0,<0.3.0']
-
-entry_points = \
-{'console_scripts': ['volttron-sqlite-historian = '
-                     'historian.sql.historian:main']}
-
-setup_kwargs = {
-    'name': 'volttron-sqlite-historian',
-    'version': '0.2.0rc0',
-    'description': 'None',
-    'long_description': '[![Run Pytests](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-sqlite-historian/actions/workflows/run-test.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-sqlite-historian.svg)](https://pypi.org/project/volttron-sqlite-historian/)\n\nVOLTTRON historian agent that stores data into a SQLite database\n\n\n## Requirements\n\n - Python >= 3.8\n\n## Installation\n\n1. Create and activate a virtual environment.\n\n   ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n2. Installing volttron-sqlite-historian requires a running volttron instance.\n\n    ```shell\n    pip install volttron\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n\n3. Create a agent configuration file \n   SQLite historian supports two parameters\n    \n    - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. sqlite) and params \n                    containing the path the database file.\n    \n    - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.\n    \n    The configuration can be in a json or yaml formatted file.\n\n    Yaml Format:\n\n    ```yaml\n    connection:\n      # type should be sqlite\n      type: sqlite\n      params:\n        # Relative to the agents data directory\n        database: "data/historian.sqlite"\n    \n      tables_def:\n        # prefix for data, topics, and (in version < 4.0.0 metadata tables)\n        # default is ""\n        table_prefix: ""\n        # table name for time series data. default "data"\n        data_table: data\n        # table name for list of topics. default "topics"\n        topics_table: topics\n    ```\n    \n4. Install and start the volttron-sqlite-historian.\n\n    ```shell\n    vctl install volttron-sqlite-historian --agent-config <path to configuration> --start\n    ```\n\n5. View the status of the installed agent\n\n    ```shell\n    vctl status\n    ```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
-    'author': 'VOLTTRON Team',
-    'author_email': 'volttron@pnnl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/VOLTTRON/volttron-sqlite-historian',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

