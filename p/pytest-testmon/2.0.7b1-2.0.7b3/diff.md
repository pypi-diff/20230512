# Comparing `tmp/pytest-testmon-2.0.7b1.tar.gz` & `tmp/pytest-testmon-2.0.7b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testmon-2.0.7b1.tar", last modified: Tue May  2 07:59:57 2023, max compression
+gzip compressed data, was "pytest-testmon-2.0.7b3.tar", last modified: Fri May 12 12:45:43 2023, max compression
```

## Comparing `pytest-testmon-2.0.7b1.tar` & `pytest-testmon-2.0.7b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/
--rw-r--r--   0 poko      (1000) poko      (1000)    34633 2023-01-12 14:59:27.000000 pytest-testmon-2.0.7b1/LICENSE
--rw-r--r--   0 poko      (1000) poko      (1000)       74 2023-03-09 09:22:22.000000 pytest-testmon-2.0.7b1/MANIFEST.in
--rw-r--r--   0 poko      (1000) poko      (1000)     2431 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/PKG-INFO
--rw-r--r--   0 poko      (1000) poko      (1000)     1208 2023-04-27 09:24:29.000000 pytest-testmon-2.0.7b1/README.md
--rw-r--r--   0 poko      (1000) poko      (1000)     1619 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/pyproject.toml
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.171580 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/
--rw-r--r--   0 poko      (1000) poko      (1000)     2431 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/PKG-INFO
--rw-r--r--   0 poko      (1000) poko      (1000)      463 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/SOURCES.txt
--rw-r--r--   0 poko      (1000) poko      (1000)        1 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/dependency_links.txt
--rw-r--r--   0 poko      (1000) poko      (1000)       51 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/entry_points.txt
--rw-r--r--   0 poko      (1000) poko      (1000)       28 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/requires.txt
--rw-r--r--   0 poko      (1000) poko      (1000)        8 2023-05-02 07:59:57.000000 pytest-testmon-2.0.7b1/pytest_testmon.egg-info/top_level.txt
--rw-r--r--   0 poko      (1000) poko      (1000)     1219 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/setup.cfg
--rw-r--r--   0 poko      (1000) poko      (1000)       69 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/setup.py
-drwxr-xr-x   0 poko      (1000) poko      (1000)        0 2023-05-02 07:59:57.175580 pytest-testmon-2.0.7b1/testmon/
--rw-r--r--   0 poko      (1000) poko      (1000)       46 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/__init__.py
--rw-r--r--   0 poko      (1000) poko      (1000)     1495 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/common.py
--rw-r--r--   0 poko      (1000) poko      (1000)     3786 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/configure.py
--rw-r--r--   0 poko      (1000) poko      (1000)    22138 2023-05-02 07:51:35.000000 pytest-testmon-2.0.7b1/testmon/db.py
--rw-r--r--   0 poko      (1000) poko      (1000)     7969 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/process_code.py
--rw-r--r--   0 poko      (1000) poko      (1000)    17066 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/pytest_testmon.py
--rw-r--r--   0 poko      (1000) poko      (1000)    19048 2023-05-02 07:51:34.000000 pytest-testmon-2.0.7b1/testmon/testmon_core.py
--rw-r--r--   0 poko      (1000) poko      (1000)     1232 2023-01-12 14:59:27.000000 pytest-testmon-2.0.7b1/testmon/tox_testmon.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.294234 pytest-testmon-2.0.7b3/
+-rw-r--r--   0 tibor      (502) staff       (20)    34633 2023-01-17 15:34:55.000000 pytest-testmon-2.0.7b3/LICENSE
+-rw-r--r--   0 tibor      (502) staff       (20)       74 2023-05-02 14:55:45.000000 pytest-testmon-2.0.7b3/MANIFEST.in
+-rw-r--r--   0 tibor      (502) staff       (20)     2431 2023-05-12 12:45:43.294311 pytest-testmon-2.0.7b3/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)     1208 2023-05-02 14:55:45.000000 pytest-testmon-2.0.7b3/README.md
+-rw-r--r--   0 tibor      (502) staff       (20)     1619 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/pyproject.toml
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.292067 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/
+-rw-r--r--   0 tibor      (502) staff       (20)     2431 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/PKG-INFO
+-rw-r--r--   0 tibor      (502) staff       (20)      463 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/SOURCES.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        1 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/dependency_links.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       51 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/entry_points.txt
+-rw-r--r--   0 tibor      (502) staff       (20)       28 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/requires.txt
+-rw-r--r--   0 tibor      (502) staff       (20)        8 2023-05-12 12:45:43.000000 pytest-testmon-2.0.7b3/pytest_testmon.egg-info/top_level.txt
+-rw-r--r--   0 tibor      (502) staff       (20)     1219 2023-05-12 12:45:43.294598 pytest-testmon-2.0.7b3/setup.cfg
+-rw-r--r--   0 tibor      (502) staff       (20)       69 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/setup.py
+drwxr-xr-x   0 tibor      (502) staff       (20)        0 2023-05-12 12:45:43.294012 pytest-testmon-2.0.7b3/testmon/
+-rw-r--r--   0 tibor      (502) staff       (20)       46 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/__init__.py
+-rw-r--r--   0 tibor      (502) staff       (20)     2125 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/common.py
+-rw-r--r--   0 tibor      (502) staff       (20)     3786 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/configure.py
+-rw-r--r--   0 tibor      (502) staff       (20)    22743 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/db.py
+-rw-r--r--   0 tibor      (502) staff       (20)     8052 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/process_code.py
+-rw-r--r--   0 tibor      (502) staff       (20)    16979 2023-05-12 12:40:21.000000 pytest-testmon-2.0.7b3/testmon/pytest_testmon.py
+-rw-r--r--   0 tibor      (502) staff       (20)    19133 2023-05-12 12:40:22.000000 pytest-testmon-2.0.7b3/testmon/testmon_core.py
+-rw-r--r--   0 tibor      (502) staff       (20)     1232 2023-01-18 05:16:27.000000 pytest-testmon-2.0.7b3/testmon/tox_testmon.py
```

### Comparing `pytest-testmon-2.0.7b1/LICENSE` & `pytest-testmon-2.0.7b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b1/PKG-INFO` & `pytest-testmon-2.0.7b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.7b1
+Version: 2.0.7b3
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b1 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b3 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.7b1/README.md` & `pytest-testmon-2.0.7b3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b1/pyproject.toml` & `pytest-testmon-2.0.7b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b1/pytest_testmon.egg-info/PKG-INFO` & `pytest-testmon-2.0.7b3/pytest_testmon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testmon
-Version: 2.0.7b1
+Version: 2.0.7b3
 Summary: selects tests affected by changed files and methods
 Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic
 Author-email: Tibor Arpas <tibor@testmon.org>
 License: AGPL
 Project-URL: Source, https://github.com/tarpas/pytest-testmon
 Keywords: testing,pytest,plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b1 Summary: selects
