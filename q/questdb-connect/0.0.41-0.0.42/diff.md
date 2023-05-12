# Comparing `tmp/questdb-connect-0.0.41.tar.gz` & `tmp/questdb-connect-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.41.tar", last modified: Wed May 10 09:18:08 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.42.tar", last modified: Fri May 12 10:34:20 2023, max compression
```

## Comparing `questdb-connect-0.0.41.tar` & `questdb-connect-0.0.42.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.344699 questdb-connect-0.0.41/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.41/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-10 09:18:08.344554 questdb-connect-0.0.41/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2670 2023-05-08 10:47:52.000000 questdb-connect-0.0.41/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2520 2023-05-10 09:17:08.000000 questdb-connect-0.0.41/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-10 09:18:08.344733 questdb-connect-0.0.41/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.338707 questdb-connect-0.0.41/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.341460 questdb-connect-0.0.41/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.41/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.41/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.41/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.41/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.41/src/examples/sqlalchemy_raw.py
--rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.41/src/examples/trigonometry.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.342597 questdb-connect-0.0.41/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.41/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.41/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.41/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10946 2023-05-10 09:15:20.000000 questdb-connect-0.0.41/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.41/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.343609 questdb-connect-0.0.41/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.344265 questdb-connect-0.0.41/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.41/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     4325 2023-05-10 09:15:13.000000 questdb-connect-0.0.41/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.41/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.848903 questdb-connect-0.0.42/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.42/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3442 2023-05-12 10:34:20.848765 questdb-connect-0.0.42/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2735 2023-05-10 11:01:02.000000 questdb-connect-0.0.42/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2568 2023-05-12 10:33:25.000000 questdb-connect-0.0.42/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-12 10:34:20.848940 questdb-connect-0.0.42/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.843820 questdb-connect-0.0.42/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.845886 questdb-connect-0.0.42/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.42/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.42/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2431 2023-05-10 11:39:52.000000 questdb-connect-0.0.42/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2785 2023-05-12 10:32:13.000000 questdb-connect-0.0.42/src/examples/server_utilisation.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.42/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.42/src/examples/sqlalchemy_raw.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.847016 questdb-connect-0.0.42/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-10 12:28:09.000000 questdb-connect-0.0.42/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.42/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.42/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10966 2023-05-12 10:30:30.000000 questdb-connect-0.0.42/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.42/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.847832 questdb-connect-0.0.42/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3442 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      709 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-12 10:34:20.000000 questdb-connect-0.0.42/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-12 10:34:20.848491 questdb-connect-0.0.42/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.42/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2563 2023-05-12 10:31:23.000000 questdb-connect-0.0.42/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.42/tests/test_types.py
```

### Comparing `questdb-connect-0.0.41/LICENSE` & `questdb-connect-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/PKG-INFO` & `questdb-connect-0.0.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.41
+Version: 0.0.42
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -96,8 +96,8 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository.
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
```

### Comparing `questdb-connect-0.0.41/README.md` & `questdb-connect-0.0.42/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository.
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
```

### Comparing `questdb-connect-0.0.41/pyproject.toml` & `questdb-connect-0.0.42/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.41"
+version = "0.0.42"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
@@ -77,7 +77,8 @@
 
 [tool.ruff.per-file-ignores]
 "tests/test_dialect.py" = ["S101"]
 "tests/test_types.py" = ["S101"]
 "tests/test_superset.py" = ["S101"]
 "tests/conftest.py" = ["S608"]
 "src/examples/sqlalchemy_raw.py" = ["S608"]
+"src/examples/server_utilisation.py" = ["S311"]
```

### Comparing `questdb-connect-0.0.41/src/examples/__init__.py` & `questdb-connect-0.0.42/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/examples/hello_world.py` & `questdb-connect-0.0.42/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.42/src/examples/psycopg2_connect.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 
 """
-This code makes use of connects to a running QuestDB displays information about the
-tables and partitions in the database. It uses two SQL statements to
-retrieve this information: "tables()" and "table_partitions()". The output
+This code connects to a running QuestDB instance and displays information
+about the tables and partitions in the database. It uses two SQL statements
+to retrieve this information: "tables()" and "table_partitions()". The output
 is formatted and printed to the console.
-
-
 """
 import json
 
 from questdb_connect import connect
 
 from examples import CONNECTION_ATTRS
```

### Comparing `questdb-connect-0.0.41/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.42/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.42/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/examples/trigonometry.py` & `questdb-connect-0.0.42/src/examples/server_utilisation.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,67 +17,87 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 import datetime
-import math
+import enum
 import os
+import random
+import time
 
 os.environ.setdefault('SQLALCHEMY_SILENCE_UBER_WARNING', '1')
 
-import time
-
 import questdb_connect.dialect as qdbc
-from sqlalchemy import Column, MetaData, text
+from sqlalchemy import Column, MetaData, create_engine, insert
 from sqlalchemy.orm import Session, declarative_base
 
-from examples import CONNECTION_ATTRS
+
+class BaseEnum(enum.Enum):
+    @classmethod
+    def rand(cls):
+        return cls._value2member_map_[random.randint(0, len(cls._member_map_) - 1)]
+
+
+class Nodes(BaseEnum):
+    NODE0 = 0
+    NODE1 = 1
+
+
+class Metrics(BaseEnum):
+    CPU = 0
+    RAM = 1
+    HDD0 = 2
+    HDD1 = 3
+    NETWORK = 4
+
 
 Base = declarative_base(metadata=MetaData())
 
 
