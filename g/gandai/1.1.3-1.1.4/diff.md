# Comparing `tmp/gandai-1.1.3.tar.gz` & `tmp/gandai-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.3.tar", last modified: Thu May 11 12:12:21 2023, max compression
+gzip compressed data, was "gandai-1.1.4.tar", last modified: Fri May 12 20:54:13 2023, max compression
```

## Comparing `gandai-1.1.3.tar` & `gandai-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.742109 gandai-1.1.3/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.3/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-11 12:12:21.741998 gandai-1.1.3/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.738617 gandai-1.1.3/gandai/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-05-11 12:03:39.000000 gandai-1.1.3/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.740565 gandai-1.1.3/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-1.1.3/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.3/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.3/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.3/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.3/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-1.1.3/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-1.1.3/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16707 2023-05-10 05:05:31.000000 gandai-1.1.3/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.3/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-1.1.3/gandai/__pycache__/sources.cpython-311.pyc
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741019 gandai-1.1.3/gandai/adapters/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.3/gandai/adapters/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741548 gandai-1.1.3/gandai/adapters/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.3/gandai/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.3/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.3/gandai/adapters/__pycache__/filters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.3/gandai/adapters/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-1.1.3/gandai/adapters/dealcloud.py
--rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.3/gandai/adapters/filters.py
--rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-1.1.3/gandai/adapters/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-1.1.3/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.3/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     2382 2023-05-11 11:58:58.000000 gandai-1.1.3/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-1.1.3/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.741859 gandai-1.1.3/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.3/gandai/migrations/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-1.1.3/gandai/migrations/create_db.sql
--rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-1.1.3/gandai/migrations/dealcloud_to_gandai.py
--rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-1.1.3/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)     8110 2023-05-11 12:01:31.000000 gandai-1.1.3/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-1.1.3/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-11 12:12:21.739166 gandai-1.1.3/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1133 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-11 12:12:21.000000 gandai-1.1.3/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-11 12:12:10.000000 gandai-1.1.3/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-11 12:12:21.742137 gandai-1.1.3/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.3/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.354554 gandai-1.1.4/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.4/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-12 20:54:13.354427 gandai-1.1.4/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.348103 gandai-1.1.4/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-05-11 12:03:39.000000 gandai-1.1.4/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.351535 gandai-1.1.4/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      179 2023-05-11 12:17:29.000000 gandai-1.1.4/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.4/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.4/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.4/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1981 2023-05-11 12:17:30.000000 gandai-1.1.4/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.4/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5068 2023-05-12 19:30:40.000000 gandai-1.1.4/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6064 2023-05-12 19:41:17.000000 gandai-1.1.4/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15927 2023-05-11 13:39:01.000000 gandai-1.1.4/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.4/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7849 2023-05-12 19:25:42.000000 gandai-1.1.4/gandai/__pycache__/sources.cpython-311.pyc
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.352512 gandai-1.1.4/gandai/adapters/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.4/gandai/adapters/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.353583 gandai-1.1.4/gandai/adapters/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.4/gandai/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.4/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.4/gandai/adapters/__pycache__/filters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.4/gandai/adapters/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1299 2023-05-11 12:41:01.000000 gandai-1.1.4/gandai/adapters/dealcloud.py
+-rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.4/gandai/adapters/filters.py
+-rw-r--r--   0 parker     (501) staff       (20)    10624 2023-05-11 12:52:58.000000 gandai-1.1.4/gandai/adapters/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1742 2023-05-12 20:52:41.000000 gandai-1.1.4/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.4/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     2382 2023-05-11 11:58:58.000000 gandai-1.1.4/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     3286 2023-05-12 19:30:37.000000 gandai-1.1.4/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.354152 gandai-1.1.4/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.4/gandai/migrations/__init__.py
+-rw-r--r--   0 parker     (501) staff       (20)     3653 2023-05-12 19:32:11.000000 gandai-1.1.4/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     2072 2023-05-12 19:25:46.000000 gandai-1.1.4/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     1868 2023-05-11 12:41:47.000000 gandai-1.1.4/gandai/migrations/dealcloud_to_gandai.py
+-rw-r--r--   0 parker     (501) staff       (20)     2592 2023-05-12 19:41:16.000000 gandai-1.1.4/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)     8401 2023-05-11 13:39:00.000000 gandai-1.1.4/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5418 2023-05-12 19:25:41.000000 gandai-1.1.4/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-12 20:54:13.348643 gandai-1.1.4/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-12 20:54:13.000000 gandai-1.1.4/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1199 2023-05-12 20:54:13.000000 gandai-1.1.4/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-12 20:54:13.000000 gandai-1.1.4/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-12 20:54:13.000000 gandai-1.1.4/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-12 20:54:00.000000 gandai-1.1.4/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-12 20:54:13.354585 gandai-1.1.4/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.4/setup.py
```

### Comparing `gandai-1.1.3/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc6925a64 (Tue May  9 18:36:54 2023 UTC)
-files sz: 2560
+moddate:  0x5c965e64 (Fri May 12 19:41:16 2023 UTC)
+files sz: 2592
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a046d
@@ -99,140 +99,140 @@
                166 LOAD_CONST              11 ('EventType')
                168 LOAD_NAME               12 (str)
                170 LOAD_NAME                4 (Enum)
                172 PRECALL                  4
                176 CALL                     4
                186 STORE_NAME              13 (EventType)
    
-    34         188 LOAD_NAME                8 (dataclass)
+    35         188 LOAD_NAME                8 (dataclass)
    
-    35         190 PUSH_NULL
+    36         190 PUSH_NULL
                192 LOAD_BUILD_CLASS
-               194 LOAD_CONST              12 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 34>)
+               194 LOAD_CONST              12 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 35>)
                196 MAKE_FUNCTION            0
                198 LOAD_CONST              13 ('Event')
                200 PRECALL                  2
                204 CALL                     2
    
-    34         214 PRECALL                  0
+    35         214 PRECALL                  0
                218 CALL                     0
    
-    35         228 STORE_NAME              14 (Event)
+    36         228 STORE_NAME              14 (Event)
    
-    46         230 LOAD_NAME                8 (dataclass)
+    47         230 LOAD_NAME                8 (dataclass)
    
-    47         232 PUSH_NULL
+    48         232 PUSH_NULL
                234 LOAD_BUILD_CLASS
-               236 LOAD_CONST              14 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 46>)
+               236 LOAD_CONST              14 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 47>)
                238 MAKE_FUNCTION            0
                240 LOAD_CONST              15 ('Comment')
                242 LOAD_NAME               14 (Event)
                244 PRECALL                  3
                248 CALL                     3
    
-    46         258 PRECALL                  0
+    47         258 PRECALL                  0
                262 CALL                     0
    
-    47         272 STORE_NAME              15 (Comment)
+    48         272 STORE_NAME              15 (Comment)
    
-    52         274 LOAD_NAME                8 (dataclass)
+    53         274 LOAD_NAME                8 (dataclass)
    
-    53         276 PUSH_NULL
+    54         276 PUSH_NULL
                278 LOAD_BUILD_CLASS
-               280 LOAD_CONST              16 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 52>)
+               280 LOAD_CONST              16 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 53>)
                282 MAKE_FUNCTION            0
                284 LOAD_CONST              17 ('Rating')
                286 LOAD_NAME               14 (Event)
                288 PRECALL                  3
                292 CALL                     3
    
-    52         302 PRECALL                  0
+    53         302 PRECALL                  0
                306 CALL                     0
    
-    53         316 STORE_NAME              16 (Rating)
+    54         316 STORE_NAME              16 (Rating)
    
-    57         318 LOAD_NAME                8 (dataclass)
+    58         318 LOAD_NAME                8 (dataclass)
    
-    58         320 PUSH_NULL
+    59         320 PUSH_NULL
                322 LOAD_BUILD_CLASS
-               324 LOAD_CONST              18 (<code object Checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 57>)
+               324 LOAD_CONST              18 (<code object Checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 58>)
                326 MAKE_FUNCTION            0
                328 LOAD_CONST              19 ('Checkpoint')
                330 PRECALL                  2
                334 CALL                     2
    
-    57         344 PRECALL                  0
+    58         344 PRECALL                  0
                348 CALL                     0
    
-    58         358 STORE_NAME              17 (Checkpoint)
+    59         358 STORE_NAME              17 (Checkpoint)
    
-    64         360 PUSH_NULL
+    65         360 PUSH_NULL
                362 LOAD_NAME                8 (dataclass)
                364 LOAD_CONST               6 (True)
                366 KW_NAMES                 7
                368 PRECALL                  1
                372 CALL                     1
    
-    65         382 PUSH_NULL
+    66         382 PUSH_NULL
                384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              20 (<code object Target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 64>)
+               386 LOAD_CONST              20 (<code object Target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 65>)
                388 MAKE_FUNCTION            0
                390 LOAD_CONST              21 ('Target')
                392 PRECALL                  2
                396 CALL                     2
    
-    64         406 PRECALL                  0
+    65         406 PRECALL                  0
                410 CALL                     0
    
-    65         420 STORE_NAME              18 (Target)
+    66         420 STORE_NAME              18 (Target)
    
-    76         422 LOAD_NAME                8 (dataclass)
+    77         422 LOAD_NAME                8 (dataclass)
    
-    77         424 PUSH_NULL
+    78         424 PUSH_NULL
                426 LOAD_BUILD_CLASS
-               428 LOAD_CONST              22 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 76>)
+               428 LOAD_CONST              22 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 77>)
                430 MAKE_FUNCTION            0
                432 LOAD_CONST              23 ('Criteria')
                434 PRECALL                  2
                438 CALL                     2
    
-    76         448 PRECALL                  0
+    77         448 PRECALL                  0
                452 CALL                     0
    
-    77         462 STORE_NAME              19 (Criteria)
+    78         462 STORE_NAME              19 (Criteria)
    
-    92         464 LOAD_NAME                8 (dataclass)
+    93         464 LOAD_NAME                8 (dataclass)
    
-    93         466 PUSH_NULL
+    94         466 PUSH_NULL
                468 LOAD_BUILD_CLASS
-               470 LOAD_CONST              24 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 92>)
+               470 LOAD_CONST              24 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 93>)
                472 MAKE_FUNCTION            0
                474 LOAD_CONST              25 ('Search')
                476 PRECALL                  2
                480 CALL                     2
    
-    92         490 PRECALL                  0
+    93         490 PRECALL                  0
                494 CALL                     0
    
-    93         504 STORE_NAME              20 (Search)
+    94         504 STORE_NAME              20 (Search)
    
-   107         506 LOAD_NAME                8 (dataclass)
+   108         506 LOAD_NAME                8 (dataclass)
    
-   108         508 PUSH_NULL
+   109         508 PUSH_NULL
                510 LOAD_BUILD_CLASS
-               512 LOAD_CONST              26 (<code object Sort, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 107>)
+               512 LOAD_CONST              26 (<code object Sort, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 108>)
                514 MAKE_FUNCTION            0
                516 LOAD_CONST              27 ('Sort')
                518 PRECALL                  2
                522 CALL                     2
    
-   107         532 PRECALL                  0
+   108         532 PRECALL                  0
                536 CALL                     0
    
-   108         546 STORE_NAME              21 (Sort)
+   109         546 STORE_NAME              21 (Sort)
                548 LOAD_CONST              28 (None)
                550 RETURN_VALUE
    consts
       0
       ('List', 'Optional')
       ('Enum', 'auto')
       ('asdict', 'dataclass', 'field')
@@ -376,15 +376,15 @@
          flags     : 0
          code
             0x970065005a0164005a0202006503a6000000ab0000000000000000005a
             0402006503a6000000ab0000000000000000005a0502006503a6000000ab
             0000000000000000005a0602006503a6000000ab0000000000000000005a
             0702006503a6000000ab0000000000000000005a0802006503a6000000ab
             0000000000000000005a0902006503a6000000ab0000000000000000005a
-            0a64015300
+            0a02006503a6000000ab0000000000000000005a0b64015300
           24           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('EventType')
                        8 STORE_NAME               2 (__qualname__)
          
           25          10 PUSH_NULL
@@ -424,124 +424,132 @@
                      128 STORE_NAME               9 (CONFLICT)
          
           31         130 PUSH_NULL
                      132 LOAD_NAME                3 (auto)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 STORE_NAME              10 (REJECT)
-                     150 LOAD_CONST               1 (None)
-                     152 RETURN_VALUE
+         
+          32         150 PUSH_NULL
+                     152 LOAD_NAME                3 (auto)
+                     154 PRECALL                  0
+                     158 CALL                     0
+                     168 STORE_NAME              11 (CRITERIA)
+                     170 LOAD_CONST               1 (None)
+                     172 RETURN_VALUE
          consts
             'EventType'
             None
-         names      ('__name__', '__module__', '__qualname__', 'auto', 'CREATE', 'ADVANCE', 'VALIDATE', 'SEND', 'CLIENT_ACCEPT', 'CONFLICT', 'REJECT')
+         names      ('__name__', '__module__', '__qualname__', 'auto', 'CREATE', 'ADVANCE', 'VALIDATE', 'SEND', 'CLIENT_ACCEPT', 'CONFLICT', 'REJECT', 'CRITERIA')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'EventType'
          firstlineno 24
-         lnotab 0x0a01140114011401140114011401
+         lnotab 0x0a011401140114011401140114011401
       'EventType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c0000006505650464023c
-            0000006505650464033c0000006505650464043c000000020065066507ac
-            05a6010000ab0100000000000000005a086507650464063c000000020065
-            066407ac08a6010000ab0100000000000000005a096503650464093c0000
-            0064075300
-          34           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c00000065056506190000
+            00000000000000650464023c0000006506650464033c0000006506650464
+            043c000000020065076508ac05a6010000ab0100000000000000005a0965
+            08650464063c000000020065076407ac08a6010000ab0100000000000000
+            005a0a6503650464093c00000064075300
+          35           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Event')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          37          12 LOAD_NAME                3 (int)
+          38          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('search_uid')
                       18 STORE_SUBSCR
          
-          38          22 LOAD_NAME                5 (str)
-                      24 LOAD_NAME                4 (__annotations__)
-                      26 LOAD_CONST               2 ('domain')
-                      28 STORE_SUBSCR
-         
-          39          32 LOAD_NAME                5 (str)
-                      34 LOAD_NAME                4 (__annotations__)
-                      36 LOAD_CONST               3 ('actor_key')
-                      38 STORE_SUBSCR
-         
-          40          42 LOAD_NAME                5 (str)
-                      44 LOAD_NAME                4 (__annotations__)
-                      46 LOAD_CONST               4 ('type')
-                      48 STORE_SUBSCR
-         
-          41          52 PUSH_NULL
-                      54 LOAD_NAME                6 (field)
-                      56 LOAD_NAME                7 (dict)
-                      58 KW_NAMES                 5
-                      60 PRECALL                  1
-                      64 CALL                     1
-                      74 STORE_NAME               8 (data)
-                      76 LOAD_NAME                7 (dict)
-                      78 LOAD_NAME                4 (__annotations__)
-                      80 LOAD_CONST               6 ('data')
-                      82 STORE_SUBSCR
-         
-          42          86 PUSH_NULL
-                      88 LOAD_NAME                6 (field)
-                      90 LOAD_CONST               7 (None)
-                      92 KW_NAMES                 8
-                      94 PRECALL                  1
-                      98 CALL                     1
-                     108 STORE_NAME               9 (id)
-                     110 LOAD_NAME                3 (int)
-                     112 LOAD_NAME                4 (__annotations__)
-                     114 LOAD_CONST               9 ('id')
-                     116 STORE_SUBSCR
-                     120 LOAD_CONST               7 (None)
-                     122 RETURN_VALUE
+          39          22 LOAD_NAME                5 (Optional)
+                      24 LOAD_NAME                6 (str)
+                      26 BINARY_SUBSCR
+                      36 LOAD_NAME                4 (__annotations__)
+                      38 LOAD_CONST               2 ('domain')
+                      40 STORE_SUBSCR
+         
+          40          44 LOAD_NAME                6 (str)
+                      46 LOAD_NAME                4 (__annotations__)
+                      48 LOAD_CONST               3 ('actor_key')
+                      50 STORE_SUBSCR
+         
+          41          54 LOAD_NAME                6 (str)
+                      56 LOAD_NAME                4 (__annotations__)
+                      58 LOAD_CONST               4 ('type')
+                      60 STORE_SUBSCR
+         
+          42          64 PUSH_NULL
+                      66 LOAD_NAME                7 (field)
+                      68 LOAD_NAME                8 (dict)
+                      70 KW_NAMES                 5
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 STORE_NAME               9 (data)
+                      88 LOAD_NAME                8 (dict)
+                      90 LOAD_NAME                4 (__annotations__)
+                      92 LOAD_CONST               6 ('data')
+                      94 STORE_SUBSCR
+         
+          43          98 PUSH_NULL
+                     100 LOAD_NAME                7 (field)
+                     102 LOAD_CONST               7 (None)
+                     104 KW_NAMES                 8
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 STORE_NAME              10 (id)
+                     122 LOAD_NAME                3 (int)
+                     124 LOAD_NAME                4 (__annotations__)
+                     126 LOAD_CONST               9 ('id')
+                     128 STORE_SUBSCR
+                     132 LOAD_CONST               7 (None)
+                     134 RETURN_VALUE
          consts
             'Event'
             'search_uid'
             'domain'
             'actor_key'
             'type'
             ('default_factory',)
             'data'
             None
             ('default',)
             'id'
-         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'data', 'id')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'Optional', 'str', 'field', 'dict', 'data', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Event'
-         firstlineno 34
-         lnotab 0x0c030a010a010a010a012201
+         firstlineno 35
+         lnotab 0x0c030a0116010a010a012201
       'Event'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          46           0 RESUME                   0
+          47           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Comment')
                        8 STORE_NAME               2 (__qualname__)
          
-          48          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 48>)
+          49          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 49>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Comment'
             code
@@ -549,17 +557,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                48           0 RESUME                   0
+                49           0 RESUME                   0
                
-                49           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                50           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('comment')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (str)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -573,39 +581,39 @@
                   'comment'
                names      ('isinstance', 'data', 'str')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 48
+               firstlineno 49
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Comment'
-         firstlineno 46
+         firstlineno 47
          lnotab 0x0a02
       'Comment'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          52           0 RESUME                   0
+          53           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Rating')
                        8 STORE_NAME               2 (__qualname__)
          
-          54          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 54>)
+          55          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 55>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Rating'
             code
@@ -613,17 +621,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                54           0 RESUME                   0
+                55           0 RESUME                   0
                
-                55           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                56           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('rating')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (int)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -637,48 +645,48 @@
                   'rating'
                names      ('isinstance', 'data', 'int')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 54
+               firstlineno 55
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Rating'
-         firstlineno 52
+         firstlineno 53
          lnotab 0x0a02
       'Rating'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c000000020065056402ac
             03a6010000ab0100000000000000005a066503650464043c000000640253
             00
-          57           0 RESUME                   0
+          58           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Checkpoint')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          60          12 LOAD_NAME                3 (int)
+          61          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('event_id')
                       18 STORE_SUBSCR
          
-          61          22 PUSH_NULL
+          62          22 PUSH_NULL
                       24 LOAD_NAME                5 (field)
                       26 LOAD_CONST               2 (None)
                       28 KW_NAMES                 3
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_NAME               6 (id)
                       46 LOAD_NAME                3 (int)
@@ -695,70 +703,70 @@
             'id'
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'field', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Checkpoint'
-         firstlineno 57
+         firstlineno 58
          lnotab 0x0c030a01
       'Checkpoint'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
             0000006505650464033c0000006503650464043c0000006506650464053c
             0000006503650464063c0000006505650464073c0000006507650464083c
             00000064095300
-          64           0 RESUME                   0
+          65           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Target')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          66          12 LOAD_NAME                3 (str)
+          67          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('domain')
                       18 STORE_SUBSCR
          
-          67          22 LOAD_NAME                3 (str)
+          68          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('name')
                       28 STORE_SUBSCR
          
-          68          32 LOAD_NAME                5 (int)
+          69          32 LOAD_NAME                5 (int)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('search_id')
                       38 STORE_SUBSCR
          
-          69          42 LOAD_NAME                3 (str)
+          70          42 LOAD_NAME                3 (str)
                       44 LOAD_NAME                4 (__annotations__)
                       46 LOAD_CONST               4 ('description')
                       48 STORE_SUBSCR
          
-          70          52 LOAD_NAME                6 (List)
+          71          52 LOAD_NAME                6 (List)
                       54 LOAD_NAME                4 (__annotations__)
                       56 LOAD_CONST               5 ('event')
                       58 STORE_SUBSCR
          
-          71          62 LOAD_NAME                3 (str)
+          72          62 LOAD_NAME                3 (str)
                       64 LOAD_NAME                4 (__annotations__)
                       66 LOAD_CONST               6 ('last_event_type')
                       68 STORE_SUBSCR
          
-          72          72 LOAD_NAME                5 (int)
+          73          72 LOAD_NAME                5 (int)
                       74 LOAD_NAME                4 (__annotations__)
                       76 LOAD_CONST               7 ('last_rating')
                       78 STORE_SUBSCR
          
-          73          82 LOAD_NAME                7 (dict)
+          74          82 LOAD_NAME                7 (dict)
                       84 LOAD_NAME                4 (__annotations__)
                       86 LOAD_CONST               8 ('meta')
                       88 STORE_SUBSCR
                       92 LOAD_CONST               9 (None)
                       94 RETURN_VALUE
          consts
             'Target'
@@ -773,91 +781,91 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'int', 'List', 'dict')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Target'
-         firstlineno 64
+         firstlineno 65
          lnotab 0x0c020a010a010a010a010a010a010a01
       'Target'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             0000006505650464033c0000006506650464043c0000006506650464053c
             0000006506650464063c0000006506650464073c0000006506650464083c
             0000006506650464093c00000065066504640a3c00000065036504640b3c
             00000065036504640c3c000000640d5300
-          76           0 RESUME                   0
+          77           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Criteria')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          78          12 LOAD_NAME                3 (int)
+          79          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('search_id')
                       18 STORE_SUBSCR
          
-          79          22 LOAD_NAME                5 (str)
+          80          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('type')
                       28 STORE_SUBSCR
          
-          80          32 LOAD_NAME                5 (str)
+          81          32 LOAD_NAME                5 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('prompt')
                       38 STORE_SUBSCR
          
-          81          42 LOAD_NAME                6 (list)
+          82          42 LOAD_NAME                6 (list)
                       44 LOAD_NAME                4 (__annotations__)
                       46 LOAD_CONST               4 ('rating')
                       48 STORE_SUBSCR
          
-          82          52 LOAD_NAME                6 (list)
+          83          52 LOAD_NAME                6 (list)
                       54 LOAD_NAME                4 (__annotations__)
                       56 LOAD_CONST               5 ('employees_range')
                       58 STORE_SUBSCR
          
-          83          62 LOAD_NAME                6 (list)
+          84          62 LOAD_NAME                6 (list)
                       64 LOAD_NAME                4 (__annotations__)
                       66 LOAD_CONST               6 ('country')
                       68 STORE_SUBSCR
          
-          84          72 LOAD_NAME                6 (list)
+          85          72 LOAD_NAME                6 (list)
                       74 LOAD_NAME                4 (__annotations__)
                       76 LOAD_CONST               7 ('state')
                       78 STORE_SUBSCR
          
-          85          82 LOAD_NAME                6 (list)
+          86          82 LOAD_NAME                6 (list)
                       84 LOAD_NAME                4 (__annotations__)
                       86 LOAD_CONST               8 ('ownership')
                       88 STORE_SUBSCR
          
-          86          92 LOAD_NAME                6 (list)
+          87          92 LOAD_NAME                6 (list)
                       94 LOAD_NAME                4 (__annotations__)
                       96 LOAD_CONST               9 ('product')
                       98 STORE_SUBSCR
          
-          87         102 LOAD_NAME                6 (list)
+          88         102 LOAD_NAME                6 (list)
                      104 LOAD_NAME                4 (__annotations__)
                      106 LOAD_CONST              10 ('services')
                      108 STORE_SUBSCR
          
-          88         112 LOAD_NAME                3 (int)
+          89         112 LOAD_NAME                3 (int)
                      114 LOAD_NAME                4 (__annotations__)
                      116 LOAD_CONST              11 ('updated')
                      118 STORE_SUBSCR
          
-          89         122 LOAD_NAME                3 (int)
+          90         122 LOAD_NAME                3 (int)
                      124 LOAD_NAME                4 (__annotations__)
                      126 LOAD_CONST              12 ('actor_id')
                      128 STORE_SUBSCR
                      132 LOAD_CONST              13 (None)
                      134 RETURN_VALUE
          consts
             'Criteria'
@@ -876,15 +884,15 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'list')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Criteria'
-         firstlineno 76
+         firstlineno 77
          lnotab 0x0c020a010a010a010a010a010a010a010a010a010a010a01
       'Criteria'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -893,85 +901,85 @@
             0000006505650464033c000000020065066507ac04a6010000ab01000000
             00000000005a086507650464053c000000020065066507ac04a6010000ab
             0100000000000000005a096507650464063c000000020065066507ac04a6
             010000ab0100000000000000005a0a6507650464073c0000000200650665
             07ac04a6010000ab0100000000000000005a0b6507650464083c00000002
             0065066409ac0aa6010000ab0100000000000000005a0c65036504640b3c
             00000064095300
-          92           0 RESUME                   0
+          93           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          95          12 LOAD_NAME                3 (int)
+          96          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('uid')
                       18 STORE_SUBSCR
          
-          96          22 LOAD_NAME                5 (str)
+          97          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('client_domain')
                       28 STORE_SUBSCR
          
-          97          32 LOAD_NAME                5 (str)
+          98          32 LOAD_NAME                5 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('label')
                       38 STORE_SUBSCR
          
-          98          42 PUSH_NULL
+          99          42 PUSH_NULL
                       44 LOAD_NAME                6 (field)
                       46 LOAD_NAME                7 (dict)
                       48 KW_NAMES                 4
                       50 PRECALL                  1
                       54 CALL                     1
                       64 STORE_NAME               8 (meta)
                       66 LOAD_NAME                7 (dict)
                       68 LOAD_NAME                4 (__annotations__)
                       70 LOAD_CONST               5 ('meta')
                       72 STORE_SUBSCR
          
-          99          76 PUSH_NULL
+         100          76 PUSH_NULL
                       78 LOAD_NAME                6 (field)
                       80 LOAD_NAME                7 (dict)
                       82 KW_NAMES                 4
                       84 PRECALL                  1
                       88 CALL                     1
                       98 STORE_NAME               9 (inclusion)
                      100 LOAD_NAME                7 (dict)
                      102 LOAD_NAME                4 (__annotations__)
                      104 LOAD_CONST               6 ('inclusion')
                      106 STORE_SUBSCR
          
-         100         110 PUSH_NULL
+         101         110 PUSH_NULL
                      112 LOAD_NAME                6 (field)
                      114 LOAD_NAME                7 (dict)
                      116 KW_NAMES                 4
                      118 PRECALL                  1
                      122 CALL                     1
                      132 STORE_NAME              10 (exclusion)
                      134 LOAD_NAME                7 (dict)
                      136 LOAD_NAME                4 (__annotations__)
                      138 LOAD_CONST               7 ('exclusion')
                      140 STORE_SUBSCR
          
-         101         144 PUSH_NULL
+         102         144 PUSH_NULL
                      146 LOAD_NAME                6 (field)
                      148 LOAD_NAME                7 (dict)
                      150 KW_NAMES                 4
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_NAME              11 (sort)
                      168 LOAD_NAME                7 (dict)
                      170 LOAD_NAME                4 (__annotations__)
                      172 LOAD_CONST               8 ('sort')
                      174 STORE_SUBSCR
          
