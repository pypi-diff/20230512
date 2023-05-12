# Comparing `tmp/the-spymaster-api-1.8.1.tar.gz` & `tmp/the_spymaster_api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the-spymaster-api-1.8.1.tar", last modified: Sat Apr 15 15:54:44 2023, max compression
+gzip compressed data, was "the_spymaster_api-1.9.0.tar", max compression
```

## Comparing `the-spymaster-api-1.8.1.tar` & `the_spymaster_api-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,8 @@
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/
--rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      183 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/setup.cfg
--rw-rw-r--   0 akali     (1000) akali     (1000)      557 2023-04-15 15:54:37.000000 the-spymaster-api-1.8.1/setup.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/the_spymaster_api/
--rw-rw-r--   0 akali     (1000) akali     (1000)       47 2022-09-25 13:05:12.000000 the-spymaster-api-1.8.1/the_spymaster_api/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     2227 2023-01-27 15:56:25.000000 the-spymaster-api-1.8.1/the_spymaster_api/client.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/the_spymaster_api/structs/
--rw-rw-r--   0 akali     (1000) akali     (1000)       63 2022-09-25 13:05:12.000000 the-spymaster-api-1.8.1/the_spymaster_api/structs/__init__.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      789 2023-04-08 20:38:47.000000 the-spymaster-api-1.8.1/the_spymaster_api/structs/errors.py
--rw-rw-r--   0 akali     (1000) akali     (1000)      952 2022-09-27 09:51:02.000000 the-spymaster-api-1.8.1/the_spymaster_api/structs/request.py
--rw-rw-r--   0 akali     (1000) akali     (1000)     1201 2023-04-15 15:53:56.000000 the-spymaster-api-1.8.1/the_spymaster_api/structs/response.py
-drwxrwxr-x   0 akali     (1000) akali     (1000)        0 2023-04-15 15:54:44.136866 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/
--rw-rw-r--   0 akali     (1000) akali     (1000)      306 2023-04-15 15:54:44.000000 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/PKG-INFO
--rw-rw-r--   0 akali     (1000) akali     (1000)      429 2023-04-15 15:54:44.000000 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/SOURCES.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)        1 2023-04-15 15:54:44.000000 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/dependency_links.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)      102 2023-04-15 15:54:44.000000 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/requires.txt
--rw-rw-r--   0 akali     (1000) akali     (1000)       18 2023-04-15 15:54:44.000000 the-spymaster-api-1.8.1/the_spymaster_api.egg-info/top_level.txt
+-rw-r--r--   0        0        0      432 2023-05-12 12:00:47.443122 the_spymaster_api-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2022-09-25 13:05:12.295878 the_spymaster_api-1.9.0/the_spymaster_api/__init__.py
+-rw-r--r--   0        0        0     2227 2023-01-27 15:56:25.666046 the_spymaster_api-1.9.0/the_spymaster_api/client.py
+-rw-r--r--   0        0        0       93 2023-05-12 12:00:19.390270 the_spymaster_api-1.9.0/the_spymaster_api/structs/__init__.py
+-rw-r--r--   0        0        0      789 2023-04-08 20:38:47.670026 the_spymaster_api-1.9.0/the_spymaster_api/structs/errors.py
+-rw-r--r--   0        0        0      952 2022-09-27 09:51:02.090239 the_spymaster_api-1.9.0/the_spymaster_api/structs/request.py
+-rw-r--r--   0        0        0     1201 2023-04-15 16:19:36.667573 the_spymaster_api-1.9.0/the_spymaster_api/structs/response.py
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 the_spymaster_api-1.9.0/PKG-INFO
```

### Comparing `the-spymaster-api-1.8.1/the_spymaster_api/client.py` & `the_spymaster_api-1.9.0/the_spymaster_api/client.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.8.1/the_spymaster_api/structs/errors.py` & `the_spymaster_api-1.9.0/the_spymaster_api/structs/errors.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.8.1/the_spymaster_api/structs/request.py` & `the_spymaster_api-1.9.0/the_spymaster_api/structs/request.py`

 * *Files identical despite different names*

### Comparing `the-spymaster-api-1.8.1/the_spymaster_api/structs/response.py` & `the_spymaster_api-1.9.0/the_spymaster_api/structs/response.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,12 +42,12 @@
 
 class GuessResponse(BaseModel):
     given_guess: Optional[GivenGuess]
     game_state: GameState
 
 
 class NextMoveResponse(BaseModel):
+    game_state: GameState
+    used_solver: Solver
     given_hint: Optional[GivenHint]
     given_guess: Optional[GivenGuess]
-    used_solver: Solver
     used_model_identifier: Optional[ModelIdentifier]
-    game_state: GameState
```

