# Comparing `tmp/chrisbase-0.3.6.tar.gz` & `tmp/chrisbase-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.3.6.tar", last modified: Mon Mar 27 08:44:32 2023, max compression
+gzip compressed data, was "chrisbase-0.3.7.tar", last modified: Fri May 12 07:50:34 2023, max compression
```

## Comparing `chrisbase-0.3.6.tar` & `chrisbase-0.3.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:44:32.519806 chrisbase-0.3.6/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-03-27 07:49:18.000000 chrisbase-0.3.6/LICENSE
--rw-rw-r--   0 chris     (1000) chris     (1000)      866 2023-03-27 08:44:32.519806 chrisbase-0.3.6/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-03-27 07:49:18.000000 chrisbase-0.3.6/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-03-27 07:49:18.000000 chrisbase-0.3.6/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)      962 2023-03-27 08:44:32.519806 chrisbase-0.3.6/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:44:32.515806 chrisbase-0.3.6/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:44:32.515806 chrisbase-0.3.6/src/chrisbase/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-03-27 07:49:18.000000 chrisbase-0.3.6/src/chrisbase/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-03-27 07:49:18.000000 chrisbase-0.3.6/src/chrisbase/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    22841 2023-03-27 07:49:18.000000 chrisbase-0.3.6/src/chrisbase/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-03-27 07:49:18.000000 chrisbase-0.3.6/src/chrisbase/morp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-03-27 07:49:18.000000 chrisbase-0.3.6/src/chrisbase/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-03-27 08:10:11.000000 chrisbase-0.3.6/src/chrisbase/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-03-27 08:44:32.519806 chrisbase-0.3.6/src/chrisbase.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      866 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      431 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      108 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-03-27 08:44:32.000000 chrisbase-0.3.6/src/chrisbase.egg-info/zip-safe
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 07:50:34.298995 chrisbase-0.3.7/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2023-05-12 07:41:51.000000 chrisbase-0.3.7/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-05-12 07:50:34.298995 chrisbase-0.3.7/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      286 2023-05-12 07:41:51.000000 chrisbase-0.3.7/README.md
+-rw-rw-r--   0 chris     (1000) chris     (1000)       81 2023-05-12 07:41:51.000000 chrisbase-0.3.7/pyproject.toml
+-rw-rw-r--   0 chris     (1000) chris     (1000)      946 2023-05-12 07:50:34.298995 chrisbase-0.3.7/setup.cfg
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 07:50:34.298995 chrisbase-0.3.7/src/
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 07:50:34.298995 chrisbase-0.3.7/src/chrisbase/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      151 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/cli.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    23182 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/io.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/morp.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/time.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5122 2023-05-12 07:41:51.000000 chrisbase-0.3.7/src/chrisbase/util.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-12 07:50:34.298995 chrisbase-0.3.7/src/chrisbase.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      816 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      431 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       48 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/entry_points.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)      129 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       10 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-12 07:50:34.000000 chrisbase-0.3.7/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.3.6/LICENSE` & `chrisbase-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.6/PKG-INFO` & `chrisbase-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.6
+Version: 0.3.7
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chrisbase
```

### Comparing `chrisbase-0.3.6/setup.cfg` & `chrisbase-0.3.7/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [metadata]
 name = chrisbase
-version = 0.3.6
+version = 0.3.7
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 classifiers = 
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = True
 packages = find:
 package_dir = 
@@ -31,14 +30,16 @@
 	pymongo
 	tabulate
 	chrisdict
 	matplotlib
 	sqlalchemy
 	dataclasses
 	dataclasses-json
+	scikit-learn
+	seqeval
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = README.md
```

### Comparing `chrisbase-0.3.6/src/chrisbase/io.py` & `chrisbase-0.3.7/src/chrisbase/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,16 +665,22 @@
 class ProjectEnv(DataClassJsonMixin):
     project: str = field()
     hostname: str = field(init=False)
     hostaddr: str = field(init=False)
     python_path: Path = field(init=False)
     working_path: Path = field(init=False)
     running_file: Path = field(init=False)
+    running_gpus: str | None = field(default=None)
 
     def __post_init__(self):
+        assert self.project, "Project name must be provided"
         self.hostname = get_hostname()
         self.hostaddr = get_hostaddr()
         self.python_path = Path(sys.executable)
-        project_path = first_or([x for x in running_file().parents if self.project and x.name.startswith(self.project)])
-        assert project_path, f"Could not find project path for {self.project} in {[str(x) for x in running_file().parents]}"
-        self.working_path = cwd(project_path)
-        self.running_file = running_file().relative_to(self.working_path)
+        self.running_file = running_file()
+        self.project_path = first_or([x for x in self.running_file.parents if x.name.startswith(self.project)])
+        assert self.project_path, f"Could not find project path for {self.project} in {', '.join([str(x) for x in self.running_file.parents])}"
+        self.working_path = cwd(self.project_path)
+        self.running_file = self.running_file.relative_to(self.working_path)
+        if self.running_gpus:
+            from chrislab.common.util import cuda_visible_devices
+            self.running_gpus = cuda_visible_devices(self.running_gpus)
```

### Comparing `chrisbase-0.3.6/src/chrisbase/morp.py` & `chrisbase-0.3.7/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.6/src/chrisbase/time.py` & `chrisbase-0.3.7/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.6/src/chrisbase/util.py` & `chrisbase-0.3.7/src/chrisbase/util.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.3.6/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.3.7/src/chrisbase.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.3.6
+Version: 0.3.7
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chrisbase
```