-         102         178 PUSH_NULL
+         103         178 PUSH_NULL
                      180 LOAD_NAME                6 (field)
                      182 LOAD_CONST               9 (None)
                      184 KW_NAMES                10
                      186 PRECALL                  1
                      190 CALL                     1
                      200 STORE_NAME              12 (id)
                      202 LOAD_NAME                3 (int)
@@ -995,48 +1003,48 @@
             'id'
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'inclusion', 'exclusion', 'sort', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
-         firstlineno 92
+         firstlineno 93
          lnotab 0x0c030a010a010a012201220122012201
       'Search'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550067006401a2015a036402640367025a0465
             05650664043c0000006505650664053c00000064065300
-         107           0 RESUME                   0
+         108           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Sort')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         109          12 BUILD_LIST               0
+         110          12 BUILD_LIST               0
                       14 LOAD_CONST               1 (('employee_count', 'rating', 'state', 'country', 'year_founded', 'name'))
                       16 LIST_EXTEND              1
                       18 STORE_NAME               3 (FIELDS)
          
-         110          20 LOAD_CONST               2 ('asc')
+         111          20 LOAD_CONST               2 ('asc')
                       22 LOAD_CONST               3 ('desc')
                       24 BUILD_LIST               2
                       26 STORE_NAME               4 (ORDERS)
          
-         112          28 LOAD_NAME                5 (str)
+         113          28 LOAD_NAME                5 (str)
                       30 LOAD_NAME                6 (__annotations__)
                       32 LOAD_CONST               4 ('field')
                       34 STORE_SUBSCR
          
-         113          38 LOAD_NAME                5 (str)
+         114          38 LOAD_NAME                5 (str)
                       40 LOAD_NAME                6 (__annotations__)
                       42 LOAD_CONST               5 ('order')
                       44 STORE_SUBSCR
                       48 LOAD_CONST               6 (None)
                       50 RETURN_VALUE
          consts
             'Sort'
@@ -1048,23 +1056,23 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'FIELDS', 'ORDERS', 'str', '__annotations__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Sort'
-         firstlineno 107
+         firstlineno 108
          lnotab 0x0c02080108020a01
       'Sort'
       None
    names      ('typing', 'List', 'Optional', 'enum', 'Enum', 'auto', 'dataclasses', 'asdict', 'dataclass', 'field', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Checkpoint', 'Target', 'Criteria', 'Search', 'Sort')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201100110011402020118ff0e010209160118ff0e0102081e0a02
+      0x00ff0201100110011402020118ff0e010209160118ff0e0102081e0b02
       0118ff0e01020b02011aff0e01020502011aff0e010204020118ff0e0102
       06160118ff0e01020b020118ff0e01020f020118ff0e01020e020118ff0e
       01
```

### Comparing `gandai-1.1.3/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,31 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x78095b64 (Wed May 10 03:03:20 2023 UTC)
-files sz: 17549
+moddate:  0xf4ef5c64 (Thu May 11 13:39:00 2023 UTC)
+files sz: 8401
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c036d045a0401
       00640064036c056d065a060100640064046c076d085a086d095a096d0a5a
-      0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064016c0e5a0e640064016c0f5a
-      0f640064056c0f6d105a100100640064066c116d125a120100640064076c
-      136d145a14010002006514a6000000ab0000000000000000000100640884
-      005a1502006515a6000000ab0000000000000000005a1664096509660264
-      0a84045a17640b6508640c65086604640d84045a18640e650b640c650b66
-      04640f84045a196410650c640c650c6604641184045a1a6412650d640c65
-      0d6604641384045a1b641484005a1c64226416651d6417651e6604641884
-      055a1f6416651d640c65026a2000000000000000006604641984045a2164
-      16651d640c65026a2000000000000000006604641a84045a22640c65026a
-      2000000000000000006602641b84045a236416651d640c65026a20000000
-      00000000006604641c84045a246416651d640c650c6604641d84045a2564
-      1e651e640c65096604641f84045a2664096509640c64016604642084045a
-      276410650c640c64016604642184045a2864015300
+      0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064016c0e5a0e640064056c0f6d
+      105a100100640064066c116d125a12010002006512a6000000ab00000000
+      00000000000100640064076c136d145a14010002006514a6000000ab0000
+      000000000000005a15640865096602640984045a16640a6508640b650866
+      04640c84045a17640d650b640b650b6604640e84045a18640f650c640b65
+      0c6604641084045a196411650d640b650d6604641284045a1a641384005a
+      1b64206414651c6415651d6604641684055a1e6414651c640b65026a1f00
+      000000000000006604641784045a206414651c640b65026a1f0000000000
+      0000006604641884045a21640b65026a1f00000000000000006602641984
+      045a226414651c640b65026a1f00000000000000006604641a84045a2364
+      14651c640b650c6604641b84045a24641c651d640b65096604641d84045a
+      2564086509640b64016604641e84045a26640f650c640b64016604641f84
+      045a2764015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (json)
                  8 STORE_NAME               0 (json)
    
@@ -63,1550 +63,1415 @@
                 66 STORE_NAME              12 (Search)
                 68 IMPORT_FROM             13 (Checkpoint)
                 70 STORE_NAME              13 (Checkpoint)
                 72 POP_TOP
    
     15          74 LOAD_CONST               0 (0)
                 76 LOAD_CONST               1 (None)
-                78 IMPORT_NAME             14 (os)
-                80 STORE_NAME              14 (os)
+                78 IMPORT_NAME             14 (sqlalchemy)
+                80 STORE_NAME              14 (sqlalchemy)
    
-    16          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               1 (None)
-                86 IMPORT_NAME             15 (sqlalchemy)
-                88 STORE_NAME              15 (sqlalchemy)
-   
-    17          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               5 (('text',))
-                94 IMPORT_NAME             15 (sqlalchemy)
-                96 IMPORT_FROM             16 (text)
-                98 STORE_NAME              16 (text)
-               100 POP_TOP
-   
-    18         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               6 (('Connector',))
-               106 IMPORT_NAME             17 (google.cloud.sql.connector)
-               108 IMPORT_FROM             18 (Connector)
-               110 STORE_NAME              18 (Connector)
-               112 POP_TOP
-   
-    19         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               7 (('load_dotenv',))
-               118 IMPORT_NAME             19 (dotenv)
-               120 IMPORT_FROM             20 (load_dotenv)
-               122 STORE_NAME              20 (load_dotenv)
+    17          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               5 (('Connector',))
+                86 IMPORT_NAME             15 (google.cloud.sql.connector)
+                88 IMPORT_FROM             16 (Connector)
+                90 STORE_NAME              16 (Connector)
+                92 POP_TOP
+   
+    18          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               6 (('load_dotenv',))
+                98 IMPORT_NAME             17 (dotenv)
+               100 IMPORT_FROM             18 (load_dotenv)
+               102 STORE_NAME              18 (load_dotenv)
+               104 POP_TOP
+   
+    19         106 PUSH_NULL
+               108 LOAD_NAME               18 (load_dotenv)
+               110 PRECALL                  0
+               114 CALL                     0
                124 POP_TOP
    
-    21         126 PUSH_NULL
-               128 LOAD_NAME               20 (load_dotenv)
-               130 PRECALL                  0
-               134 CALL                     0
-               144 POP_TOP
-   
-    24         146 LOAD_CONST               8 (<code object get_engine, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 24>)
-               148 MAKE_FUNCTION            0
-               150 STORE_NAME              21 (get_engine)
-   
-    49         152 PUSH_NULL
-               154 LOAD_NAME               21 (get_engine)
-               156 PRECALL                  0
-               160 CALL                     0
-               170 STORE_NAME              22 (engine)
-   
-    55         172 LOAD_CONST               9 ('company')
-               174 LOAD_NAME                9 (Company)
-               176 BUILD_TUPLE              2
-               178 LOAD_CONST              10 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 55>)
-               180 MAKE_FUNCTION            4 (annotations)
-               182 STORE_NAME              23 (insert_company)
-   
-    69         184 LOAD_CONST              11 ('event')
-               186 LOAD_NAME                8 (Event)
-               188 LOAD_CONST              12 ('return')
-               190 LOAD_NAME                8 (Event)
-               192 BUILD_TUPLE              4
-               194 LOAD_CONST              13 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 69>)
-               196 MAKE_FUNCTION            4 (annotations)
-               198 STORE_NAME              24 (insert_event)
-   
-    90         200 LOAD_CONST              14 ('actor')
-               202 LOAD_NAME               11 (Actor)
-               204 LOAD_CONST              12 ('return')
-               206 LOAD_NAME               11 (Actor)
-               208 BUILD_TUPLE              4
-               210 LOAD_CONST              15 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 90>)
-               212 MAKE_FUNCTION            4 (annotations)
-               214 STORE_NAME              25 (insert_actor)
-   
-   105         216 LOAD_CONST              16 ('search')
-               218 LOAD_NAME               12 (Search)
-               220 LOAD_CONST              12 ('return')
-               222 LOAD_NAME               12 (Search)
-               224 BUILD_TUPLE              4
-               226 LOAD_CONST              17 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 105>)
-               228 MAKE_FUNCTION            4 (annotations)
-               230 STORE_NAME              26 (insert_search)
-   
-   124         232 LOAD_CONST              18 ('checkpoint')
-               234 LOAD_NAME               13 (Checkpoint)
-               236 LOAD_CONST              12 ('return')
-               238 LOAD_NAME               13 (Checkpoint)
-               240 BUILD_TUPLE              4
-               242 LOAD_CONST              19 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 124>)
-               244 MAKE_FUNCTION            4 (annotations)
-               246 STORE_NAME              27 (insert_checkpoint)
-   
-   140         248 LOAD_CONST              20 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 140>)
-               250 MAKE_FUNCTION            0
-               252 STORE_NAME              28 (search)
-   
-   147         254 LOAD_CONST              34 (('advance',))
-               256 LOAD_CONST              22 ('search_uid')
-               258 LOAD_NAME               29 (int)
-               260 LOAD_CONST              23 ('last_event_type')
-               262 LOAD_NAME               30 (str)
-               264 BUILD_TUPLE              4
-               266 LOAD_CONST              24 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 147>)
-               268 MAKE_FUNCTION            5 (defaults, annotations)
-               270 STORE_NAME              31 (target)
-   
-   171         272 LOAD_CONST              22 ('search_uid')
-               274 LOAD_NAME               29 (int)
-               276 LOAD_CONST              12 ('return')
-               278 LOAD_NAME                2 (pd)
-               280 LOAD_ATTR               32 (DataFrame)
-               290 BUILD_TUPLE              4
-               292 LOAD_CONST              25 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 171>)
-               294 MAKE_FUNCTION            4 (annotations)
-               296 STORE_NAME              33 (target_count)
-   
-   187         298 LOAD_CONST              22 ('search_uid')
-               300 LOAD_NAME               29 (int)
-               302 LOAD_CONST              12 ('return')
-               304 LOAD_NAME                2 (pd)
-               306 LOAD_ATTR               32 (DataFrame)
-               316 BUILD_TUPLE              4
-               318 LOAD_CONST              26 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 187>)
-               320 MAKE_FUNCTION            4 (annotations)
-               322 STORE_NAME              34 (event)
-   
-   199         324 LOAD_CONST              12 ('return')
-               326 LOAD_NAME                2 (pd)
-               328 LOAD_ATTR               32 (DataFrame)
-               338 BUILD_TUPLE              2
-               340 LOAD_CONST              27 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 199>)
-               342 MAKE_FUNCTION            4 (annotations)
-               344 STORE_NAME              35 (checkpoint)
-   
-   210         346 LOAD_CONST              22 ('search_uid')
-               348 LOAD_NAME               29 (int)
-               350 LOAD_CONST              12 ('return')
-               352 LOAD_NAME                2 (pd)
-               354 LOAD_ATTR               32 (DataFrame)
-               364 BUILD_TUPLE              4
-               366 LOAD_CONST              28 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 210>)
-               368 MAKE_FUNCTION            4 (annotations)
-               370 STORE_NAME              36 (comment_by_domain)
-   
-   231         372 LOAD_CONST              22 ('search_uid')
-               374 LOAD_NAME               29 (int)
-               376 LOAD_CONST              12 ('return')
-               378 LOAD_NAME               12 (Search)
-               380 BUILD_TUPLE              4
-               382 LOAD_CONST              29 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 231>)
-               384 MAKE_FUNCTION            4 (annotations)
-               386 STORE_NAME              37 (find_search_by_uid)
-   
-   247         388 LOAD_CONST              30 ('domain')
-               390 LOAD_NAME               30 (str)
-               392 LOAD_CONST              12 ('return')
-               394 LOAD_NAME                9 (Company)
-               396 BUILD_TUPLE              4
-               398 LOAD_CONST              31 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 247>)
-               400 MAKE_FUNCTION            4 (annotations)
-               402 STORE_NAME              38 (find_company_by_domain)
-   
-   266         404 LOAD_CONST               9 ('company')
-               406 LOAD_NAME                9 (Company)
-               408 LOAD_CONST              12 ('return')
-               410 LOAD_CONST               1 (None)
-               412 BUILD_TUPLE              4
-               414 LOAD_CONST              32 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 266>)
-               416 MAKE_FUNCTION            4 (annotations)
-               418 STORE_NAME              39 (update_company)
-   
-   290         420 LOAD_CONST              16 ('search')
-               422 LOAD_NAME               12 (Search)
-               424 LOAD_CONST              12 ('return')
-               426 LOAD_CONST               1 (None)
-               428 BUILD_TUPLE              4
-               430 LOAD_CONST              33 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 290>)
-               432 MAKE_FUNCTION            4 (annotations)
-               434 STORE_NAME              40 (update_search)
-               436 LOAD_CONST               1 (None)
-               438 RETURN_VALUE
+    21         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST               7 (('connect_with_connector',))
+               130 IMPORT_NAME             19 (gandai.db)
+               132 IMPORT_FROM             20 (connect_with_connector)
+               134 STORE_NAME              20 (connect_with_connector)
+               136 POP_TOP
+   
+    23         138 PUSH_NULL
+               140 LOAD_NAME               20 (connect_with_connector)
+               142 PRECALL                  0
+               146 CALL                     0
+               156 STORE_NAME              21 (db)
+   
+    29         158 LOAD_CONST               8 ('company')
+               160 LOAD_NAME                9 (Company)
+               162 BUILD_TUPLE              2
+               164 LOAD_CONST               9 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 29>)
+               166 MAKE_FUNCTION            4 (annotations)
+               168 STORE_NAME              22 (insert_company)
+   
+    43         170 LOAD_CONST              10 ('event')
+               172 LOAD_NAME                8 (Event)
+               174 LOAD_CONST              11 ('return')
+               176 LOAD_NAME                8 (Event)
+               178 BUILD_TUPLE              4
+               180 LOAD_CONST              12 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 43>)
+               182 MAKE_FUNCTION            4 (annotations)
+               184 STORE_NAME              23 (insert_event)
+   
+    64         186 LOAD_CONST              13 ('actor')
+               188 LOAD_NAME               11 (Actor)
+               190 LOAD_CONST              11 ('return')
+               192 LOAD_NAME               11 (Actor)
+               194 BUILD_TUPLE              4
+               196 LOAD_CONST              14 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 64>)
+               198 MAKE_FUNCTION            4 (annotations)
+               200 STORE_NAME              24 (insert_actor)
+   
+    79         202 LOAD_CONST              15 ('search')
+               204 LOAD_NAME               12 (Search)
+               206 LOAD_CONST              11 ('return')
+               208 LOAD_NAME               12 (Search)
+               210 BUILD_TUPLE              4
+               212 LOAD_CONST              16 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 79>)
+               214 MAKE_FUNCTION            4 (annotations)
+               216 STORE_NAME              25 (insert_search)
+   
+    98         218 LOAD_CONST              17 ('checkpoint')
+               220 LOAD_NAME               13 (Checkpoint)
+               222 LOAD_CONST              11 ('return')
+               224 LOAD_NAME               13 (Checkpoint)
+               226 BUILD_TUPLE              4
+               228 LOAD_CONST              18 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 98>)
+               230 MAKE_FUNCTION            4 (annotations)
+               232 STORE_NAME              26 (insert_checkpoint)
+   
+   114         234 LOAD_CONST              19 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 114>)
+               236 MAKE_FUNCTION            0
+               238 STORE_NAME              27 (search)
+   
+   121         240 LOAD_CONST              32 ((None,))
+               242 LOAD_CONST              20 ('search_uid')
+               244 LOAD_NAME               28 (int)
+               246 LOAD_CONST              21 ('last_event_type')
+               248 LOAD_NAME               29 (str)
+               250 BUILD_TUPLE              4
+               252 LOAD_CONST              22 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 121>)
+               254 MAKE_FUNCTION            5 (defaults, annotations)
+               256 STORE_NAME              30 (target)
+   
+   153         258 LOAD_CONST              20 ('search_uid')
+               260 LOAD_NAME               28 (int)
+               262 LOAD_CONST              11 ('return')
+               264 LOAD_NAME                2 (pd)
+               266 LOAD_ATTR               31 (DataFrame)
+               276 BUILD_TUPLE              4
+               278 LOAD_CONST              23 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 153>)
+               280 MAKE_FUNCTION            4 (annotations)
+               282 STORE_NAME              32 (target_count)
+   
+   169         284 LOAD_CONST              20 ('search_uid')
+               286 LOAD_NAME               28 (int)
+               288 LOAD_CONST              11 ('return')
+               290 LOAD_NAME                2 (pd)
+               292 LOAD_ATTR               31 (DataFrame)
+               302 BUILD_TUPLE              4
+               304 LOAD_CONST              24 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 169>)
+               306 MAKE_FUNCTION            4 (annotations)
+               308 STORE_NAME              33 (event)
+   
+   181         310 LOAD_CONST              11 ('return')
+               312 LOAD_NAME                2 (pd)
+               314 LOAD_ATTR               31 (DataFrame)
+               324 BUILD_TUPLE              2
+               326 LOAD_CONST              25 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 181>)
+               328 MAKE_FUNCTION            4 (annotations)
+               330 STORE_NAME              34 (checkpoint)
+   
+   192         332 LOAD_CONST              20 ('search_uid')
+               334 LOAD_NAME               28 (int)
+               336 LOAD_CONST              11 ('return')
+               338 LOAD_NAME                2 (pd)
+               340 LOAD_ATTR               31 (DataFrame)
+               350 BUILD_TUPLE              4
+               352 LOAD_CONST              26 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 192>)
+               354 MAKE_FUNCTION            4 (annotations)
+               356 STORE_NAME              35 (comment_by_domain)
+   
+   213         358 LOAD_CONST              20 ('search_uid')
+               360 LOAD_NAME               28 (int)
+               362 LOAD_CONST              11 ('return')
+               364 LOAD_NAME               12 (Search)
+               366 BUILD_TUPLE              4
+               368 LOAD_CONST              27 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 213>)
+               370 MAKE_FUNCTION            4 (annotations)
+               372 STORE_NAME              36 (find_search_by_uid)
+   
+   229         374 LOAD_CONST              28 ('domain')
+               376 LOAD_NAME               29 (str)
+               378 LOAD_CONST              11 ('return')
+               380 LOAD_NAME                9 (Company)
+               382 BUILD_TUPLE              4
+               384 LOAD_CONST              29 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 229>)
+               386 MAKE_FUNCTION            4 (annotations)
+               388 STORE_NAME              37 (find_company_by_domain)
+   
+   248         390 LOAD_CONST               8 ('company')
+               392 LOAD_NAME                9 (Company)
+               394 LOAD_CONST              11 ('return')
+               396 LOAD_CONST               1 (None)
+               398 BUILD_TUPLE              4
+               400 LOAD_CONST              30 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 248>)
+               402 MAKE_FUNCTION            4 (annotations)
+               404 STORE_NAME              38 (update_company)
+   
+   272         406 LOAD_CONST              15 ('search')
+               408 LOAD_NAME               12 (Search)
+               410 LOAD_CONST              11 ('return')
+               412 LOAD_CONST               1 (None)
+               414 BUILD_TUPLE              4
+               416 LOAD_CONST              31 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 272>)
+               418 MAKE_FUNCTION            4 (annotations)
+               420 STORE_NAME              39 (update_search)
+               422 LOAD_CONST               1 (None)
+               424 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('from_dict',)
       ('Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint')
-      ('text',)
       ('Connector',)
       ('load_dotenv',)
-      code
-         argcount  : 0
-         nlocals   : 3
-         stacksize : 5
-         flags     : 3
-         code
-            0x870397007401000000000000000000007403000000000000000000006a
-            0200000000000000006401a6010000ab010000000000000000a6010000ab
-            01000000000000000001007403000000000000000000006a020000000000
-            0000006401a6010000ab01000000000000000064026b0200000000721664
-            037d007407000000000000000000006a0400000000000000007c00a60100
-            00ab01000000000000000053007403000000000000000000006a02000000
-            00000000006401a6010000ab01000000000000000064046b020000000072
-            2b740b00000000000000000000a6000000ab0000000000000000008a0388
-            036601640584087d017407000000000000000000006a0400000000000000
-            0064067c01ac07a6020000ab0200000000000000007d027c025300640053
-            00
-                       0 MAKE_CELL                3 (connector)
-         
-          24           2 RESUME                   0
-         
-          25           4 LOAD_GLOBAL              1 (NULL + print)
-                      16 LOAD_GLOBAL              3 (NULL + os)
-                      28 LOAD_ATTR                2 (getenv)
-                      38 LOAD_CONST               1 ('ENV_STAGE')
-                      40 PRECALL                  1
-                      44 CALL                     1
-                      54 PRECALL                  1
-                      58 CALL                     1
-                      68 POP_TOP
-         
-          26          70 LOAD_GLOBAL              3 (NULL + os)
-                      82 LOAD_ATTR                2 (getenv)
-                      92 LOAD_CONST               1 ('ENV_STAGE')
-                      94 PRECALL                  1
-                      98 CALL                     1
-                     108 LOAD_CONST               2 ('local')
-                     110 COMPARE_OP               2 (==)
-                     116 POP_JUMP_FORWARD_IF_FALSE    22 (to 162)
-         
-          27         118 LOAD_CONST               3 ('postgresql://postgres@localhost/parker')
-                     120 STORE_FAST               0 (DB_URI)
-         
-          28         122 LOAD_GLOBAL              7 (NULL + sqlalchemy)
-                     134 LOAD_ATTR                4 (create_engine)
-                     144 LOAD_FAST                0 (DB_URI)
-                     146 PRECALL                  1
-                     150 CALL                     1
-                     160 RETURN_VALUE
-         
-          29     >>  162 LOAD_GLOBAL              3 (NULL + os)
-                     174 LOAD_ATTR                2 (getenv)
-                     184 LOAD_CONST               1 ('ENV_STAGE')
-                     186 PRECALL                  1
-                     190 CALL                     1
-                     200 LOAD_CONST               4 ('dev')
-                     202 COMPARE_OP               2 (==)
-                     208 POP_JUMP_FORWARD_IF_FALSE    43 (to 296)
-         
-          31         210 LOAD_GLOBAL             11 (NULL + Connector)
-                     222 PRECALL                  0
-                     226 CALL                     0
-                     236 STORE_DEREF              3 (connector)
-         
-          33         238 LOAD_CLOSURE             3 (connector)
-                     240 BUILD_TUPLE              1
-                     242 LOAD_CONST               5 (<code object getconn, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 33>)
-                     244 MAKE_FUNCTION            8 (closure)
-                     246 STORE_FAST               1 (getconn)
-         
-          42         248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
-                     260 LOAD_ATTR                4 (create_engine)
-         
-          43         270 LOAD_CONST               6 ('postgresql+pg8000://')
-         
-          44         272 LOAD_FAST                1 (getconn)
-         
-          42         274 KW_NAMES                 7
-                     276 PRECALL                  2
-                     280 CALL                     2
-                     290 STORE_FAST               2 (pool)
-         
-          46         292 LOAD_FAST                2 (pool)
-                     294 RETURN_VALUE
-         
-          29     >>  296 LOAD_CONST               0 (None)
-                     298 RETURN_VALUE
-         consts
-            None
-            'ENV_STAGE'
-            'local'
-            'postgresql://postgres@localhost/parker'
-            'dev'
-            code
-               argcount  : 0
-               nlocals   : 1
-               stacksize : 9
-               flags     : 19
-               code
-                  0x950197008901a000000000000000000000000000000000000000000074
-                  03000000000000000000006a0200000000000000006401a6010000ab0100
-                  0000000000000064027403000000000000000000006a0200000000000000
-                  006403a6010000ab0100000000000000007403000000000000000000006a
-                  0200000000000000006404a6010000ab0100000000000000007403000000
-                  000000000000006a0200000000000000006405a6010000ab010000000000
-                  000000ac06a6050000ab0500000000000000007d007c005300
-                             0 COPY_FREE_VARS           1
-               
-                33           2 RESUME                   0
-               
-                34           4 LOAD_DEREF               1 (connector)
-                             6 LOAD_METHOD              0 (connect)
-               
-                35          28 LOAD_GLOBAL              3 (NULL + os)
-                            40 LOAD_ATTR                2 (getenv)
-                            50 LOAD_CONST               1 ('INSTANCE_CONNECTION_NAME')
-                            52 PRECALL                  1
-                            56 CALL                     1
-               
-                36          66 LOAD_CONST               2 ('pg8000')
-               
-                37          68 LOAD_GLOBAL              3 (NULL + os)
-                            80 LOAD_ATTR                2 (getenv)
-                            90 LOAD_CONST               3 ('DB_USER')
-                            92 PRECALL                  1
-                            96 CALL                     1
-               
-                38         106 LOAD_GLOBAL              3 (NULL + os)
-                           118 LOAD_ATTR                2 (getenv)
-                           128 LOAD_CONST               4 ('DB_PASS')
-                           130 PRECALL                  1
-                           134 CALL                     1
-               
-                39         144 LOAD_GLOBAL              3 (NULL + os)
-                           156 LOAD_ATTR                2 (getenv)
-                           166 LOAD_CONST               5 ('DB_NAME')
-                           168 PRECALL                  1
-                           172 CALL                     1
-               
-                34         182 KW_NAMES                 6
-                           184 PRECALL                  5
-                           188 CALL                     5
-                           198 STORE_FAST               0 (conn)
-               
-                41         200 LOAD_FAST                0 (conn)
-                           202 RETURN_VALUE
-               consts
-                  None
-                  'INSTANCE_CONNECTION_NAME'
-                  'pg8000'
-                  'DB_USER'
-                  'DB_PASS'
-                  'DB_NAME'
-                  ('user', 'password', 'db')
-               names      ('connect', 'os', 'getenv')
-               varnames   ('conn',)
-               freevars   ('connector',)
-               cellvars   ()
-               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
-               name       'getconn'
-               firstlineno 33
-               lnotab 0x04011801260102012601260126fb1207
-            'postgresql+pg8000://'
-            ('creator',)
-         names      ('print', 'os', 'getenv', 'sqlalchemy', 'create_engine', 'Connector')
-         varnames   ('DB_URI', 'getconn', 'pool')
-         freevars   ()
-         cellvars   ('connector',)
-         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
-         name       'get_engine'
-         firstlineno 24
-         lnotab 0x0401420130010401280130021c020a091601020102fe120404ef
+      ('connect_with_connector',)
       'company'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017405000000
-            000000000000006401a6010000ab0100000000000000007d027c01a00300
-            000000000000000000000000000000000000007c02740900000000000000
-            0000007c00a6010000ab010000000000000000a6020000ab020000000000
-            00000001007c01a0050000000000000000000000000000000000000000a6
-            000000ab0000000000000000000100640064006400a6020000ab02000000
-            000000000001006e0b230031007304770278035900770101005900010001
-            007c005300
-          55           0 RESUME                   0
+            000000000000006a0300000000000000006401a6010000ab010000000000
+            0000007d027c01a00400000000000000000000000000000000000000007c
+            02740b000000000000000000007c00a6010000ab010000000000000000a6
+            020000ab02000000000000000001007c01a0060000000000000000000000
+            000000000000000000a6000000ab00000000000000000001006400640064
+            00a6020000ab02000000000000000001006e0b2300310073047702780359
+            00770101005900010001007c005300
+          29           0 RESUME                   0
          