+Metadata-Version: 2.1 Name: pytest-testmon Version: 2.0.7b3 Summary: selects
 tests affected by changed files and methods Home-page: https://testmon.org
 Author: Tibor Arpas, Tomas Matlovic Author-email: Tibor Arpas
 testmon.org> License: AGPL Project-URL: Source, https://github.com/tarpas/
 pytest-testmon Keywords: testing,pytest,plugin Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Operating System :: POSIX Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
```

### Comparing `pytest-testmon-2.0.7b1/setup.cfg` & `pytest-testmon-2.0.7b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b1/testmon/configure.py` & `pytest-testmon-2.0.7b3/testmon/configure.py`

 * *Files identical despite different names*

### Comparing `pytest-testmon-2.0.7b1/testmon/db.py` & `pytest-testmon-2.0.7b3/testmon/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from collections import namedtuple
 from functools import lru_cache
 
 from testmon.process_code import blob_to_checksums, checksums_to_blob
 
 
-DATA_VERSION = 9
+DATA_VERSION = 12
 
 ChangedFileData = namedtuple(
     "ChangedFileData", "filename name method_checksums id failed"
 )
 
 
 class TestmonDbException(Exception):
@@ -80,15 +80,15 @@
 
     def _test_execution_fk_table(self):
         return "environment"
 
     def update_mtimes(self, new_mtimes):
         with self.con as con:
             con.executemany(
-                "UPDATE file_fp SET mtime=?, checksum=? WHERE id = ?", new_mtimes
+                "UPDATE file_fp SET mtime=?, fsha=? WHERE id = ?", new_mtimes
             )
 
     def finish_execution(self, exec_id, duration=None, select=True):
         self.update_saving_stats(exec_id, select)
         self.fetch_or_create_file_fp.cache_clear()
         with self.con as con:
             con.execute(
@@ -174,24 +174,24 @@
             total_saved_time,
             total_all_time,
             total_saved_tests,
             total_all_tests,
         )
 
     @lru_cache(1000)
