# Comparing `tmp/volttron_postgresql_historian-0.1.1a4.tar.gz` & `tmp/volttron_postgresql_historian-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_postgresql_historian-0.1.1a4.tar", max compression
+gzip compressed data, was "volttron_postgresql_historian-0.1.2rc0.tar", max compression
```

## Comparing `volttron_postgresql_historian-0.1.1a4.tar` & `volttron_postgresql_historian-0.1.2rc0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11928 2023-05-12 20:42:39.441441 volttron_postgresql_historian-0.1.1a4/LICENSE
--rwxr-xr-x   0        0        0     9154 2023-05-12 20:42:39.441441 volttron_postgresql_historian-0.1.1a4/README.md
--rw-r--r--   0        0        0     1373 2023-05-12 20:44:41.653945 volttron_postgresql_historian-0.1.1a4/pyproject.toml
--rw-r--r--   0        0        0     1082 2023-05-12 20:42:39.441441 volttron_postgresql_historian-0.1.1a4/src/historian/postgresql/__init__.py
--rw-r--r--   0        0        0    18297 2023-05-12 20:42:39.441441 volttron_postgresql_historian-0.1.1a4/src/historian/postgresql/postgresqlfuncts.py
--rw-r--r--   0        0        0    10469 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.1a4/setup.py
--rw-r--r--   0        0        0     9976 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.1a4/PKG-INFO
+-rw-r--r--   0        0        0    11928 2023-05-12 20:43:46.632365 volttron_postgresql_historian-0.1.2rc0/LICENSE
+-rwxr-xr-x   0        0        0     9154 2023-05-12 20:44:41.469448 volttron_postgresql_historian-0.1.2rc0/README.md
+-rw-r--r--   0        0        0     1400 2023-05-12 20:46:59.159836 volttron_postgresql_historian-0.1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-05-12 20:43:46.632365 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-12 20:44:49.841596 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    16058 2023-05-12 20:44:49.841596 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__pycache__/postgresqlfuncts.cpython-310.pyc
+-rw-r--r--   0        0        0    18297 2023-05-12 20:44:41.469448 volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/postgresqlfuncts.py
+-rw-r--r--   0        0        0     9977 1970-01-01 00:00:00.000000 volttron_postgresql_historian-0.1.2rc0/PKG-INFO
```

### Comparing `volttron_postgresql_historian-0.1.1a4/LICENSE` & `volttron_postgresql_historian-0.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.1a4/README.md` & `volttron_postgresql_historian-0.1.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.1a4/pyproject.toml` & `volttron_postgresql_historian-0.1.2rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volttron-postgresql-historian"
-version = "0.1.1a4"
+version = "0.1.2rc0"
 description = "VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-postgresql-historian"
 keywords = []
@@ -26,14 +26,15 @@
 safety = "^1.10.3"
 mypy = "^0.942"
 coverage = "^6.3.2"
 pytest-cov = "^3.0.0"
 Sphinx = "^6.0.0"
 sphinx-rtd-theme = "^1.2.0"
 volttron-testing = "^0.4.0rc3"
