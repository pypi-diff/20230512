# Comparing `tmp/mkdocs-monorepo-plugin-1.0.4.tar.gz` & `tmp/mkdocs-monorepo-plugin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-monorepo-plugin-1.0.4.tar", last modified: Thu Sep 29 12:09:11 2022, max compression
+gzip compressed data, was "dist/mkdocs-monorepo-plugin-1.0.5.tar", last modified: Fri May 12 12:01:50 2023, max compression
```

## Comparing `mkdocs-monorepo-plugin-1.0.4.tar` & `mkdocs-monorepo-plugin-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3680 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/edit_uri.py
--rw-r--r--   0 runner    (1001) docker     (121)     2993 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/merger.py
--rw-r--r--   0 runner    (1001) docker     (121)    12337 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3635 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/tests/test_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-29 12:09:10.000000 mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-29 12:09:11.000000 mkdocs-monorepo-plugin-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-09-29 12:09:05.000000 mkdocs-monorepo-plugin-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/edit_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 12:01:49.000000 mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 12:01:50.000000 mkdocs-monorepo-plugin-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-12 12:01:44.000000 mkdocs-monorepo-plugin-1.0.5/setup.py
```

### Comparing `mkdocs-monorepo-plugin-1.0.4/PKG-INFO` & `mkdocs-monorepo-plugin-1.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 1.2
 Name: mkdocs-monorepo-plugin
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plugin for adding monorepository support in Mkdocs.
 Home-page: https://github.com/backstage/mkdocs-monorepo-plugin
 Author: Bilawal Hameed
 Author-email: bil@spotify.com
 License: Apache-2.0
 Description: 
                 This introduces support for the !include syntax in mkdocs.yml, allowing you to import additional Mkdocs navigation.
                 It enables large or complex repositories to have their own sets of docs/ folders, whilst generating only a single Mkdocs site.
                 This is built and maintained by the engineering community at Spotify.
             
 Keywords: mkdocs monorepo
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
```

### Comparing `mkdocs-monorepo-plugin-1.0.4/README.md` & `mkdocs-monorepo-plugin-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 ### Release
 
 1. Update the [CHANGELOG.md](./docs/CHANGELOG.md).
 2. Bump up the version number in `setup.py` which triggers the release workflow on [GitHub Actions](.github/workflows/deploy.yml) to publish a new version in PyPI.
 
 ## Supported Versions
 
-- Python 3 &mdash; 3.6, 3.7
+- Python 3 &mdash; 3.7, 3.8, 3.9, 3.10, 3.11
 - [Mkdocs] 1.0.4 and above.
 
 ## Changelog
 
 Check out our [CHANGELOG.md](./docs/CHANGELOG.md) for details.
 
 ## License
```

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/edit_uri.py` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/edit_uri.py`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/merger.py` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/merger.py`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/parser.py` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/parser.py`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/plugin.py` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin/tests/test_plugin.py` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/PKG-INFO` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 1.2
 Name: mkdocs-monorepo-plugin
-Version: 1.0.4
+Version: 1.0.5
 Summary: Plugin for adding monorepository support in Mkdocs.
 Home-page: https://github.com/backstage/mkdocs-monorepo-plugin
 Author: Bilawal Hameed
 Author-email: bil@spotify.com
 License: Apache-2.0
 Description: 
                 This introduces support for the !include syntax in mkdocs.yml, allowing you to import additional Mkdocs navigation.
                 It enables large or complex repositories to have their own sets of docs/ folders, whilst generating only a single Mkdocs site.
                 This is built and maintained by the engineering community at Spotify.
             
 Keywords: mkdocs monorepo
 Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
```

### Comparing `mkdocs-monorepo-plugin-1.0.4/mkdocs_monorepo_plugin.egg-info/SOURCES.txt` & `mkdocs-monorepo-plugin-1.0.5/mkdocs_monorepo_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-monorepo-plugin-1.0.4/setup.py` & `mkdocs-monorepo-plugin-1.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name='mkdocs-monorepo-plugin',
-    version='1.0.4',
+    version='1.0.5',
     description='Plugin for adding monorepository support in Mkdocs.',
     long_description="""
         This introduces support for the !include syntax in mkdocs.yml, allowing you to import additional Mkdocs navigation.
         It enables large or complex repositories to have their own sets of docs/ folders, whilst generating only a single Mkdocs site.
         This is built and maintained by the engineering community at Spotify.
     """,  # noqa: E501
     keywords='mkdocs monorepo',
@@ -17,21 +17,24 @@
     license='Apache-2.0',
     python_requires='>=3',
     install_requires=[
         'mkdocs>=1.0.4',
         'python-slugify>=4.0.1'
     ],
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7'
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     packages=setuptools.find_packages(),
     entry_points={
         'mkdocs.plugins': [
             "monorepo = mkdocs_monorepo_plugin.plugin:MonorepoPlugin"
         ]
     }
```