-          56           2 LOAD_GLOBAL              0 (engine)
+          30           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          57          54 LOAD_GLOBAL              5 (NULL + text)
-         
-          58          66 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
+          31          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                      66 LOAD_ATTR                3 (text)
          
-          57          68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               2 (statement)
-         
-          64          84 LOAD_FAST                1 (con)
-                      86 LOAD_METHOD              3 (execute)
-                     108 LOAD_FAST                2 (statement)
-                     110 LOAD_GLOBAL              9 (NULL + asdict)
-                     122 LOAD_FAST                0 (company)
-                     124 PRECALL                  1
-                     128 CALL                     1
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 POP_TOP
-         
-          65         154 LOAD_FAST                1 (con)
-                     156 LOAD_METHOD              5 (commit)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 POP_TOP
+          32          76 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
          
-          56         194 LOAD_CONST               0 (None)
-                     196 LOAD_CONST               0 (None)
-                     198 LOAD_CONST               0 (None)
-                     200 PRECALL                  2
-                     204 CALL                     2
-                     214 POP_TOP
-                     216 JUMP_FORWARD            11 (to 240)
-                 >>  218 PUSH_EXC_INFO
-                     220 WITH_EXCEPT_START
-                     222 POP_JUMP_FORWARD_IF_TRUE     4 (to 232)
-                     224 RERAISE                  2
-                 >>  226 COPY                     3
-                     228 POP_EXCEPT
-                     230 RERAISE                  1
-                 >>  232 POP_TOP
-                     234 POP_EXCEPT
-                     236 POP_TOP
-                     238 POP_TOP
+          31          78 PRECALL                  1
+                      82 CALL                     1
+                      92 STORE_FAST               2 (statement)
+         
+          38          94 LOAD_FAST                1 (con)
+                      96 LOAD_METHOD              4 (execute)
+                     118 LOAD_FAST                2 (statement)
+                     120 LOAD_GLOBAL             11 (NULL + asdict)
+                     132 LOAD_FAST                0 (company)
+                     134 PRECALL                  1
+                     138 CALL                     1
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+         
+          39         164 LOAD_FAST                1 (con)
+                     166 LOAD_METHOD              6 (commit)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 POP_TOP
+         
+          30         204 LOAD_CONST               0 (None)
+                     206 LOAD_CONST               0 (None)
+                     208 LOAD_CONST               0 (None)
+                     210 PRECALL                  2
+                     214 CALL                     2
+                     224 POP_TOP
+                     226 JUMP_FORWARD            11 (to 250)
+                 >>  228 PUSH_EXC_INFO
+                     230 WITH_EXCEPT_START
+                     232 POP_JUMP_FORWARD_IF_TRUE     4 (to 242)
+                     234 RERAISE                  2
+                 >>  236 COPY                     3
+                     238 POP_EXCEPT
+                     240 RERAISE                  1
+                 >>  242 POP_TOP
+                     244 POP_EXCEPT
+                     246 POP_TOP
+                     248 POP_TOP
          
-          66     >>  240 LOAD_FAST                0 (company)
-                     242 RETURN_VALUE
+          40     >>  250 LOAD_FAST                0 (company)
+                     252 RETURN_VALUE
          ExceptionTable:
