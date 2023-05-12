# Comparing `tmp/volttron_lib_sql_historian-0.1.1a9.tar.gz` & `tmp/volttron_lib_sql_historian-0.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_sql_historian-0.1.1a9.tar", max compression
+gzip compressed data, was "volttron_lib_sql_historian-0.2.0rc0.tar", max compression
```

## Comparing `volttron_lib_sql_historian-0.1.1a9.tar` & `volttron_lib_sql_historian-0.2.0rc0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11928 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/LICENSE
--rw-r--r--   0        0        0     3179 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/README.md
--rw-r--r--   0        0        0     1139 2023-05-12 17:02:41.333751 volttron_lib_sql_historian-0.1.1a9/pyproject.toml
--rw-r--r--   0        0        0     1134 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/src/historian/sql/__init__.py
--rw-r--r--   0        0        0    20476 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/src/historian/sql/basedb.py
--rw-r--r--   0        0        0    15683 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/src/historian/sql/historian.py
--rw-r--r--   0        0        0     1672 2023-05-12 17:01:57.952921 volttron_lib_sql_historian-0.1.1a9/src/historian/sql/sqlutils.py
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 volttron_lib_sql_historian-0.1.1a9/PKG-INFO
+-rw-r--r--   0        0        0    11928 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/LICENSE
+-rw-r--r--   0        0        0     2920 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/README.md
+-rw-r--r--   0        0        0     1225 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1134 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/__init__.py
+-rw-r--r--   0        0        0    20476 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/basedb.py
+-rw-r--r--   0        0        0    15683 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/historian.py
+-rw-r--r--   0        0        0     1672 2022-11-29 22:04:54.967989 volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/sqlutils.py
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 volttron_lib_sql_historian-0.2.0rc0/setup.py
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 volttron_lib_sql_historian-0.2.0rc0/PKG-INFO
```

### Comparing `volttron_lib_sql_historian-0.1.1a9/LICENSE` & `volttron_lib_sql_historian-0.2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.1.1a9/README.md` & `volttron_lib_sql_historian-0.2.0rc0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,34 @@
-[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
-![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
-![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
-[![pypi version](https://img.shields.io/pypi/v/volttron-lib-sql-historian.svg)](https://pypi.org/project/volttron-lib-sql-historian/)
-![Passing?](https://github.com/VOLTTRON/volttron-lib-sql-historian/actions/workflows/run-tests.yml/badge.svg)
-
-Generic SQL Historian library that can be used to implement a historian agent with a relational database backend.
-This library cannot be installed as a VOLTTRON agent as is. Only a concrete database implementation package such as
-[sqlite-historian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) that depends on this library can be
-installed as a VOLTTRON agent.
-
-## Requirements
-
- - Python >= 3.10
-
-## Installation
-
-This library can be installed using ```pip install volttron-lib-sql-historian```. However, this is not necessary. Any
-historian agent that uses this library will automatically install it as part of its installation. For example,
-installing [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) will automatically install
-volttron-lib-sql-historian
-
-## Development
-
-Please see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).
-
-Please see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)
-
-To create a new relational database based historian by extending this library, subclass
-[DBDriver](https://github.com/eclipse-volttron/volttron-lib-sql-historian/blob/develop/src/historian/sql/basedb.py#L79).
-The subclass should be in a module historian.<database_type>.<database_type>functs.py for it to be dynamically loaded
-by the base DBDriver. Please refer to [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) as
-an example
-
-# Disclaimer Notice
-
-This material was prepared as an account of work sponsored by an agency of the
-United States Government.  Neither the United States Government nor the United
-States Department of Energy, nor Battelle, nor any of their employees, nor any
-jurisdiction or organization that has cooperated in the development of these
-materials, makes any warranty, express or implied, or assumes any legal
-liability or responsibility for the accuracy, completeness, or usefulness or any
-information, apparatus, product, software, or process disclosed, or represents
-that its use would not infringe privately owned rights.
-
-Reference herein to any specific commercial product, process, or service by
-trade name, trademark, manufacturer, or otherwise does not necessarily
-constitute or imply its endorsement, recommendation, or favoring by the United
-States Government or any agency thereof, or Battelle Memorial Institute. The
-views and opinions of authors expressed herein do not necessarily state or
-reflect those of the United States Government or any agency thereof.
+# -*- coding: utf-8 -*-
+from setuptools import setup
+
+package_dir = \
+{'': 'src'}
+
+packages = \
+['historian', 'historian.sql']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['volttron-lib-base-historian>=0.2.0rc0,<0.3.0']
+
+setup_kwargs = {
+    'name': 'volttron-lib-sql-historian',
+    'version': '0.2.0rc0',
+    'description': 'A library for supporting sql based historians.',
+    'long_description': '[![pypi version](https://img.shields.io/pypi/v/volttron-lib-sql-historian.svg)](https://pypi.org/project/volttron-lib-sql-historian/)\n![Passing?](https://github.com/VOLTTRON/volttron-lib-sql-historian/actions/workflows/run-tests.yml/badge.svg)\n\nGeneric SQL Historian library that can be used to implement a historian agent with a relational database backend.\nThis library cannot be installed as a VOLTTRON agent as is. Only a concrete database implementation package such as\n[sqlite-historian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) that depends on this library can be\ninstalled as a VOLTTRON agent.\n\n## Requirements\n\n - Python >= 3.8\n\n## Installation\n\nThis library can be installed using ```pip install volttron-lib-sql-historian```. However, this is not necessary. Any\nhistorian agent that uses this library will automatically install it as part of its installation. For example,\ninstalling [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) will automatically install\nvolttron-lib-sql-historian\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\nTo create a new relational database based historian by extending this library, subclass\n[DBDriver](https://github.com/eclipse-volttron/volttron-lib-sql-historian/blob/develop/src/historian/sql/basedb.py#L79).\nThe subclass should be in a module historian.<database_type>.<database_type>functs.py for it to be dynamically loaded\nby the base DBDriver. Please refer to [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) as\nan example\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n',
+    'author': 'VOLTTRON Team',
+    'author_email': 'volttron@pnnl.gov',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/eclipse-volttron/volttron-lib-sql-historian',
+    'package_dir': package_dir,
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.8,<4.0',
+}
+
+
+setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `volttron_lib_sql_historian-0.1.1a9/pyproject.toml` & `volttron_lib_sql_historian-0.2.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [build-system]
-requires = ["poetry-core>=1.2.0"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+git-changelog = ">=0.5.0"
+httpx = ">=0.16.1"
+jinja2-cli = ">=0.7.0"
+toml = ">=0.10.2"
 
 [tool.poetry]
 name = "volttron-lib-sql-historian"
-version = "0.1.1a9"
+version = "0.2.0-rc"
 description = "A library for supporting sql based historians."
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-sql-historian"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-sql-historian"
 keywords = []
 packages = [ { include = "historian", from = "src" } ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4.0"
-volttron-lib-base-historian = "^0.2.0rc4"
+python = ">=3.8,<4.0"
+volttron-lib-base-historian = "^0.2.0rc0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.5"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
 yapf = "^0.32.0"
 toml = "^0.10.2"
 isort = "^5.10.1"
 safety = "^1.10.3"
 mypy = "^0.942"
 coverage = "^6.3.2"
 pytest-cov = "^3.0.0"
-Sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.2.0"
+Sphinx = "^4.5.0"
+sphinx-rtd-theme = "^1.0.0"
 
 [tool.yapf]
 based_on_style = "pep8"
 spaces_before_comment = 4
 column_limit = 99
 split_before_logical_operator = true
```

### Comparing `volttron_lib_sql_historian-0.1.1a9/src/historian/sql/__init__.py` & `volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.1.1a9/src/historian/sql/basedb.py` & `volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/basedb.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.1.1a9/src/historian/sql/historian.py` & `volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/historian.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.1.1a9/src/historian/sql/sqlutils.py` & `volttron_lib_sql_historian-0.2.0rc0/src/historian/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_sql_historian-0.1.1a9/PKG-INFO` & `volttron_lib_sql_historian-0.2.0rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: volttron-lib-sql-historian
-Version: 0.1.1a9
+Version: 0.2.0rc0
 Summary: A library for supporting sql based historians.
 Home-page: https://github.com/eclipse-volttron/volttron-lib-sql-historian
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: volttron-lib-base-historian (>=0.2.0rc4,<0.3.0)
+Requires-Dist: volttron-lib-base-historian (>=0.2.0rc0,<0.3.0)
 Project-URL: Repository, https://github.com/eclipse-volttron/volttron-lib-sql-historian
 Description-Content-Type: text/markdown
 
-[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://volttron.readthedocs.io/en/latest/)
-![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
-![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)
 [![pypi version](https://img.shields.io/pypi/v/volttron-lib-sql-historian.svg)](https://pypi.org/project/volttron-lib-sql-historian/)
 ![Passing?](https://github.com/VOLTTRON/volttron-lib-sql-historian/actions/workflows/run-tests.yml/badge.svg)
 
 Generic SQL Historian library that can be used to implement a historian agent with a relational database backend.
 This library cannot be installed as a VOLTTRON agent as is. Only a concrete database implementation package such as
 [sqlite-historian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) that depends on this library can be
 installed as a VOLTTRON agent.
 
 ## Requirements
 
- - Python >= 3.10
+ - Python >= 3.8
 
 ## Installation
 
 This library can be installed using ```pip install volttron-lib-sql-historian```. However, this is not necessary. Any
 historian agent that uses this library will automatically install it as part of its installation. For example,
 installing [SQLiteHistorian](https://github.com/eclipse-volttron/volttron-sqlitehistorian) will automatically install
 volttron-lib-sql-historian
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