-    def fetch_or_create_file_fp(self, filename, checksum, method_checksums):
+    def fetch_or_create_file_fp(self, filename, fsha, method_checksums):
         cursor = self.con.cursor()
         try:
             cursor.execute(
                 """
                 INSERT INTO file_fp
-                (filename, method_checksums, checksum)
+                (filename, method_checksums, fsha)
                 VALUES (?, ?, ?)
                 """,
-                (filename, method_checksums, checksum),
+                (filename, method_checksums, fsha),
             )
 
             fingerprint_id = cursor.lastrowid
         except sqlite3.IntegrityError:
             fingerprint_id, *_ = cursor.execute(
                 """
                 SELECT
@@ -247,43 +247,47 @@
             cursor.executemany(
                 f"DELETE FROM test_execution WHERE {self._test_execution_fk_column()}=? AND test_name=?",
                 [(exec_id, test_name) for test_name in tests_deps_n_outcomes],
             )
 
             test_execution_file_fps = []
             for test_name, deps_n_outcomes in tests_deps_n_outcomes.items():
-                failed = deps_n_outcomes.get("failed", None)
-                duration = deps_n_outcomes.get("duration", None)
-                forced = deps_n_outcomes.get("forced", None)
                 te_id = self._insert_test_execution(
                     con,
                     exec_id,
                     test_name,
-                    duration,
-                    failed,
-                    forced,
+                    deps_n_outcomes.get("duration", None),
+                    deps_n_outcomes.get("failed", None),
+                    deps_n_outcomes.get("forced", None),
                 )
 
                 fingerprints = deps_n_outcomes["deps"]
+                files_fshas = set()
                 for record in fingerprints:
                     fingerprint_id = self.fetch_or_create_file_fp(
                         record["filename"],
-                        record["checksum"],
+                        record["fsha"],
                         checksums_to_blob(record["method_checksums"]),
                     )
 
                     test_execution_file_fps.append((te_id, fingerprint_id))
+                    files_fshas.add((record["filename"], record["fsha"]))
             cursor.executemany(
                 "INSERT INTO test_execution_file_fp VALUES (?, ?)",
                 test_execution_file_fps,
             )
             self.fetch_or_create_file_fp.cache_clear()
             cursor.execute(
-                "DELETE FROM file_fp where id not in (select fingerprint_id from test_execution_file_fp)"
+                "DELETE FROM file_fp WHERE "
+                "    id NOT IN (select fingerprint_id from test_execution_file_fp)"
             )
+            self.insert_into_suite_files_fshas(con, exec_id, files_fshas)
+
+    def insert_into_suite_files_fshas(self, con, exec_id, files_fshas):
+        pass
 
     def _fetch_data_version(self):
         con = self.con
 
         return con.execute("PRAGMA user_version").fetchone()[0]
 
     def write_attribute(self, attribute, data, exec_id=None):
@@ -345,44 +349,52 @@
                 test_name TEXT,
                 duration FLOAT,
                 failed BIT,
                 forced BIT,
                 FOREIGN KEY({self._test_execution_fk_column()}) REFERENCES {self._test_execution_fk_table()}(id));
                 CREATE INDEX test_execution_fk_name ON test_execution ({self._test_execution_fk_column()}, test_name);
 
-                CREATE TABLE temp_files_checksums (exec_id INTEGER, filename TEXT, checksum TEXT);
-                CREATE INDEX temp_files_checksums_mcall ON temp_files_checksums (exec_id);
+                CREATE TABLE changed_files_fshas (exec_id INTEGER, filename TEXT, fsha TEXT);
+                CREATE INDEX changed_files_fshas_mcall ON changed_files_fshas (exec_id, filename, fsha);
 
-                CREATE TABLE temp_filenames (exec_id INTEGER, filename TEXT);
-                CREATE INDEX temp_filenames_eid ON temp_filenames (exec_id);
+                CREATE TABLE changed_files_mhashes (exec_id INTEGER, filename TEXT, mhashes BLOB);
+                CREATE INDEX changed_files_mhashes_eid ON changed_files_mhashes (exec_id);
             """
 
     def _create_file_fp_statement(self):
         return """
             CREATE TABLE file_fp
             (
                 id INTEGER PRIMARY KEY,
                 filename TEXT,
                 method_checksums BLOB,
                 mtime FLOAT,
-                checksum TEXT,
-                UNIQUE (filename, method_checksums)
+                fsha TEXT,
+                UNIQUE (filename, fsha, method_checksums)
             );"""
 
     def _create_test_execution_ffp_statement(
         self,
     ):
         return """
             CREATE TABLE test_execution_file_fp (
                 test_execution_id INTEGER,
                 fingerprint_id INTEGER,
                 FOREIGN KEY(test_execution_id) REFERENCES test_execution(id),
                 FOREIGN KEY(fingerprint_id) REFERENCES file_fp(id)
             );
             CREATE INDEX test_execution_file_fp_both ON test_execution_file_fp (test_execution_id, fingerprint_id);
+            -- the following table stores the same data coarsely, but is used for faster queries
+            CREATE TABLE suite_execution_file_fsha (
+                suite_execution_id INTEGER,
+                filename TEXT,
+                fsha text,
+                FOREIGN KEY(suite_execution_id) REFERENCES suite_execution(id)
+                );
+                CREATE UNIQUE INDEX sefch_suite_id_filename_sha ON suite_execution_file_fsha(suite_execution_id, filename, fsha);
             """
 
     def init_tables(self):
         connection = self.con
 
         connection.executescript(
             self._create_metadata_statement()
@@ -427,85 +439,77 @@
                     row["failed"],
                     row["duration"],
                 ]
             )
 
         return result
 