-           52 to 192 -> 218 [1] lasti
-           218 to 224 -> 226 [3] lasti
-           232 to 232 -> 226 [3] lasti
+           52 to 202 -> 228 [1] lasti
+           228 to 234 -> 236 [3] lasti
+           242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            '
-         names      ('engine', 'connect', 'text', 'execute', 'asdict', 'commit')
+         names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('company', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_company'
-         firstlineno 55
-         lnotab 0x020134010c0102ff1007460128f72e0a
+         firstlineno 29
+         lnotab 0x02013401160102ff1007460128f72e0a
       'event'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017405000000
-            000000000000006401a6010000ab0100000000000000007d027407000000
-            000000000000007c00a6010000ab0100000000000000007d037409000000
-            000000000000006a0500000000000000007c036402190000000000000000
-            00a6010000ab0100000000000000007c0364023c0000007c01a006000000
-            00000000000000000000000000000000007c027c03a6020000ab02000000
-            00000000007d047c04a00700000000000000000000000000000000000000
-            00a6000000ab0000000000000000007d057c0572087c0564031900000000
-            00000000006e0164007c005f0800000000000000007c01a0060000000000
-            0000000000000000000000000000007405000000000000000000006404a6
-            010000ab010000000000000000a6010000ab01000000000000000001007c
-            01a0090000000000000000000000000000000000000000a6000000ab0000
-            000000000000000100640064006400a6020000ab02000000000000000001
-            006e0b230031007304770278035900770101005900010001007c005300
-          69           0 RESUME                   0
+            000000000000006a0300000000000000006401a6010000ab010000000000
+            0000007d027409000000000000000000007c00a6010000ab010000000000
+            0000007d03740b000000000000000000006a0600000000000000007c0364
+            0219000000000000000000a6010000ab0100000000000000007c0364023c
+            0000007c01a00700000000000000000000000000000000000000007c027c
+            03a6020000ab0200000000000000007d047c04a008000000000000000000
+            0000000000000000000000a6000000ab0000000000000000007d057c0572
+            087c056403190000000000000000006e0164007c005f0900000000000000
+            007c01a00700000000000000000000000000000000000000007405000000
+            000000000000006a0300000000000000006404a6010000ab010000000000
+            000000a6010000ab01000000000000000001007c01a00a00000000000000
+            00000000000000000000000000a6000000ab000000000000000000010064
+            0064006400a6020000ab02000000000000000001006e0b23003100730477
+            0278035900770101005900010001007c005300
+          43           0 RESUME                   0
          
-          70           2 LOAD_GLOBAL              0 (engine)
+          44           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          71          54 LOAD_GLOBAL              5 (NULL + text)
+          45          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                      66 LOAD_ATTR                3 (text)
          
-          72          66 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
-         
-          71          68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               2 (statement)
-         
-          79          84 LOAD_GLOBAL              7 (NULL + asdict)
-                      96 LOAD_FAST                0 (event)
-                      98 PRECALL                  1
-                     102 CALL                     1
-                     112 STORE_FAST               3 (obj)
-         
-          80         114 LOAD_GLOBAL              9 (NULL + json)
-                     126 LOAD_ATTR                5 (dumps)
-                     136 LOAD_FAST                3 (obj)
-                     138 LOAD_CONST               2 ('data')
-                     140 BINARY_SUBSCR
-                     150 PRECALL                  1
-                     154 CALL                     1
-                     164 LOAD_FAST                3 (obj)
-                     166 LOAD_CONST               2 ('data')
-                     168 STORE_SUBSCR
-         
-          81         172 LOAD_FAST                1 (con)
-                     174 LOAD_METHOD              6 (execute)
-                     196 LOAD_FAST                2 (statement)
-                     198 LOAD_FAST                3 (obj)
-                     200 PRECALL                  2
-                     204 CALL                     2
-                     214 STORE_FAST               4 (result)
-         
-          83         216 LOAD_FAST                4 (result)
-                     218 LOAD_METHOD              7 (first)
-                     240 PRECALL                  0
-                     244 CALL                     0
-                     254 STORE_FAST               5 (_id)
-         
-          84         256 LOAD_FAST                5 (_id)
-                     258 POP_JUMP_FORWARD_IF_FALSE     8 (to 276)
-                     260 LOAD_FAST                5 (_id)
-                     262 LOAD_CONST               3 (0)
-                     264 BINARY_SUBSCR
-                     274 JUMP_FORWARD             1 (to 278)
-                 >>  276 LOAD_CONST               0 (None)
-                 >>  278 LOAD_FAST                0 (event)
-                     280 STORE_ATTR               8 (id)
-         
-          85         290 LOAD_FAST                1 (con)
-                     292 LOAD_METHOD              6 (execute)
-                     314 LOAD_GLOBAL              5 (NULL + text)
-                     326 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW target')
-                     328 PRECALL                  1
-                     332 CALL                     1
-                     342 PRECALL                  1
-                     346 CALL                     1
-                     356 POP_TOP
-         
-          86         358 LOAD_FAST                1 (con)
-                     360 LOAD_METHOD              9 (commit)
-                     382 PRECALL                  0
-                     386 CALL                     0
-                     396 POP_TOP
+          46          76 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
          
-          70         398 LOAD_CONST               0 (None)
-                     400 LOAD_CONST               0 (None)
-                     402 LOAD_CONST               0 (None)
-                     404 PRECALL                  2
-                     408 CALL                     2
-                     418 POP_TOP
-                     420 JUMP_FORWARD            11 (to 444)
-                 >>  422 PUSH_EXC_INFO
-                     424 WITH_EXCEPT_START
-                     426 POP_JUMP_FORWARD_IF_TRUE     4 (to 436)
-                     428 RERAISE                  2
-                 >>  430 COPY                     3
-                     432 POP_EXCEPT
-                     434 RERAISE                  1
-                 >>  436 POP_TOP
-                     438 POP_EXCEPT
-                     440 POP_TOP
-                     442 POP_TOP
+          45          78 PRECALL                  1
+                      82 CALL                     1
+                      92 STORE_FAST               2 (statement)
+         
+          53          94 LOAD_GLOBAL              9 (NULL + asdict)
+                     106 LOAD_FAST                0 (event)
+                     108 PRECALL                  1
+                     112 CALL                     1
+                     122 STORE_FAST               3 (obj)
+         
+          54         124 LOAD_GLOBAL             11 (NULL + json)
+                     136 LOAD_ATTR                6 (dumps)
+                     146 LOAD_FAST                3 (obj)
+                     148 LOAD_CONST               2 ('data')
+                     150 BINARY_SUBSCR
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 LOAD_FAST                3 (obj)
+                     176 LOAD_CONST               2 ('data')
+                     178 STORE_SUBSCR
+         
+          55         182 LOAD_FAST                1 (con)
+                     184 LOAD_METHOD              7 (execute)
+                     206 LOAD_FAST                2 (statement)
+                     208 LOAD_FAST                3 (obj)
+                     210 PRECALL                  2
+                     214 CALL                     2
+                     224 STORE_FAST               4 (result)
+         
+          57         226 LOAD_FAST                4 (result)
+                     228 LOAD_METHOD              8 (first)
+                     250 PRECALL                  0
+                     254 CALL                     0
+                     264 STORE_FAST               5 (_id)
+         
+          58         266 LOAD_FAST                5 (_id)
+                     268 POP_JUMP_FORWARD_IF_FALSE     8 (to 286)
+                     270 LOAD_FAST                5 (_id)
+                     272 LOAD_CONST               3 (0)
+                     274 BINARY_SUBSCR
+                     284 JUMP_FORWARD             1 (to 288)
+                 >>  286 LOAD_CONST               0 (None)
+                 >>  288 LOAD_FAST                0 (event)
+                     290 STORE_ATTR               9 (id)
+         
+          59         300 LOAD_FAST                1 (con)
+                     302 LOAD_METHOD              7 (execute)
+                     324 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                     336 LOAD_ATTR                3 (text)
+                     346 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW target')
+                     348 PRECALL                  1
+                     352 CALL                     1
+                     362 PRECALL                  1
+                     366 CALL                     1
+                     376 POP_TOP
+         
+          60         378 LOAD_FAST                1 (con)
+                     380 LOAD_METHOD             10 (commit)
+                     402 PRECALL                  0
+                     406 CALL                     0
+                     416 POP_TOP
+         
+          44         418 LOAD_CONST               0 (None)
+                     420 LOAD_CONST               0 (None)
+                     422 LOAD_CONST               0 (None)
+                     424 PRECALL                  2
+                     428 CALL                     2
+                     438 POP_TOP
+                     440 JUMP_FORWARD            11 (to 464)
+                 >>  442 PUSH_EXC_INFO
+                     444 WITH_EXCEPT_START
+                     446 POP_JUMP_FORWARD_IF_TRUE     4 (to 456)
+                     448 RERAISE                  2
+                 >>  450 COPY                     3
+                     452 POP_EXCEPT
+                     454 RERAISE                  1
+                 >>  456 POP_TOP
+                     458 POP_EXCEPT
+                     460 POP_TOP
+                     462 POP_TOP
          
-          87     >>  444 LOAD_FAST                0 (event)
-                     446 RETURN_VALUE
+          61     >>  464 LOAD_FAST                0 (event)
+                     466 RETURN_VALUE
          ExceptionTable:
-           52 to 396 -> 422 [1] lasti
-           422 to 428 -> 430 [3] lasti
-           436 to 436 -> 430 [3] lasti
+           52 to 416 -> 442 [1] lasti
+           442 to 448 -> 450 [3] lasti
+           456 to 456 -> 450 [3] lasti
          consts
             None
             '\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            '
             'data'
             0
             'REFRESH MATERIALIZED VIEW target'
-         names      ('engine', 'connect', 'text', 'asdict', 'json', 'dumps', 'execute', 'first', 'id', 'commit')
+         names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'first', 'id', 'commit')
          varnames   ('event', 'con', 'statement', 'obj', 'result', '_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_event'
-         firstlineno 69
-         lnotab 0x020134010c0102ff10081e013a012c0228012201440128f02e11
+         firstlineno 43
+         lnotab 0x02013401160102ff10081e013a012c02280122014e0128f02e11
       'actor'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017405000000
-            000000000000006401a6010000ab0100000000000000007d027407000000
-            000000000000007c00a6010000ab0100000000000000007d037c01a00400
-            000000000000000000000000000000000000007c027c03a6020000ab0200
-            0000000000000001007c01a0050000000000000000000000000000000000
-            000000a6000000ab0000000000000000000100640064006400a6020000ab
-            02000000000000000001006e0b2300310073047702780359007701010059
-            00010001007c005300
-          90           0 RESUME                   0
+            000000000000006a0300000000000000006401a6010000ab010000000000
+            0000007d027409000000000000000000007c00a6010000ab010000000000
+            0000007d037c01a00500000000000000000000000000000000000000007c
+            027c03a6020000ab02000000000000000001007c01a00600000000000000
+            00000000000000000000000000a6000000ab000000000000000000010064
+            0064006400a6020000ab02000000000000000001006e0b23003100730477
+            0278035900770101005900010001007c005300
+          64           0 RESUME                   0
          
-          91           2 LOAD_GLOBAL              0 (engine)
+          65           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          92          54 LOAD_GLOBAL              5 (NULL + text)
-         
-          93          66 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
-         
-          92          68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               2 (statement)
-         
-          99          84 LOAD_GLOBAL              7 (NULL + asdict)
-                      96 LOAD_FAST                0 (actor)
-                      98 PRECALL                  1
-                     102 CALL                     1
-                     112 STORE_FAST               3 (obj)
-         
-         100         114 LOAD_FAST                1 (con)
-                     116 LOAD_METHOD              4 (execute)
-                     138 LOAD_FAST                2 (statement)
-                     140 LOAD_FAST                3 (obj)
-                     142 PRECALL                  2
-                     146 CALL                     2
-                     156 POP_TOP
+          66          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                      66 LOAD_ATTR                3 (text)
          
-         101         158 LOAD_FAST                1 (con)
-                     160 LOAD_METHOD              5 (commit)
-                     182 PRECALL                  0
-                     186 CALL                     0
-                     196 POP_TOP
+          67          76 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
          
-          91         198 LOAD_CONST               0 (None)
-                     200 LOAD_CONST               0 (None)
-                     202 LOAD_CONST               0 (None)
-                     204 PRECALL                  2
-                     208 CALL                     2
-                     218 POP_TOP
-                     220 JUMP_FORWARD            11 (to 244)
-                 >>  222 PUSH_EXC_INFO
-                     224 WITH_EXCEPT_START
-                     226 POP_JUMP_FORWARD_IF_TRUE     4 (to 236)
-                     228 RERAISE                  2
-                 >>  230 COPY                     3
-                     232 POP_EXCEPT
-                     234 RERAISE                  1
-                 >>  236 POP_TOP
-                     238 POP_EXCEPT
-                     240 POP_TOP
-                     242 POP_TOP
+          66          78 PRECALL                  1
+                      82 CALL                     1
+                      92 STORE_FAST               2 (statement)
+         
+          73          94 LOAD_GLOBAL              9 (NULL + asdict)
+                     106 LOAD_FAST                0 (actor)
+                     108 PRECALL                  1
+                     112 CALL                     1
+                     122 STORE_FAST               3 (obj)
+         
+          74         124 LOAD_FAST                1 (con)
+                     126 LOAD_METHOD              5 (execute)
+                     148 LOAD_FAST                2 (statement)
+                     150 LOAD_FAST                3 (obj)
+                     152 PRECALL                  2
+                     156 CALL                     2
+                     166 POP_TOP
+         
+          75         168 LOAD_FAST                1 (con)
+                     170 LOAD_METHOD              6 (commit)
+                     192 PRECALL                  0
+                     196 CALL                     0
+                     206 POP_TOP
+         
+          65         208 LOAD_CONST               0 (None)
+                     210 LOAD_CONST               0 (None)
+                     212 LOAD_CONST               0 (None)
+                     214 PRECALL                  2
+                     218 CALL                     2
+                     228 POP_TOP
+                     230 JUMP_FORWARD            11 (to 254)
+                 >>  232 PUSH_EXC_INFO
+                     234 WITH_EXCEPT_START
+                     236 POP_JUMP_FORWARD_IF_TRUE     4 (to 246)
+                     238 RERAISE                  2
+                 >>  240 COPY                     3
+                     242 POP_EXCEPT
+                     244 RERAISE                  1
+                 >>  246 POP_TOP
+                     248 POP_EXCEPT
+                     250 POP_TOP
+                     252 POP_TOP
          
-         102     >>  244 LOAD_FAST                0 (actor)
-                     246 RETURN_VALUE
+          76     >>  254 LOAD_FAST                0 (actor)
+                     256 RETURN_VALUE
          ExceptionTable:
-           52 to 196 -> 222 [1] lasti
-           222 to 228 -> 230 [3] lasti
-           236 to 236 -> 230 [3] lasti
+           52 to 206 -> 232 [1] lasti
+           232 to 238 -> 240 [3] lasti
+           246 to 246 -> 240 [3] lasti
          consts
             None
             '\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            '
-         names      ('engine', 'connect', 'text', 'asdict', 'execute', 'commit')
+         names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'execute', 'commit')
          varnames   ('actor', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_actor'
-         firstlineno 90
-         lnotab 0x020134010c0102ff10071e012c0128f62e0b
+         firstlineno 64
+         lnotab 0x02013401160102ff10071e012c0128f62e0b
       'search'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017405000000
-            000000000000006401a6010000ab0100000000000000007d027407000000
-            000000000000007c00a6010000ab0100000000000000007d037409000000
-            000000000000006a0500000000000000007c036402190000000000000000
-            00a6010000ab0100000000000000007c0364023c00000074090000000000
-            00000000006a0500000000000000007c03640319000000000000000000a6
-            010000ab0100000000000000007c0364033c000000740900000000000000
-            0000006a0500000000000000007c03640419000000000000000000a60100
-            00ab0100000000000000007c0364043c0000007409000000000000000000
-            006a0500000000000000007c03640519000000000000000000a6010000ab
-            0100000000000000007c0364053c0000007c01a006000000000000000000
-            00000000000000000000007c027c03a6020000ab02000000000000000001
-            007c01a0070000000000000000000000000000000000000000a6000000ab
-            0000000000000000000100640064006400a6020000ab0200000000000000
-            0001006e0b230031007304770278035900770101005900010001007c0053
-            00
-         105           0 RESUME                   0
+            000000000000006a0300000000000000006401a6010000ab010000000000
+            0000007d027409000000000000000000007c00a6010000ab010000000000
+            0000007d03740b000000000000000000006a0600000000000000007c0364
+            0219000000000000000000a6010000ab0100000000000000007c0364023c
+            000000740b000000000000000000006a0600000000000000007c03640319
+            000000000000000000a6010000ab0100000000000000007c0364033c0000
+            00740b000000000000000000006a0600000000000000007c036404190000
+            00000000000000a6010000ab0100000000000000007c0364043c00000074
+            0b000000000000000000006a0600000000000000007c0364051900000000
+            0000000000a6010000ab0100000000000000007c0364053c0000007c01a0
+            0700000000000000000000000000000000000000007c027c03a6020000ab
+            02000000000000000001007c01a008000000000000000000000000000000
+            0000000000a6000000ab0000000000000000000100640064006400a60200
+            00ab02000000000000000001006e0b230031007304770278035900770101
+            005900010001007c005300
+          79           0 RESUME                   0
          
-         106           2 LOAD_GLOBAL              0 (engine)
+          80           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         107          54 LOAD_GLOBAL              5 (NULL + text)
+          81          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                      66 LOAD_ATTR                3 (text)
          
-         108          66 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
+          82          76 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
          
-         107          68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               2 (statement)
-         
-         114          84 LOAD_GLOBAL              7 (NULL + asdict)
-                      96 LOAD_FAST                0 (search)
-                      98 PRECALL                  1
-                     102 CALL                     1
-                     112 STORE_FAST               3 (obj)
-         
-         115         114 LOAD_GLOBAL              9 (NULL + json)
-                     126 LOAD_ATTR                5 (dumps)
-                     136 LOAD_FAST                3 (obj)
-                     138 LOAD_CONST               2 ('meta')
-                     140 BINARY_SUBSCR
-                     150 PRECALL                  1
-                     154 CALL                     1
-                     164 LOAD_FAST                3 (obj)
-                     166 LOAD_CONST               2 ('meta')
-                     168 STORE_SUBSCR
-         
-         116         172 LOAD_GLOBAL              9 (NULL + json)
-                     184 LOAD_ATTR                5 (dumps)
-                     194 LOAD_FAST                3 (obj)
-                     196 LOAD_CONST               3 ('inclusion')
-                     198 BINARY_SUBSCR
-                     208 PRECALL                  1
-                     212 CALL                     1
-                     222 LOAD_FAST                3 (obj)
-                     224 LOAD_CONST               3 ('inclusion')
-                     226 STORE_SUBSCR
-         
-         117         230 LOAD_GLOBAL              9 (NULL + json)
-                     242 LOAD_ATTR                5 (dumps)
-                     252 LOAD_FAST                3 (obj)
-                     254 LOAD_CONST               4 ('exclusion')
-                     256 BINARY_SUBSCR
-                     266 PRECALL                  1
-                     270 CALL                     1
-                     280 LOAD_FAST                3 (obj)
-                     282 LOAD_CONST               4 ('exclusion')
-                     284 STORE_SUBSCR
-         
-         118         288 LOAD_GLOBAL              9 (NULL + json)
-                     300 LOAD_ATTR                5 (dumps)
-                     310 LOAD_FAST                3 (obj)
-                     312 LOAD_CONST               5 ('sort')
-                     314 BINARY_SUBSCR
-                     324 PRECALL                  1
-                     328 CALL                     1
-                     338 LOAD_FAST                3 (obj)
-                     340 LOAD_CONST               5 ('sort')
-                     342 STORE_SUBSCR
-         
-         119         346 LOAD_FAST                1 (con)
-                     348 LOAD_METHOD              6 (execute)
-                     370 LOAD_FAST                2 (statement)
-                     372 LOAD_FAST                3 (obj)
-                     374 PRECALL                  2
-                     378 CALL                     2
-                     388 POP_TOP
+          81          78 PRECALL                  1
+                      82 CALL                     1
+                      92 STORE_FAST               2 (statement)
+         
+          88          94 LOAD_GLOBAL              9 (NULL + asdict)
+                     106 LOAD_FAST                0 (search)
+                     108 PRECALL                  1
+                     112 CALL                     1
+                     122 STORE_FAST               3 (obj)
+         
+          89         124 LOAD_GLOBAL             11 (NULL + json)
+                     136 LOAD_ATTR                6 (dumps)
+                     146 LOAD_FAST                3 (obj)
+                     148 LOAD_CONST               2 ('meta')
+                     150 BINARY_SUBSCR
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 LOAD_FAST                3 (obj)
+                     176 LOAD_CONST               2 ('meta')
+                     178 STORE_SUBSCR
+         
+          90         182 LOAD_GLOBAL             11 (NULL + json)
+                     194 LOAD_ATTR                6 (dumps)
+                     204 LOAD_FAST                3 (obj)
+                     206 LOAD_CONST               3 ('inclusion')
+                     208 BINARY_SUBSCR
+                     218 PRECALL                  1
+                     222 CALL                     1
+                     232 LOAD_FAST                3 (obj)
+                     234 LOAD_CONST               3 ('inclusion')
+                     236 STORE_SUBSCR
+         
+          91         240 LOAD_GLOBAL             11 (NULL + json)
+                     252 LOAD_ATTR                6 (dumps)
+                     262 LOAD_FAST                3 (obj)
+                     264 LOAD_CONST               4 ('exclusion')
+                     266 BINARY_SUBSCR
+                     276 PRECALL                  1
+                     280 CALL                     1
+                     290 LOAD_FAST                3 (obj)
+                     292 LOAD_CONST               4 ('exclusion')
+                     294 STORE_SUBSCR
+         
+          92         298 LOAD_GLOBAL             11 (NULL + json)
+                     310 LOAD_ATTR                6 (dumps)
+                     320 LOAD_FAST                3 (obj)
+                     322 LOAD_CONST               5 ('sort')
+                     324 BINARY_SUBSCR
+                     334 PRECALL                  1
+                     338 CALL                     1
+                     348 LOAD_FAST                3 (obj)
+                     350 LOAD_CONST               5 ('sort')
+                     352 STORE_SUBSCR
+         
+          93         356 LOAD_FAST                1 (con)
+                     358 LOAD_METHOD              7 (execute)
+                     380 LOAD_FAST                2 (statement)
+                     382 LOAD_FAST                3 (obj)
+                     384 PRECALL                  2
+                     388 CALL                     2
+                     398 POP_TOP
+         
+          94         400 LOAD_FAST                1 (con)
+                     402 LOAD_METHOD              8 (commit)
+                     424 PRECALL                  0
+                     428 CALL                     0
+                     438 POP_TOP
+         
+          80         440 LOAD_CONST               0 (None)
+                     442 LOAD_CONST               0 (None)
+                     444 LOAD_CONST               0 (None)
+                     446 PRECALL                  2
+                     450 CALL                     2
+                     460 POP_TOP
+                     462 JUMP_FORWARD            11 (to 486)
+                 >>  464 PUSH_EXC_INFO
+                     466 WITH_EXCEPT_START
+                     468 POP_JUMP_FORWARD_IF_TRUE     4 (to 478)
+                     470 RERAISE                  2
+                 >>  472 COPY                     3
+                     474 POP_EXCEPT
+                     476 RERAISE                  1
+                 >>  478 POP_TOP
+                     480 POP_EXCEPT
+                     482 POP_TOP
+                     484 POP_TOP
          
-         120         390 LOAD_FAST                1 (con)
-                     392 LOAD_METHOD              7 (commit)
-                     414 PRECALL                  0
-                     418 CALL                     0
-                     428 POP_TOP
-         
-         106         430 LOAD_CONST               0 (None)
-                     432 LOAD_CONST               0 (None)
-                     434 LOAD_CONST               0 (None)
-                     436 PRECALL                  2
-                     440 CALL                     2
-                     450 POP_TOP
-                     452 JUMP_FORWARD            11 (to 476)
-                 >>  454 PUSH_EXC_INFO
-                     456 WITH_EXCEPT_START
-                     458 POP_JUMP_FORWARD_IF_TRUE     4 (to 468)
-                     460 RERAISE                  2
-                 >>  462 COPY                     3
-                     464 POP_EXCEPT
-                     466 RERAISE                  1
-                 >>  468 POP_TOP
-                     470 POP_EXCEPT
-                     472 POP_TOP
-                     474 POP_TOP
-         
-         121     >>  476 LOAD_FAST                0 (search)
-                     478 RETURN_VALUE
+          95     >>  486 LOAD_FAST                0 (search)
+                     488 RETURN_VALUE
          ExceptionTable:
-           52 to 428 -> 454 [1] lasti
-           454 to 460 -> 462 [3] lasti
-           468 to 468 -> 462 [3] lasti
+           52 to 438 -> 464 [1] lasti
+           464 to 470 -> 472 [3] lasti
+           478 to 478 -> 472 [3] lasti
          consts
             None
             '\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            '
             'meta'
             'inclusion'
             'exclusion'
             'sort'
-         names      ('engine', 'connect', 'text', 'asdict', 'json', 'dumps', 'execute', 'commit')
+         names      ('db', 'connect', 'sqlalchemy', 'text', 'asdict', 'json', 'dumps', 'execute', 'commit')
          varnames   ('search', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
-         firstlineno 105
-         lnotab 0x020134010c0102ff10071e013a013a013a013a012c0128f22e0f
+         firstlineno 79
+         lnotab 0x02013401160102ff10071e013a013a013a013a012c0128f22e0f
       'checkpoint'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017405000000
-            000000000000006401a6010000ab0100000000000000007d027c01a00300
-            000000000000000000000000000000000000007c02740900000000000000
-            0000007c00a6010000ab010000000000000000a6020000ab020000000000
-            00000001007c01a0050000000000000000000000000000000000000000a6
-            000000ab0000000000000000000100640064006400a6020000ab02000000
-            000000000001006e0b230031007304770278035900770101005900010001
-            007c005300
-         124           0 RESUME                   0
+            000000000000006a0300000000000000006401a6010000ab010000000000
+            0000007d027c01a00400000000000000000000000000000000000000007c
+            02740b000000000000000000007c00a6010000ab010000000000000000a6
+            020000ab02000000000000000001007c01a0060000000000000000000000
+            000000000000000000a6000000ab00000000000000000001006400640064
+            00a6020000ab02000000000000000001006e0b2300310073047702780359
+            00770101005900010001007c005300
+          98           0 RESUME                   0
          
-         125           2 LOAD_GLOBAL              0 (engine)
+          99           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         126          54 LOAD_GLOBAL              5 (NULL + text)
-         
-         127          66 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
+         100          54 LOAD_GLOBAL              5 (NULL + sqlalchemy)
+                      66 LOAD_ATTR                3 (text)
          
-         126          68 PRECALL                  1
-                      72 CALL                     1
-                      82 STORE_FAST               2 (statement)
-         
-         132          84 LOAD_FAST                1 (con)
-                      86 LOAD_METHOD              3 (execute)
-                     108 LOAD_FAST                2 (statement)
-                     110 LOAD_GLOBAL              9 (NULL + asdict)
-                     122 LOAD_FAST                0 (checkpoint)
-                     124 PRECALL                  1
-                     128 CALL                     1
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 POP_TOP
+         101          76 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
          
-         133         154 LOAD_FAST                1 (con)
-                     156 LOAD_METHOD              5 (commit)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 POP_TOP
-         
-         125         194 LOAD_CONST               0 (None)
-                     196 LOAD_CONST               0 (None)
-                     198 LOAD_CONST               0 (None)
-                     200 PRECALL                  2
-                     204 CALL                     2
-                     214 POP_TOP
-                     216 JUMP_FORWARD            11 (to 240)
-                 >>  218 PUSH_EXC_INFO
-                     220 WITH_EXCEPT_START
-                     222 POP_JUMP_FORWARD_IF_TRUE     4 (to 232)
-                     224 RERAISE                  2
-                 >>  226 COPY                     3
-                     228 POP_EXCEPT
-                     230 RERAISE                  1
-                 >>  232 POP_TOP
-                     234 POP_EXCEPT
-                     236 POP_TOP
-                     238 POP_TOP
+         100          78 PRECALL                  1
+                      82 CALL                     1
+                      92 STORE_FAST               2 (statement)
+         
+         106          94 LOAD_FAST                1 (con)
+                      96 LOAD_METHOD              4 (execute)
+                     118 LOAD_FAST                2 (statement)
+                     120 LOAD_GLOBAL             11 (NULL + asdict)
+                     132 LOAD_FAST                0 (checkpoint)
+                     134 PRECALL                  1
+                     138 CALL                     1
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+         
+         107         164 LOAD_FAST                1 (con)
+                     166 LOAD_METHOD              6 (commit)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 POP_TOP
+         
+          99         204 LOAD_CONST               0 (None)
+                     206 LOAD_CONST               0 (None)
+                     208 LOAD_CONST               0 (None)
+                     210 PRECALL                  2
+                     214 CALL                     2
+                     224 POP_TOP
+                     226 JUMP_FORWARD            11 (to 250)
+                 >>  228 PUSH_EXC_INFO
+                     230 WITH_EXCEPT_START
+                     232 POP_JUMP_FORWARD_IF_TRUE     4 (to 242)
+                     234 RERAISE                  2
+                 >>  236 COPY                     3
+                     238 POP_EXCEPT
+                     240 RERAISE                  1
+                 >>  242 POP_TOP
+                     244 POP_EXCEPT
+                     246 POP_TOP
+                     248 POP_TOP
          
-         134     >>  240 LOAD_FAST                0 (checkpoint)
-                     242 RETURN_VALUE
+         108     >>  250 LOAD_FAST                0 (checkpoint)
+                     252 RETURN_VALUE
          ExceptionTable:
-           52 to 192 -> 218 [1] lasti
-           218 to 224 -> 226 [3] lasti
-           232 to 232 -> 226 [3] lasti
+           52 to 202 -> 228 [1] lasti
+           228 to 234 -> 236 [3] lasti
+           242 to 242 -> 236 [3] lasti
          consts
             None
             '\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            '
-         names      ('engine', 'connect', 'text', 'execute', 'asdict', 'commit')
+         names      ('db', 'connect', 'sqlalchemy', 'text', 'execute', 'asdict', 'commit')
          varnames   ('checkpoint', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_checkpoint'
-         firstlineno 124
-         lnotab 0x020134010c0102ff1006460128f82e09
+         firstlineno 98
+         lnotab 0x02013401160102ff1006460128f82e09
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d007c00a00200
             000000000000000000000000000000000000007407000000000000000000
-            006401a6010000ab010000000000000000a6010000ab0100000000000000
-            007d017409000000000000000000006a0500000000000000007c01a00600
-            00000000000000000000000000000000000000a6000000ab000000000000
-            0000007c01a0070000000000000000000000000000000000000000a60000
-            00ab000000000000000000ac02a6020000ab0200000000000000007d0264
-            0064006400a6020000ab02000000000000000001006e0b23003100730477
-            0278035900770101005900010001007c025300
-         140           0 RESUME                   0
+            006a0400000000000000006401a6010000ab010000000000000000a60100
+            00ab0100000000000000007d01740b000000000000000000006a06000000
+            00000000007c01a0070000000000000000000000000000000000000000a6
+            000000ab0000000000000000007c01a00800000000000000000000000000
+            00000000000000a6000000ab000000000000000000ac02a6020000ab0200
+            000000000000007d02640064006400a6020000ab02000000000000000001
+            006e0b230031007304770278035900770101005900010001007c025300
+         114           0 RESUME                   0
          
-         141           2 LOAD_GLOBAL              0 (engine)
+         115           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         142          54 LOAD_FAST                0 (conn)
+         116          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
-                      78 LOAD_GLOBAL              7 (NULL + text)
-                      90 LOAD_CONST               1 ("SELECT *, meta->>'group' as group FROM search")
-                      92 PRECALL                  1
-                      96 CALL                     1
-                     106 PRECALL                  1
-                     110 CALL                     1
-                     120 STORE_FAST               1 (result)
-         
-         143         122 LOAD_GLOBAL              9 (NULL + pd)
-                     134 LOAD_ATTR                5 (DataFrame)
-                     144 LOAD_FAST                1 (result)
-                     146 LOAD_METHOD              6 (fetchall)
-                     168 PRECALL                  0
-                     172 CALL                     0
-                     182 LOAD_FAST                1 (result)
-                     184 LOAD_METHOD              7 (keys)
-                     206 PRECALL                  0
-                     210 CALL                     0
-                     220 KW_NAMES                 2
-                     222 PRECALL                  2
-                     226 CALL                     2
-                     236 STORE_FAST               2 (df)
+                      78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      90 LOAD_ATTR                4 (text)
+                     100 LOAD_CONST               1 ("SELECT *, meta->>'group' as group FROM search")
+                     102 PRECALL                  1
+                     106 CALL                     1
+                     116 PRECALL                  1
+                     120 CALL                     1
+                     130 STORE_FAST               1 (result)
+         
+         117         132 LOAD_GLOBAL             11 (NULL + pd)
+                     144 LOAD_ATTR                6 (DataFrame)
+                     154 LOAD_FAST                1 (result)
+                     156 LOAD_METHOD              7 (fetchall)
+                     178 PRECALL                  0
+                     182 CALL                     0
+                     192 LOAD_FAST                1 (result)
+                     194 LOAD_METHOD              8 (keys)
+                     216 PRECALL                  0
+                     220 CALL                     0
+                     230 KW_NAMES                 2
+                     232 PRECALL                  2
+                     236 CALL                     2
+                     246 STORE_FAST               2 (df)
          
-         141         238 LOAD_CONST               0 (None)
-                     240 LOAD_CONST               0 (None)
-                     242 LOAD_CONST               0 (None)
-                     244 PRECALL                  2
-                     248 CALL                     2
-                     258 POP_TOP
-                     260 JUMP_FORWARD            11 (to 284)
-                 >>  262 PUSH_EXC_INFO
-                     264 WITH_EXCEPT_START
-                     266 POP_JUMP_FORWARD_IF_TRUE     4 (to 276)
-                     268 RERAISE                  2
-                 >>  270 COPY                     3
-                     272 POP_EXCEPT
-                     274 RERAISE                  1
-                 >>  276 POP_TOP
-                     278 POP_EXCEPT
-                     280 POP_TOP
-                     282 POP_TOP
+         115         248 LOAD_CONST               0 (None)
+                     250 LOAD_CONST               0 (None)
+                     252 LOAD_CONST               0 (None)
+                     254 PRECALL                  2
+                     258 CALL                     2
+                     268 POP_TOP
+                     270 JUMP_FORWARD            11 (to 294)
+                 >>  272 PUSH_EXC_INFO
+                     274 WITH_EXCEPT_START
+                     276 POP_JUMP_FORWARD_IF_TRUE     4 (to 286)
+                     278 RERAISE                  2
+                 >>  280 COPY                     3
+                     282 POP_EXCEPT
+                     284 RERAISE                  1
+                 >>  286 POP_TOP
+                     288 POP_EXCEPT
+                     290 POP_TOP
+                     292 POP_TOP
          
-         144     >>  284 LOAD_FAST                2 (df)
-                     286 RETURN_VALUE
+         118     >>  294 LOAD_FAST                2 (df)
+                     296 RETURN_VALUE
          ExceptionTable:
-           52 to 236 -> 262 [1] lasti
-           262 to 268 -> 270 [3] lasti
-           276 to 276 -> 270 [3] lasti
+           52 to 246 -> 272 [1] lasti
+           272 to 278 -> 280 [3] lasti
+           286 to 286 -> 280 [3] lasti
          consts
             None
             "SELECT *, meta->>'group' as group FROM search"
             ('columns',)
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 140
-         lnotab 0x02013401440174fe2e03
-      'advance'
+         firstlineno 114
+         lnotab 0x020134014e0174fe2e03
       'search_uid'
       'last_event_type'
       code
          argcount  : 2
          nlocals   : 8
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
-            00000000000000a6000000ab00000000000000000035007d0264017d037c
-            02a002000000000000000000000000000000000000000074070000000000
-            00000000007c03a6010000ab0100000000000000007c007c0164029c02a6
-            020000ab0200000000000000007d047409000000000000000000006a0500
-            000000000000007c04a00600000000000000000000000000000000000000
-            00a6000000ab0000000000000000007c04a0070000000000000000000000
-            000000000000000000a6000000ab000000000000000000ac03a6020000ab
-            0200000000000000007d05640064006400a6020000ab0200000000000000
-            0001006e0b23003100730477027803590077010100590001000100741100
-            0000000000000000007c00a6010000ab0100000000000000007d067c05a0
-            0900000000000000000000000000000000000000007c0664046405ac06a6
-            030000ab0300000000000000007d057415000000000000000000007c00a6
-            010000ab0100000000000000007d077c05a00b0000000000000000000000
-            0000000000000000007c076a0c0000000000000000a00d00000000000000
-            0000000000000000000000000064076404a6020000ab0200000000000000
-            007c076a0c0000000000000000a00d000000000000000000000000000000
-            00000000006408a6010000ab01000000000000000064096b0200000000ac
-            0aa6020000ab0200000000000000007d057c055300
-         147           0 RESUME                   0
+            00000000000000a6000000ab00000000000000000035007d027c01812e64
+            017d037c02a0020000000000000000000000000000000000000000740700
+            0000000000000000006a0400000000000000007c03a6010000ab01000000
+            00000000007c007c0164029c02a6020000ab0200000000000000007d046e
+            2c64037d037c02a002000000000000000000000000000000000000000074
+            07000000000000000000006a0400000000000000007c03a6010000ab0100
+            0000000000000064047c006901a6020000ab0200000000000000007d0474
+            0b000000000000000000006a0600000000000000007c04a0070000000000
+            000000000000000000000000000000a6000000ab0000000000000000007c
+            04a0080000000000000000000000000000000000000000a6000000ab0000
+            00000000000000ac05a6020000ab0200000000000000007d056400640064
+            00a6020000ab02000000000000000001006e0b2300310073047702780359
+            00770101005900010001007413000000000000000000007c00a6010000ab
+            0100000000000000007d067c05a00a000000000000000000000000000000
+            00000000007c0664066407ac08a6030000ab0300000000000000007d0574
+            17000000000000000000007c00a6010000ab0100000000000000007d077c
+            05a00c00000000000000000000000000000000000000007c076a0d000000
+            0000000000a00e0000000000000000000000000000000000000000640964
+            06a6020000ab0200000000000000007c076a0d0000000000000000a00e00
+            00000000000000000000000000000000000000640aa6010000ab01000000
+            0000000000640b6b0200000000ac0ca6020000ab0200000000000000007d
+            057c055300
+         121           0 RESUME                   0
          
-         148           2 LOAD_GLOBAL              0 (engine)
+         122           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               2 (conn)
          
-         149          54 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
-                      56 STORE_FAST               3 (statement)
+         123          54 LOAD_FAST                1 (last_event_type)
+                      56 POP_JUMP_FORWARD_IF_NONE    46 (to 150)
          
-         150          58 LOAD_FAST                2 (conn)
-                      60 LOAD_METHOD              2 (execute)
+         124          58 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
+                      60 STORE_FAST               3 (statement)
          
-         151          82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                3 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-         
-         152         110 LOAD_FAST                0 (search_uid)
-                     112 LOAD_FAST                1 (last_event_type)
-                     114 LOAD_CONST               2 (('search_uid', 'last_event_type'))
-                     116 BUILD_CONST_KEY_MAP      2
-         
-         150         118 PRECALL                  2
-                     122 CALL                     2
-                     132 STORE_FAST               4 (result)
-         
-         154         134 LOAD_GLOBAL              9 (NULL + pd)
-                     146 LOAD_ATTR                5 (DataFrame)
-                     156 LOAD_FAST                4 (result)
-                     158 LOAD_METHOD              6 (fetchall)
-                     180 PRECALL                  0
-                     184 CALL                     0
-                     194 LOAD_FAST                4 (result)
-                     196 LOAD_METHOD              7 (keys)
-                     218 PRECALL                  0
-                     222 CALL                     0
-                     232 KW_NAMES                 3
-                     234 PRECALL                  2
-                     238 CALL                     2
-                     248 STORE_FAST               5 (targets)
+         125          62 LOAD_FAST                2 (conn)
+                      64 LOAD_METHOD              2 (execute)
          
-         148         250 LOAD_CONST               0 (None)
-                     252 LOAD_CONST               0 (None)
-                     254 LOAD_CONST               0 (None)
-                     256 PRECALL                  2
-                     260 CALL                     2
-                     270 POP_TOP
-                     272 JUMP_FORWARD            11 (to 296)
-                 >>  274 PUSH_EXC_INFO
-                     276 WITH_EXCEPT_START
-                     278 POP_JUMP_FORWARD_IF_TRUE     4 (to 288)
-                     280 RERAISE                  2
-                 >>  282 COPY                     3
-                     284 POP_EXCEPT
-                     286 RERAISE                  1
-                 >>  288 POP_TOP
-                     290 POP_EXCEPT
-                     292 POP_TOP
-                     294 POP_TOP
+         126          86 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      98 LOAD_ATTR                4 (text)
+                     108 LOAD_FAST                3 (statement)
+                     110 PRECALL                  1
+                     114 CALL                     1
+         
+         127         124 LOAD_FAST                0 (search_uid)
+                     126 LOAD_FAST                1 (last_event_type)
+                     128 LOAD_CONST               2 (('search_uid', 'last_event_type'))
+                     130 BUILD_CONST_KEY_MAP      2
+         
+         125         132 PRECALL                  2
+                     136 CALL                     2
+                     146 STORE_FAST               4 (result)
+                     148 JUMP_FORWARD            44 (to 238)
+         
+         131     >>  150 LOAD_CONST               3 ('SELECT * FROM target WHERE search_uid = :search_uid')
+                     152 STORE_FAST               3 (statement)
+         
+         132         154 LOAD_FAST                2 (conn)
+                     156 LOAD_METHOD              2 (execute)
+         
+         133         178 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                     190 LOAD_ATTR                4 (text)
+                     200 LOAD_FAST                3 (statement)
+                     202 PRECALL                  1
+                     206 CALL                     1
+         
+         134         216 LOAD_CONST               4 ('search_uid')
+                     218 LOAD_FAST                0 (search_uid)
+                     220 BUILD_MAP                1
+         
+         132         222 PRECALL                  2
+                     226 CALL                     2
+                     236 STORE_FAST               4 (result)
+         
+         137     >>  238 LOAD_GLOBAL             11 (NULL + pd)
+                     250 LOAD_ATTR                6 (DataFrame)
+                     260 LOAD_FAST                4 (result)
+                     262 LOAD_METHOD              7 (fetchall)
+                     284 PRECALL                  0
+                     288 CALL                     0
+                     298 LOAD_FAST                4 (result)
+                     300 LOAD_METHOD              8 (keys)
+                     322 PRECALL                  0
+                     326 CALL                     0
+                     336 KW_NAMES                 5
+                     338 PRECALL                  2
+                     342 CALL                     2
+                     352 STORE_FAST               5 (targets)
+         
+         122         354 LOAD_CONST               0 (None)
+                     356 LOAD_CONST               0 (None)
+                     358 LOAD_CONST               0 (None)
+                     360 PRECALL                  2
+                     364 CALL                     2
+                     374 POP_TOP
+                     376 JUMP_FORWARD            11 (to 400)
+                 >>  378 PUSH_EXC_INFO
+                     380 WITH_EXCEPT_START
+                     382 POP_JUMP_FORWARD_IF_TRUE     4 (to 392)
+                     384 RERAISE                  2
+                 >>  386 COPY                     3
+                     388 POP_EXCEPT
+                     390 RERAISE                  1
+                 >>  392 POP_TOP
+                     394 POP_EXCEPT
+                     396 POP_TOP
+                     398 POP_TOP
          
-         156     >>  296 LOAD_GLOBAL             17 (NULL + comment_by_domain)
-                     308 LOAD_FAST                0 (search_uid)
-                     310 PRECALL                  1
-                     314 CALL                     1
-                     324 STORE_FAST               6 (comments)
-         
-         157         326 LOAD_FAST                5 (targets)
-                     328 LOAD_METHOD              9 (merge)
-                     350 LOAD_FAST                6 (comments)
-                     352 LOAD_CONST               4 ('domain')
-                     354 LOAD_CONST               5 ('left')
-                     356 KW_NAMES                 6
-                     358 PRECALL                  3
-                     362 CALL                     3
-                     372 STORE_FAST               5 (targets)
-         
-         161         374 LOAD_GLOBAL             21 (NULL + find_search_by_uid)
-                     386 LOAD_FAST                0 (search_uid)
-                     388 PRECALL                  1
-                     392 CALL                     1
-                     402 STORE_FAST               7 (search)
-         
-         162         404 LOAD_FAST                5 (targets)
-                     406 LOAD_METHOD             11 (sort_values)
-         
-         163         428 LOAD_FAST                7 (search)
-                     430 LOAD_ATTR               12 (sort)
-                     440 LOAD_METHOD             13 (get)
-                     462 LOAD_CONST               7 ('field')
-                     464 LOAD_CONST               4 ('domain')
-                     466 PRECALL                  2
-                     470 CALL                     2
-         
-         164         480 LOAD_FAST                7 (search)
-                     482 LOAD_ATTR               12 (sort)
-                     492 LOAD_METHOD             13 (get)
-                     514 LOAD_CONST               8 ('order')
-                     516 PRECALL                  1
-                     520 CALL                     1
-                     530 LOAD_CONST               9 ('asc')
-                     532 COMPARE_OP               2 (==)
-         
-         162         538 KW_NAMES                10
-                     540 PRECALL                  2
-                     544 CALL                     2
-                     554 STORE_FAST               5 (targets)
+         139     >>  400 LOAD_GLOBAL             19 (NULL + comment_by_domain)
+                     412 LOAD_FAST                0 (search_uid)
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 STORE_FAST               6 (comments)
+         
+         140         430 LOAD_FAST                5 (targets)
+                     432 LOAD_METHOD             10 (merge)
+                     454 LOAD_FAST                6 (comments)
+                     456 LOAD_CONST               6 ('domain')
+                     458 LOAD_CONST               7 ('left')
+                     460 KW_NAMES                 8
+                     462 PRECALL                  3
+                     466 CALL                     3
+                     476 STORE_FAST               5 (targets)
+         
+         143         478 LOAD_GLOBAL             23 (NULL + find_search_by_uid)
+                     490 LOAD_FAST                0 (search_uid)
+                     492 PRECALL                  1
+                     496 CALL                     1
+                     506 STORE_FAST               7 (search)
+         
+         144         508 LOAD_FAST                5 (targets)
+                     510 LOAD_METHOD             12 (sort_values)
+         
+         145         532 LOAD_FAST                7 (search)
+                     534 LOAD_ATTR               13 (sort)
+                     544 LOAD_METHOD             14 (get)
+                     566 LOAD_CONST               9 ('field')
+                     568 LOAD_CONST               6 ('domain')
+                     570 PRECALL                  2
+                     574 CALL                     2
+         
+         146         584 LOAD_FAST                7 (search)
+                     586 LOAD_ATTR               13 (sort)
+                     596 LOAD_METHOD             14 (get)
+                     618 LOAD_CONST              10 ('order')
+                     620 PRECALL                  1
+                     624 CALL                     1
+                     634 LOAD_CONST              11 ('asc')
+                     636 COMPARE_OP               2 (==)
+         
+         144         642 KW_NAMES                12
+                     644 PRECALL                  2
+                     648 CALL                     2
+                     658 STORE_FAST               5 (targets)
          
-         168         556 LOAD_FAST                5 (targets)
-                     558 RETURN_VALUE
+         150         660 LOAD_FAST                5 (targets)
+                     662 RETURN_VALUE
          ExceptionTable:
-           52 to 248 -> 274 [1] lasti
-           274 to 280 -> 282 [3] lasti
-           288 to 288 -> 282 [3] lasti
+           52 to 352 -> 378 [1] lasti
+           378 to 384 -> 386 [3] lasti
+           392 to 392 -> 386 [3] lasti
          consts
             None
             'SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type'
             ('search_uid', 'last_event_type')
+            'SELECT * FROM target WHERE search_uid = :search_uid'
+            'search_uid'
             ('columns',)
             'domain'
             'left'
             ('on', 'how')
             'field'
             'order'
             'asc'
             ('by', 'ascending')
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
          varnames   ('search_uid', 'last_event_type', 'conn', 'statement', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target'
-         firstlineno 147
+         firstlineno 121
          lnotab
-            0x02013401040118011c0108fe100474fa2e081e0130041e01180134013a
-            fe1206
+            0x02013401040104011801260108fe120604011801260106fe100574f12e
+            111e0130031e01180134013afe1206
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab01000000000000000064027c006901a60200
-            00ab0200000000000000007d037409000000000000000000006a05000000
-            00000000007c03a0060000000000000000000000000000000000000000a6
-            000000ab0000000000000000007c03a00700000000000000000000000000
-            00000000000000a6000000ab000000000000000000ac03a6020000ab0200
-            000000000000007d04640064006400a6020000ab02000000000000000001
-            006e0b230031007304770278035900770101005900010001007c045300
-         171           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c045300
+         153           0 RESUME                   0
          
-         172           2 LOAD_GLOBAL              0 (engine)
+         154           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         173          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
+         155          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
                       56 STORE_FAST               2 (statement)
          
-         179          58 LOAD_FAST                1 (conn)
+         161          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         180          82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-         
-         181         110 LOAD_CONST               2 ('search_uid')
-                     112 LOAD_FAST                0 (search_uid)
-                     114 BUILD_MAP                1
-         
-         179         116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               3 (result)
-         
-         183         132 LOAD_GLOBAL              9 (NULL + pd)
-                     144 LOAD_ATTR                5 (DataFrame)
-                     154 LOAD_FAST                3 (result)
-                     156 LOAD_METHOD              6 (fetchall)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 LOAD_FAST                3 (result)
-                     194 LOAD_METHOD              7 (keys)
-                     216 PRECALL                  0
-                     220 CALL                     0
-                     230 KW_NAMES                 3
-                     232 PRECALL                  2
-                     236 CALL                     2
-                     246 STORE_FAST               4 (df)
+         162          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
          
-         172         248 LOAD_CONST               0 (None)
-                     250 LOAD_CONST               0 (None)
-                     252 LOAD_CONST               0 (None)
-                     254 PRECALL                  2
-                     258 CALL                     2
-                     268 POP_TOP
-                     270 JUMP_FORWARD            11 (to 294)
-                 >>  272 PUSH_EXC_INFO
-                     274 WITH_EXCEPT_START
-                     276 POP_JUMP_FORWARD_IF_TRUE     4 (to 286)
-                     278 RERAISE                  2
-                 >>  280 COPY                     3
-                     282 POP_EXCEPT
-                     284 RERAISE                  1
-                 >>  286 POP_TOP
-                     288 POP_EXCEPT
-                     290 POP_TOP
-                     292 POP_TOP
+         163         120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+         
+         161         126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         165         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
+         
+         154         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
+                     292 POP_EXCEPT
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
          
-         184     >>  294 LOAD_FAST                4 (df)
-                     296 RETURN_VALUE
+         166     >>  304 LOAD_FAST                4 (df)
+                     306 RETURN_VALUE
          ExceptionTable:
-           52 to 246 -> 272 [1] lasti
-           272 to 278 -> 280 [3] lasti
-           286 to 286 -> 280 [3] lasti
+           52 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
          consts
             None
             '\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            '
             'search_uid'
             ('columns',)
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 171
-         lnotab 0x02013401040618011c0106fe100474f52e0c
+         firstlineno 153
+         lnotab 0x0201340104061801260106fe100474f52e0c
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab01000000000000000064027c006901a60200
-            00ab0200000000000000007d037409000000000000000000006a05000000
-            00000000007c03a0060000000000000000000000000000000000000000a6
-            000000ab0000000000000000007c03a00700000000000000000000000000
-            00000000000000a6000000ab000000000000000000ac03a6020000ab0200
-            000000000000007d04640064006400a6020000ab02000000000000000001
-            006e0b230031007304770278035900770101005900010001007c045300
-         187           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c045300
+         169           0 RESUME                   0
          
-         188           2 LOAD_GLOBAL              0 (engine)
+         170           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         189          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         171          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         194          58 LOAD_FAST                1 (conn)
+         176          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
-                      82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 LOAD_CONST               2 ('search_uid')
-                     112 LOAD_FAST                0 (search_uid)
-                     114 BUILD_MAP                1
-                     116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               3 (result)
-         
-         195         132 LOAD_GLOBAL              9 (NULL + pd)
-                     144 LOAD_ATTR                5 (DataFrame)
-                     154 LOAD_FAST                3 (result)
-                     156 LOAD_METHOD              6 (fetchall)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 LOAD_FAST                3 (result)
-                     194 LOAD_METHOD              7 (keys)
-                     216 PRECALL                  0
-                     220 CALL                     0
-                     230 KW_NAMES                 3
-                     232 PRECALL                  2
-                     236 CALL                     2
-                     246 STORE_FAST               4 (df)
-         
-         188         248 LOAD_CONST               0 (None)
-                     250 LOAD_CONST               0 (None)
-                     252 LOAD_CONST               0 (None)
-                     254 PRECALL                  2
-                     258 CALL                     2
-                     268 POP_TOP
-                     270 JUMP_FORWARD            11 (to 294)
-                 >>  272 PUSH_EXC_INFO
-                     274 WITH_EXCEPT_START
-                     276 POP_JUMP_FORWARD_IF_TRUE     4 (to 286)
-                     278 RERAISE                  2
-                 >>  280 COPY                     3
-                     282 POP_EXCEPT
-                     284 RERAISE                  1
-                 >>  286 POP_TOP
-                     288 POP_EXCEPT
-                     290 POP_TOP
-                     292 POP_TOP
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         177         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
+         
+         170         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
+                     292 POP_EXCEPT
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
          
-         196     >>  294 LOAD_FAST                4 (df)
-                     296 RETURN_VALUE
+         178     >>  304 LOAD_FAST                4 (df)
+                     306 RETURN_VALUE
          ExceptionTable:
-           52 to 246 -> 272 [1] lasti
-           272 to 278 -> 280 [3] lasti
-           286 to 286 -> 280 [3] lasti
+           52 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
          consts
             None
             '\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            '
             'search_uid'
             ('columns',)
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 187
-         lnotab 0x0201340104054a0174f92e08
+         firstlineno 169
+         lnotab 0x020134010405540174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0064017d017c
             00a002000000000000000000000000000000000000000074070000000000
-            00000000007c01a6010000ab010000000000000000a6010000ab01000000
-            00000000007d027409000000000000000000006a0500000000000000007c
-            02a0060000000000000000000000000000000000000000a6000000ab0000
-            000000000000007c02a00700000000000000000000000000000000000000
-            00a6000000ab000000000000000000ac02a6020000ab0200000000000000
-            007d03640064006400a6020000ab02000000000000000001006e0b230031
-            007304770278035900770101005900010001007c035300
-         199           0 RESUME                   0
+            00000000006a0400000000000000007c01a6010000ab0100000000000000
+            00a6010000ab0100000000000000007d02740b000000000000000000006a
+            0600000000000000007c02a0070000000000000000000000000000000000
+            000000a6000000ab0000000000000000007c02a008000000000000000000
+            0000000000000000000000a6000000ab000000000000000000ac02a60200
+            00ab0200000000000000007d03640064006400a6020000ab020000000000
+            00000001006e0b230031007304770278035900770101005900010001007c
+            035300
+         181           0 RESUME                   0
          
-         200           2 LOAD_GLOBAL              0 (engine)
+         182           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         201          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
+         183          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
                       56 STORE_FAST               1 (statement)
          
-         205          58 LOAD_FAST                0 (conn)
+         187          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
-                      82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                1 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 PRECALL                  1
-                     114 CALL                     1
-                     124 STORE_FAST               2 (result)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                1 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 STORE_FAST               2 (result)
+         
+         188         136 LOAD_GLOBAL             11 (NULL + pd)
+                     148 LOAD_ATTR                6 (DataFrame)
+                     158 LOAD_FAST                2 (result)
+                     160 LOAD_METHOD              7 (fetchall)
+                     182 PRECALL                  0
+                     186 CALL                     0
+                     196 LOAD_FAST                2 (result)
+                     198 LOAD_METHOD              8 (keys)
+                     220 PRECALL                  0
+                     224 CALL                     0
+                     234 KW_NAMES                 2
+                     236 PRECALL                  2
+                     240 CALL                     2
+                     250 STORE_FAST               3 (df)
          
-         206         126 LOAD_GLOBAL              9 (NULL + pd)
-                     138 LOAD_ATTR                5 (DataFrame)
-                     148 LOAD_FAST                2 (result)
-                     150 LOAD_METHOD              6 (fetchall)
-                     172 PRECALL                  0
-                     176 CALL                     0
-                     186 LOAD_FAST                2 (result)
-                     188 LOAD_METHOD              7 (keys)
-                     210 PRECALL                  0
-                     214 CALL                     0
-                     224 KW_NAMES                 2
-                     226 PRECALL                  2
-                     230 CALL                     2
-                     240 STORE_FAST               3 (df)
-         
-         200         242 LOAD_CONST               0 (None)
-                     244 LOAD_CONST               0 (None)
-                     246 LOAD_CONST               0 (None)
-                     248 PRECALL                  2
-                     252 CALL                     2
-                     262 POP_TOP
-                     264 JUMP_FORWARD            11 (to 288)
-                 >>  266 PUSH_EXC_INFO
-                     268 WITH_EXCEPT_START
-                     270 POP_JUMP_FORWARD_IF_TRUE     4 (to 280)
-                     272 RERAISE                  2
-                 >>  274 COPY                     3
-                     276 POP_EXCEPT
-                     278 RERAISE                  1
-                 >>  280 POP_TOP
-                     282 POP_EXCEPT
-                     284 POP_TOP
-                     286 POP_TOP
+         182         252 LOAD_CONST               0 (None)
+                     254 LOAD_CONST               0 (None)
+                     256 LOAD_CONST               0 (None)
+                     258 PRECALL                  2
+                     262 CALL                     2
+                     272 POP_TOP
+                     274 JUMP_FORWARD            11 (to 298)
+                 >>  276 PUSH_EXC_INFO
+                     278 WITH_EXCEPT_START
+                     280 POP_JUMP_FORWARD_IF_TRUE     4 (to 290)
+                     282 RERAISE                  2
+                 >>  284 COPY                     3
+                     286 POP_EXCEPT
+                     288 RERAISE                  1
+                 >>  290 POP_TOP
+                     292 POP_EXCEPT
+                     294 POP_TOP
+                     296 POP_TOP
          
-         207     >>  288 LOAD_FAST                3 (df)
-                     290 RETURN_VALUE
+         189     >>  298 LOAD_FAST                3 (df)
+                     300 RETURN_VALUE
          ExceptionTable:
-           52 to 240 -> 266 [1] lasti
-           266 to 272 -> 274 [3] lasti
-           280 to 280 -> 274 [3] lasti
+           52 to 250 -> 276 [1] lasti
+           276 to 282 -> 284 [3] lasti
+           290 to 290 -> 284 [3] lasti
          consts
             None
             '\n                SELECT *\n                FROM checkpoint\n            '
             ('columns',)
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 199
-         lnotab 0x020134010404440174fa2e07
+         firstlineno 181
+         lnotab 0x0201340104044e0174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab01000000000000000064027c006901a60200
-            00ab0200000000000000007d037409000000000000000000006a05000000
-            00000000007c03a0060000000000000000000000000000000000000000a6
-            000000ab0000000000000000007c03a00700000000000000000000000000
-            00000000000000a6000000ab000000000000000000ac03a6020000ab0200
-            000000000000007d04640064006400a6020000ab02000000000000000001
-            006e0b230031007304770278035900770101005900010001007c04a00800
-            000000000000000000000000000000000000006404a6010000ab01000000
-            0000000000a0090000000000000000000000000000000000000000640564
-            0684006901a6010000ab010000000000000000a00a000000000000000000
-            0000000000000000000000a6000000ab0000000000000000005300
-         210           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c04a009000000000000000000000000000000000000000064
+            04a6010000ab010000000000000000a00a00000000000000000000000000
+            000000000000006405640684006901a6010000ab010000000000000000a0
+            0b0000000000000000000000000000000000000000a6000000ab00000000
+            00000000005300
+         192           0 RESUME                   0
          
-         211           2 LOAD_GLOBAL              0 (engine)
+         193           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         212          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         194          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         219          58 LOAD_FAST                1 (conn)
+         201          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         220          82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-         
-         221         110 LOAD_CONST               2 ('search_uid')
-                     112 LOAD_FAST                0 (search_uid)
-                     114 BUILD_MAP                1
-         
-         219         116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               3 (result)
-         
-         223         132 LOAD_GLOBAL              9 (NULL + pd)
-                     144 LOAD_ATTR                5 (DataFrame)
-                     154 LOAD_FAST                3 (result)
-                     156 LOAD_METHOD              6 (fetchall)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 LOAD_FAST                3 (result)
-                     194 LOAD_METHOD              7 (keys)
-                     216 PRECALL                  0
-                     220 CALL                     0
-                     230 KW_NAMES                 3
-                     232 PRECALL                  2
-                     236 CALL                     2
-                     246 STORE_FAST               4 (df)
-         
-         211         248 LOAD_CONST               0 (None)
-                     250 LOAD_CONST               0 (None)
-                     252 LOAD_CONST               0 (None)
-                     254 PRECALL                  2
-                     258 CALL                     2
-                     268 POP_TOP
-                     270 JUMP_FORWARD            11 (to 294)
-                 >>  272 PUSH_EXC_INFO
-                     274 WITH_EXCEPT_START
-                     276 POP_JUMP_FORWARD_IF_TRUE     4 (to 286)
-                     278 RERAISE                  2
-                 >>  280 COPY                     3
-                     282 POP_EXCEPT
-                     284 RERAISE                  1
-                 >>  286 POP_TOP
-                     288 POP_EXCEPT
-                     290 POP_TOP
-                     292 POP_TOP
+         202          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
          
-         225     >>  294 LOAD_FAST                4 (df)
-                     296 LOAD_METHOD              8 (groupby)
-                     318 LOAD_CONST               4 ('domain')
-                     320 PRECALL                  1
-                     324 CALL                     1
-                     334 LOAD_METHOD              9 (agg)
-                     356 LOAD_CONST               5 ('comment')
-                     358 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 225>)
-                     360 MAKE_FUNCTION            0
-                     362 BUILD_MAP                1
-                     364 PRECALL                  1
-                     368 CALL                     1
-                     378 LOAD_METHOD             10 (reset_index)
-                     400 PRECALL                  0
-                     404 CALL                     0
-                     414 RETURN_VALUE
+         203         120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+         
+         201         126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         205         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
+         
+         193         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
+                     292 POP_EXCEPT
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
+         
+         207     >>  304 LOAD_FAST                4 (df)
+                     306 LOAD_METHOD              9 (groupby)
+                     328 LOAD_CONST               4 ('domain')
+                     330 PRECALL                  1
+                     334 CALL                     1
+                     344 LOAD_METHOD             10 (agg)
+                     366 LOAD_CONST               5 ('comment')
+                     368 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 207>)
+                     370 MAKE_FUNCTION            0
+                     372 BUILD_MAP                1
+                     374 PRECALL                  1
+                     378 CALL                     1
+                     388 LOAD_METHOD             11 (reset_index)
+                     410 PRECALL                  0
+                     414 CALL                     0
+                     424 RETURN_VALUE
          ExceptionTable:
-           52 to 246 -> 272 [1] lasti
-           272 to 278 -> 280 [3] lasti
-           286 to 286 -> 280 [3] lasti
+           52 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
          consts
             None
             "\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            "
             'search_uid'
             ('columns',)
             'domain'
             'comment'
@@ -1614,493 +1479,499 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               225           0 RESUME                   0
+               207           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 225
+               firstlineno 207
                lnotab 0x
-         names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 210
-         lnotab 0x02013401040718011c0106fe100474f42e0e
+         firstlineno 192
+         lnotab 0x0201340104071801260106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab01000000000000000064027c006901a60200
-            00ab0200000000000000007d03640064006400a6020000ab020000000000
-            00000001006e0b230031007304770278035900770101005900010001007c
-            036a04000000000000000064036b0200000000720264005300740b000000
-            00000000000000740d000000000000000000007c03a00700000000000000
-            00000000000000000000000000a6000000ab0000000000000000007c03a0
-            080000000000000000000000000000000000000000a6000000ab00000000
-            0000000000a6020000ab020000000000000000a6010000ab010000000000
-            0000007d047413000000000000000000007414000000000000000000007c
-            04a6020000ab0200000000000000005300
-         231           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03640064006400a6
+            020000ab02000000000000000001006e0b23003100730477027803590077
+            0101005900010001007c036a05000000000000000064036b020000000072
+            0264005300740d00000000000000000000740f000000000000000000007c
+            03a0080000000000000000000000000000000000000000a6000000ab0000
+            000000000000007c03a00900000000000000000000000000000000000000
+            00a6000000ab000000000000000000a6020000ab020000000000000000a6
+            010000ab0100000000000000007d04741500000000000000000000741600
+            0000000000000000007c04a6020000ab0200000000000000005300
+         213           0 RESUME                   0
          
-         232           2 LOAD_GLOBAL              0 (engine)
+         214           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         233          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         215          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         238          58 LOAD_FAST                1 (conn)
+         220          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
-                      82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 LOAD_CONST               2 ('search_uid')
-                     112 LOAD_FAST                0 (search_uid)
-                     114 BUILD_MAP                1
-                     116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               3 (result)
-         
-         232         132 LOAD_CONST               0 (None)
-                     134 LOAD_CONST               0 (None)
-                     136 LOAD_CONST               0 (None)
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 POP_TOP
-                     154 JUMP_FORWARD            11 (to 178)
-                 >>  156 PUSH_EXC_INFO
-                     158 WITH_EXCEPT_START
-                     160 POP_JUMP_FORWARD_IF_TRUE     4 (to 170)
-                     162 RERAISE                  2
-                 >>  164 COPY                     3
-                     166 POP_EXCEPT
-                     168 RERAISE                  1
-                 >>  170 POP_TOP
-                     172 POP_EXCEPT
-                     174 POP_TOP
-                     176 POP_TOP
-         
-         240     >>  178 LOAD_FAST                3 (result)
-                     180 LOAD_ATTR                4 (rowcount)
-                     190 LOAD_CONST               3 (0)
-                     192 COMPARE_OP               2 (==)
-                     198 POP_JUMP_FORWARD_IF_FALSE     2 (to 204)
-         
-         241         200 LOAD_CONST               0 (None)
-                     202 RETURN_VALUE
-         
-         243     >>  204 LOAD_GLOBAL             11 (NULL + dict)
-                     216 LOAD_GLOBAL             13 (NULL + zip)
-                     228 LOAD_FAST                3 (result)
-                     230 LOAD_METHOD              7 (keys)
-                     252 PRECALL                  0
-                     256 CALL                     0
-                     266 LOAD_FAST                3 (result)
-                     268 LOAD_METHOD              8 (fetchone)
-                     290 PRECALL                  0
-                     294 CALL                     0
-                     304 PRECALL                  2
-                     308 CALL                     2
-                     318 PRECALL                  1
-                     322 CALL                     1
-                     332 STORE_FAST               4 (obj)
-         
-         244         334 LOAD_GLOBAL             19 (NULL + from_dict)
-                     346 LOAD_GLOBAL             20 (Search)
-                     358 LOAD_FAST                4 (obj)
-                     360 PRECALL                  2
-                     364 CALL                     2
-                     374 RETURN_VALUE
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         214         142 LOAD_CONST               0 (None)
+                     144 LOAD_CONST               0 (None)
+                     146 LOAD_CONST               0 (None)
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+                     164 JUMP_FORWARD            11 (to 188)
+                 >>  166 PUSH_EXC_INFO
+                     168 WITH_EXCEPT_START
+                     170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                     172 RERAISE                  2
+                 >>  174 COPY                     3
+                     176 POP_EXCEPT
+                     178 RERAISE                  1
+                 >>  180 POP_TOP
+                     182 POP_EXCEPT
+                     184 POP_TOP
+                     186 POP_TOP
+         
+         222     >>  188 LOAD_FAST                3 (result)
+                     190 LOAD_ATTR                5 (rowcount)
+                     200 LOAD_CONST               3 (0)
+                     202 COMPARE_OP               2 (==)
+                     208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
+         
+         223         210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
+         
+         225     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+                     226 LOAD_GLOBAL             15 (NULL + zip)
+                     238 LOAD_FAST                3 (result)
+                     240 LOAD_METHOD              8 (keys)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_FAST                3 (result)
+                     278 LOAD_METHOD              9 (fetchone)
+                     300 PRECALL                  0
+                     304 CALL                     0
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 PRECALL                  1
+                     332 CALL                     1
+                     342 STORE_FAST               4 (obj)
+         
+         226         344 LOAD_GLOBAL             21 (NULL + from_dict)
+                     356 LOAD_GLOBAL             22 (Search)
+                     368 LOAD_FAST                4 (obj)
+                     370 PRECALL                  2
+                     374 CALL                     2
+                     384 RETURN_VALUE
          ExceptionTable:
-           52 to 130 -> 156 [1] lasti
-           156 to 162 -> 164 [3] lasti
-           170 to 170 -> 164 [3] lasti
+           52 to 140 -> 166 [1] lasti
+           166 to 172 -> 174 [3] lasti
+           180 to 180 -> 174 [3] lasti
          consts
             None
             '\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            '
             'search_uid'
             0
-         names      ('engine', 'connect', 'execute', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 231
-         lnotab 0x0201340104054afa2e08160104028201
+         firstlineno 213
+         lnotab 0x02013401040554fa2e08160104028201
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab01000000000000000064027c006901a60200
-            00ab0200000000000000007d03640064006400a6020000ab020000000000
-            00000001006e0b230031007304770278035900770101005900010001007c
-            036a04000000000000000064036b0200000000720264005300740b000000
-            00000000000000740d000000000000000000007c03a00700000000000000
-            00000000000000000000000000a6000000ab0000000000000000007c03a0
-            080000000000000000000000000000000000000000a6000000ab00000000
-            0000000000a6020000ab020000000000000000a6010000ab010000000000
-            0000007d047413000000000000000000007414000000000000000000007c
-            04a6020000ab0200000000000000005300
-         247           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03640064006400a6
+            020000ab02000000000000000001006e0b23003100730477027803590077
+            0101005900010001007c036a05000000000000000064036b020000000072
+            0264005300740d00000000000000000000740f000000000000000000007c
+            03a0080000000000000000000000000000000000000000a6000000ab0000
+            000000000000007c03a00900000000000000000000000000000000000000
+            00a6000000ab000000000000000000a6020000ab020000000000000000a6
+            010000ab0100000000000000007d04741500000000000000000000741600
+            0000000000000000007c04a6020000ab0200000000000000005300
+         229           0 RESUME                   0
          
-         248           2 LOAD_GLOBAL              0 (engine)
+         230           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         249          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         231          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         254          58 LOAD_FAST                1 (conn)
+         236          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
-                      82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 LOAD_CONST               2 ('domain')
-                     112 LOAD_FAST                0 (domain)
-                     114 BUILD_MAP                1
-                     116 PRECALL                  2
-                     120 CALL                     2
-                     130 STORE_FAST               3 (result)
-         
-         248         132 LOAD_CONST               0 (None)
-                     134 LOAD_CONST               0 (None)
-                     136 LOAD_CONST               0 (None)
-                     138 PRECALL                  2
-                     142 CALL                     2
-                     152 POP_TOP
-                     154 JUMP_FORWARD            11 (to 178)
-                 >>  156 PUSH_EXC_INFO
-                     158 WITH_EXCEPT_START
-                     160 POP_JUMP_FORWARD_IF_TRUE     4 (to 170)
-                     162 RERAISE                  2
-                 >>  164 COPY                     3
-                     166 POP_EXCEPT
-                     168 RERAISE                  1
-                 >>  170 POP_TOP
-                     172 POP_EXCEPT
-                     174 POP_TOP
-                     176 POP_TOP
-         
-         256     >>  178 LOAD_FAST                3 (result)
-                     180 LOAD_ATTR                4 (rowcount)
-                     190 LOAD_CONST               3 (0)
-                     192 COMPARE_OP               2 (==)
-                     198 POP_JUMP_FORWARD_IF_FALSE     2 (to 204)
-         
-         257         200 LOAD_CONST               0 (None)
-                     202 RETURN_VALUE
-         
-         259     >>  204 LOAD_GLOBAL             11 (NULL + dict)
-                     216 LOAD_GLOBAL             13 (NULL + zip)
-                     228 LOAD_FAST                3 (result)
-                     230 LOAD_METHOD              7 (keys)
-                     252 PRECALL                  0
-                     256 CALL                     0
-                     266 LOAD_FAST                3 (result)
-                     268 LOAD_METHOD              8 (fetchone)
-                     290 PRECALL                  0
-                     294 CALL                     0
-                     304 PRECALL                  2
-                     308 CALL                     2
-                     318 PRECALL                  1
-                     322 CALL                     1
-                     332 STORE_FAST               4 (obj)
-         
-         260         334 LOAD_GLOBAL             19 (NULL + from_dict)
-                     346 LOAD_GLOBAL             20 (Company)
-                     358 LOAD_FAST                4 (obj)
-                     360 PRECALL                  2
-                     364 CALL                     2
-                     374 RETURN_VALUE
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 LOAD_CONST               2 ('domain')
+                     122 LOAD_FAST                0 (domain)
+                     124 BUILD_MAP                1
+                     126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         230         142 LOAD_CONST               0 (None)
+                     144 LOAD_CONST               0 (None)
+                     146 LOAD_CONST               0 (None)
+                     148 PRECALL                  2
+                     152 CALL                     2
+                     162 POP_TOP
+                     164 JUMP_FORWARD            11 (to 188)
+                 >>  166 PUSH_EXC_INFO
+                     168 WITH_EXCEPT_START
+                     170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                     172 RERAISE                  2
+                 >>  174 COPY                     3
+                     176 POP_EXCEPT
+                     178 RERAISE                  1
+                 >>  180 POP_TOP
+                     182 POP_EXCEPT
+                     184 POP_TOP
+                     186 POP_TOP
+         
+         238     >>  188 LOAD_FAST                3 (result)
+                     190 LOAD_ATTR                5 (rowcount)
+                     200 LOAD_CONST               3 (0)
+                     202 COMPARE_OP               2 (==)
+                     208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
+         
+         239         210 LOAD_CONST               0 (None)
+                     212 RETURN_VALUE
+         
+         241     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+                     226 LOAD_GLOBAL             15 (NULL + zip)
+                     238 LOAD_FAST                3 (result)
+                     240 LOAD_METHOD              8 (keys)
+                     262 PRECALL                  0
+                     266 CALL                     0
+                     276 LOAD_FAST                3 (result)
+                     278 LOAD_METHOD              9 (fetchone)
+                     300 PRECALL                  0
+                     304 CALL                     0
+                     314 PRECALL                  2
+                     318 CALL                     2
+                     328 PRECALL                  1
+                     332 CALL                     1
+                     342 STORE_FAST               4 (obj)
+         
+         242         344 LOAD_GLOBAL             21 (NULL + from_dict)
+                     356 LOAD_GLOBAL             22 (Company)
+                     368 LOAD_FAST                4 (obj)
+                     370 PRECALL                  2
+                     374 CALL                     2
+                     384 RETURN_VALUE
          ExceptionTable:
-           52 to 130 -> 156 [1] lasti
-           156 to 162 -> 164 [3] lasti
-           170 to 170 -> 164 [3] lasti
+           52 to 140 -> 166 [1] lasti
+           166 to 172 -> 174 [3] lasti
+           180 to 180 -> 174 [3] lasti
          consts
             None
             '\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            '
             'domain'
             0
-         names      ('engine', 'connect', 'execute', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 247
-         lnotab 0x0201340104054afa2e08160104028201
+         firstlineno 229
+         lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 10
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
-            00000000007c02a6010000ab0100000000000000007c006a040000000000
-            0000007c006a0500000000000000007c006a060000000000000000740f00
-            0000000000000000006a0800000000000000007c006a0900000000000000
-            00a6010000ab01000000000000000064029c04a6020000ab020000000000
-            00000001007c01a002000000000000000000000000000000000000000074
-            07000000000000000000006403a6010000ab010000000000000000a60100
-            00ab01000000000000000001007c01a00a00000000000000000000000000
-            00000000000000a6000000ab0000000000000000000100640064006400a6
-            020000ab0200000000000000000100640053002300310073047702780359
-            007701010059000100010064005300
-         266           0 RESUME                   0
+            00000000006a0400000000000000007c02a6010000ab0100000000000000
+            007c006a0500000000000000007c006a0600000000000000007c006a0700
+            000000000000007411000000000000000000006a0900000000000000007c
+            006a0a0000000000000000a6010000ab01000000000000000064029c04a6
+            020000ab02000000000000000001007c01a0020000000000000000000000
+            0000000000000000007407000000000000000000006a0400000000000000
+            006403a6010000ab010000000000000000a6010000ab0100000000000000
+            0001007c01a00b0000000000000000000000000000000000000000a60000
+            00ab0000000000000000000100640064006400a6020000ab020000000000
+            000000010064005300230031007304770278035900770101005900010001
+            0064005300
+         248           0 RESUME                   0
          
-         267           2 LOAD_GLOBAL              0 (engine)
+         249           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         268          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
+         250          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         277          58 LOAD_FAST                1 (conn)
+         259          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         278          82 LOAD_GLOBAL              7 (NULL + text)
-                      94 LOAD_FAST                2 (statement)
-                      96 PRECALL                  1
-                     100 CALL                     1
-         
-         280         110 LOAD_FAST                0 (company)
-                     112 LOAD_ATTR                4 (name)
-         
-         281         122 LOAD_FAST                0 (company)
-                     124 LOAD_ATTR                5 (description)
-         
-         282         134 LOAD_FAST                0 (company)
-                     136 LOAD_ATTR                6 (domain)
-         
-         283         146 LOAD_GLOBAL             15 (NULL + json)
-                     158 LOAD_ATTR                8 (dumps)
-                     168 LOAD_FAST                0 (company)
-                     170 LOAD_ATTR                9 (meta)
-                     180 PRECALL                  1
-                     184 CALL                     1
-         
-         279         194 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
-                     196 BUILD_CONST_KEY_MAP      4
-         
-         277         198 PRECALL                  2
-                     202 CALL                     2
-                     212 POP_TOP
-         
-         286         214 LOAD_FAST                1 (conn)
-                     216 LOAD_METHOD              2 (execute)
-                     238 LOAD_GLOBAL              7 (NULL + text)
-                     250 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
-                     252 PRECALL                  1
-                     256 CALL                     1
-                     266 PRECALL                  1
-                     270 CALL                     1
-                     280 POP_TOP
-         
-         287         282 LOAD_FAST                1 (conn)
-                     284 LOAD_METHOD             10 (commit)
-                     306 PRECALL                  0
-                     310 CALL                     0
-                     320 POP_TOP
-         
-         267         322 LOAD_CONST               0 (None)
-                     324 LOAD_CONST               0 (None)
-                     326 LOAD_CONST               0 (None)
-                     328 PRECALL                  2
-                     332 CALL                     2
-                     342 POP_TOP
+         260          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                2 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+         
+         262         120 LOAD_FAST                0 (company)
+                     122 LOAD_ATTR                5 (name)
+         
+         263         132 LOAD_FAST                0 (company)
+                     134 LOAD_ATTR                6 (description)
+         
+         264         144 LOAD_FAST                0 (company)
+                     146 LOAD_ATTR                7 (domain)
+         
+         265         156 LOAD_GLOBAL             17 (NULL + json)
+                     168 LOAD_ATTR                9 (dumps)
+                     178 LOAD_FAST                0 (company)
+                     180 LOAD_ATTR               10 (meta)
+                     190 PRECALL                  1
+                     194 CALL                     1
+         
+         261         204 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
+                     206 BUILD_CONST_KEY_MAP      4
+         
+         259         208 PRECALL                  2
+                     212 CALL                     2
+                     222 POP_TOP
+         
+         268         224 LOAD_FAST                1 (conn)
+                     226 LOAD_METHOD              2 (execute)
+                     248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                     260 LOAD_ATTR                4 (text)
+                     270 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
+                     272 PRECALL                  1
+                     276 CALL                     1
+                     286 PRECALL                  1
+                     290 CALL                     1
+                     300 POP_TOP
+         
+         269         302 LOAD_FAST                1 (conn)
+                     304 LOAD_METHOD             11 (commit)
+                     326 PRECALL                  0
+                     330 CALL                     0
+                     340 POP_TOP
+         
+         249         342 LOAD_CONST               0 (None)
                      344 LOAD_CONST               0 (None)
-                     346 RETURN_VALUE
-                 >>  348 PUSH_EXC_INFO
-                     350 WITH_EXCEPT_START
-                     352 POP_JUMP_FORWARD_IF_TRUE     4 (to 362)
-                     354 RERAISE                  2
-                 >>  356 COPY                     3
-                     358 POP_EXCEPT
-                     360 RERAISE                  1
-                 >>  362 POP_TOP
-                     364 POP_EXCEPT
-                     366 POP_TOP
-                     368 POP_TOP
-                     370 LOAD_CONST               0 (None)
-                     372 RETURN_VALUE
+                     346 LOAD_CONST               0 (None)
+                     348 PRECALL                  2
+                     352 CALL                     2
+                     362 POP_TOP
+                     364 LOAD_CONST               0 (None)
+                     366 RETURN_VALUE
+                 >>  368 PUSH_EXC_INFO
+                     370 WITH_EXCEPT_START
+                     372 POP_JUMP_FORWARD_IF_TRUE     4 (to 382)
+                     374 RERAISE                  2
+                 >>  376 COPY                     3
+                     378 POP_EXCEPT
+                     380 RERAISE                  1
+                 >>  382 POP_TOP
+                     384 POP_EXCEPT
+                     386 POP_TOP
+                     388 POP_TOP
+                     390 LOAD_CONST               0 (None)
+                     392 RETURN_VALUE
          ExceptionTable:
-           52 to 320 -> 348 [1] lasti
-           348 to 354 -> 356 [3] lasti
-           362 to 362 -> 356 [3] lasti
+           52 to 340 -> 368 [1] lasti
+           368 to 374 -> 376 [3] lasti
+           382 to 382 -> 376 [3] lasti
          consts
             None
             '\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            '
             ('name', 'description', 'domain', 'meta')
             'REFRESH MATERIALIZED VIEW target'
-         names      ('engine', 'connect', 'execute', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 266
-         lnotab 0x02013401040918011c020c010c010c0130fc04fe1009440128ec
+         firstlineno 248
+         lnotab 0x020134010409180126020c010c010c0130fc04fe10094e0128ec
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 9
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d017c01a00200
             000000000000000000000000000000000000007407000000000000000000
-            006401a6010000ab0100000000000000007409000000000000000000006a
-            0500000000000000007c006a060000000000000000a6010000ab01000000
-            00000000007409000000000000000000006a0500000000000000007c006a
-            070000000000000000a6010000ab01000000000000000074090000000000
-            00000000006a0500000000000000007c006a080000000000000000a60100
-            00ab0100000000000000007c006a09000000000000000064029c04a60200
-            00ab02000000000000000001007c01a00a00000000000000000000000000
-            00000000000000a6000000ab0000000000000000000100640064006400a6
-            020000ab0200000000000000000100640053002300310073047702780359
-            007701010059000100010064005300
-         290           0 RESUME                   0
+            006a0400000000000000006401a6010000ab010000000000000000740b00
+            0000000000000000006a0600000000000000007c006a0700000000000000
+            00a6010000ab010000000000000000740b000000000000000000006a0600
+            000000000000007c006a080000000000000000a6010000ab010000000000
+            000000740b000000000000000000006a0600000000000000007c006a0900
+            00000000000000a6010000ab0100000000000000007c006a0a0000000000
+            00000064029c04a6020000ab02000000000000000001007c01a00b000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            000100640064006400a6020000ab02000000000000000001006400530023
+            00310073047702780359007701010059000100010064005300
+         272           0 RESUME                   0
          
-         291           2 LOAD_GLOBAL              0 (engine)
+         273           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         292          54 LOAD_FAST                1 (conn)
+         274          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         293          78 LOAD_GLOBAL              7 (NULL + text)
+         275          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      90 LOAD_ATTR                4 (text)
          
-         294          90 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
+         276         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
          
-         293          92 PRECALL                  1
-                      96 CALL                     1
+         275         102 PRECALL                  1
+                     106 CALL                     1
          
-         304         106 LOAD_GLOBAL              9 (NULL + json)
-                     118 LOAD_ATTR                5 (dumps)
-                     128 LOAD_FAST                0 (search)
-                     130 LOAD_ATTR                6 (sort)
-                     140 PRECALL                  1
-                     144 CALL                     1
-         
-         305         154 LOAD_GLOBAL              9 (NULL + json)
-                     166 LOAD_ATTR                5 (dumps)
-                     176 LOAD_FAST                0 (search)
-                     178 LOAD_ATTR                7 (inclusion)
-                     188 PRECALL                  1
-                     192 CALL                     1
-         
-         306         202 LOAD_GLOBAL              9 (NULL + json)
-                     214 LOAD_ATTR                5 (dumps)
-                     224 LOAD_FAST                0 (search)
-                     226 LOAD_ATTR                8 (exclusion)
-                     236 PRECALL                  1
-                     240 CALL                     1
-         
-         307         250 LOAD_FAST                0 (search)
-                     252 LOAD_ATTR                9 (uid)
-         
-         303         262 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
-                     264 BUILD_CONST_KEY_MAP      4
-         
-         292         266 PRECALL                  2
-                     270 CALL                     2
-                     280 POP_TOP
-         
-         310         282 LOAD_FAST                1 (conn)
-                     284 LOAD_METHOD             10 (commit)
-                     306 PRECALL                  0
-                     310 CALL                     0
-                     320 POP_TOP
-         
-         291         322 LOAD_CONST               0 (None)
-                     324 LOAD_CONST               0 (None)
-                     326 LOAD_CONST               0 (None)
-                     328 PRECALL                  2
-                     332 CALL                     2
-                     342 POP_TOP
-                     344 LOAD_CONST               0 (None)
-                     346 RETURN_VALUE
-                 >>  348 PUSH_EXC_INFO
-                     350 WITH_EXCEPT_START
-                     352 POP_JUMP_FORWARD_IF_TRUE     4 (to 362)
-                     354 RERAISE                  2
-                 >>  356 COPY                     3
-                     358 POP_EXCEPT
-                     360 RERAISE                  1
-                 >>  362 POP_TOP
-                     364 POP_EXCEPT
-                     366 POP_TOP
-                     368 POP_TOP
-                     370 LOAD_CONST               0 (None)
-                     372 RETURN_VALUE
+         286         116 LOAD_GLOBAL             11 (NULL + json)
+                     128 LOAD_ATTR                6 (dumps)
+                     138 LOAD_FAST                0 (search)
+                     140 LOAD_ATTR                7 (sort)
+                     150 PRECALL                  1
+                     154 CALL                     1
+         
+         287         164 LOAD_GLOBAL             11 (NULL + json)
+                     176 LOAD_ATTR                6 (dumps)
+                     186 LOAD_FAST                0 (search)
+                     188 LOAD_ATTR                8 (inclusion)
+                     198 PRECALL                  1
+                     202 CALL                     1
+         
+         288         212 LOAD_GLOBAL             11 (NULL + json)
+                     224 LOAD_ATTR                6 (dumps)
+                     234 LOAD_FAST                0 (search)
+                     236 LOAD_ATTR                9 (exclusion)
+                     246 PRECALL                  1
+                     250 CALL                     1
+         
+         289         260 LOAD_FAST                0 (search)
+                     262 LOAD_ATTR               10 (uid)
+         
+         285         272 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
+                     274 BUILD_CONST_KEY_MAP      4
+         
+         274         276 PRECALL                  2
+                     280 CALL                     2
+                     290 POP_TOP
+         
+         292         292 LOAD_FAST                1 (conn)
+                     294 LOAD_METHOD             11 (commit)
+                     316 PRECALL                  0
+                     320 CALL                     0
+                     330 POP_TOP
+         
+         273         332 LOAD_CONST               0 (None)
+                     334 LOAD_CONST               0 (None)
+                     336 LOAD_CONST               0 (None)
+                     338 PRECALL                  2
+                     342 CALL                     2
+                     352 POP_TOP
+                     354 LOAD_CONST               0 (None)
+                     356 RETURN_VALUE
+                 >>  358 PUSH_EXC_INFO
+                     360 WITH_EXCEPT_START
+                     362 POP_JUMP_FORWARD_IF_TRUE     4 (to 372)
+                     364 RERAISE                  2
+                 >>  366 COPY                     3
+                     368 POP_EXCEPT
+                     370 RERAISE                  1
+                 >>  372 POP_TOP
+                     374 POP_EXCEPT
+                     376 POP_TOP
+                     378 POP_TOP
+                     380 LOAD_CONST               0 (None)
+                     382 RETURN_VALUE
          ExceptionTable:
-           52 to 320 -> 348 [1] lasti
-           348 to 354 -> 356 [3] lasti
-           362 to 362 -> 356 [3] lasti
+           52 to 330 -> 358 [1] lasti
+           358 to 364 -> 366 [3] lasti
+           372 to 372 -> 366 [3] lasti
          consts
             None
             '\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                '
             ('sort', 'inclusion', 'exclusion', 'uid')
-         names      ('engine', 'connect', 'execute', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 290
-         lnotab 0x0201340118010c0102ff0e0b3001300130010cfc04f5101228ed
-      ('advance',)
-   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'os', 'sqlalchemy', 'text', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'get_engine', 'engine', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
+         firstlineno 272
+         lnotab 0x020134011801160102ff0e0b3001300130010cfc04f5101228ed
+      (None,)
+   names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'sqlalchemy', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'gandai.db', 'connect_with_connector', 'db', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c010c01200a080108010c010c010c021403061914
-      060c0e1015100f10131010060712181a101a0c160b1a15101010131018
+      0x00ff0201080108010c010c01200a08020c010c0114020c0214060c0e10
+      15100f10131010060712201a101a0c160b1a15101010131018
```

### Comparing `gandai-1.1.3/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.4/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x278f5a64 (Tue May  9 18:21:27 2023 UTC)
-files sz: 5348
+moddate:  0xb5925e64 (Fri May 12 19:25:41 2023 UTC)
+files sz: 5418
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
@@ -56,17 +56,17 @@
                 78 LOAD_CONST               5 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 10>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               6 ('GrataWrapper')
                 84 PRECALL                  2
                 88 CALL                     2
                 98 STORE_NAME               8 (GrataWrapper)
    
-   164         100 PUSH_NULL
+   165         100 PUSH_NULL
                102 LOAD_BUILD_CLASS
-               104 LOAD_CONST               7 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 164>)
+               104 LOAD_CONST               7 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 165>)
                106 MAKE_FUNCTION            0
                108 LOAD_CONST               8 ('SourceScrubWrapper')
                110 PRECALL                  2
                114 CALL                     2
                124 STORE_NAME               9 (SourceScrubWrapper)
                126 LOAD_CONST               3 (None)
                128 RETURN_VALUE
@@ -126,29 +126,29 @@
                       78 LOAD_CONST               7 ('return')
                       80 LOAD_NAME               10 (dict)
                       82 BUILD_TUPLE              4
                       84 LOAD_CONST               9 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 36>)
                       86 MAKE_FUNCTION            4 (annotations)
                       88 STORE_NAME              11 (find_by_criteria)
          
-          53          90 LOAD_CONST               5 ('domain')
+          54          90 LOAD_CONST               5 ('domain')
                       92 LOAD_NAME                6 (str)
                       94 LOAD_CONST               7 ('return')
                       96 LOAD_NAME               10 (dict)
                       98 BUILD_TUPLE              4
-                     100 LOAD_CONST              10 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 53>)
+                     100 LOAD_CONST              10 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 54>)
                      102 MAKE_FUNCTION            4 (annotations)
                      104 STORE_NAME              12 (enrich)
          
-          62         106 LOAD_CONST               6 ('search')
+          63         106 LOAD_CONST               6 ('search')
                      108 LOAD_NAME                7 (Search)
                      110 LOAD_CONST               7 ('return')
                      112 LOAD_NAME               10 (dict)
                      114 BUILD_TUPLE              4
-                     116 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 62>)
+                     116 LOAD_CONST              11 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 63>)
                      118 MAKE_FUNCTION            4 (annotations)
                      120 STORE_NAME              13 (_get_api_filter)
                      122 LOAD_CONST              12 (None)
                      124 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
