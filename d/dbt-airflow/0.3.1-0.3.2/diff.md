# Comparing `tmp/dbt_airflow-0.3.1.tar.gz` & `tmp/dbt_airflow-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_airflow-0.3.1.tar", max compression
+gzip compressed data, was "dbt_airflow-0.3.2.tar", max compression
```

## Comparing `dbt_airflow-0.3.1.tar` & `dbt_airflow-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     8321 2023-04-28 13:52:27.117215 dbt_airflow-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 13:52:27.117215 dbt_airflow-0.3.1/dbt_airflow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/__init__.py
--rw-r--r--   0        0        0     2827 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/operators.py
--rw-r--r--   0        0        0     3839 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/task.py
--rw-r--r--   0        0        0     7996 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/task_builder.py
--rw-r--r--   0        0        0     2560 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/task_group.py
--rw-r--r--   0        0        0     1739 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/core/task_list.py
--rw-r--r--   0        0        0        0 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/domain/__init__.py
--rw-r--r--   0        0        0      702 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/parser/__init__.py
--rw-r--r--   0        0        0     1948 2023-04-28 13:52:27.121215 dbt_airflow-0.3.1/dbt_airflow/parser/dbt.py
--rw-r--r--   0        0        0     1169 2023-04-28 13:52:27.137215 dbt_airflow-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9149 1970-01-01 00:00:00.000000 dbt_airflow-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     8768 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/__init__.py
+-rw-r--r--   0        0        0     2827 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/operators.py
+-rw-r--r--   0        0        0     3839 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/task.py
+-rw-r--r--   0        0        0     7996 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/task_builder.py
+-rw-r--r--   0        0        0     2560 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/task_group.py
+-rw-r--r--   0        0        0     1739 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/core/task_list.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/domain/__init__.py
+-rw-r--r--   0        0        0      702 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-12 10:55:52.947380 dbt_airflow-0.3.2/dbt_airflow/parser/__init__.py
+-rw-r--r--   0        0        0     2120 2023-05-12 10:55:52.951380 dbt_airflow-0.3.2/dbt_airflow/parser/dbt.py
+-rw-r--r--   0        0        0     1169 2023-05-12 10:55:52.955380 dbt_airflow-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9596 1970-01-01 00:00:00.000000 dbt_airflow-0.3.2/PKG-INFO
```

### Comparing `dbt_airflow-0.3.1/README.md` & `dbt_airflow-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+![deploy](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/deploy.yml/badge.svg?branch=main)
+![docs](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/docs.yml/badge.svg?branch=main)
+![main](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/main.yml/badge.svg?branch=main)
+![validate_pull_request](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/validate_pull_request.yml/badge.svg?branch=main)
+
 # dbt-airflow
 A Python package that helps Data and Analytics engineers render dbt projects in Apache Airflow DAGs such that
 models, seeds, snapshots and tests are represented by individual Airflow Task.
 
 `dbt` is a command-line tool that enables data teams build, maintain and test data models in a scalable fashion. The 
 biggest challenge though is how to embed `dbt` in modern data workflows and infrastructure. dbt CLI is indeed a powerful
 tool, but if used as is, it will create silos in the way an organisation manages its data. Every contributor is able to
```

### Comparing `dbt_airflow-0.3.1/dbt_airflow/core/operators.py` & `dbt_airflow-0.3.2/dbt_airflow/core/operators.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/core/task.py` & `dbt_airflow-0.3.2/dbt_airflow/core/task.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/core/task_builder.py` & `dbt_airflow-0.3.2/dbt_airflow/core/task_builder.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/core/task_group.py` & `dbt_airflow-0.3.2/dbt_airflow/core/task_group.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/core/task_list.py` & `dbt_airflow-0.3.2/dbt_airflow/core/task_list.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/exceptions.py` & `dbt_airflow-0.3.2/dbt_airflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_airflow-0.3.1/dbt_airflow/parser/dbt.py` & `dbt_airflow-0.3.2/dbt_airflow/parser/dbt.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 class DbtResourceType(str, Enum):
     model = 'model'
     test = 'test'
     snapshot = 'snapshot'
     seed = 'seed'
 
+    # dbt resource types we are not interested in, but we still need them in order for
+    # dbt-airflow to be able to parse the manifest file
+    operation = 'operation'
+
 
 class NodeDeps(BaseModel):
     nodes: List[str]
 
     def __getitem__(self, item):
         return getattr(self, item)
```

### Comparing `dbt_airflow-0.3.1/pyproject.toml` & `dbt_airflow-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-airflow"
-version = "0.3.1"
+version = "0.3.2"
 description = "A Python package that creates fine-grained Airflow tasks for dbt"
 repository = "https://github.com/gmyrianthous/dbt-airflow"
 authors = ["Giorgos Myrianthous <giorgos.myrianthous@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dbt_airflow" }]
 
@@ -18,15 +18,15 @@
 pytest = ">=7.1,<8"
 commitizen = "^2.40.0"
 mkdocs-material = "^8.2"
 mkdocstrings-python = "^0.8.2"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.1"
+version = "0.3.2"
 version_files = [
     "pyproject.toml:^version"
 ]
 update_changelog_on_bump = true
 style = [
     ["qmark", "fg:#ff9d00 bold"],
     ["question", "bold"],
```

### Comparing `dbt_airflow-0.3.1/PKG-INFO` & `dbt_airflow-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-airflow
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python package that creates fine-grained Airflow tasks for dbt
 Home-page: https://github.com/gmyrianthous/dbt-airflow
 License: MIT
 Author: Giorgos Myrianthous
 Author-email: giorgos.myrianthous@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: apache-airflow (>=2.0.0,<3)
 Requires-Dist: dbt-core (>=1.2.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/gmyrianthous/dbt-airflow
 Description-Content-Type: text/markdown
 
+![deploy](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/deploy.yml/badge.svg?branch=main)
+![docs](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/docs.yml/badge.svg?branch=main)
+![main](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/main.yml/badge.svg?branch=main)
+![validate_pull_request](https://github.com/gmyrianthous/dbt-airflow/actions/workflows/validate_pull_request.yml/badge.svg?branch=main)
+
 # dbt-airflow
 A Python package that helps Data and Analytics engineers render dbt projects in Apache Airflow DAGs such that
 models, seeds, snapshots and tests are represented by individual Airflow Task.
 
 `dbt` is a command-line tool that enables data teams build, maintain and test data models in a scalable fashion. The 
 biggest challenge though is how to embed `dbt` in modern data workflows and infrastructure. dbt CLI is indeed a powerful
 tool, but if used as is, it will create silos in the way an organisation manages its data. Every contributor is able to
```