+pytest-timeout = "^2.1.0"
 
 [tool.yapfignore]
 ignore_patterns = [
     ".venv/**",
     ".pytest_cache/**",
     "dist/**",
     "docs/**"
```

### Comparing `volttron_postgresql_historian-0.1.1a4/src/historian/postgresql/__init__.py` & `volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.1a4/src/historian/postgresql/postgresqlfuncts.py` & `volttron_postgresql_historian-0.1.2rc0/src/historian/postgresql/postgresqlfuncts.py`

 * *Files identical despite different names*

### Comparing `volttron_postgresql_historian-0.1.1a4/setup.py` & `volttron_postgresql_historian-0.1.2rc0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,248 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volttron-postgresql-historian
+Version: 0.1.2rc0
+Summary: VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class.
+Home-page: https://github.com/eclipse-volttron/volttron-postgresql-historian
+License: Apache-2.0
+Author: VOLTTRON Team
+Author-email: volttron@pnnl.gov
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
+Requires-Dist: volttron-lib-sql-historian (>=0.1.1a8,<0.2.0)
+Project-URL: Repository, https://github.com/eclipse-volttron/volttron-postgresql-historian
+Description-Content-Type: text/markdown
+
+[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
+![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
+![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
+[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml)
+[![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)
+![Passing?](https://github.com/VOLTTRON/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)
+
+VOLTTRON historian agent that stores data into a PostgreSQL database
+
+### Installation notes
+
+1.  The PostgreSQL database driver supports recent PostgreSQL versions.
+    It was tested on 10.x, but should work with 9.x and 11.x.
+2.  The user must have SELECT, INSERT, and UPDATE privileges on
+    historian tables.
+3.  The tables in the database are created as part of the execution of
+    the SQLHistorianAgent, but this will fail if the database user does
+    not have CREATE privileges.
+4.  Care must be exercised when using multiple historians with the same
+    database. This configuration may be used only if there is no overlap
+    in the topics handled by each instance. Otherwise, duplicate topic
+    IDs may be created, producing strange results.
+
+
+### Configuration
+
+PostgreSQL historian supports two configuration parameters
+    
+   - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. postgresql) and params containing the database access details
+   - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.
+    
+The configuration can be in a json or yaml formatted file. The following examples show minimal connection 
+configurations for a psycopg2-based historian. Other options are available and are [documented here](https://www.psycopg.org/docs/module.html#psycopg2.connect) 
+**Not all parameters have been tested,  use at your own risk**.
+
+#### Local PostgreSQL Database
+
+The following snippet demonstrates how to configure the historian to use a PostgreSQL database on the local system that
+is configured to use Unix domain sockets. The user executing volttron must have appropriate privileges.
+
+
+##### Yaml Format:
+```yaml
+    connection:
+          # type should be postgresql
+          type: postgresql
+          params:
+            # Relative to the agents data directory
+            dbname: "volttron"
+        
+    tables_def:
+        # prefix for data, topics, and (in version < 4.0.0 metadata tables)
+        # default is ""
+        table_prefix: ""
+        # table name for time series data. default "data"
+        data_table: data
+        # table name for list of topics. default "topics"
+        topics_table: topics
+ ```
+
+##### JSON format:
+```json
+    {
+        "connection": {
+            "type": "postgresql", 
+            "params": { "dbname": "volttron" }
+        }
+    }
+```
+
+#### Remote PostgreSQL Database
+
+The following snippet demonstrates how to configure the historian to use a remote PostgreSQL database.
+```json
+    {
+        "connection": {
+            "type": "postgresql", 
+            "params": { 
+                "dbname": "volttron", 
+                "host": "historian.example.com", 
+                "port": 5432, 
+                "user": "volttron", 
+                "password": "secret" }
+        }
+    }
+```
+
+#### TimescaleDB Support
+
+Both of the above PostgreSQL connection types can make use of TimescaleDB\'s high performance Hypertable backend for 
+the primary timeseries table. The agent assumes you have completed the TimescaleDB installation and setup the 
+database by following the instructions here: <https://docs.timescale.com/latest/getting-started/setup> To use, simply
+add \'timescale_dialect: true\' to the connection params in the agent config as below
+
+```json
+    {
+        "connection": {
+            "type": "postgresql", 
+            "params": { 
+                "dbname": "volttron", 
+                "host": "historian.example.com", 
+                "port": 5432, 
+                "user": "volttron", 
+                "password": "secret" ,
+                "timescale_dialect": true }
+        }
+
+    }
+```
+
+## Requirements
+
+ - Python >= 3.10
+ - psycopg2 library
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
+2. Installing volttron-postgresql-historian requires a running volttron instance and the psycopg2 library 
+
+    ```shell
+    pip install volttron
+    pip install psycopg2-binary
+    
+    # Start platform with output going to volttron.log
+    volttron -vv -l volttron.log &
+    ```
+3. Setup database
+   
+   If this is not a development environment we highly recommend that you create the database and database tables using
+   a user with appropriate permissions. This way the database user used by the historian need not have CREATE privileges
+   Postgres historian expects two tables 
+   a. A topics tables that stores the list of unique topics and its metadata. The default name is "topics". If you use 
+      a different name please specify it as part of "tables_def" configuration parameter in agent config. See [example configuration](#yaml-format)
+   b. A data table that stores the timeseries data and refers to the topic table using a topic id. The default name is 
+      "data". If you use a different name please specify it as part of "tables_def" configuration parameter in 
+      agent config. See [example configuration](#yaml-format)
+
+   Below are the sql statements to create database and tables
+   <u>Create Database</u>
+    ```
+       CREATE DATABASE volttron
+    ```
+   <u>TOPICS tables:</u>
+    ```
+        CREATE TABLE IF NOT EXISTS topics (
+            topic_id SERIAL PRIMARY KEY NOT NULL, 
+            topic_name VARCHAR(512) NOT NULL, 
+            metadata TEXT, 
+            UNIQUE (topic_name)
+       )
+    ```
+    <u>DATA table:</u>
+    ```
+       CREATE TABLE IF NOT EXISTS data (
+           ts TIMESTAMP NOT NULL, 
+           topic_id INTEGER NOT NULL, 
+           value_string TEXT NOT NULL, 
+           UNIQUE (topic_id, ts)
+       )
+    ```
+     <u>Optional timescale hypertable</u>
+    ```
+       SELECT create_hypertable(data, 'ts', if_not_exists => true)
+    ```
+     <u>Create index to speed up data access</u>
+       If using hypertables:
+    ```
+        CREATE INDEX IF NOT EXISTS idx_data ON data (topic_id, ts)
+    ```
+      If not using hypertables:
+    ```
+        CREATE INDEX IF NOT EXISTS idx_data ON data (ts ASC)
+    ```
+    <u>Provide correct user permissions for database user to be used by historian agent</u>
+    ```
+        CREATE USER <some username> with encrypted password <some password>
+        GRANT SELECT, INSERT, UPDATE on database <historian db name> to <username used above>
+    ``` 
+    **NOTE**
+    For development environments, you can create a test database and test user, grant all privileges on that test 
+    database to the test user and let the historian create tables and indexes at startup. We do not recommend this for 
+    production environments
+
+4. Create an agent configuration file 
+
+    Create an agent configuration with appropriate connection parameters as described in the [Configurations section](#Configuration)
+
+5. Install and start the volttron-postgresql-historian.
+
+    ```shell
+    vctl install volttron-postgresql-historian --agent-config <path to configuration> --start
+    ```
+
+6. View the status of the installed agent
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
-['historian', 'historian.postgresql']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['psycopg2-binary>=2.9.5,<3.0.0', 'volttron-lib-sql-historian>=0.1.1a8,<0.2.0']
-
-entry_points = \
-{'console_scripts': ['volttron-postgresql-historian = '
-                     'historian.sql.historian:main']}
-
-setup_kwargs = {
-    'name': 'volttron-postgresql-historian',
-    'version': '0.1.1a4',
-    'description': 'VOLTTRON historian agent that stores data in a PostgreSQL database. It extends the SQLHistorian class.',
-    'long_description': '[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-postgresql-historian/actions/workflows/run-test.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-postgresql-historian.svg)](https://pypi.org/project/volttron-postgresql-historian/)\n![Passing?](https://github.com/VOLTTRON/volttron-postgresql-historian/actions/workflows/run-tests.yml/badge.svg)\n\nVOLTTRON historian agent that stores data into a PostgreSQL database\n\n### Installation notes\n\n1.  The PostgreSQL database driver supports recent PostgreSQL versions.\n    It was tested on 10.x, but should work with 9.x and 11.x.\n2.  The user must have SELECT, INSERT, and UPDATE privileges on\n    historian tables.\n3.  The tables in the database are created as part of the execution of\n    the SQLHistorianAgent, but this will fail if the database user does\n    not have CREATE privileges.\n4.  Care must be exercised when using multiple historians with the same\n    database. This configuration may be used only if there is no overlap\n    in the topics handled by each instance. Otherwise, duplicate topic\n    IDs may be created, producing strange results.\n\n\n### Configuration\n\nPostgreSQL historian supports two configuration parameters\n    \n   - connection -  This is a mandatory parameter with type indicating the type of sql historian (i.e. postgresql) and params containing the database access details\n   - tables_def - Optional parameter to provide custom table names for topics, data, and metadata.\n    \nThe configuration can be in a json or yaml formatted file. The following examples show minimal connection \nconfigurations for a psycopg2-based historian. Other options are available and are [documented here](https://www.psycopg.org/docs/module.html#psycopg2.connect) \n**Not all parameters have been tested,  use at your own risk**.\n\n#### Local PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a PostgreSQL database on the local system that\nis configured to use Unix domain sockets. The user executing volttron must have appropriate privileges.\n\n\n##### Yaml Format:\n```yaml\n    connection:\n          # type should be postgresql\n          type: postgresql\n          params:\n            # Relative to the agents data directory\n            dbname: "volttron"\n        \n    tables_def:\n        # prefix for data, topics, and (in version < 4.0.0 metadata tables)\n        # default is ""\n        table_prefix: ""\n        # table name for time series data. default "data"\n        data_table: data\n        # table name for list of topics. default "topics"\n        topics_table: topics\n ```\n\n##### JSON format:\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { "dbname": "volttron" }\n        }\n    }\n```\n\n#### Remote PostgreSQL Database\n\nThe following snippet demonstrates how to configure the historian to use a remote PostgreSQL database.\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" }\n        }\n    }\n```\n\n#### TimescaleDB Support\n\nBoth of the above PostgreSQL connection types can make use of TimescaleDB\\\'s high performance Hypertable backend for \nthe primary timeseries table. The agent assumes you have completed the TimescaleDB installation and setup the \ndatabase by following the instructions here: <https://docs.timescale.com/latest/getting-started/setup> To use, simply\nadd \\\'timescale_dialect: true\\\' to the connection params in the agent config as below\n\n```json\n    {\n        "connection": {\n            "type": "postgresql", \n            "params": { \n                "dbname": "volttron", \n                "host": "historian.example.com", \n                "port": 5432, \n                "user": "volttron", \n                "password": "secret" ,\n                "timescale_dialect": true }\n        }\n\n    }\n```\n\n## Requirements\n\n - Python >= 3.10\n - psycopg2 library\n\n## Installation\n\n1. Create and activate a virtual environment.\n\n   ```shell\n    python -m venv env\n    source env/bin/activate\n    ```\n\n2. Installing volttron-postgresql-historian requires a running volttron instance and the psycopg2 library \n\n    ```shell\n    pip install volttron\n    pip install psycopg2-binary\n    \n    # Start platform with output going to volttron.log\n    volttron -vv -l volttron.log &\n    ```\n3. Setup database\n   \n   If this is not a development environment we highly recommend that you create the database and database tables using\n   a user with appropriate permissions. This way the database user used by the historian need not have CREATE privileges\n   Postgres historian expects two tables \n   a. A topics tables that stores the list of unique topics and its metadata. The default name is "topics". If you use \n      a different name please specify it as part of "tables_def" configuration parameter in agent config. See [example configuration](#yaml-format)\n   b. A data table that stores the timeseries data and refers to the topic table using a topic id. The default name is \n      "data". If you use a different name please specify it as part of "tables_def" configuration parameter in \n      agent config. See [example configuration](#yaml-format)\n\n   Below are the sql statements to create database and tables\n   <u>Create Database</u>\n    ```\n       CREATE DATABASE volttron\n    ```\n   <u>TOPICS tables:</u>\n    ```\n        CREATE TABLE IF NOT EXISTS topics (\n            topic_id SERIAL PRIMARY KEY NOT NULL, \n            topic_name VARCHAR(512) NOT NULL, \n            metadata TEXT, \n            UNIQUE (topic_name)\n       )\n    ```\n    <u>DATA table:</u>\n    ```\n       CREATE TABLE IF NOT EXISTS data (\n           ts TIMESTAMP NOT NULL, \n           topic_id INTEGER NOT NULL, \n           value_string TEXT NOT NULL, \n           UNIQUE (topic_id, ts)\n       )\n    ```\n     <u>Optional timescale hypertable</u>\n    ```\n       SELECT create_hypertable(data, \'ts\', if_not_exists => true)\n    ```\n     <u>Create index to speed up data access</u>\n       If using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (topic_id, ts)\n    ```\n      If not using hypertables:\n    ```\n        CREATE INDEX IF NOT EXISTS idx_data ON data (ts ASC)\n    ```\n    <u>Provide correct user permissions for database user to be used by historian agent</u>\n    ```\n        CREATE USER <some username> with encrypted password <some password>\n        GRANT SELECT, INSERT, UPDATE on database <historian db name> to <username used above>\n    ``` \n    **NOTE**\n    For development environments, you can create a test database and test user, grant all privileges on that test \n    database to the test user and let the historian create tables and indexes at startup. We do not recommend this for \n    production environments\n\n4. Create an agent configuration file \n\n    Create an agent configuration with appropriate connection parameters as described in the [Configurations section](#Configuration)\n\n5. Install and start the volttron-postgresql-historian.\n\n    ```shell\n    vctl install volttron-postgresql-historian --agent-config <path to configuration> --start\n    ```\n\n6. View the status of the installed agent\n\n    ```shell\n    vctl status\n    ```\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
-    'author': 'VOLTTRON Team',
-    'author_email': 'volttron@pnnl.gov',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/eclipse-volttron/volttron-postgresql-historian',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