@@ -186,18 +186,18 @@
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000007d027405000000
                   000000000000006a03000000000000000064017400000000000000000000
                   006a0400000000000000007c007c026402190000000000000000007c0264
                   031900000000000000000064049c03ac05a6030000ab0300000000000000
                   007d037c03a0050000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d04740d000000000000000000007c04a60100
-                  00ab01000000000000000001007c04a00700000000000000000000000000
-                  0000000000000064066700a6020000ab0200000000000000007c0464073c
-                  0000007c046407190000000000000000005300
+                  00ab0000000000000000007d04740d0000000000000000000064067c04a6
+                  020000ab02000000000000000001007c04a0070000000000000000000000
+                  00000000000000000064076700a6020000ab0200000000000000007c0464
+                  083c0000007c046408190000000000000000005300
                 19           0 RESUME                   0
                
                 20           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                1 (search)
                             38 PRECALL                  1
                             42 CALL                     1
@@ -232,65 +232,69 @@
                 30         152 LOAD_FAST                3 (response)
                            154 LOAD_METHOD              5 (json)
                            176 PRECALL                  0
                            180 CALL                     0
                            190 STORE_FAST               4 (data)
                
                 31         192 LOAD_GLOBAL             13 (NULL + print)
-                           204 LOAD_FAST                4 (data)
-                           206 PRECALL                  1
-                           210 CALL                     1
-                           220 POP_TOP
-               
-                32         222 LOAD_FAST                4 (data)
-                           224 LOAD_METHOD              7 (get)
-                           246 LOAD_CONST               6 ('results')
-                           248 BUILD_LIST               0
-                           250 PRECALL                  2
-                           254 CALL                     2
-                           264 LOAD_FAST                4 (data)
-                           266 LOAD_CONST               7 ('companies')
-                           268 STORE_SUBSCR
-               
-                34         272 LOAD_FAST                4 (data)
-                           274 LOAD_CONST               7 ('companies')
-                           276 BINARY_SUBSCR
-                           286 RETURN_VALUE
+                           204 LOAD_CONST               6 ('find_similar:')
+                           206 LOAD_FAST                4 (data)
+                           208 PRECALL                  2
+                           212 CALL                     2
+                           222 POP_TOP
+               
+                32         224 LOAD_FAST                4 (data)
+                           226 LOAD_METHOD              7 (get)
+                           248 LOAD_CONST               7 ('results')
+                           250 BUILD_LIST               0
+                           252 PRECALL                  2
+                           256 CALL                     2
+                           266 LOAD_FAST                4 (data)
+                           268 LOAD_CONST               8 ('companies')
+                           270 STORE_SUBSCR
+               
+                34         274 LOAD_FAST                4 (data)
+                           276 LOAD_CONST               8 ('companies')
+                           278 BINARY_SUBSCR
+                           288 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/search-similar/'
                   'employees_range'
                   'headquarters'
                   ('domain', 'employees_range', 'headquarters')
                   ('headers', 'json')