-    def fetch_unknown_files(self, files_checksums, exec_id):
+    def fetch_unknown_files(self, files_fshas, exec_id):
         with self.con as con:
-            con.execute(
-                "DELETE FROM temp_files_checksums WHERE exec_id = ?", (exec_id,)
-            )
+            con.execute("DELETE FROM changed_files_fshas WHERE exec_id = ?", (exec_id,))
             con.executemany(
-                "INSERT INTO temp_files_checksums VALUES (?, ?, ?)",
-                [
-                    (exec_id, file, checksum)
-                    for file, checksum in files_checksums.items()
-                ],
+                "INSERT INTO changed_files_fshas VALUES (?, ?, ?)",
+                [(exec_id, file, fsha) for file, fsha in files_fshas.items()],
             )
             return self._fetch_unknown_files_from_one_v(con, exec_id, exec_id)
 
     def _fetch_unknown_files_from_one_v(self, con, exec_id, files_shas_id):
         result = []
         for row in con.execute(
             f"""
                 SELECT DISTINCT
                     f.filename
                 FROM test_execution te, test_execution_file_fp te_ffp, file_fp f
-                LEFT OUTER JOIN temp_files_checksums tfc
-                ON f.filename = tfc.filename and f.checksum = tfc.checksum AND tfc.exec_id = :files_shas_id
+                LEFT OUTER JOIN changed_files_fshas chff
+                ON f.filename = chff.filename and f.fsha = chff.fsha AND chff.exec_id = :files_shas_id
                 WHERE
                     te.{self._test_execution_fk_column()} = :exec_id AND
                     te.id = te_ffp.test_execution_id AND
                     te_ffp.fingerprint_id = f.id AND
-                    (f.checksum IS NULL OR tfc.checksum IS NULL)
+                    (f.fsha IS NULL OR chff.fsha IS NULL)
                 """,
             {"files_shas_id": files_shas_id, "exec_id": exec_id},
         ):
             result.append(row["filename"])
         return result
 
     def delete_filenames(self, con):
