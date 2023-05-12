# Comparing `tmp/biobricks-0.1.62.tar.gz` & `tmp/biobricks-0.1.63.tar.gz`

## Comparing `biobricks-0.1.62.tar` & `biobricks-0.1.63.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.62/coverage.xml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.62/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.62/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.62/.vscode/tasks.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/api.py
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/brick.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/checks.py
--rwxr-xr-x   0        0        0     4653 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/config.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.62/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.62/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.62/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.62/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.62/LICENSE
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.62/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.62/pyproject.toml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.62/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.63/coverage.xml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.63/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.63/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.63/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.63/.vscode/tasks.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/api.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/brick.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/checks.py
+-rwxr-xr-x   0        0        0     4750 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/config.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.63/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.63/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.63/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.63/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.63/LICENSE
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.63/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.63/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.63/PKG-INFO
```

### Comparing `biobricks-0.1.62/biobricks.svg` & `biobricks-0.1.63/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/coverage.xml` & `biobricks-0.1.63/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/.github/workflows/biobricks.yml` & `biobricks-0.1.63/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/api.py` & `biobricks-0.1.63/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/brick.py` & `biobricks-0.1.63/biobricks/brick.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/checks.py` & `biobricks-0.1.63/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/cli.py` & `biobricks-0.1.63/biobricks/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     config = read_config()
 
     # CHECK IF CONFIG WILL OVERWRITE EXISTING
     msg = click.style("WARNING: overwrite existing config?", fg="red")
     if path.exists() and not overwrite and not click.confirm(msg):
         sys.exit(0)
     
+    # EMAIL PROMPT 
+    email = click.prompt("Choose Email", type=click.Path())
+
     # BBLIB PROMPT - DEFAULT TO EXISTING
     conmsg = lambda: f"use current BBLIB '{bblib or config['BBLIB']}'?"
     if not bblib and config.keys() >= {"BBLIB"} and click.confirm(conmsg(), default=True):
         bblib = config["BBLIB"]
     elif not bblib:
         bblib = click.prompt("Choose path to store bricks", type=click.Path())
 
@@ -49,15 +52,15 @@
     # VALIDATE TOKEN    
     while token != deftoken and not check_token(token, silent=True):
         click.echo(click.style("invalid token. check your token at https://biobricks.ai/token", fg="red"))
         token = click.prompt("Input a token from biobricks.ai/token",hide_input=True, default=deftoken)
     token = "VQF6Q2U-NKktZ31ioVYa9w" if token == deftoken else token
 
     # write configuration
-    config = { "BBLIB": bblib, "TOKEN": token }
+    config = { "BBLIB": bblib, "TOKEN": token, "EMAIL": email }
     write_config(config)
 
     # initialize bblib
     bblib = init_bblib()
 
     msg = f"Done! BioBricks has BBLIB {bblib} and config {path}"
     click.echo(click.style(msg, fg="green"))
```

### Comparing `biobricks-0.1.62/biobricks/config.py` & `biobricks-0.1.63/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/local_bb.py` & `biobricks-0.1.63/biobricks/local_bb.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/biobricks/tests/test_init.py` & `biobricks-0.1.63/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/docker/Dockerfile` & `biobricks-0.1.63/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/LICENSE` & `biobricks-0.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/README.md` & `biobricks-0.1.63/README.md`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.62/pyproject.toml` & `biobricks-0.1.63/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.62"
+version = "0.1.63"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.62/PKG-INFO` & `biobricks-0.1.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.62
+Version: 0.1.63
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