+                  'find_similar:'
                   'results'
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'print', 'get')
                varnames   ('domain', 'search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
                firstlineno 19
-               lnotab 0x0201340116010201160202010e010efd04fd120928011e013202
+               lnotab 0x0201340116010201160202010e010efd04fd1209280120013202
             code
                argcount  : 1
                nlocals   : 4
-               stacksize : 10
+               stacksize : 11
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c00a6010000ab0100000000000000007d017405000000
                   000000000000006a03000000000000000064017400000000000000000000
                   006a04000000000000000064027c006a0500000000000000006403190000
                   000000000000007c006a0600000000000000006403190000000000000000
-                  007c016404190000000000000000007c0164051900000000000000000064
-                  069c05ac07a6030000ab0300000000000000007d027c02a0070000000000
-                  000000000000000000000000000000a6000000ab0000000000000000007d
-                  037c035300
+                  007c016404190000000000000000007c016405190000000000000000007c
+                  0164061900000000000000000064079c06ac08a6030000ab030000000000
+                  0000007d027c02a0070000000000000000000000000000000000000000a6
+                  000000ab0000000000000000007d0374110000000000000000000064097c
+                  03a6020000ab02000000000000000001007c03640a190000000000000000
+                  005300
                 36           0 RESUME                   0
                
                 37           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                0 (search)
                             38 PRECALL                  1
                             42 CALL                     1
@@ -316,100 +320,118 @@
                            138 LOAD_CONST               3 ('keywords')
                            140 BINARY_SUBSCR
                
                 45         150 LOAD_FAST                1 (api_filters)
                            152 LOAD_CONST               4 ('employees_range')
                            154 BINARY_SUBSCR
                
-                47         164 LOAD_FAST                1 (api_filters)
-                           166 LOAD_CONST               5 ('headquarters')
+                46         164 LOAD_FAST                1 (api_filters)
+                           166 LOAD_CONST               5 ('ownership')
                            168 BINARY_SUBSCR
                
-                41         178 LOAD_CONST               6 (('op', 'include', 'exclude', 'employees_range', 'headquarters'))
-                           180 BUILD_CONST_KEY_MAP      5
-               
-                38         182 KW_NAMES                 7
-                           184 PRECALL                  3
-                           188 CALL                     3
-                           198 STORE_FAST               2 (response)
-               
-                50         200 LOAD_FAST                2 (response)
-                           202 LOAD_METHOD              7 (json)
-                           224 PRECALL                  0
-                           228 CALL                     0
-                           238 STORE_FAST               3 (data)
-               
-                51         240 LOAD_FAST                3 (data)
-                           242 RETURN_VALUE
+                47         178 LOAD_FAST                1 (api_filters)
+                           180 LOAD_CONST               6 ('headquarters')
+                           182 BINARY_SUBSCR
+               
+                41         192 LOAD_CONST               7 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
+                           194 BUILD_CONST_KEY_MAP      6
+               
+                38         196 KW_NAMES                 8
+                           198 PRECALL                  3
+                           202 CALL                     3
+                           212 STORE_FAST               2 (response)
+               
+                50         214 LOAD_FAST                2 (response)
+                           216 LOAD_METHOD              7 (json)
+                           238 PRECALL                  0
+                           242 CALL                     0
+                           252 STORE_FAST               3 (data)
+               
+                51         254 LOAD_GLOBAL             17 (NULL + print)
+                           266 LOAD_CONST               9 ('find_by_criteria: ')
+                           268 LOAD_FAST                3 (data)
+                           270 PRECALL                  2
+                           274 CALL                     2
+                           284 POP_TOP
+               
+                52         286 LOAD_FAST                3 (data)
+                           288 LOAD_CONST              10 ('companies')
+                           290 BINARY_SUBSCR
+                           300 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/search/'
                   'any'
                   'keywords'
                   'employees_range'
+                  'ownership'
                   'headquarters'
-                  ('op', 'include', 'exclude', 'employees_range', 'headquarters')
+                  ('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters')
                   ('headers', 'json')
-               names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'inclusion', 'exclusion', 'json')
+                  'find_by_criteria: '
+                  'companies'
+               names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'inclusion', 'exclusion', 'json', 'print')
                varnames   ('search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
                firstlineno 36
-               lnotab 0x020134011601020116020201180118010e020efa04fd120c2801
+               lnotab
+                  0x020134011601020116020201180118010e010e010efa04fd120c280120
+                  01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000006401740400
                   0000000000000000006a03000000000000000064027c006901ac03a60300
                   00ab0300000000000000007d017c01a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d027c025300
-                53           0 RESUME                   0
+                54           0 RESUME                   0
                
-                54           2 LOAD_GLOBAL              1 (NULL + requests)
+                55           2 LOAD_GLOBAL              1 (NULL + requests)
                             14 LOAD_ATTR                1 (post)
                
-                55          24 LOAD_CONST               1 ('https://search.grata.com/api/v1/enrich/')
+                56          24 LOAD_CONST               1 ('https://search.grata.com/api/v1/enrich/')
                
-                56          26 LOAD_GLOBAL              4 (GrataWrapper)
+                57          26 LOAD_GLOBAL              4 (GrataWrapper)
                             38 LOAD_ATTR                3 (HEADERS)
                
-                57          48 LOAD_CONST               2 ('domain')
+                58          48 LOAD_CONST               2 ('domain')
                             50 LOAD_FAST                0 (domain)
                             52 BUILD_MAP                1
                
-                54          54 KW_NAMES                 3
+                55          54 KW_NAMES                 3
                             56 PRECALL                  3
                             60 CALL                     3
                             70 STORE_FAST               1 (response)
                
-                59          72 LOAD_FAST                1 (response)
+                60          72 LOAD_FAST                1 (response)
                             74 LOAD_METHOD              4 (json)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 STORE_FAST               2 (data)
                
-                60         112 LOAD_FAST                2 (data)
+                61         112 LOAD_FAST                2 (data)
                            114 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1/enrich/'
                   'domain'
                   ('headers', 'json')
                names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json')
                varnames   ('domain', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 53
+               firstlineno 54
                lnotab 0x020116010201160106fd12052801
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 8
                flags     : 3
                code
@@ -432,350 +454,350 @@
                   701900000000000000000002007c01a6000000ab00000000000000000002
                   007c02a6000000ab00000000000000000002007c03a6000000ab00000000
                   000000000064719c0264729c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                4 (COUNTRIES)
                              4 MAKE_CELL                5 (STATES)
                
-                62           6 RESUME                   0
+                63           6 RESUME                   0
                
-                63           8 BUILD_MAP                0
+                64           8 BUILD_MAP                0
                
-                64          10 LOAD_CONST               1 ('AL')
+                65          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-                63          14 MAP_ADD                  1
+                64          14 MAP_ADD                  1
                
-                65          16 LOAD_CONST               3 ('AK')
+                66          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-                63          20 MAP_ADD                  1
+                64          20 MAP_ADD                  1
                
-                66          22 LOAD_CONST               5 ('AZ')
+                67          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-                63          26 MAP_ADD                  1
+                64          26 MAP_ADD                  1
                
-                67          28 LOAD_CONST               7 ('AR')
+                68          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-                63          32 MAP_ADD                  1
+                64          32 MAP_ADD                  1
                
-                68          34 LOAD_CONST               9 ('CA')
+                69          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-                63          38 MAP_ADD                  1
+                64          38 MAP_ADD                  1
                
-                69          40 LOAD_CONST              11 ('CO')
+                70          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-                63          44 MAP_ADD                  1
+                64          44 MAP_ADD                  1
                
-                70          46 LOAD_CONST              13 ('CT')
+                71          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-                63          50 MAP_ADD                  1
+                64          50 MAP_ADD                  1
                
-                71          52 LOAD_CONST              15 ('DE')
+                72          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-                63          56 MAP_ADD                  1
+                64          56 MAP_ADD                  1
                
-                72          58 LOAD_CONST              17 ('FL')
+                73          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-                63          62 MAP_ADD                  1
+                64          62 MAP_ADD                  1
                
-                73          64 LOAD_CONST              19 ('GA')
+                74          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-                63          68 MAP_ADD                  1
+                64          68 MAP_ADD                  1
                
-                74          70 LOAD_CONST              21 ('HI')
+                75          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-                63          74 MAP_ADD                  1
+                64          74 MAP_ADD                  1
                
-                75          76 LOAD_CONST              23 ('ID')
+                76          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-                63          80 MAP_ADD                  1
+                64          80 MAP_ADD                  1
                
-                76          82 LOAD_CONST              25 ('IL')
+                77          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-                63          86 MAP_ADD                  1
+                64          86 MAP_ADD                  1
                
-                77          88 LOAD_CONST              27 ('IN')
+                78          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-                63          92 MAP_ADD                  1
+                64          92 MAP_ADD                  1
                
-                78          94 LOAD_CONST              29 ('IA')
+                79          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-                63          98 MAP_ADD                  1
+                64          98 MAP_ADD                  1
                
-                79         100 LOAD_CONST              31 ('KS')
+                80         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-                63         104 MAP_ADD                  1
+                64         104 MAP_ADD                  1
                
-                80         106 LOAD_CONST              33 ('KY')
+                81         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-                63         110 MAP_ADD                  1
+                64         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-                81         114 LOAD_CONST              35 ('LA')
+                82         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-                63         118 MAP_ADD                  1
+                64         118 MAP_ADD                  1
                
-                82         120 LOAD_CONST              37 ('ME')
+                83         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-                63         124 MAP_ADD                  1
+                64         124 MAP_ADD                  1
                
-                83         126 LOAD_CONST              39 ('MD')
+                84         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-                63         130 MAP_ADD                  1
+                64         130 MAP_ADD                  1
                
-                84         132 LOAD_CONST              41 ('MA')
+                85         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-                63         136 MAP_ADD                  1
+                64         136 MAP_ADD                  1
                
-                85         138 LOAD_CONST              43 ('MI')
+                86         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-                63         142 MAP_ADD                  1
+                64         142 MAP_ADD                  1
                
-                86         144 LOAD_CONST              45 ('MN')
+                87         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-                63         148 MAP_ADD                  1
+                64         148 MAP_ADD                  1
                
-                87         150 LOAD_CONST              47 ('MS')
+                88         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-                63         154 MAP_ADD                  1
+                64         154 MAP_ADD                  1
                
-                88         156 LOAD_CONST              49 ('MO')
+                89         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-                63         160 MAP_ADD                  1
+                64         160 MAP_ADD                  1
                
-                89         162 LOAD_CONST              51 ('MT')
+                90         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-                63         166 MAP_ADD                  1
+                64         166 MAP_ADD                  1
                
-                90         168 LOAD_CONST              53 ('NE')
+                91         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-                63         172 MAP_ADD                  1
+                64         172 MAP_ADD                  1
                
-                91         174 LOAD_CONST              55 ('NV')
+                92         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-                63         178 MAP_ADD                  1
+                64         178 MAP_ADD                  1
                
-                92         180 LOAD_CONST              57 ('NH')
+                93         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-                63         184 MAP_ADD                  1
+                64         184 MAP_ADD                  1
                
-                93         186 LOAD_CONST              59 ('NJ')
+                94         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-                63         190 MAP_ADD                  1
+                64         190 MAP_ADD                  1
                
-                94         192 LOAD_CONST              61 ('NM')
+                95         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-                63         196 MAP_ADD                  1
+                64         196 MAP_ADD                  1
                
-                95         198 LOAD_CONST              63 ('NY')
+                96         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-                63         202 MAP_ADD                  1
+                64         202 MAP_ADD                  1
                
-                96         204 LOAD_CONST              65 ('NC')
+                97         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-                63         208 MAP_ADD                  1
+                64         208 MAP_ADD                  1
                
-                97         210 LOAD_CONST              67 ('ND')
+                98         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-                63         214 MAP_ADD                  1
+                64         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-                98         220 LOAD_CONST              69 ('OH')
+                99         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-                63         224 MAP_ADD                  1
+                64         224 MAP_ADD                  1
                
-                99         226 LOAD_CONST              71 ('OK')
+               100         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-                63         230 MAP_ADD                  1
+                64         230 MAP_ADD                  1
                
-               100         232 LOAD_CONST              73 ('OR')
+               101         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-                63         236 MAP_ADD                  1
+                64         236 MAP_ADD                  1
                
-               101         238 LOAD_CONST              75 ('PA')
+               102         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-                63         242 MAP_ADD                  1
+                64         242 MAP_ADD                  1
                
-               102         244 LOAD_CONST              77 ('RI')
+               103         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-                63         248 MAP_ADD                  1
+                64         248 MAP_ADD                  1
                
-               103         250 LOAD_CONST              79 ('SC')
+               104         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-                63         254 MAP_ADD                  1
+                64         254 MAP_ADD                  1
                
-               104         256 LOAD_CONST              81 ('SD')
+               105         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-                63         260 MAP_ADD                  1
+                64         260 MAP_ADD                  1
                
-               105         262 LOAD_CONST              83 ('TN')
+               106         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-                63         266 MAP_ADD                  1
+                64         266 MAP_ADD                  1
                
-               106         268 LOAD_CONST              85 ('TX')
+               107         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-                63         272 MAP_ADD                  1
+                64         272 MAP_ADD                  1
                
-               107         274 LOAD_CONST              87 ('UT')
+               108         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-                63         278 MAP_ADD                  1
+                64         278 MAP_ADD                  1
                
-               108         280 LOAD_CONST              89 ('VT')
+               109         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-                63         284 MAP_ADD                  1
+                64         284 MAP_ADD                  1
                
-               109         286 LOAD_CONST              91 ('VA')
+               110         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-                63         290 MAP_ADD                  1
+                64         290 MAP_ADD                  1
                
-               110         292 LOAD_CONST              93 ('WA')
+               111         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-                63         296 MAP_ADD                  1
+                64         296 MAP_ADD                  1
                
-               111         298 LOAD_CONST              95 ('WV')
+               112         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-                63         302 MAP_ADD                  1
+                64         302 MAP_ADD                  1
                
-               112         304 LOAD_CONST              97 ('WI')
+               113         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-                63         308 MAP_ADD                  1
+                64         308 MAP_ADD                  1
                
-               113         310 LOAD_CONST              99 ('WY')
+               114         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-                63         314 MAP_ADD                  1
+                64         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              5 (STATES)
                
-               117         320 LOAD_CONST             101 ('United States')
+               118         320 LOAD_CONST             101 ('United States')
                
-               118         322 LOAD_CONST             102 ('Canada')
+               119         322 LOAD_CONST             102 ('Canada')
                
-               119         324 LOAD_CONST             103 ('Mexico')
+               120         324 LOAD_CONST             103 ('Mexico')
                
-               120         326 LOAD_CONST             104 ('United Kingdom')
+               121         326 LOAD_CONST             104 ('United Kingdom')
                
-               116         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               117         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              4 (COUNTRIES)
                
-               123         334 LOAD_CONST             106 ('return')
+               124         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (dict)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             0 (search)
                            352 BUILD_TUPLE              1
-                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 123>)
+                           354 LOAD_CONST             107 (<code object _ownership_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 124>)
                            356 MAKE_FUNCTION           12 (annotations, closure)
                            358 STORE_FAST               1 (_ownership_filter)
                
-               136         360 LOAD_CONST             106 ('return')
+               137         360 LOAD_CONST             106 ('return')
                            362 LOAD_GLOBAL              2 (list)
                            374 BUILD_TUPLE              2
                            376 LOAD_CLOSURE             4 (COUNTRIES)
                            378 LOAD_CLOSURE             5 (STATES)
                            380 LOAD_CLOSURE             0 (search)
                            382 BUILD_TUPLE              3
-                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 136>)
+                           384 LOAD_CONST             108 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 137>)
                            386 MAKE_FUNCTION           12 (annotations, closure)
                            388 STORE_FAST               2 (_hq_include)
                