-        con.execute("DELETE FROM temp_filenames")
+        con.execute("DELETE FROM changed_files_mhashes")
 
     def determine_tests(self, exec_id, files_mhashes):
         with self.con as con:
             con.execute(
                 f"UPDATE test_execution set forced = NULL WHERE {self._test_execution_fk_column()} = ?",
                 [exec_id],
             )
             self.delete_filenames(con)
             con.executemany(
-                "INSERT INTO temp_filenames VALUES (?, ?)",
+                "INSERT INTO changed_files_mhashes VALUES (?, ?, ?)",
                 [
-                    (
-                        exec_id,
-                        k,
-                    )
-                    for k in files_mhashes
+                    (exec_id, file, checksums_to_blob(mhashes) if mhashes else None)
+                    for file, mhashes in files_mhashes.items()
                 ],
             )
 
             results = []
             for row in self.con.execute(
                 f"""
                 SELECT
                     f.filename,
                     te.test_name,
                     f.method_checksums,
                     te.failed,
                     te.duration
-                FROM test_execution te, test_execution_file_fp te_ffp, file_fp f, temp_filenames tf
+                FROM test_execution te, test_execution_file_fp te_ffp, file_fp f, changed_files_mhashes chfm
                 WHERE
-                    tf.exec_id = ? AND
+                    chfm.exec_id = ? AND
                     te.{self._test_execution_fk_column()} = ? AND
                     te.id = te_ffp.test_execution_id AND
                     te_ffp.fingerprint_id = f.id AND
-                    tf.filename = f.filename
+                    chfm.filename = f.filename
                 """,
                 [exec_id, exec_id],
             ):
                 results.append(
                     [
                         row["filename"],
                         row["test_name"],
@@ -584,25 +588,25 @@
 
     def filenames_fingerprints(self, exec_id):
         cursor = self.con.execute(
             f"""
             SELECT DISTINCT
                 f.filename,
                 f.mtime,
-                f.checksum,
+                f.fsha,
                 f.id as fingerprint_id,
                 sum(failed)
             FROM
                 test_execution te, test_execution_file_fp te_ffp, file_fp f
             WHERE
                 te.id = te_ffp.test_execution_id AND
                 te_ffp.fingerprint_id = f.id AND
                 {self._test_execution_fk_column()} = ?
             GROUP BY
-                f.filename, f.mtime, f.checksum, f.id
+                f.filename, f.mtime, f.fsha, f.id
             """,
             (exec_id,),
         )
 
         return [dict(row) for row in cursor]
 
     def fetch_or_create_environment(
```

### Comparing `pytest-testmon-2.0.7b1/testmon/process_code.py` & `pytest-testmon-2.0.7b3/testmon/process_code.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         )
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
 
 @lru_cache(300)
-def bytes_to_string_and_checksum(byte_stream):
+def bytes_to_string_and_fsha(byte_stream):
     byte_stream = byte_stream.replace(b"\f", b" ")
     byte_stream = byte_stream.replace(b"\r\n", b"\n")
     byte_string = byte_stream.decode(source_encoding(byte_stream), "replace")
     git_header = b"blob %u\0" % len(byte_string)
     hsh = hashlib.sha1()
     hsh.update(git_header)
     hsh.update(byte_stream)
@@ -104,25 +104,32 @@
         return end
     except AttributeError:
         return None
 
 
 class Module:
     def __init__(
-        self, source_code=None, mtime=None, ext="py", fs_checksum=None, filename=None
+        self,
+        source_code=None,
+        mtime=None,
+        ext="py",
+        fs_fsha=None,
+        filename=None,
+        rootdir=None,
     ):
         self.filename = filename
+        self.rootdir = rootdir
         self._blocks = None
         self.counter = 0
         self.mtime = mtime
         self._source_code = (
             None if source_code is None else textwrap.dedent(source_code)
         )
-        self.fs_checksum = (
-            fs_checksum or bytes_to_string_and_checksum(bytes(source_code, "utf-8"))[1]
+        self.fs_fsha = (
+            fs_fsha or bytes_to_string_and_fsha(bytes(source_code, "utf-8"))[1]
         )
         self.ext = ext
 
     def dump_and_block(self, node, end, name="unknown", into_block=False):
         if isinstance(node, ast.AST):
             class_name = node.__class__.__name__
             fields = []
@@ -180,15 +187,15 @@
             else:
                 self._blocks = [Block(1, len(lines), self.source_code)]
         return self._blocks
 
     @property
     def source_code(self):
         if self._source_code is None:
-            self._source_code = read_source_sha(self.filename)[0]
+            self._source_code = read_source_sha(Path(self.rootdir) / self.filename)[0]
         return self._source_code
 
     @property
     def method_checksums(self):
         return methods_to_checksums([block.checksum for block in self.blocks])
 
 
@@ -197,16 +204,16 @@
 
     try:
         with open(filename, "rb") as file:
             source_bytes = file.read()
     except FileNotFoundError:
         return None, None
 
-    source, checksum = bytes_to_string_and_checksum(source_bytes)
-    return source, checksum
+    source, fsha = bytes_to_string_and_fsha(source_bytes)
+    return source, fsha
 
 
 def noncached_get_files_shas(directory):
     all_shas = {}
     try:
         result = run(
             ["git", "ls-files", "--stage", "-m", directory],
```

### Comparing `pytest-testmon-2.0.7b1/testmon/pytest_testmon.py` & `pytest-testmon-2.0.7b3/testmon/pytest_testmon.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import xmlrpc.client
 import os
 
 from collections import defaultdict
 from datetime import date, timedelta
 
 import pytest
-import pkg_resources
 
 from _pytest.config import ExitCode, Config
 from _pytest.terminal import TerminalReporter
 
 from testmon.configure import TmConf
 
 from testmon.testmon_core import (
@@ -20,15 +19,15 @@
     home_file,
     TestmonException,
     get_test_execution_class_name,
     get_test_execution_module_name,
     cached_relpath,
 )
 from testmon import configure
-from testmon.common import get_logger
+from testmon.common import get_logger, get_system_packages
 
 SURVEY_NOTIFICATION_INTERVAL = timedelta(days=28)
 
 logger = get_logger(__name__)
 
 
 def pytest_addoption(parser):
@@ -124,23 +123,19 @@
         "environment_expression",
     ]:
         if config.getoption(label):
             result.append(label.replace("testmon_", ""))
     return result
 
 
-def get_system_packages():
-    return ", ".join(sorted(str(p) for p in pkg_resources.working_set))
-
-
 def init_testmon_data(config):
     environment = config.getoption("environment_expression") or eval_environment(
         config.getini("environment_expression")
     )
-    packages = get_system_packages()
+    system_packages = get_system_packages()
 
     url = config.getini("testmon_url")
     rpc_proxy = None
 
     if config.testmon_config.tmnet or getattr(config, "tmnet", None):
         rpc_proxy = getattr(config, "tmnet", None)
 
@@ -167,15 +162,15 @@
                 headers=[("x-api-key", tmnet_api_key)],
             )
 
     testmon_data = TestmonData(
         rootdir=config.rootdir.strpath,
         database=rpc_proxy,
         environment=environment,
-        system_packages=packages,
+        system_packages=system_packages,
     )
     testmon_data.determine_stable(bool(rpc_proxy))
     config.testmon_data = testmon_data
 
 
 def parallelism_status(config):
     if hasattr(config, "workerinput"):
```

### Comparing `pytest-testmon-2.0.7b1/testmon/testmon_core.py` & `pytest-testmon-2.0.7b3/testmon/testmon_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 import sysconfig
 import textwrap
 from functools import lru_cache
 from collections import defaultdict
 from xmlrpc.client import Fault, ProtocolError
 from socket import gaierror
 
-import pkg_resources
 import pytest
 from coverage import Coverage, CoverageData
 
 from testmon import db
 from testmon import VERSION as TM_CLIENT_VERSION
-
-from testmon.common import get_logger, git_current_head
+from testmon.common import (
+    get_logger,
+    get_system_packages,
+    drop_patch_version,
+    git_current_head,
+)
 
 from testmon.process_code import (
     match_fingerprint,
     create_fingerprint,
     methods_to_checksums,
     get_source_sha,
     Module,
@@ -55,23 +58,24 @@
     def __init__(self, rootdir, packages=None):
         self.rootdir = rootdir
         self.packages = packages
         self.cache = {}
 
     def get_file(self, filename):
         if filename not in self.cache:
-            code, checksum = get_source_sha(directory=self.rootdir, filename=filename)
-            if checksum:
+            code, fsha = get_source_sha(directory=self.rootdir, filename=filename)
+            if fsha:
                 fs_mtime = os.path.getmtime(os.path.join(self.rootdir, filename))
                 self.cache[filename] = Module(
                     source_code=code,
                     mtime=fs_mtime,
                     ext=filename.rsplit(".", 1)[1],
-                    fs_checksum=checksum,
+                    fs_fsha=fsha,
                     filename=filename,
+                    rootdir=self.rootdir,
                 )
             else:
                 self.cache[filename] = None
         return self.cache[filename]
 
 
 def check_mtime(file_system, record):
@@ -81,19 +85,19 @@
     try:
         fs_mtime = cache_module.mtime if cache_module else os.path.getmtime(absfilename)
     except OSError:
         return False
     return record["mtime"] == fs_mtime
 
 
-def check_checksum(file_system, record):
+def check_fsha(file_system, record):
     cache_module = file_system.get_file(record["filename"])
-    fs_checksum = cache_module.fs_checksum if cache_module else None
+    fs_fsha = cache_module.fs_fsha if cache_module else None
 
-    return record["checksum"] == fs_checksum
+    return record["fsha"] == fs_fsha
 
 
 def check_fingerprint(disk, record):
     file = record[0]
     fingerprint = record[2]
 
     module = disk.get_file(file)
@@ -135,17 +139,16 @@
         system_packages=None,
         python_version=None,
     ):
         self.rootdir = rootdir
         self.environment = environment if environment else "default"
         self.source_tree = SourceTree(rootdir=rootdir)
         if system_packages is None:
-            system_packages = ", ".join(
-                sorted(str(p) for p in pkg_resources.working_set or [])
-            )
+            system_packages = get_system_packages()
+        system_packages = drop_patch_version(system_packages)
         if not python_version:
             python_version = f"{sys.version_info.major}.{sys.version_info.minor}.{sys.version_info.micro}"
 
         if database:
             self.db = database
         else:
             self.db = db.DB(os.path.join(self.rootdir, get_data_file_path()))
@@ -159,15 +162,18 @@
                     "tm_client_version": TM_CLIENT_VERSION,
                     "git_head_sha": git_current_head(),
                     "ci": os.environ.get("CI"),
                 },
             )
         except (ConnectionRefusedError, Fault, ProtocolError, gaierror) as exc:
             logger.error(
-                "%s error when communication with testmon.net. (falling back to .testmondata locally)",
+                (
+                    "%s error when communication with testmon.net. (falling back to"
+                    " .testmondata locally)"
+                ),
                 exc,
             )
             self.db = db.DB(os.path.join(self.rootdir, get_data_file_path()))
             result = self.db.initiate_execution(
                 self.environment, system_packages, python_version, {}
             )
         self.exec_id = result["exec_id"]
