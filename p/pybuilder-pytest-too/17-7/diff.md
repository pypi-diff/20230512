# Comparing `tmp/pybuilder_pytest_too-17-py3-none-any.whl.zip` & `tmp/pybuilder_pytest_too-7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3427 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3187 b- defN 23-May-12 17:53 pybuilder_pytest_too/__init__.py
--rw-r--r--  2.0 unx       55 b- defN 23-May-12 17:53 pybuilder_pytest_too/version.py
--rw-r--r--  2.0 unx     1009 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      719 b- defN 23-May-12 17:53 pybuilder_pytest_too-17.dist-info/RECORD
-8 files, 5085 bytes uncompressed, 2139 bytes compressed:  57.9%
+Zip file size: 3366 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     2877 b- defN 21-Oct-25 21:30 pybuilder_pytest_too/__init__.py
+-rw-r--r--  2.0 unx       54 b- defN 21-Oct-25 21:30 pybuilder_pytest_too/version.py
+-rw-r--r--  2.0 unx     1027 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      713 b- defN 21-Oct-25 21:30 pybuilder_pytest_too-7.dist-info/RECORD
+8 files, 4786 bytes uncompressed, 2090 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: pybuilder_pytest_too/__init__.py
 Comment: 
 
 Filename: pybuilder_pytest_too/version.py
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/METADATA
+Filename: pybuilder_pytest_too-7.dist-info/METADATA
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/WHEEL
+Filename: pybuilder_pytest_too-7.dist-info/WHEEL
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/namespace_packages.txt
+Filename: pybuilder_pytest_too-7.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/top_level.txt
+Filename: pybuilder_pytest_too-7.dist-info/top_level.txt
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/zip-safe
+Filename: pybuilder_pytest_too-7.dist-info/zip-safe
 Comment: 
 
-Filename: pybuilder_pytest_too-17.dist-info/RECORD
+Filename: pybuilder_pytest_too-7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybuilder_pytest_too/__init__.py

```diff
@@ -33,48 +33,42 @@
 
 
 @init
 def initialize_pytest_plugin(project):
     """ Init default plugin project properties. """
     project.build_depends_on('pytest')
     project.build_depends_on('pytest-cov')
-    project.build_depends_on('pytest-xdist')
     project.set_property_if_unset("dir_source_pytest_python", "src/unittest/python")
     project.set_property_if_unset("pytest_extra_args", [])
     project.set_property_if_unset("pytest_python_env", "build")
-    project.set_property_if_unset("pytest_parallel", False)
 
 
 @task
 def run_unit_tests(project, logger:Logger,reactor):
     """ Call pytest for the sources of the given project. """
     logger.info('pytest: Run unittests.')
     test_dir = push_test_path_to_syspath(project, sys_path, 'pytest')
     extra_args = [project.expand(prop) for prop in project.get_property("pytest_extra_args")]
     try:
         pytest_args = [test_dir] + (extra_args if extra_args else [])
         if project.get_property('verbose'):
             pytest_args.append('-s')
             pytest_args.append('-v')
-        if project.get_property('pytest_unit_parallel'):
-            pytest_args.extend(['-n','auto'])
-        env_ = reactor.python_env_registry[project.get_property("pytest_python_env")]
-        cmd_args = []
-        cmd_args.extend(env_.executable)
+        env_ = reactor.python_env_registry[project.get_property("unittest_python_env")]
+        cmd_args = [env_.executable]
         cmd_args.extend(['-m','pytest'])
         cmd_args.extend(pytest_args)
         with tempfile.NamedTemporaryFile() as outfile:
             error_file_name = "{0}.err".format(outfile.name)
-            ret = env_.execute_command(cmd_args, outfile.name, cwd=project.get_property('dir_source_main_python'))
-            if os.path.exists(error_file_name):
-                error_file_lines = read_file(error_file_name)
-                for line in error_file_lines:
-                    logger.error(line.replace("\n",""))
+            ret = env_.execute_command(cmd_args,outfile.name,env=os.environ, cwd=project.get_property('dir_source_pytest_python'))
+            error_file_lines = read_file(error_file_name)
             outfile_lines = read_file(outfile.name)
+            for line in error_file_lines:
+                logger.error(line)
             for line in outfile_lines:
-                logger.info(line.replace("\n",""))
+                logger.info(line)
             if ret:
                 raise BuildFailedException('pytest: unittests failed')
             else:
                 logger.info('pytest: All unittests passed.')
     except Exception:
         raise
```

## pybuilder_pytest_too/version.py

```diff
@@ -1,2 +1,2 @@
 """ PyB filtered package version"""
-__version__ = "17"
+__version__ = "7"
```

## Comparing `pybuilder_pytest_too-17.dist-info/METADATA` & `pybuilder_pytest_too-7.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pybuilder-pytest-too
-Version: 17
+Version: 7
 Summary: PyBuilder Pytest Plugin
 Home-page: https://github.com/AlexeySanko/pybuilder_pytest
 Author: Alexey Sanko
 Author-email: alexeycount@gmail.com
 Maintainer: 
 Maintainer-email: 
 License: Apache License, Version 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -20,7 +21,8 @@
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: pytest
 
 Please visit https://github.com/AlexeySanko/pybuilder_pytest for more information!
+
```

## Comparing `pybuilder_pytest_too-17.dist-info/RECORD` & `pybuilder_pytest_too-7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pybuilder_pytest_too/__init__.py,sha256=DDyWRtw3F6HU0AyHtrzrgmJdcFJUJU9BYPMY89tJyj0,3187
-pybuilder_pytest_too/version.py,sha256=3-47rH7BhoMYyVbYHAEpBtKUadzY7dm-agl9naP9Zqg,55
-pybuilder_pytest_too-17.dist-info/METADATA,sha256=MP7QJ4e_c8G19HADUjmGtm9PX6Zt0xSqQJwMYiT1Jvc,1009
-pybuilder_pytest_too-17.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pybuilder_pytest_too-17.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pybuilder_pytest_too-17.dist-info/top_level.txt,sha256=OWiHc8m1wJYZKKdAlhwjYv14hvQoqlFTL2Ht0lrCDxw,21
-pybuilder_pytest_too-17.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pybuilder_pytest_too-17.dist-info/RECORD,,
+pybuilder_pytest_too/__init__.py,sha256=A65JkVpEW5KTrxL8CATl8zgQcS-x6sH_CF4VMhaRbsw,2877
+pybuilder_pytest_too/version.py,sha256=V_HSqWQQh8NJqbMD-WwYVl5LzFhLocgIv2OJpGkwehI,54
+pybuilder_pytest_too-7.dist-info/METADATA,sha256=lMuZm2dYdTj36BqrUiAOyMzjCHXLzW-ucCA4KzL9m8Q,1027
+pybuilder_pytest_too-7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+pybuilder_pytest_too-7.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pybuilder_pytest_too-7.dist-info/top_level.txt,sha256=OWiHc8m1wJYZKKdAlhwjYv14hvQoqlFTL2Ht0lrCDxw,21
+pybuilder_pytest_too-7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pybuilder_pytest_too-7.dist-info/RECORD,,
```