-class Trigonometry(Base):
-    __tablename__ = 'trigonometry'
-    __table_args__ = (qdbc.QDBTableEngine('trigonometry', 'ts'),)
-    angle_dec = Column(qdbc.Double)
-    angle_rad = Column(qdbc.Double)
-    sine = Column(qdbc.Double)
-    cosine = Column(qdbc.Double)
-    tangent = Column(qdbc.Double)
+class NodeMetrics(Base):
+    __tablename__ = 'node_metrics'
+    __table_args__ = (qdbc.QDBTableEngine(
+        'node_metrics',
+        'ts',
+        qdbc.PartitionBy.HOUR,
+        is_wal=True),)
+    source = Column(qdbc.Symbol)  # Nodes
+    attr_name = Column(qdbc.Symbol)  # Metrics
+    attr_value = Column(qdbc.Double)
     ts = Column(qdbc.Timestamp, primary_key=True)
 
 
 def main():
-    engine = qdbc.create_engine(**CONNECTION_ATTRS)
+    end_time = time.time() + 60.0
+    engine = create_engine('questdb://localhost:8812/main')
+    session = Session(engine)
+    max_batch_size = 3000
     try:
+        Base.metadata.drop_all(engine)
         Base.metadata.create_all(engine)
-        with Session(engine) as session:
-            now = datetime.datetime.utcnow
-            for angle_dec in range(0, 361):
-                angle_rad = math.radians(angle_dec)
-                session.add(Trigonometry(
-                    angle_dec=angle_dec,
-                    angle_rad=angle_rad,
-                    sine=math.sin(angle_rad),
-                    cosine=math.cos(angle_rad),
-                    tangent=math.tan(angle_rad),
-                    ts=now()))
-                time.sleep(0.0002)
+        batch_size = 0
+        while time.time() < end_time:
+            session.add(
+                NodeMetrics(
+                    source=Nodes.rand().name,
+                    attr_name=Metrics.rand().name,
+                    attr_value=random.random() * 100.0,
+                    ts=datetime.datetime.utcnow()
+                )
+            )
+            batch_size += 1
+            if batch_size > max_batch_size:
+                session.commit()
+                batch_size = 0
+        if batch_size > 0:
             session.commit()
-
-            columns = [col.name for col in Trigonometry.__table__.columns]
-            while True:
-                rs = session.execute(text(Trigonometry.__tablename__))
-                if rs.rowcount:
-                    print(f'rows: {rs.rowcount}')
-                    for row in rs:
-                        print(dict(zip(columns, map(str, row))))
-                    break
     finally:
+        if session:
+            session.close()
         if engine:
             engine.dispose()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `questdb-connect-0.0.41/src/questdb_connect/__init__.py` & `questdb-connect-0.0.42/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/questdb_connect/dialect.py` & `questdb-connect-0.0.42/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/questdb_connect/function_names.py` & `questdb-connect-0.0.42/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.42/src/questdb_connect/superset_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,22 +122,21 @@
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
             remove_public_schema(clause)
         return text(remove_public_schema(clause))
 
     @classmethod
-    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
-        """Generate a tuple of supported time grains.
-        :return: All time grains supported by the engine
+    def get_time_grain_expressions(cls) -> Dict[Optional[str], str]:
+        """Return a dict of all supported time grains including any
+        potential added grains but excluding any potentially disabled
+        grains in the config file.
+        :return: All time grain expressions supported by the engine
         """
-        return tuple(
-            TimeGrain(duration, duration, func, duration)
-            for duration, func in cls._time_grain_expressions.copy().items()
-        )
+        return cls._time_grain_expressions
 
     @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
```

### Comparing `questdb-connect-0.0.41/src/questdb_connect/types.py` & `questdb-connect-0.0.42/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.42/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.41
+Version: 0.0.42
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -96,8 +96,8 @@
 if __name__ == '__main__':
     main()
 ```
 
 ## Contributing
 
 This package is open-source, contributions are welcome. If you find a bug or would like to request a feature,
-please open an issue on the GitHub repository.
+please open an issue on the GitHub repository. Have a look at the instructions for [developers](DEVELOPERS.md).
```

### Comparing `questdb-connect-0.0.41/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.42/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 src/examples/__init__.py
 src/examples/hello_world.py
 src/examples/psycopg2_connect.py
+src/examples/server_utilisation.py
 src/examples/sqlalchemy_orm.py
 src/examples/sqlalchemy_raw.py
-src/examples/trigonometry.py
 src/questdb_connect/__init__.py
 src/questdb_connect/dialect.py
 src/questdb_connect/function_names.py
 src/questdb_connect/superset_engine.py
 src/questdb_connect/types.py
 src/questdb_connect.egg-info/PKG-INFO
 src/questdb_connect.egg-info/SOURCES.txt
```

### Comparing `questdb-connect-0.0.41/tests/test_dialect.py` & `questdb-connect-0.0.42/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.41/tests/test_types.py` & `questdb-connect-0.0.42/tests/test_types.py`

 * *Files identical despite different names*