@@ -197,15 +203,15 @@
                 if os.path.exists(os.path.join(self.rootdir, filename)):
                     module = self.source_tree.get_file(filename)
                     fingerprint = create_fingerprint(module, covered)
                     deps_n_outcomes["deps"].append(
                         {
                             "filename": filename,
                             "mtime": module.mtime,
-                            "checksum": module.fs_checksum,
+                            "fsha": module.fs_fsha,
                             "method_checksums": fingerprint,
                         }
                     )
 
             deps_n_outcomes.update(process_result(reports[context]))
             deps_n_outcomes["forced"] = context in self.stable_test_names
             test_executions_fingerprints[context] = deps_n_outcomes
@@ -218,38 +224,36 @@
             test_execution_file_fps = {
                 test_name: {
                     "deps": (
                         {
                             "filename": home_file(test_name),
                             "method_checksums": methods_to_checksums(["0match"]),
                             "mtime": None,
-                            "checksum": None,
+                            "fsha": None,
                         },
                     )
                 }
                 for test_name in add
                 if is_python_file(home_file(test_name))
             }
             if test_execution_file_fps:
                 self.save_test_execution_file_fps(test_execution_file_fps)
 
         to_delete = list(set(self.all_tests) - collected)
         with self.db as database:
             database.delete_test_executions(to_delete, self.exec_id)
 
     def determine_stable(self, assert_old=True):