-               145         390 LOAD_CONST             106 ('return')
+               146         390 LOAD_CONST             106 ('return')
                            392 LOAD_GLOBAL              2 (list)
                            404 BUILD_TUPLE              2
                            406 LOAD_CLOSURE             0 (search)
                            408 BUILD_TUPLE              1
-                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 145>)
+                           410 LOAD_CONST             109 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 146>)
                            412 MAKE_FUNCTION           12 (annotations, closure)
                            414 STORE_FAST               3 (_hq_exclude)
                
-               152         416 LOAD_CONST             110 ('any')
+               153         416 LOAD_CONST             110 ('any')
                
-               153         418 LOAD_DEREF               0 (search)
+               154         418 LOAD_DEREF               0 (search)
                            420 LOAD_ATTR                2 (inclusion)
                            430 LOAD_CONST             111 ('keywords')
                            432 BINARY_SUBSCR
                
-               154         442 LOAD_DEREF               0 (search)
+               155         442 LOAD_DEREF               0 (search)
                            444 LOAD_ATTR                3 (exclusion)
                            454 LOAD_CONST             111 ('keywords')
                            456 BINARY_SUBSCR
                
-               155         466 LOAD_DEREF               0 (search)
+               156         466 LOAD_DEREF               0 (search)
                            468 LOAD_ATTR                2 (inclusion)
                            478 LOAD_CONST             112 ('employees_range')
                            480 BINARY_SUBSCR
                
-               156         490 PUSH_NULL
+               157         490 PUSH_NULL
                            492 LOAD_FAST                1 (_ownership_filter)
                            494 PRECALL                  0
                            498 CALL                     0
                
-               158         508 PUSH_NULL
+               159         508 PUSH_NULL
                            510 LOAD_FAST                2 (_hq_include)
                            512 PRECALL                  0
                            516 CALL                     0
                
-               159         526 PUSH_NULL
+               160         526 PUSH_NULL
                            528 LOAD_FAST                3 (_hq_exclude)
                            530 PRECALL                  0
                            534 CALL                     0
                
-               157         544 LOAD_CONST             113 (('include', 'exclude'))
+               158         544 LOAD_CONST             113 (('include', 'exclude'))
                            546 BUILD_CONST_KEY_MAP      2
                
-               151         548 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
+               152         548 LOAD_CONST             114 (('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters'))
                            550 BUILD_CONST_KEY_MAP      6
                            552 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
@@ -892,22 +914,22 @@
                         000000000000007c00a6010000ab01000000000000000074030000000000
                         000000000089016a020000000000000000a0030000000000000000000000
                         00000000000000000064026700a6020000ab020000000000000000a60100
                         00ab0100000000000000007a0a0000a6010000ab01000000000000000053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                     123           2 RESUME                   0
+                     124           2 RESUME                   0
                      
-                     125           4 BUILD_LIST               0
-                                   6 LOAD_CONST               1 (('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add-on'))
+                     126           4 BUILD_LIST               0
+                                   6 LOAD_CONST               1 (('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add_on'))
                                    8 LIST_EXTEND              1
                                   10 STORE_FAST               0 (OWNERSHIP)
                      
-                     134          12 LOAD_GLOBAL              1 (NULL + list)
+                     135          12 LOAD_GLOBAL              1 (NULL + list)
                                   24 LOAD_GLOBAL              3 (NULL + set)
                                   36 LOAD_FAST                0 (OWNERSHIP)
                                   38 PRECALL                  1
                                   42 CALL                     1
                                   52 LOAD_GLOBAL              3 (NULL + set)
                                   64 LOAD_DEREF               1 (search)
                                   66 LOAD_ATTR                2 (exclusion)
@@ -920,23 +942,23 @@
                                  120 CALL                     1
                                  130 BINARY_OP               10 (-)
                                  134 PRECALL                  1
                                  138 CALL                     1
                                  148 RETURN_VALUE
                      consts
                         None
-                        ('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add-on')
+                        ('bootstrapped', 'investor_backed', 'public', 'public_subsidiary', 'private_subsidiary', 'private_equity', 'private_equity_add_on')
                         'ownership'
                      names      ('list', 'set', 'exclusion', 'get')
                      varnames   ('OWNERSHIP',)
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_ownership_filter'
-                     firstlineno 123
+                     firstlineno 124
                      lnotab 0x04020809
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 6
                      flags     : 19
                      code
@@ -947,142 +969,142 @@
                         00000001008c2089056a000000000000000000a001000000000000000000
                         000000000000000000000064026700a6020000ab02000000000000000044
                         005d1f7d027c00a002000000000000000000000000000000000000000064
                         0289037c02190000000000000000006901a6010000ab0100000000000000
                         0001008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     136           2 RESUME                   0
+                     137           2 RESUME                   0
                      
-                     137           4 BUILD_LIST               0
+                     138           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     138           8 LOAD_DEREF               5 (search)
+                     139           8 LOAD_DEREF               5 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     140          66 LOAD_FAST                0 (include)
+                     141          66 LOAD_FAST                0 (include)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_DEREF               4 (STATES)
                                   94 LOAD_FAST                1 (state)
                                   96 BINARY_SUBSCR
                                  106 BUILD_MAP                1
                                  108 PRECALL                  1
                                  112 CALL                     1
                                  122 POP_TOP
                                  124 JUMP_BACKWARD           32 (to 62)
                      
-                     141     >>  126 LOAD_DEREF               5 (search)
+                     142     >>  126 LOAD_DEREF               5 (search)
                                  128 LOAD_ATTR                0 (inclusion)
                                  138 LOAD_METHOD              1 (get)
                                  160 LOAD_CONST               2 ('country')
                                  162 BUILD_LIST               0
                                  164 PRECALL                  2
                                  168 CALL                     2
                                  178 GET_ITER
                              >>  180 FOR_ITER                31 (to 244)
                                  182 STORE_FAST               2 (country)
                      
-                     142         184 LOAD_FAST                0 (include)
+                     143         184 LOAD_FAST                0 (include)
                                  186 LOAD_METHOD              2 (append)
                                  208 LOAD_CONST               2 ('country')
                                  210 LOAD_DEREF               3 (COUNTRIES)
                                  212 LOAD_FAST                2 (country)
                                  214 BINARY_SUBSCR
                                  224 BUILD_MAP                1
                                  226 PRECALL                  1
                                  230 CALL                     1
                                  240 POP_TOP
                                  242 JUMP_BACKWARD           32 (to 180)
                      
