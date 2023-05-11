# Comparing `tmp/np_jobs-0.0.3.tar.gz` & `tmp/np_jobs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_jobs-0.0.3.tar", last modified: Wed May 10 06:13:59 2023, max compression
+gzip compressed data, was "np_jobs-0.0.4.tar", last modified: Thu May 11 23:29:42 2023, max compression
```

## Comparing `np_jobs-0.0.3.tar` & `np_jobs-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      110 2023-05-10 01:20:18.221900 np_jobs-0.0.3/README.md
--rw-r--r--   0        0        0     2358 2023-05-10 06:13:59.807206 np_jobs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      243 2023-05-10 05:18:07.654589 np_jobs-0.0.3/src/np_jobs/__init__.py
--rw-r--r--   0        0        0       75 2023-05-10 01:25:17.321180 np_jobs-0.0.3/src/np_jobs/jobs/__init__.py
--rw-r--r--   0        0        0     1112 2023-05-10 01:37:07.453140 np_jobs-0.0.3/src/np_jobs/jobs/base.py
--rw-r--r--   0        0        0      150 2023-05-10 01:25:17.320182 np_jobs-0.0.3/src/np_jobs/jobs/pipeline_sorting.py
--rw-r--r--   0        0        0       42 2023-05-10 00:44:55.816888 np_jobs-0.0.3/src/np_jobs/queues/__init__.py
--rw-r--r--   0        0        0      443 2023-05-10 06:12:46.620875 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/__init__.py
--rw-r--r--   0        0        0    11538 2023-05-10 01:15:00.936326 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/base.py
--rw-r--r--   0        0        0      161 2023-05-10 01:06:56.845630 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/codeocean_upload_queue.py
--rw-r--r--   0        0        0      161 2023-05-10 01:06:39.090798 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/datajoint_upload_queue.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      161 2023-05-10 00:57:38.731220 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/pipeline_npexp_upload_queue.py
--rw-r--r--   0        0        0      142 2023-05-10 00:57:35.004534 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/pipeline_qc_queue.py
--rw-r--r--   0        0        0      348 2023-05-10 00:54:41.870192 np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/pipeline_sorting_queue.py
--rw-r--r--   0        0        0     4938 2023-05-10 01:08:07.498322 np_jobs-0.0.3/src/np_jobs/types.py
--rw-r--r--   0        0        0     2579 2023-05-10 01:25:17.321180 np_jobs-0.0.3/src/np_jobs/utils.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 np_jobs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-05-10 01:20:18.221900 np_jobs-0.0.4/README.md
+-rw-r--r--   0        0        0     2358 2023-05-11 23:29:42.562076 np_jobs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-05-10 05:18:07.654589 np_jobs-0.0.4/src/np_jobs/__init__.py
+-rw-r--r--   0        0        0       75 2023-05-10 01:25:17.321180 np_jobs-0.0.4/src/np_jobs/jobs/__init__.py
+-rw-r--r--   0        0        0     1112 2023-05-10 01:37:07.453140 np_jobs-0.0.4/src/np_jobs/jobs/base.py
+-rw-r--r--   0        0        0      150 2023-05-10 01:25:17.320182 np_jobs-0.0.4/src/np_jobs/jobs/pipeline_sorting.py
+-rw-r--r--   0        0        0       42 2023-05-10 00:44:55.816888 np_jobs-0.0.4/src/np_jobs/queues/__init__.py
+-rw-r--r--   0        0        0      443 2023-05-10 06:12:46.620875 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/__init__.py
+-rw-r--r--   0        0        0    11538 2023-05-10 01:15:00.936326 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/base.py
+-rw-r--r--   0        0        0      161 2023-05-10 01:06:56.845630 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/codeocean_upload_queue.py
+-rw-r--r--   0        0        0      161 2023-05-10 01:06:39.090798 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/datajoint_upload_queue.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      161 2023-05-10 00:57:38.731220 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/pipeline_npexp_upload_queue.py
+-rw-r--r--   0        0        0      142 2023-05-10 00:57:35.004534 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      348 2023-05-10 00:54:41.870192 np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0     4938 2023-05-10 01:08:07.498322 np_jobs-0.0.4/src/np_jobs/types.py
+-rw-r--r--   0        0        0     2772 2023-05-11 23:27:56.478961 np_jobs-0.0.4/src/np_jobs/utils.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 np_jobs-0.0.4/PKG-INFO
```

### Comparing `np_jobs-0.0.3/pyproject.toml` & `np_jobs-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_jobs"
-version = "0.0.3"
+version = "0.0.4"
 description = "Interfaces for job queues used to coordinate distributed tasks for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np-config>=0.4.17",
     "np-logging>=0.5.1",
```

### Comparing `np_jobs-0.0.3/src/np_jobs/jobs/base.py` & `np_jobs-0.0.4/src/np_jobs/jobs/base.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/base.py` & `np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/base.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.3/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py` & `np_jobs-0.0.4/src/np_jobs/queues/sqlite_isilon/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.3/src/np_jobs/types.py` & `np_jobs-0.0.4/src/np_jobs/types.py`

 * *Files identical despite different names*

### Comparing `np_jobs-0.0.3/src/np_jobs/utils.py` & `np_jobs-0.0.4/src/np_jobs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,23 @@
 
 def get_session(session_or_job: SessionArgs | Job) -> np_session.Session:
     """Parse a session argument into a Neuropixels Session.
     
     >>> get_session('123456789_366122_20230422')
     PipelineSession('123456789_366122_20230422')
     >>> assert _ == get_session(np_session.Session('123456789_366122_20230422'))
+    >>> get_session('DRpilot_644866_20230207')
+    DRPilotSession('DRpilot_644866_20230207')
     """
     if isinstance(session_or_job, np_session.Session):
         return session_or_job
+    if isinstance(session_or_job, Job):
+        return get_session(session_or_job.session)
     try:
-        return np_session.Session(session_or_job)
+        return np_session.Session(str(session_or_job))
     except np_session.SessionError as exc:
         raise TypeError(
             f'Unknown type for session_or_job: {session_or_job!r}'
             ) from exc
 
     
 def get_job(session_or_job: SessionArgs | Job, job_type: Type[JobT] = JobDataclass) -> JobT:
```

### Comparing `np_jobs-0.0.3/PKG-INFO` & `np_jobs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-jobs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Interfaces for job queues used to coordinate distributed tasks for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