-        files_checksums = {}
+        files_fshas = {}
         for filename in self.files_of_interest:
             module = self.source_tree.get_file(filename)
             if module:
-                files_checksums[filename] = module.fs_checksum
+                files_fshas[filename] = module.fs_fsha
 
-        new_changed_file_data = self.db.fetch_unknown_files(
-            files_checksums, self.exec_id
-        )
+        new_changed_file_data = self.db.fetch_unknown_files(files_fshas, self.exec_id)
 
         files_mhashes = collect_mhashes(self.source_tree, new_changed_file_data)
 
         affected_tests = self.db.determine_tests(self.exec_id, files_mhashes)[
             "affected"
         ]
 
@@ -266,20 +270,20 @@
 
         self.stable_test_names = set(self.all_tests) - self.unstable_test_names
         self.stable_files = set(self.all_files) - self.unstable_files
 
     def assert_old_determin_stable(self, new_fingerprint_misses):
         filenames_fingerprints = self.db.filenames_fingerprints(self.exec_id)
 
-        _, checksum_misses = split_filter(
-            self.source_tree, check_checksum, filenames_fingerprints
+        _, fsha_misses = split_filter(
+            self.source_tree, check_fsha, filenames_fingerprints
         )
 
         changed_file_data = self.db.fetch_changed_file_data(
-            [checksum_miss["fingerprint_id"] for checksum_miss in (checksum_misses)],
+            [fsha_miss["fingerprint_id"] for fsha_miss in (fsha_misses)],
             self.exec_id,
         )
 
         _, fingerprint_misses = split_filter(
             self.source_tree, check_fingerprint, changed_file_data
         )
 
@@ -335,20 +339,20 @@
 
 
 def get_new_mtimes(filesystem, hits):
     try:
         for hit in hits:
             module = filesystem.get_file(hit[0])
             if module:
-                yield module.mtime, module.fs_checksum, hit[3]
+                yield module.mtime, module.fs_fsha, hit[3]
     except KeyError:
         for hit in hits:
             module = filesystem.get_file(hit["filename"])
             if module:
-                yield module.mtime, module.fs_checksum, hit["fingerprint_id"]
+                yield module.mtime, module.fs_fsha, hit["fingerprint_id"]
 
 
 def get_test_execution_class_name(node_id):
     if len(node_id.split("::")) > 2:
         return node_id.split("::")[1]
     return None
 
@@ -460,16 +464,19 @@
 
     def discard_current(self):
         self._interrupted_at = self._test_name
 
     def get_batch_coverage_data(self):
         if self.check_stack != TestmonCollector.coverage_stack:
             pytest.exit(
-                f"Exiting pytest!!!! This test corrupts Testmon.coverage_stack: "
-                f"{self._test_name} {self.check_stack}, {TestmonCollector.coverage_stack}",
+                (
+                    "Exiting pytest!!!! This test corrupts Testmon.coverage_stack:"
+                    f" {self._test_name} {self.check_stack},"
+                    f" {TestmonCollector.coverage_stack}"
+                ),
                 returncode=3,
             )
 
         nodes_files_lines = {}
 
         if self.cov and (
             len(self.batched_test_names) >= TEST_BATCH_SIZE
```

### Comparing `pytest-testmon-2.0.7b1/testmon/tox_testmon.py` & `pytest-testmon-2.0.7b3/testmon/tox_testmon.py`

 * *Files identical despite different names*