-                     143     >>  244 LOAD_FAST                0 (include)
+                     144     >>  244 LOAD_FAST                0 (include)
                                  246 RETURN_VALUE
                      consts
                         None
                         'state'
                         'country'
                      names      ('inclusion', 'get', 'append')
                      varnames   ('include', 'state', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 136
+                     firstlineno 137
                      lnotab 0x040104013a023c013a013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007d0089026a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d197d017c00a00200000000000000000000000000000000000000
                         0064017c016901a6010000ab01000000000000000001008c1a7c005300
                                    0 COPY_FREE_VARS           1
                      
-                     145           2 RESUME                   0
+                     146           2 RESUME                   0
                      
-                     146           4 BUILD_LIST               0
+                     147           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     147           8 LOAD_DEREF               2 (search)
+                     148           8 LOAD_DEREF               2 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                25 (to 114)
                                   64 STORE_FAST               1 (state)
                      
-                     148          66 LOAD_FAST                0 (exclude)
+                     149          66 LOAD_FAST                0 (exclude)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_FAST                1 (state)
                                   94 BUILD_MAP                1
                                   96 PRECALL                  1
                                  100 CALL                     1
                                  110 POP_TOP
                                  112 JUMP_BACKWARD           26 (to 62)
                      
-                     149     >>  114 LOAD_FAST                0 (exclude)
+                     150     >>  114 LOAD_FAST                0 (exclude)
                                  116 RETURN_VALUE
                      consts
                         None
                         'state'
                      names      ('exclusion', 'get', 'append')
                      varnames   ('exclude', 'state')
                      freevars   ('search',)
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_exclude'
-                     firstlineno 145
+                     firstlineno 146
                      lnotab 0x040104013a013001
                   'any'
                   'keywords'
                   'employees_range'
                   ('include', 'exclude')
                   ('op', 'include', 'exclude', 'employees_range', 'ownership', 'headquarters')
                names      ('dict', 'list', 'inclusion', 'exclusion')
                varnames   ('search', '_ownership_filter', '_hq_include', '_hq_exclude')
                freevars   ()
                cellvars   ('search', 'COUNTRIES', 'STATES')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_get_api_filter'
-               firstlineno 62
+               firstlineno 63
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
@@ -1092,57 +1114,57 @@
          names      ('__name__', '__module__', '__qualname__', 'os', 'getenv', 'HEADERS', 'str', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
          firstlineno 10
-         lnotab 0x0a021e0102fe06050603141110111009
+         lnotab 0x0a021e0102fe06050603141110121009
       'GrataWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026401650364026504640365056606640484045a
             0664026504640365056604640584045a0764016503640365056604640684
             045a0864075300
-         164           0 RESUME                   0
+         165           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         165          10 LOAD_CONST               1 ('domain')
+         166          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 165>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 166>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         168          30 LOAD_CONST               2 ('search')
+         169          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 168>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 169>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         171          46 LOAD_CONST               1 ('domain')
+         172          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 171>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 172>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -1150,79 +1172,79 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               165           0 RESUME                   0
+               166           0 RESUME                   0
                
-               166           2 LOAD_CONST               0 (None)
+               167           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 165
+               firstlineno 166
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               168           0 RESUME                   0
+               169           0 RESUME                   0
                
-               169           2 LOAD_CONST               0 (None)
+               170           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 168
+               firstlineno 169
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               171           0 RESUME                   0
+               172           0 RESUME                   0
                
-               172           2 LOAD_CONST               0 (None)
+               173           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 171
+               firstlineno 172
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 164
+         firstlineno 165
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
    names      ('gandai', 'query', 'gandai.models', 'Search', 'requests', 'os', 'dotenv', 'load_dotenv', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c01080108010c0214031a7f001b
+   lnotab 0x00ff02010c010c01080108010c0214031a7f001c
```

### Comparing `gandai-1.1.3/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.4/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/adapters/__pycache__/filters.cpython-311.pyc` & `gandai-1.1.4/gandai/adapters/__pycache__/filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/adapters/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.4/gandai/adapters/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/adapters/dealcloud.py` & `gandai-1.1.4/gandai/adapters/dealcloud.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import json
-from gandai.datastore import Cloudstore
-import pandas as pd
-
-ds = Cloudstore()
-keys = ds.keys()
+# import json
+# from gandai.datastore import Cloudstore
+# import pandas as pd
+
+# ds = Cloudstore()
+# keys = ds.keys()
 
 
 
-def seed_search(engagement: pd.Series, force=False) -> None:
-    data = json.loads(engagement.dropna().to_json())  # ugly
-
-    DEFAULT_KEYWORDS = []
-
-    DEFAULT_FILTER =  {
-        "employees_range": [25,2500],
-        "country": ["USA", "CAN", "MEX"],
-        "state": [],
-    }
-
-    DEFAULT_SORT = {
-        "sort_field": "employee_count", 
-        "sort_order": "desc"
-    }
-
-    search = {
-        "key": data["dealcloud_id"],
-        "label": data["engagement_name"],
-        "meta": data
-    }
-
-    SEARCH_BASE = f'searches/{search["key"]}'
-    search_key: str = f'{SEARCH_BASE}/search'
-    filters_key: str = f'{SEARCH_BASE}/filters'
-    sort_key: str = f'{SEARCH_BASE}/sort'
-    keywords_key: str = f'{SEARCH_BASE}/keywords'
-
-    if search_key in keys:
-        print(f"already exists: {search_key}")
-        if force:
-            print("force update")
-            ds[search_key] = search
+# def seed_search(engagement: pd.Series, force=False) -> None:
+#     data = json.loads(engagement.dropna().to_json())  # ugly
+
+#     DEFAULT_KEYWORDS = []
+
+#     DEFAULT_FILTER =  {
+#         "employees_range": [25,2500],
+#         "country": ["USA", "CAN", "MEX"],
+#         "state": [],
+#     }
+
+#     DEFAULT_SORT = {
+#         "sort_field": "employee_count", 
+#         "sort_order": "desc"
+#     }
+
+#     search = {
+#         "key": data["dealcloud_id"],
+#         "label": data["engagement_name"],
+#         "meta": data
+#     }
+
+#     SEARCH_BASE = f'searches/{search["key"]}'
+#     search_key: str = f'{SEARCH_BASE}/search'
+#     filters_key: str = f'{SEARCH_BASE}/filters'
+#     sort_key: str = f'{SEARCH_BASE}/sort'
+#     keywords_key: str = f'{SEARCH_BASE}/keywords'
+
+#     if search_key in keys:
+#         print(f"already exists: {search_key}")
+#         if force:
+#             print("force update")
+#             ds[search_key] = search
             
-    else:
-        ds[search_key] = search
-        ds[filters_key] = DEFAULT_FILTER
-        ds[sort_key] = DEFAULT_SORT
-        ds[keywords_key] = DEFAULT_KEYWORDS
-        print(f"seeded: {search_key}")
+#     else:
+#         ds[search_key] = search
+#         ds[filters_key] = DEFAULT_FILTER
+#         ds[sort_key] = DEFAULT_SORT
+#         ds[keywords_key] = DEFAULT_KEYWORDS
+#         print(f"seeded: {search_key}")
```

### Comparing `gandai-1.1.3/gandai/adapters/filters.py` & `gandai-1.1.4/gandai/adapters/filters.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/adapters/grata.py` & `gandai-1.1.4/gandai/adapters/grata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-import os
-import pandas as pd
-import requests
-from pathlib import Path
-from dotenv import load_dotenv
-
-from gandai.datastore import Cloudstore
-from gandai.adapters import filters
-
-# load_dotenv(f'{Path(__file__).parent.parent.parent}/.env') # well this doesn't feel good
-
-ds = Cloudstore()
-
-class GrataWrapper:
-    def __init__(self) -> None:
-        self.token = self._authenticate()
-        self.headers = {"authorization": self.token}
-
-    def build_similiar_targets_from_id(self, search_key: str, id: str, k=25) -> None:
-        """Gets + Caches Feature Table, returns the id"""
-
-        json_data = {
-            "filters": {
-                "similar_companies": self._get_similiars_filter([id]),
-                "tolerance": 100,
-            },
-            "page": 1,
-            "page_size": k,
-            "paging": True,
-            "query": "",
-        }
-
-        response = requests.post(
-            "https://search.grata.com/api/search/",
-            headers=self.headers,
-            json=json_data,
-        )
-
-        if response.status_code != 200:
-            print(response)  # .code, response.content)
-            return data
-
-        data = response.json()
-        # print(data.keys(), "todo handle suggested keywords")
-        features: pd.DataFrame = self._get_companies_features(data['companies'])
-        gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{id}.feather"
-        features.to_feather(gs_url)
-        print(features.shape, gs_url)
-
-    def build_targets_from_keyword(self, search_key: str, keyword: str, k=25) -> None:
-        """Gets + Caches Feature Table"""
-
-        def _get_targets_from_keyword(self, keyword: str, k=25) -> dict:
-            payload = {
-                "filters": {
-                    "keywords": self._get_keywords_filter([keyword]),
-                    "locations": filters.CORE_LOCATION_FILTER,
-                },
-                "page": 1,
-                "page_size": k,
-                "query": "",
-            }
-            response = requests.post(
-                "https://search.grata.com/api/search/",
-                headers=self.headers,
-                json=payload,
-            )
-            data = response.json()
-            return data
-
-        data = _get_targets_from_keyword(self, keyword, k)
-        features: pd.DataFrame = self._get_companies_features(data['companies'])
-        gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{str(keyword)}.feather"
-        features.to_feather(gs_url)
-
-    def get_company_id_by_domain(self, domain: str) -> str:
-        params = {"query": domain}
-        response = requests.get(
-            "https://search.grata.com/api/v3/suggest/",
-            headers=self.headers,
-            params=params,
-        )
-        data = response.json()
-        for company in data["companies"]:
-            if domain in company['domains']:
-                return company['id']
+# import os
+# import pandas as pd
+# import requests
+# from pathlib import Path
+# from dotenv import load_dotenv
+
+# from gandai.datastore import Cloudstore
+# from gandai.adapters import filters
+
+# # load_dotenv(f'{Path(__file__).parent.parent.parent}/.env') # well this doesn't feel good
+
+# ds = Cloudstore()
+
+# class GrataWrapper:
+#     def __init__(self) -> None:
+#         self.token = self._authenticate()
+#         self.headers = {"authorization": self.token}
+
+#     def build_similiar_targets_from_id(self, search_key: str, id: str, k=25) -> None:
+#         """Gets + Caches Feature Table, returns the id"""
+
+#         json_data = {
+#             "filters": {
+#                 "similar_companies": self._get_similiars_filter([id]),
+#                 "tolerance": 100,
+#             },
+#             "page": 1,
+#             "page_size": k,
+#             "paging": True,
+#             "query": "",
+#         }
+
+#         response = requests.post(
+#             "https://search.grata.com/api/search/",
+#             headers=self.headers,
+#             json=json_data,
+#         )
+
+#         if response.status_code != 200:
+#             print(response)  # .code, response.content)
+#             return data
+
+#         data = response.json()
+#         # print(data.keys(), "todo handle suggested keywords")
+#         features: pd.DataFrame = self._get_companies_features(data['companies'])
+#         gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{id}.feather"
+#         features.to_feather(gs_url)
+#         print(features.shape, gs_url)
+
+#     def build_targets_from_keyword(self, search_key: str, keyword: str, k=25) -> None:
+#         """Gets + Caches Feature Table"""
+
+#         def _get_targets_from_keyword(self, keyword: str, k=25) -> dict:
+#             payload = {
+#                 "filters": {
+#                     "keywords": self._get_keywords_filter([keyword]),
+#                     "locations": filters.CORE_LOCATION_FILTER,
+#                 },
+#                 "page": 1,
+#                 "page_size": k,
+#                 "query": "",
+#             }
+#             response = requests.post(
+#                 "https://search.grata.com/api/search/",
+#                 headers=self.headers,
+#                 json=payload,
+#             )
+#             data = response.json()
+#             return data
+
+#         data = _get_targets_from_keyword(self, keyword, k)
+#         features: pd.DataFrame = self._get_companies_features(data['companies'])
+#         gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{str(keyword)}.feather"
+#         features.to_feather(gs_url)
+
+#     def get_company_id_by_domain(self, domain: str) -> str:
+#         params = {"query": domain}
+#         response = requests.get(
+#             "https://search.grata.com/api/v3/suggest/",
+#             headers=self.headers,
+#             params=params,
+#         )
+#         data = response.json()
+#         for company in data["companies"]:
+#             if domain in company['domains']:
+#                 return company['id']
         
 
-    def get_company_features_by_id(self, id: str) -> dict:
-        """company from direct endpoint(s)"""
+#     def get_company_features_by_id(self, id: str) -> dict:
+#         """company from direct endpoint(s)"""
 
-        def _get_company_by_id(id: str) -> dict:
-            response = requests.get(
-                f"https://search.grata.com/api/company/{id}/", headers=self.headers
-            )
-            company = response.json()
-            return company
-
-        def _get_locations_by_id(id: str) -> list:
-            params = {
-                "type": "locations",
-            }
-            response = requests.get(
-                f"https://search.grata.com/api/company/{id}/additional/",
-                params=params,
-                headers=self.headers,
-            )
-            data = response.json()
-            return data
-
-        def _get_hq_by_id(id: str) -> dict:
-            def _get_hq(locations: list):
-                for location in locations:
-                    if location["location_type"] == "HQ":
-                        return location
+#         def _get_company_by_id(id: str) -> dict:
+#             response = requests.get(
+#                 f"https://search.grata.com/api/company/{id}/", headers=self.headers
+#             )
+#             company = response.json()
+#             return company
+
+#         def _get_locations_by_id(id: str) -> list:
+#             params = {
+#                 "type": "locations",
+#             }
+#             response = requests.get(
+#                 f"https://search.grata.com/api/company/{id}/additional/",
+#                 params=params,
+#                 headers=self.headers,
+#             )
+#             data = response.json()
+#             return data
+
+#         def _get_hq_by_id(id: str) -> dict:
+#             def _get_hq(locations: list):
+#                 for location in locations:
+#                     if location["location_type"] == "HQ":
+#                         return location
                     
-                return {} # todo handle no hq
+#                 return {} # todo handle no hq
 
-            locations = _get_locations_by_id(id)
-            return _get_hq(locations)
+#             locations = _get_locations_by_id(id)
+#             return _get_hq(locations)
 
-        def _get_employee_count(company) -> int:
-            try:
-                return company["employees_estimate"]["grata"]["count"]
-            except:
-                print("Could not find employee count for ", company)
-                return None
+#         def _get_employee_count(company) -> int:
+#             try:
+#                 return company["employees_estimate"]["grata"]["count"]
+#             except:
+#                 print("Could not find employee count for ", company)
+#                 return None
 
-        def _get_linkedin(company) -> str:
-            return company.get("social_linkedin")
+#         def _get_linkedin(company) -> str:
+#             return company.get("social_linkedin")
 
-        def _get_state(company_hq) -> str:
-            return company_hq.get("region_iso")
+#         def _get_state(company_hq) -> str:
+#             return company_hq.get("region_iso")
 
-        def _get_country(company_hq) -> str:
-            return company_hq.get("country_iso3")
+#         def _get_country(company_hq) -> str:
+#             return company_hq.get("country_iso3")
 
-        def _get_city_state(company_hq) -> str:
-            return f"{company_hq.get('city_name')}, {_get_state(company_hq)}"
+#         def _get_city_state(company_hq) -> str:
+#             return f"{company_hq.get('city_name')}, {_get_state(company_hq)}"
             
         
 
-        company = _get_company_by_id(id)
-        company_hq = _get_hq_by_id(id)
-        # ^ async opportunity
-
-        return {
-            "id": company.get("id"),
-            "name": company.get("name"),
-            "domain": company.get("domain"),
-            "description": company.get("description"),
-            "year_founded": company.get("year_founded"),
-            "employee_count": _get_employee_count(company),
-            "linkedin": _get_linkedin(company),
-            "city_state": _get_city_state(company_hq),
-            "state": _get_state(company_hq),
-            "country": _get_country(company_hq),
-        }
+#         company = _get_company_by_id(id)
+#         company_hq = _get_hq_by_id(id)
+#         # ^ async opportunity
+
+#         return {
+#             "id": company.get("id"),
+#             "name": company.get("name"),
+#             "domain": company.get("domain"),
+#             "description": company.get("description"),
+#             "year_founded": company.get("year_founded"),
+#             "employee_count": _get_employee_count(company),
+#             "linkedin": _get_linkedin(company),
+#             "city_state": _get_city_state(company_hq),
+#             "state": _get_state(company_hq),
+#             "country": _get_country(company_hq),
+#         }
     
-    def build_target_from_domain(self, search_key: str, domain: str) -> str:
-        company_id = self.get_company_id_by_domain(domain=domain)
-        company_features = self.get_company_features_by_id(company_id)
-        df = pd.DataFrame([company_features])
-        gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{company_id}-insert.feather"
-        df.to_feather(gs_url)
-        return company_id
-
-    @staticmethod
-    def _authenticate():
-        json_data = {
-            "email": os.getenv("GRATA_USER"),  
-            "password": os.getenv("GRATA_PASSWORD"),
-        }
-        response = requests.post(
-            "https://login.grata.com/api/authenticate/", json=json_data
-        )
-        data = response.json()
-        token = data["user"]["token"]
-        os.environ["GRATA_TOKEN"] = f"Token {token}"
-        return f"Token {token}"
-
-    @staticmethod
-    def _get_keywords_filter(keywords: list) -> dict:
-        return {
-            "op": "and",
-            "conditions": [
-                {
-                    "include": keywords,
-                    "exclude": [],
-                    "op": "any",
-                    "match": "core",
-                    "weight": 3,
-                    "type": "filter",
-                },
-            ],
-        }
-
-    @staticmethod
-    def _get_similiars_filter(ids: list) -> dict:
-        # NB filters also takes a tolerance, e.g. 100
-        return {
-            "op": "and",
-            "conditions": [
-                {
-                    "include": ids,
-                    "exclude": [],
-                    "op": "any",
-                },
-            ],
-        }
-
-    @staticmethod
-    def _get_companies_features(companies: list) -> pd.DataFrame:
-        df = pd.DataFrame(companies)
-
-        # add features
-        # df["employee_count"] = df["employees"].apply(lambda x: x.get("value"))
-        def _get_employee_count(row: dict):
-            try:
-                # return row['employees']['value']
-                return row["employees_estimate"]["grata"]["count"]
-            except:
-                return None
+#     def build_target_from_domain(self, search_key: str, domain: str) -> str:
+#         company_id = self.get_company_id_by_domain(domain=domain)
+#         company_features = self.get_company_features_by_id(company_id)
+#         df = pd.DataFrame([company_features])
+#         gs_url = f"gs://{ds.BUCKET_NAME}/searches/{search_key}/companies/{company_id}-insert.feather"
+#         df.to_feather(gs_url)
+#         return company_id
+
+#     @staticmethod
+#     def _authenticate():
+#         json_data = {
+#             "email": os.getenv("GRATA_USER"),  
+#             "password": os.getenv("GRATA_PASSWORD"),
+#         }
+#         response = requests.post(
+#             "https://login.grata.com/api/authenticate/", json=json_data
+#         )
+#         data = response.json()
+#         token = data["user"]["token"]
+#         os.environ["GRATA_TOKEN"] = f"Token {token}"
+#         return f"Token {token}"
+
+#     @staticmethod
+#     def _get_keywords_filter(keywords: list) -> dict:
+#         return {
+#             "op": "and",
+#             "conditions": [
+#                 {
+#                     "include": keywords,
+#                     "exclude": [],
+#                     "op": "any",
+#                     "match": "core",
+#                     "weight": 3,
+#                     "type": "filter",
+#                 },
+#             ],
+#         }
+
+#     @staticmethod
+#     def _get_similiars_filter(ids: list) -> dict:
+#         # NB filters also takes a tolerance, e.g. 100
+#         return {
+#             "op": "and",
+#             "conditions": [
+#                 {
+#                     "include": ids,
+#                     "exclude": [],
+#                     "op": "any",
+#                 },
+#             ],
+#         }
+
+#     @staticmethod
+#     def _get_companies_features(companies: list) -> pd.DataFrame:
+#         df = pd.DataFrame(companies)
+
+#         # add features
+#         # df["employee_count"] = df["employees"].apply(lambda x: x.get("value"))
+#         def _get_employee_count(row: dict):
+#             try:
+#                 # return row['employees']['value']
+#                 return row["employees_estimate"]["grata"]["count"]
+#             except:
+#                 return None
 
-        def _get_country(headquarters: dict) -> str:
-            return headquarters.get("country_iso")
+#         def _get_country(headquarters: dict) -> str:
+#             return headquarters.get("country_iso")
 
-        df["employee_count"] = df.apply(_get_employee_count, axis=1)
+#         df["employee_count"] = df.apply(_get_employee_count, axis=1)
         
-        # null hq is a problem
-        if 'headquarters' in df.columns:
-            df["country"] = df["headquarters"].dropna().apply(_get_country)
-            df["state"] = df["headquarters"].dropna().apply(lambda x: x.get("region_iso"))
-        else:
-            df["country"] = None
-            df["state"] = None
-        if 'headquarters_pretty' in df.columns:
-            df["city_state"] = df["headquarters_pretty"]
-        else:
-            df["city_state"] = None
-
-        df = df.dropna(subset=["employee_count", "domain"])
-        df = df[
-            [
-                "name",
-                "domain",
-                "description",
-                "employee_count",
-                "linkedin",
-                "year_founded",
-                "city_state",
-                "state",
-                "country",
-                "id",
-                # "ownership", # dont really trust this
-                # "web_hit_count",
-                # "primary_business_model_name",
-            ]
-        ]
-
-        df = df.reset_index(drop=True)
-        return df
-
-    @staticmethod
-    def _get_company_features(company: dict) -> pd.DataFrame:
-        """
-        takes in grata company from https://search.grata.com/api/company/
-        normalizes against
-        """
-
-        def _get_employee_count(company) -> int:
-            pass
-
-        def _get_linkedin(company) -> str:
-            pass
-
-        def _get_state(company) -> str:
-            pass
-
-        def _get_country(company) -> str:
-            pass
-
-        def _get_city_state(company) -> str:
-            pass
-
-        features = {
-            "id": company.get("id"),
-            "name": company.get("name"),
-            "domain": company.get("domain"),
-            "description": company.get("description"),
-            "year_founded": company.get("year_founded"),
-            "employee_count": _get_employee_count(company),
-            "linkedin": _get_linkedin(company),
-            "city_state": _get_city_state(company),
-            "state": _get_state(company),
-            "country": _get_country(company),
-        }
-
-        df = df[
-            [
-                "name",
-                "domain",
-                "description",
-                "employee_count",
-                "linkedin",
-                "year_founded",
-                "city_state",
-                "state",
-                "country",
-                "id",
-            ]
-        ]
-        return df
+#         # null hq is a problem
+#         if 'headquarters' in df.columns:
+#             df["country"] = df["headquarters"].dropna().apply(_get_country)
+#             df["state"] = df["headquarters"].dropna().apply(lambda x: x.get("region_iso"))
+#         else:
+#             df["country"] = None
+#             df["state"] = None
+#         if 'headquarters_pretty' in df.columns:
+#             df["city_state"] = df["headquarters_pretty"]
+#         else:
+#             df["city_state"] = None
+
+#         df = df.dropna(subset=["employee_count", "domain"])
+#         df = df[
+#             [
+#                 "name",
+#                 "domain",
+#                 "description",
+#                 "employee_count",
+#                 "linkedin",
+#                 "year_founded",
+#                 "city_state",
+#                 "state",
+#                 "country",
+#                 "id",
+#                 # "ownership", # dont really trust this
+#                 # "web_hit_count",
+#                 # "primary_business_model_name",
+#             ]
+#         ]
+
+#         df = df.reset_index(drop=True)
+#         return df
+
+#     @staticmethod
+#     def _get_company_features(company: dict) -> pd.DataFrame:
+#         """
+#         takes in grata company from https://search.grata.com/api/company/
+#         normalizes against
+#         """
+
+#         def _get_employee_count(company) -> int:
+#             pass
+
+#         def _get_linkedin(company) -> str:
+#             pass
+
+#         def _get_state(company) -> str:
+#             pass
+
+#         def _get_country(company) -> str:
+#             pass
+
+#         def _get_city_state(company) -> str:
+#             pass
+
+#         features = {
+#             "id": company.get("id"),
+#             "name": company.get("name"),
+#             "domain": company.get("domain"),
+#             "description": company.get("description"),
+#             "year_founded": company.get("year_founded"),
+#             "employee_count": _get_employee_count(company),
+#             "linkedin": _get_linkedin(company),
+#             "city_state": _get_city_state(company),
+#             "state": _get_state(company),
+#             "country": _get_country(company),
+#         }
+
+#         df = df[
+#             [
+#                 "name",
+#                 "domain",
+#                 "description",
+#                 "employee_count",
+#                 "linkedin",
+#                 "year_founded",
+#                 "city_state",
+#                 "state",
+#                 "country",
+#                 "id",
+#             ]
+#         ]
+#         return df
```

### Comparing `gandai-1.1.3/gandai/auth.py` & `gandai-1.1.4/gandai/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import random
 from dataclasses import asdict, dataclass, field
 from hashlib import md5
 from time import time
 import os
 from twilio.rest import Client
 
-from gandai.datastore import Cloudstore
+# from gandai.datastore import Cloudstore
 
 # from gandai.models.User import user_exists # create_user
 
-ds = Cloudstore()
+# ds = Cloudstore()
 twilio_client = Client(os.getenv("TWILIO_APP"), os.getenv("TWILIO_TOKEN"))
 
 
 @dataclass
 class Auth:
     key: str = field(init=False)
     phone: str
@@ -31,34 +31,35 @@
         self.token = md5(self.key.encode()).hexdigest()
 
 
 def _send_code(auth: Auth) -> None:
     message = twilio_client.messages.create(
         to=auth.phone,
         from_=os.getenv("TWILIO_NUMBER"),
-        body=f"{auth.code} is your G&AI Research authentication code.",
+        body=f"{auth.code} is your GA Research authentication code.",
     )
     print(f"Login Sent to {auth.phone}")
 
 
 def send_code(phone: str) -> None:
     # Event.create(actor_key=phone)
     auth_code = str(random.randint(100000, 999999))
     auth = Auth(phone=phone, code=auth_code)
-    ds[auth.key] = asdict(auth)
+    # ds[auth.key] = asdict(auth)
     _send_code(auth)
 
 
 def authenticate(code: str) -> Auth:
-    keys = ds.keys("auth/")[1::]
-    df = pd.DataFrame(ds.load_async(keys))
-    df = df[df["expires"] > int(time())]
-    df = df[df["code"] == code]
-    if len(df) > 0:
-        # could parse to Auth and back to dict
-        return df.to_dict(orient="records")[0]
-    else:
-        return None
+    return None
+    # keys = ds.keys("auth/")[1::]
+    # df = pd.DataFrame(ds.load_async(keys))
+    # df = df[df["expires"] > int(time())]
+    # df = df[df["code"] == code]
+    # if len(df) > 0:
+    #     # could parse to Auth and back to dict
+    #     return df.to_dict(orient="records")[0]
+    # else:
+    #     return None
 
 
 def validate(token: str) -> bool:
     pass
```

### Comparing `gandai-1.1.3/gandai/datastore.py` & `gandai-1.1.4/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/db.py` & `gandai-1.1.4/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.3/gandai/main.py` & `gandai-1.1.4/gandai/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,104 @@
-
+import pandas as pd
 from dacite import from_dict
 from dataclasses import dataclass, field
 
 
 from gandai.models import Event, Company, Checkpoint
 from gandai import query
 
 from gandai.sources import GrataWrapper as grata
 
 
-
-
 def process_event(e: Event) -> None:
-    print(e)
-    search_uid = e.search_uid
-    search = query.find_search_by_uid(search_uid)
-
-    if e.type == "create":
-        pass
-    elif e.type == "advance":
-        # enrich the company
-        company = query.find_company_by_domain(e.domain)
-        resp = grata.enrich(company.domain)
-        if resp.get("status") == 404:
-            print(f"{company} not found")
-        else:
-            print(resp)
-            company.name = resp.get("name")
-            company.description = resp.get("description")
-            company.meta = company.meta | resp # merge 
-            query.update_company(company)
-
-
-    elif e.type == "validate":
-        # find similar companies
 
-        companies = grata.find_similar(domain=e.domain, search=search)
-        
+    def _insert_companies(companies: list, existing_domains: list) -> None:
+        # rewrite this in less db txns
         for company in companies:
-            print(company)
-            # first make sure the company is there
+            if company.get("domain") is None:
+                print(f"Missing domain: {company}. Skipping")
+                continue
+
+            if company["domain"] in existing_domains:
+                print(f"Skipping {company['domain']} as already a target")
+                continue
+            print(f"Adding {company['domain']} as target")
             query.insert_company(
                 Company(
                     domain=company["domain"],
                     name=company.get("name"),
                     description=company.get("description"),
-                    # meta=company, # merge this?
                 )
             )
-
-            # and "create"
             query.insert_event(
                 Event(
                     search_uid=search_uid,
                     domain=company.get("domain"),
-                    actor_key="gratabot",
+                    actor_key="grata",
                     type="create",
                 )
             )
-            # suggestions = suggestions.extend(
-            #     source_scrub.find_similar(domain=e.domain, search=search)
-            # )
-
-            # caching for page token
-            # TBD if I care
-            # query.insert_event(
-            #     Event(
-            #         domain=e.domain,
-            #         search_uid=search_uid,
-            #         type="generate",
-            #         actor_key="gratabot",
-            #         data=suggestions,
-            #     )
-            # )
 
+    search_uid = e.search_uid
+    if e.type == "create":
+        pass
+    elif e.type == "advance":
+        # enrich the company
+        company = query.find_company_by_domain(e.domain)
+        # might consider a check here to see if the company is already enriched
+        resp = grata.enrich(company.domain)
+        if resp.get("status") == 404:
+            print(f"{company} not found")
+        else:
+            print(resp)
+            company.name = resp.get("name")
+            company.description = resp.get("description")
+            company.meta = company.meta | resp  # merge
+            query.update_company(company)
+
+    elif e.type == "validate":
+        search = query.find_search_by_uid(search_uid)
+        _insert_companies(
+            companies=grata.find_similar(domain=e.domain, search=search), 
+            existing_domains=query.target(search_uid=search_uid)["domain"].tolist()
+        )
     elif e.type == "send":
         pass
     elif e.type == "accept":
         pass
     elif e.type == "reject":
         pass
     elif e.type == "conflict":
         pass
-    
     elif e.type == "criteria":
-        pass
-    
+        print("criteria search here we gooo")
+        search = query.find_search_by_uid(search_uid)
+        _insert_companies(
+            companies=grata.find_by_criteria(search), 
+            existing_domains=query.target(search_uid=search_uid)["domain"].tolist()
+        )
+
     # finally, record we processed the event
     query.insert_checkpoint(Checkpoint(event_id=e.id))
+    print(f"processed: {e}")
 
 
 def process_events(search_uid: int) -> int:
     """
     Process all events for a given search
     Could tidy
     """
     events = []
 
-    for event in query.event(search_uid).to_dict(orient='records'):
-        # event["data"] = json.loads(event["data"])
+    for event in query.event(search_uid).to_dict(orient="records"):
         event = from_dict(Event, event)
         events.append(event)
-        print(event)
 
     checkpoints = query.checkpoint()
+    print(checkpoints)
     processed_count = 0
     for e in events:
         if e.id not in checkpoints["event_id"]:
             process_event(e)
             processed_count += 1
 
     return processed_count
```

### Comparing `gandai-1.1.3/gandai/migrations/create_db.sql` & `gandai-1.1.4/gandai/migrations/db_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,114 @@
-CREATE TABLE search (
-    id SERIAL PRIMARY KEY,
-	uid INTEGER UNIQUE NOT NULL,
-    meta JSONB,
-    label VARCHAR(255) UNIQUE,
-    client_domain VARCHAR(255),
-    inclusion JSONB DEFAULT '{}'::jsonb,
-    exclusion JSONB DEFAULT '{}'::jsonb,
-    sort JSONB DEFAULT '{}'::jsonb,
-    created TIMESTAMP NOT NULL DEFAULT NOW(),
-    updated TIMESTAMP NOT NULL DEFAULT NOW()
-);
-
-CREATE TABLE company (
-    id SERIAL PRIMARY KEY,
-    domain VARCHAR(255) UNIQUE NOT NULL,
-    name VARCHAR(255),
-    description TEXT,
-    meta JSONB DEFAULT '{}'::jsonb, 
-    created TIMESTAMP NOT NULL DEFAULT NOW(),
-    updated TIMESTAMP NOT NULL DEFAULT NOW()
-
-);
-
-CREATE TABLE actor (
-    id SERIAL PRIMARY KEY,
-    key VARCHAR(255) UNIQUE NOT NULL,
-    type VARCHAR(255) NOT NULL,
-    name VARCHAR(255),
-    created TIMESTAMP NOT NULL DEFAULT NOW(),
-    updated TIMESTAMP NOT NULL DEFAULT NOW()
-);
-
-
-CREATE TABLE event (
-    id SERIAL PRIMARY KEY,
-    search_uid INTEGER NOT NULL REFERENCES search(uid),
-    domain VARCHAR(255) NOT NULL REFERENCES company(domain),
-    actor_key VARCHAR(255) NOT NULL REFERENCES actor(key),
-    type VARCHAR(255) NOT NULL,
-    data JSONB DEFAULT '{}'::jsonb,
-    created TIMESTAMP NOT NULL DEFAULT NOW()
-);
-
---ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid UNIQUE (type, domain, search_uid);
-
-
-CREATE TABLE checkpoint (
-    id SERIAL PRIMARY KEY,
-    event_id INTEGER NOT NULL REFERENCES event(id),
-    created TIMESTAMP NOT NULL DEFAULT NOW()
-);
-
-CREATE MATERIALIZED VIEW target AS
-SELECT 
-    e.id, 
-    e.search_uid, 
-    e.domain, 
-    e.data, 
-    e.type AS last_event_type, 
-    e.created AS last_event_dt,
-    c.name as name,
-    c.description as description,
-    c.meta as meta,
-    (c.meta->>'employees')::int AS employees,
-    (c.meta->>'ownership_status') AS ownership_status,
-    (c.meta->>'social_linkedin') AS linkedin,    
-    (r.data->>'rating')::int AS rating
-FROM (
-    SELECT 
-        domain, 
-        MAX(created) AS max_created
-    FROM 
-        event
-    WHERE 
-        type NOT IN ('comment','rating','generate')
-    GROUP BY 
-        domain
-) AS max_event
-JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created
-JOIN company c ON c.domain = e.domain
-LEFT JOIN (
-    SELECT 
-        domain, 
-        MAX(created) AS max_created
-    FROM 
-        event
-    WHERE 
-        type = 'rating'
-    GROUP BY 
-        domain
-) AS max_rating ON e.domain = max_rating.domain
-LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;
+import sqlalchemy
+from gandai.db import connect_with_connector
+from dotenv import load_dotenv
+
+load_dotenv()
+
+
+def create_db():
+    db = connect_with_connector()
+
+    statement = sqlalchemy.text(
+        """
+            CREATE TABLE IF NOT EXISTS search  (
+            id SERIAL PRIMARY KEY,
+            uid INTEGER UNIQUE NOT NULL,
+            meta JSONB,
+            label VARCHAR(255) UNIQUE,
+            client_domain VARCHAR(255),
+            inclusion JSONB DEFAULT '{}'::jsonb,
+            exclusion JSONB DEFAULT '{}'::jsonb,
+            sort JSONB DEFAULT '{}'::jsonb,
+            created TIMESTAMP NOT NULL DEFAULT NOW(),
+            updated TIMESTAMP NOT NULL DEFAULT NOW()
+        );
+
+        CREATE TABLE IF NOT EXISTS company (
+            id SERIAL PRIMARY KEY,
+            domain VARCHAR(255) UNIQUE NOT NULL,
+            name VARCHAR(255),
+            description TEXT,
+            meta JSONB DEFAULT '{}'::jsonb, 
+            created TIMESTAMP NOT NULL DEFAULT NOW(),
+            updated TIMESTAMP NOT NULL DEFAULT NOW()
+
+        );
+
+        CREATE TABLE IF NOT EXISTS actor (
+            id SERIAL PRIMARY KEY,
+            key VARCHAR(255) UNIQUE NOT NULL,
+            type VARCHAR(255) NOT NULL,
+            name VARCHAR(255),
+            created TIMESTAMP NOT NULL DEFAULT NOW(),
+            updated TIMESTAMP NOT NULL DEFAULT NOW()
+        );
+
+
+        CREATE TABLE IF NOT EXISTS event (
+            id SERIAL PRIMARY KEY,
+            search_uid INTEGER NOT NULL REFERENCES search(uid),
+            domain VARCHAR(255) REFERENCES company(domain),
+            actor_key VARCHAR(255) NOT NULL REFERENCES actor(key),
+            type VARCHAR(255) NOT NULL,
+            data JSONB DEFAULT '{}'::jsonb,
+            created TIMESTAMP NOT NULL DEFAULT NOW()
+        );
+
+        --ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid UNIQUE (type, domain, search_uid);
+
+
+        CREATE TABLE IF NOT EXISTS checkpoint (
+            id SERIAL PRIMARY KEY,
+            event_id INTEGER NOT NULL REFERENCES event(id),
+            created TIMESTAMP NOT NULL DEFAULT NOW()
+        );
+
+        CREATE MATERIALIZED VIEW IF NOT EXISTS target AS
+        SELECT 
+            e.id, 
+            e.search_uid, 
+            e.domain, 
+            e.data, 
+            e.type AS last_event_type, 
+            e.created AS last_event_dt,
+            c.name as name,
+            c.description as description,
+            c.meta as meta,
+            (c.meta->>'employees')::int AS employees,
+            (c.meta->>'ownership_status') AS ownership_status,
+            (c.meta->>'social_linkedin') AS linkedin,    
+            (r.data->>'rating')::int AS rating
+        FROM (
+            SELECT 
+                domain, 
+                MAX(created) AS max_created
+            FROM 
+                event
+            WHERE 
+                type NOT IN ('comment','rating','generate','criteria')
+            GROUP BY 
+                domain
+        ) AS max_event
+        JOIN event e ON e.domain = max_event.domain AND e.created = max_event.max_created
+        JOIN company c ON c.domain = e.domain
+        LEFT JOIN (
+            SELECT 
+                domain, 
+                MAX(created) AS max_created
+            FROM 
+                event
+            WHERE 
+                type = 'rating'
+            GROUP BY 
+                domain
+        ) AS max_rating ON e.domain = max_rating.domain
+        LEFT JOIN event r ON r.domain = max_rating.domain AND r.created = max_rating.max_created;
+    """
+    )
+    with db.connect() as conn:
+        conn.execute(statement)
+        conn.commit()
 
+
+if __name__ == "__main__":
+    create_db()
```

### Comparing `gandai-1.1.3/gandai/models.py` & `gandai-1.1.4/gandai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,22 @@
     CREATE = auto()
     ADVANCE = auto()
     VALIDATE = auto()
     SEND = auto()
     CLIENT_ACCEPT = auto()
     CONFLICT = auto()
     REJECT = auto()
+    CRITERIA = auto()
 
 
 @dataclass
 class Event:
     
     search_uid: int  # fk # add index 
-    domain: str  # fk
+    domain: Optional[str]  # fk
     actor_key: str  # fk
     type: str  # build, advance, qualify, reject, conflict, rate
     data: dict = field(default_factory=dict)
     id: int = field(default=None)  # pk
     # created: int = field(init=False)
```

### Comparing `gandai-1.1.3/gandai/query.py` & `gandai-1.1.4/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     EventType,
     Actor,
     Search,
     Checkpoint,
 )
 
 
-import os
 import sqlalchemy
 
 from google.cloud.sql.connector import Connector
 from dotenv import load_dotenv
 load_dotenv()
 
 from gandai.db import connect_with_connector
@@ -115,27 +114,35 @@
 def search():
     with db.connect() as conn:
         result = conn.execute(sqlalchemy.text("SELECT *, meta->>'group' as group FROM search"))
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     return df
 
 
-def target(search_uid: int, last_event_type: str = "advance"):
+def target(search_uid: int, last_event_type: str = None):
     with db.connect() as conn:
-        statement = "SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type"
-        result = conn.execute(
-            sqlalchemy.text(statement),
-            {"search_uid": search_uid, "last_event_type": last_event_type},
-        )
+        if last_event_type is not None:
+            statement = "SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type"
+            result = conn.execute(
+                sqlalchemy.text(statement),
+                {"search_uid": search_uid, "last_event_type": last_event_type},
+            )
+            
+        else:
+            statement = "SELECT * FROM target WHERE search_uid = :search_uid"
+            result = conn.execute(
+                sqlalchemy.text(statement),
+                {"search_uid": search_uid},
+            )
+            
         targets = pd.DataFrame(result.fetchall(), columns=result.keys())
-    
+
     comments = comment_by_domain(search_uid)
     targets = targets.merge(comments, on="domain", how="left")
     
-    
     # handle sorting
     search = find_search_by_uid(search_uid)
     targets = targets.sort_values(
         by=search.sort.get("field", "domain"), 
         ascending=search.sort.get("order") == "asc"
     )
```

### Comparing `gandai-1.1.3/gandai/sources.py` & `gandai-1.1.4/gandai/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,35 +24,36 @@
             json={
                 "domain": domain,
                 "employees_range": api_filters["employees_range"],
                 "headquarters": api_filters["headquarters"],
             },
         )
         data = response.json()
-        print(data)
+        print("find_similar:", data)
         data["companies"] = data.get("results",[])  # asking grata about this
         
         return data['companies']
 
     def find_by_criteria(search: Search) -> dict:
         api_filters = GrataWrapper._get_api_filter(search)
         response = requests.post(
             "https://search.grata.com/api/v1/search/",
             headers=GrataWrapper.HEADERS,
             json={
                 "op": "any",
                 "include": search.inclusion["keywords"],
                 "exclude": search.exclusion["keywords"],
                 "employees_range": api_filters["employees_range"],
-                # "ownership": api_filters["ownership"],
+                "ownership": api_filters["ownership"],
                 "headquarters": api_filters["headquarters"],
             },
         )
         data = response.json()
-        return data
+        print("find_by_criteria: ", data)
+        return data['companies']
 
     def enrich(domain: str) -> dict:
         response = requests.post(
             "https://search.grata.com/api/v1/enrich/",
             headers=GrataWrapper.HEADERS,
             json={"domain": domain},
         )
@@ -125,15 +126,15 @@
             OWNERSHIP = [
                 "bootstrapped",
                 "investor_backed",
                 "public",
                 "public_subsidiary",
                 "private_subsidiary",
                 "private_equity",
-                "private_equity_add-on",
+                "private_equity_add_on",
             ]
             return list(set(OWNERSHIP) - set(search.exclusion.get("ownership",[])))
 
         def _hq_include() -> list:
             include = []
             for state in search.inclusion.get("state", []):
                 # NB: API wants full state name, but product wants code
```

### Comparing `gandai-1.1.3/gandai.egg-info/SOURCES.txt` & `gandai-1.1.4/gandai.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 gandai.egg-info/SOURCES.txt
 gandai.egg-info/dependency_links.txt
 gandai.egg-info/top_level.txt
 gandai/__pycache__/__init__.cpython-311.pyc
 gandai/__pycache__/adapters.cpython-311.pyc
 gandai/__pycache__/auth.cpython-311.pyc
 gandai/__pycache__/datastore.cpython-311.pyc
+gandai/__pycache__/db.cpython-311.pyc
 gandai/__pycache__/grata.cpython-311.pyc
 gandai/__pycache__/main.cpython-311.pyc
 gandai/__pycache__/models.cpython-311.pyc
 gandai/__pycache__/query.cpython-311.pyc
 gandai/__pycache__/services.cpython-311.pyc
 gandai/__pycache__/sources.cpython-311.pyc
 gandai/adapters/__init__.py
@@ -28,9 +29,10 @@
 gandai/adapters/filters.py
 gandai/adapters/grata.py
 gandai/adapters/__pycache__/__init__.cpython-311.pyc
 gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
 gandai/adapters/__pycache__/filters.cpython-311.pyc
 gandai/adapters/__pycache__/grata.cpython-311.pyc
 gandai/migrations/__init__.py
-gandai/migrations/create_db.sql
+gandai/migrations/db_create.py
+gandai/migrations/db_seed.py
 gandai/migrations/dealcloud_to_gandai.py
```

