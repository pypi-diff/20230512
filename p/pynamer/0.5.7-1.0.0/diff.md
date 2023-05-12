# Comparing `tmp/pynamer-0.5.7.tar.gz` & `tmp/pynamer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.5.7.tar", last modified: Tue May  9 19:45:57 2023, max compression
+gzip compressed data, was "pynamer-1.0.0.tar", last modified: Fri May 12 18:11:58 2023, max compression
```

## Comparing `pynamer-0.5.7.tar` & `pynamer-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.484321 pynamer-0.5.7/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.5.7/AUTHORS.md
--rw-rw-rw-   0        0        0     5732 2023-05-09 19:45:45.000000 pynamer-0.5.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.5.7/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.5.7/MANIFEST.in
--rw-rw-rw-   0        0        0    16714 2023-05-09 19:45:57.484321 pynamer-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0    15235 2023-05-03 20:43:07.000000 pynamer-0.5.7/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.5.7/pyproject.toml
--rw-rw-rw-   0        0        0     1804 2023-05-09 19:45:57.484321 pynamer-0.5.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.352698 pynamer-0.5.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.415239 pynamer-0.5.7/src/pynamer/
--rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.5.7/src/pynamer/README.md
--rw-rw-rw-   0        0        0     1578 2023-05-09 19:45:45.000000 pynamer-0.5.7/src/pynamer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.430847 pynamer-0.5.7/src/pynamer/project_name/
--rw-rw-rw-   0        0        0       35 2023-05-07 16:00:13.000000 pynamer-0.5.7/src/pynamer/project_name/__init__.py
--rw-rw-rw-   0        0        0    25839 2023-05-09 13:02:45.000000 pynamer-0.5.7/src/pynamer/pynamer.py
--rw-rw-rw-   0        0        0      387 2023-05-07 16:01:32.000000 pynamer-0.5.7/src/pynamer/setup.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.430847 pynamer-0.5.7/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0    16714 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      957 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 19:45:57.000000 pynamer-0.5.7/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 19:45:57.484321 pynamer-0.5.7/tests/
--rw-rw-rw-   0        0        0     1861 2023-05-09 15:24:18.000000 pynamer-0.5.7/tests/test_build_dist.py
--rw-rw-rw-   0        0        0     1082 2023-05-08 14:07:21.000000 pynamer-0.5.7/tests/test_cleanup.py
--rw-rw-rw-   0        0        0      835 2023-05-07 16:03:15.000000 pynamer-0.5.7/tests/test_create_setup_file.py
--rw-rw-rw-   0        0        0     1671 2023-05-09 19:41:31.000000 pynamer-0.5.7/tests/test_defaults.py
--rw-rw-rw-   0        0        0      533 2023-05-07 16:03:14.000000 pynamer-0.5.7/tests/test_delete_director.py
--rw-rw-rw-   0        0        0     1230 2023-05-03 15:59:40.000000 pynamer-0.5.7/tests/test_feedback.py
--rw-rw-rw-   0        0        0     2698 2023-05-09 14:10:02.000000 pynamer-0.5.7/tests/test_final_analysis.py
--rw-rw-rw-   0        0        0      749 2023-05-08 16:23:32.000000 pynamer-0.5.7/tests/test_find_pypirc_file.py
--rw-rw-rw-   0        0        0      799 2023-05-08 16:21:10.000000 pynamer-0.5.7/tests/test_generate_pypi_index.py
--rw-rw-rw-   0        0        0      199 2023-05-09 19:42:58.000000 pynamer-0.5.7/tests/test_main TBC.py
--rw-rw-rw-   0        0        0      787 2023-05-08 14:43:58.000000 pynamer-0.5.7/tests/test_ping_json.py
--rw-rw-rw-   0        0        0      616 2023-05-08 14:43:58.000000 pynamer-0.5.7/tests/test_ping_project.py
--rw-rw-rw-   0        0        0      491 2023-05-08 14:51:41.000000 pynamer-0.5.7/tests/test_process_input_file.py
--rw-rw-rw-   0        0        0     1092 2023-05-08 14:51:41.000000 pynamer-0.5.7/tests/test_pypi_search.py
--rw-rw-rw-   0        0        0      456 2023-05-08 14:51:39.000000 pynamer-0.5.7/tests/test_pypi_search_index.py
--rw-rw-rw-   0        0        0      737 2023-05-08 13:03:26.000000 pynamer-0.5.7/tests/test_rename_project_dir.py
--rw-rw-rw-   0        0        0      406 2023-05-07 16:03:12.000000 pynamer-0.5.7/tests/test_run_command TBD.py
--rw-rw-rw-   0        0        0      558 2023-05-09 19:42:58.000000 pynamer-0.5.7/tests/test_upload_dist TBD.py
--rw-rw-rw-   0        0        0      623 2023-05-08 14:51:42.000000 pynamer-0.5.7/tests/test_write_output_file.py
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:58.146896 pynamer-1.0.0/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-1.0.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     6473 2023-05-12 18:11:44.000000 pynamer-1.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17676 2023-05-12 18:11:58.147923 pynamer-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16166 2023-05-12 18:01:03.000000 pynamer-1.0.0/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1817 2023-05-12 18:11:58.149985 pynamer-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:57.949424 pynamer-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:57.996314 pynamer-1.0.0/src/pynamer/
+-rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-1.0.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1578 2023-05-12 18:11:44.000000 pynamer-1.0.0/src/pynamer/__init__.py
+-rw-rw-rw-   0        0        0       17 2023-05-12 15:48:30.000000 pynamer-1.0.0/src/pynamer/project_count.pickle
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:58.023049 pynamer-1.0.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       35 2023-05-07 16:00:13.000000 pynamer-1.0.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0    28676 2023-05-12 18:04:11.000000 pynamer-1.0.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      387 2023-05-07 16:01:32.000000 pynamer-1.0.0/src/pynamer/setup.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:58.007389 pynamer-1.0.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    17676 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 18:11:57.000000 pynamer-1.0.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 18:11:58.144838 pynamer-1.0.0/tests/
+-rw-rw-rw-   0        0        0     1843 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_args.py
+-rw-rw-rw-   0        0        0     1923 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_build_dist.py
+-rw-rw-rw-   0        0        0     1080 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_cleanup.py
+-rw-rw-rw-   0        0        0      835 2023-05-07 16:03:15.000000 pynamer-1.0.0/tests/test_create_setup_file.py
+-rw-rw-rw-   0        0        0     1588 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_defaults.py
+-rw-rw-rw-   0        0        0      538 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_delete_director.py
+-rw-rw-rw-   0        0        0     1282 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_feedback.py
+-rw-rw-rw-   0        0        0     2698 2023-05-09 14:10:02.000000 pynamer-1.0.0/tests/test_final_analysis.py
+-rw-rw-rw-   0        0        0      738 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_find_pypirc_file.py
+-rw-rw-rw-   0        0        0     1259 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_generate_pypi_index.py
+-rw-rw-rw-   0        0        0      282 2023-05-12 16:17:19.000000 pynamer-1.0.0/tests/test_is_valid_package_name.py
+-rw-rw-rw-   0        0        0      199 2023-05-09 19:42:58.000000 pynamer-1.0.0/tests/test_main TBC.py
+-rw-rw-rw-   0        0        0     1664 2023-05-11 09:16:33.000000 pynamer-1.0.0/tests/test_ping_json.py
+-rw-rw-rw-   0        0        0     1496 2023-05-11 08:50:00.000000 pynamer-1.0.0/tests/test_ping_project.py
+-rw-rw-rw-   0        0        0      522 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_process_input_file.py
+-rw-rw-rw-   0        0        0     1117 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_pypi_search.py
+-rw-rw-rw-   0        0        0      405 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_pypi_search_index.py
+-rw-rw-rw-   0        0        0      737 2023-05-08 13:03:26.000000 pynamer-1.0.0/tests/test_rename_project_dir.py
+-rw-rw-rw-   0        0        0      232 2023-05-12 11:41:53.000000 pynamer-1.0.0/tests/test_run_command TBD.py
+-rw-rw-rw-   0        0        0      882 2023-05-12 17:32:19.000000 pynamer-1.0.0/tests/test_upload_dist.py
+-rw-rw-rw-   0        0        0      647 2023-05-12 17:31:19.000000 pynamer-1.0.0/tests/test_write_output_file.py
```

### Comparing `pynamer-0.5.7/CHANGELOG.md` & `pynamer-1.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.0 (2023-05-12)
+### Feature
+* Add name validity check function + others ([`b520245`](https://github.com/Stephen-RA-King/pynamer/commit/b5202458752ea1298ab450269a1b3cd341907f1e))
+
+### Fix
+* Update and fix failing tests ([`2e67751`](https://github.com/Stephen-RA-King/pynamer/commit/2e677512a7c58a1c8115d7f6567bfc050391f086))
+* Some broken tests ([`33227e8`](https://github.com/Stephen-RA-King/pynamer/commit/33227e804ef08ff74f69cfb3530084bd3043e18b))
+
+### Documentation
+* Add limitations section ([`741154d`](https://github.com/Stephen-RA-King/pynamer/commit/741154ddf0dc1cdaf6353b635acda33afa383254))
+* Update pngs ([`8eec345`](https://github.com/Stephen-RA-King/pynamer/commit/8eec345e0e5a268f770c93ccab330dd978c8baeb))
+
 ## v0.5.7 (2023-05-09)
 
 
 ## v0.5.6 (2023-05-09)
 ### Fix
 * Logic error in fanal analysis function ([`46dbee0`](https://github.com/Stephen-RA-King/pynamer/commit/46dbee0983cb7c97d2f11931222fbdf3f64cf7c6))
 * Broken tests ([`5b92893`](https://github.com/Stephen-RA-King/pynamer/commit/5b9289364ab9ad770c744c70e181812f77b9627b))
```

### Comparing `pynamer-0.5.7/LICENSE` & `pynamer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.7/PKG-INFO` & `pynamer-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.5.7
+Version: 1.0.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: Any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# pynamer
-
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
@@ -88,15 +86,15 @@
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
 pip search zaphod
 ```
 
-```commandline
+```bash
 ERROR: XMLRPC request failed [code: -32500]
 RuntimeError: PyPI no longer supports 'pip search' (or XML-RPC search).
 Please use https://pypi.org/search (via a browser) instead.
 See https://warehouse.pypa.io/api-reference/xml-rpc.html#deprecated-methods for more information.
 ```
 
 A quick search will show the internet replete with articles explaining the situation:
@@ -112,16 +110,16 @@
 So, I go ahead and code my new project, along with all the test files, documentation and meta data.
 I diligently debug and commit and push to git and github so I have a history.
 
 Finally the project is good enough to release and publish as an installable package on PyPI.
 
 Here goes....
 
-```commandline
-python -m twine upload --config-file .pypirc dist/*
+```bash
+~ $ python -m twine upload --config-file .pypirc dist/*
 Uploading distributions to https://upload.pypi.org/legacy/
 Uploading zaphod-0.0.0-py3-none-any.whl
 100% ---------------------------------------- 3.8/3.8 kB • 00:00 • ?
 WARNING  Error during upload. Retry with the --verbose option for more details.
 ERROR    HTTPError: 403 Forbidden from https://upload.pypi.org/legacy/
          The user 'stephenking' isn't allowed to upload to project 'zaphod'. See https://pypi.org/help/#project-name for more information.
 ```
@@ -176,31 +174,31 @@
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = your_API_token_here
 ```
 
 ### Installation
 
-```sh
+```bash
 ~ $ pipx install pynamer
 ```
 
 ### Basic Usage
 
 #### A package name that is not available
 
-```commandline
+```bash
 ~ $ pynamer pynball
 ```
 
 ![](assets/usage_pynball.png)
 
 #### A package name that is available
 
-```commandline
+```bash
 ~ $ pynamer allitnil
 ```
 
 ![](assets/usage_available.png)
 
 Holy smoke batman! You've managed to identify a unique name.
 
@@ -212,19 +210,19 @@
 
 # Usage
 
 ---
 
 Display the help menu with the -h argument
 
-```commandline
+```bash
 ~ $ pynamer -h
 ```
 
-```commandline
+```bash
 usage: pynamer [-h] [-r] [-f FILE] [-o OUTPUT] [-v] [-g] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
   projects              Optional - one or more project names
 
@@ -238,15 +236,15 @@
   -g, --generate        Generate a new PyPI simple index
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
-```commandline
+```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
 You can use the -f argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
@@ -256,29 +254,29 @@
 ```file
 ganymede europa
 IO callisto
 ```
 
 Then specify the -f argument
 
-```commandline
+```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
 You can specify a file to write the result to by using the -o argument. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
 results
 
@@ -300,27 +298,27 @@
 
 ## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-```commandline
+```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
 ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
-```commandline
+```bash
 ~ $ pynamer pynamer -v
 ```
 
 ![](assets/usage_verbose.png)
 
 ## Regenerate the PyPI simple Repository Index
 
@@ -332,58 +330,78 @@
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 
 The PyPI Simple Index is updated every few hours
 
 Using the -r argument can be used to regenerate the local file contents.
 
-```commandline
+```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
 The reason I wrote this application in the first place.
 
-```commandline
+```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
 Even worse ...
 
-```commandline
+```bash
 ~ $ pynamer zem
 ```
 
 ![](assets/usage_zem.png)
 
-## Planned Future improvements
+## Limitations
 
--   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
--   Filter out invalid PyPI package names at the start
+There will be occasions where all the tests pass, the name appears to be available but the upload to PyPI still fails.
+This can be several reasons for this:
+
+-   You are trying to use an internally "reserved" keyword for PyPI.
+-   The name you are using is too similar to an existing project name and you get the following error message:
+
+```bash
+...
+Error during upload. Retry with the --verbose option for more details.
+HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
+The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
+```
+
+Using a name similar to to an existing package name is a security issue.
+
+Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
+## Planned Future improvements
+
+-   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
+
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
@@ -424,15 +442,15 @@
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
-[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
 [pypi-url]: https://pypi.org/project/pynamer/
```

### Comparing `pynamer-0.5.7/README.md` & `pynamer-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# pynamer
-
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
@@ -60,15 +58,15 @@
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
 pip search zaphod
 ```
 
-```commandline
+```bash
 ERROR: XMLRPC request failed [code: -32500]
 RuntimeError: PyPI no longer supports 'pip search' (or XML-RPC search).
 Please use https://pypi.org/search (via a browser) instead.
 See https://warehouse.pypa.io/api-reference/xml-rpc.html#deprecated-methods for more information.
 ```
 
 A quick search will show the internet replete with articles explaining the situation:
@@ -84,16 +82,16 @@
 So, I go ahead and code my new project, along with all the test files, documentation and meta data.
 I diligently debug and commit and push to git and github so I have a history.
 
 Finally the project is good enough to release and publish as an installable package on PyPI.
 
 Here goes....
 
-```commandline
-python -m twine upload --config-file .pypirc dist/*
+```bash
+~ $ python -m twine upload --config-file .pypirc dist/*
 Uploading distributions to https://upload.pypi.org/legacy/
 Uploading zaphod-0.0.0-py3-none-any.whl
 100% ---------------------------------------- 3.8/3.8 kB • 00:00 • ?
 WARNING  Error during upload. Retry with the --verbose option for more details.
 ERROR    HTTPError: 403 Forbidden from https://upload.pypi.org/legacy/
          The user 'stephenking' isn't allowed to upload to project 'zaphod'. See https://pypi.org/help/#project-name for more information.
 ```
@@ -148,31 +146,31 @@
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = your_API_token_here
 ```
 
 ### Installation
 
-```sh
+```bash
 ~ $ pipx install pynamer
 ```
 
 ### Basic Usage
 
 #### A package name that is not available
 
-```commandline
+```bash
 ~ $ pynamer pynball
 ```
 
 ![](assets/usage_pynball.png)
 
 #### A package name that is available
 
-```commandline
+```bash
 ~ $ pynamer allitnil
 ```
 
 ![](assets/usage_available.png)
 
 Holy smoke batman! You've managed to identify a unique name.
 
@@ -184,19 +182,19 @@
 
 # Usage
 
 ---
 
 Display the help menu with the -h argument
 
-```commandline
+```bash
 ~ $ pynamer -h
 ```
 
-```commandline
+```bash
 usage: pynamer [-h] [-r] [-f FILE] [-o OUTPUT] [-v] [-g] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
   projects              Optional - one or more project names
 
@@ -210,15 +208,15 @@
   -g, --generate        Generate a new PyPI simple index
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
-```commandline
+```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
 You can use the -f argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
@@ -228,29 +226,29 @@
 ```file
 ganymede europa
 IO callisto
 ```
 
 Then specify the -f argument
 
-```commandline
+```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
 You can specify a file to write the result to by using the -o argument. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
 results
 
@@ -272,27 +270,27 @@
 
 ## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-```commandline
+```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
 ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
-```commandline
+```bash
 ~ $ pynamer pynamer -v
 ```
 
 ![](assets/usage_verbose.png)
 
 ## Regenerate the PyPI simple Repository Index
 
@@ -304,58 +302,78 @@
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 
 The PyPI Simple Index is updated every few hours
 
 Using the -r argument can be used to regenerate the local file contents.
 
-```commandline
+```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
 The reason I wrote this application in the first place.
 
-```commandline
+```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
 Even worse ...
 
-```commandline
+```bash
 ~ $ pynamer zem
 ```
 
 ![](assets/usage_zem.png)
 
-## Planned Future improvements
+## Limitations
 
--   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
--   Filter out invalid PyPI package names at the start
+There will be occasions where all the tests pass, the name appears to be available but the upload to PyPI still fails.
+This can be several reasons for this:
+
+-   You are trying to use an internally "reserved" keyword for PyPI.
+-   The name you are using is too similar to an existing project name and you get the following error message:
+
+```bash
+...
+Error during upload. Retry with the --verbose option for more details.
+HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
+The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
+```
+
+Using a name similar to to an existing package name is a security issue.
+
+Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
+## Planned Future improvements
+
+-   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
+
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
@@ -396,15 +414,15 @@
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
-[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
 [pypi-url]: https://pypi.org/project/pynamer/
```

### Comparing `pynamer-0.5.7/pyproject.toml` & `pynamer-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.7/setup.cfg` & `pynamer-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -32,82 +32,83 @@
 000001f0: 6974 6875 622e 636f 6d2f 5374 6570 6865  ithub.com/Stephe
 00000200: 6e2d 5241 2d4b 696e 672f 7079 6e61 6d65  n-RA-King/pyname
 00000210: 722f 6172 6368 6976 652f 7265 6673 2f68  r/archive/refs/h
 00000220: 6561 6473 2f6d 6169 6e2e 7a69 700d 0a6c  eads/main.zip..l
 00000230: 6963 656e 7365 203d 204d 4954 0d0a 636c  icense = MIT..cl
 00000240: 6173 7369 6669 6572 7320 3d20 0d0a 0944  assifiers = ...D
 00000250: 6576 656c 6f70 6d65 6e74 2053 7461 7475  evelopment Statu
-00000260: 7320 3a3a 2034 202d 2042 6574 610d 0a09  s :: 4 - Beta...
-00000270: 456e 7669 726f 6e6d 656e 7420 3a3a 2043  Environment :: C
-00000280: 6f6e 736f 6c65 0d0a 0949 6e74 656e 6465  onsole...Intende
-00000290: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000002a0: 7665 6c6f 7065 7273 0d0a 094f 7065 7261  velopers...Opera
-000002b0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000002c0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-000002d0: 4e61 7475 7261 6c20 4c61 6e67 7561 6765  Natural Language
-000002e0: 203a 3a20 456e 676c 6973 680d 0a09 5072   :: English...Pr
-000002f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000300: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000310: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
-00000320: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000330: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
-00000340: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000350: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000360: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
-00000370: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000380: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
-00000390: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000003a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003b0: 6e20 3a3a 2033 2e31 310d 0a0d 0a5b 6f70  n :: 3.11....[op
-000003c0: 7469 6f6e 735d 0d0a 7061 636b 6167 655f  tions]..package_
-000003d0: 6469 7220 3d20 0d0a 093d 7372 630d 0a70  dir = ...=src..p
-000003e0: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-000003f0: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000400: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
-00000410: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
-00000420: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000430: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
-00000440: 7265 7175 6972 6573 203d 200d 0a09 6a69  requires = ...ji
-00000450: 6e6a 6132 0d0a 0962 7334 0d0a 0962 7569  nja2...bs4...bui
-00000460: 6c64 0d0a 0963 6f6c 6f72 616d 610d 0a09  ld...colorama...
-00000470: 7079 7961 6d6c 0d0a 0972 6571 7565 7374  pyyaml...request
-00000480: 730d 0a09 7269 6368 0d0a 0974 7769 6e65  s...rich...twine
-00000490: 0d0a 0974 7164 6d0d 0a09 7768 6565 6c0d  ...tqdm...wheel.
-000004a0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000004b0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000004c0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
-000004d0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-000004e0: 5d0d 0a70 796e 616d 6572 203d 200d 0a09  ]..pynamer = ...
-000004f0: 7365 7475 702e 7478 740d 0a09 5245 4144  setup.txt...READ
-00000500: 4d45 2e6d 640d 0a09 7072 6f6a 6563 745f  ME.md...project_
-00000510: 6e61 6d65 0d0a 0970 726f 6a65 6374 5f6e  name...project_n
-00000520: 616d 652f 5f5f 696e 6974 5f5f 2e70 790d  ame/__init__.py.
-00000530: 0a09 7072 6f6a 6563 745f 636f 756e 742e  ..project_count.
-00000540: 7069 636b 6c65 0d0a 0970 7970 695f 696e  pickle...pypi_in
-00000550: 6465 782e 7478 740d 0a0d 0a5b 6f70 7469  dex.txt....[opti
-00000560: 6f6e 732e 656e 7472 795f 706f 696e 7473  ons.entry_points
-00000570: 5d0d 0a63 6f6e 736f 6c65 5f73 6372 6970  ]..console_scrip
-00000580: 7473 203d 200d 0a09 7079 6e61 6d65 7220  ts = ...pynamer 
-00000590: 3d20 7079 6e61 6d65 722e 7079 6e61 6d65  = pynamer.pyname
-000005a0: 723a 6d61 696e 0d0a 0d0a 5b66 6c61 6b65  r:main....[flake
-000005b0: 385d 0d0a 646f 6373 7472 696e 672d 636f  8]..docstring-co
-000005c0: 6e76 656e 7469 6f6e 203d 206e 756d 7079  nvention = numpy
-000005d0: 0d0a 6d61 782d 636f 6d70 6c65 7869 7479  ..max-complexity
-000005e0: 203d 2031 380d 0a6d 6178 2d6c 696e 652d   = 18..max-line-
-000005f0: 6c65 6e67 7468 203d 2038 380d 0a73 656c  length = 88..sel
-00000600: 6563 7420 3d20 422c 2042 392c 2043 2c20  ect = B, B9, C, 
-00000610: 442c 2045 2c20 462c 204e 2c20 570d 0a65  D, E, F, N, W..e
-00000620: 7863 6c75 6465 203d 2074 6573 7473 2f2a  xclude = tests/*
-00000630: 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a 2c64  ,.tox/*,.nox/*,d
-00000640: 6f63 732f 2a2c 2e67 6974 2f2a 2c2e 6769  ocs/*,.git/*,.gi
-00000650: 7468 7562 2f2a 0d0a 6967 6e6f 7265 203d  thub/*..ignore =
-00000660: 200d 0a09 4532 3033 2c0d 0a09 5735 3033   ...E203,...W503
-00000670: 2c0d 0a09 4634 3031 2c0d 0a70 6572 2d66  ,...F401,..per-f
-00000680: 696c 652d 6967 6e6f 7265 7320 3d20 0d0a  ile-ignores = ..
-00000690: 095f 5f69 6e69 745f 5f2e 7079 3a46 3430  .__init__.py:F40
-000006a0: 310d 0a09 7061 7468 6d61 6769 632e 7079  1...pathmagic.py
-000006b0: 3a46 3430 310d 0a09 7465 7374 5f70 796e  :F401...test_pyn
-000006c0: 616d 6572 2e70 793a 4634 3031 0d0a 0970  amer.py:F401...p
-000006d0: 796e 616d 6572 2e70 793a 4634 3031 0d0a  ynamer.py:F401..
-000006e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000006f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000700: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000260: 7320 3a3a 2035 202d 2050 726f 6475 6374  s :: 5 - Product
+00000270: 696f 6e2f 5374 6162 6c65 0d0a 0945 6e76  ion/Stable...Env
+00000280: 6972 6f6e 6d65 6e74 203a 3a20 436f 6e73  ironment :: Cons
+00000290: 6f6c 650d 0a09 496e 7465 6e64 6564 2041  ole...Intended A
+000002a0: 7564 6965 6e63 6520 3a3a 2044 6576 656c  udience :: Devel
+000002b0: 6f70 6572 730d 0a09 4f70 6572 6174 696e  opers...Operatin
+000002c0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000002d0: 6e64 6570 656e 6465 6e74 0d0a 094e 6174  ndependent...Nat
+000002e0: 7572 616c 204c 616e 6775 6167 6520 3a3a  ural Language ::
+000002f0: 2045 6e67 6c69 7368 0d0a 0950 726f 6772   English...Progr
+00000300: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000310: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
+00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000340: 3a3a 2033 203a 3a20 4f6e 6c79 0d0a 0950  :: 3 :: Only...P
+00000350: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000360: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000370: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+00000380: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000390: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+000003a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000003b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000003c0: 3a20 332e 3131 0d0a 0d0a 5b6f 7074 696f  : 3.11....[optio
+000003d0: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+000003e0: 203d 200d 0a09 3d73 7263 0d0a 7061 636b   = ...=src..pack
+000003f0: 6167 6573 203d 2066 696e 643a 0d0a 7072  ages = find:..pr
+00000400: 6f6a 6563 745f 7572 6c73 203d 200d 0a69  oject_urls = ..i
+00000410: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000420: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
+00000430: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000440: 332e 390d 0a69 6e73 7461 6c6c 5f72 6571  3.9..install_req
+00000450: 7569 7265 7320 3d20 0d0a 096a 696e 6a61  uires = ...jinja
+00000460: 320d 0a09 6273 340d 0a09 6275 696c 640d  2...bs4...build.
+00000470: 0a09 636f 6c6f 7261 6d61 0d0a 0970 7979  ..colorama...pyy
+00000480: 616d 6c0d 0a09 7265 7175 6573 7473 0d0a  aml...requests..
+00000490: 0972 6963 680d 0a09 7477 696e 650d 0a09  .rich...twine...
+000004a0: 7471 646d 0d0a 0977 6865 656c 0d0a 0d0a  tqdm...wheel....
+000004b0: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+000004c0: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+000004d0: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
+000004e0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+000004f0: 7079 6e61 6d65 7220 3d20 0d0a 0973 6574  pynamer = ...set
+00000500: 7570 2e74 7874 0d0a 0952 4541 444d 452e  up.txt...README.
+00000510: 6d64 0d0a 0970 726f 6a65 6374 5f6e 616d  md...project_nam
+00000520: 650d 0a09 7072 6f6a 6563 745f 6e61 6d65  e...project_name
+00000530: 2f5f 5f69 6e69 745f 5f2e 7079 0d0a 0970  /__init__.py...p
+00000540: 726f 6a65 6374 5f63 6f75 6e74 2e70 6963  roject_count.pic
+00000550: 6b6c 650d 0a09 7079 7069 5f69 6e64 6578  kle...pypi_index
+00000560: 2e74 7874 0d0a 0d0a 5b6f 7074 696f 6e73  .txt....[options
+00000570: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
+00000580: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
+00000590: 3d20 0d0a 0970 796e 616d 6572 203d 2070  = ...pynamer = p
+000005a0: 796e 616d 6572 2e70 796e 616d 6572 3a6d  ynamer.pynamer:m
+000005b0: 6169 6e0d 0a0d 0a5b 666c 616b 6538 5d0d  ain....[flake8].
+000005c0: 0a64 6f63 7374 7269 6e67 2d63 6f6e 7665  .docstring-conve
+000005d0: 6e74 696f 6e20 3d20 6e75 6d70 790d 0a6d  ntion = numpy..m
+000005e0: 6178 2d63 6f6d 706c 6578 6974 7920 3d20  ax-complexity = 
+000005f0: 3138 0d0a 6d61 782d 6c69 6e65 2d6c 656e  18..max-line-len
+00000600: 6774 6820 3d20 3838 0d0a 7365 6c65 6374  gth = 88..select
+00000610: 203d 2042 2c20 4239 2c20 432c 2044 2c20   = B, B9, C, D, 
+00000620: 452c 2046 2c20 4e2c 2057 0d0a 6578 636c  E, F, N, W..excl
+00000630: 7564 6520 3d20 7465 7374 732f 2a2c 2e74  ude = tests/*,.t
+00000640: 6f78 2f2a 2c2e 6e6f 782f 2a2c 646f 6373  ox/*,.nox/*,docs
+00000650: 2f2a 2c2e 6769 742f 2a2c 2e67 6974 6875  /*,.git/*,.githu
+00000660: 622f 2a0d 0a69 676e 6f72 6520 3d20 0d0a  b/*..ignore = ..
+00000670: 0945 3230 332c 0d0a 0957 3530 332c 0d0a  .E203,...W503,..
+00000680: 0946 3430 312c 0d0a 7065 722d 6669 6c65  .F401,..per-file
+00000690: 2d69 676e 6f72 6573 203d 200d 0a09 5f5f  -ignores = ...__
+000006a0: 696e 6974 5f5f 2e70 793a 4634 3031 0d0a  init__.py:F401..
+000006b0: 0970 6174 686d 6167 6963 2e70 793a 4634  .pathmagic.py:F4
+000006c0: 3031 0d0a 0974 6573 745f 7079 6e61 6d65  01...test_pyname
+000006d0: 722e 7079 3a46 3430 310d 0a09 7079 6e61  r.py:F401...pyna
+000006e0: 6d65 722e 7079 3a46 3430 310d 0a0d 0a5b  mer.py:F401....[
+000006f0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000700: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000710: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `pynamer-0.5.7/src/pynamer/__init__.py` & `pynamer-1.0.0/src/pynamer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pickle
 from importlib.resources import as_file, files
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "0.5.7"
+__version__ = "1.0.0"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
```

### Comparing `pynamer-0.5.7/src/pynamer/pynamer.py` & `pynamer-1.0.0/src/pynamer/pynamer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,754 +1,808 @@
-#!/usr/bin/env python3
-
-# Core Library modules
-import argparse
-import json
-import logging
-import os
-import pickle
-import re
-import shutil
-import string
-import subprocess
-import sys
-from datetime import datetime
-from pathlib import Path
-from typing import Any, Optional, Union
-
-# Third party modules
-import build
-import requests
-from bs4 import BeautifulSoup
-from colorama import Back, Fore, Style
-from jinja2 import Template
-from rich.console import Console
-from rich.table import Table
-from tqdm import tqdm
-
-# Local modules
-from . import project_count, project_path, setup_text
-
-logger = logging.getLogger()
-for handler in logger.handlers:
-    logger.removeHandler(handler)
-
-
-class Config:
-    """Configuration class"""
-
-    pypirc: Optional[Path] = None
-    original_project_name = "project_name"
-    no_cleanup: bool = False
-    project_count = 0
-    package_version = "0.0.0"
-    pypi_search_url: str = "https://pypi.org/search/"
-    pypi_project_url: str = "https://pypi.org/project/"
-    pypi_json_url: str = "https://pypi.org/pypi/"
-    pypi_simple_index_url: str = "https://pypi.org/simple/"
-    idlemode = 1 if "idlelib.run" in sys.modules else 0
-
-
-config = Config()
-config.project_count = project_count
-
-
-def _feedback(message: str, feedback_type: str) -> None:
-    """Generates a formatted messages appropriate to the message type.
-
-    Args:
-        message:        Text to be echoed.
-        feedback_type:  identifies type of message to display.
-    """
-    if feedback_type not in ["null", "nominal", "warning", "error"]:
-        return
-    if config.idlemode == 1:
-        print(message)
-    else:
-        if feedback_type == "null":
-            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "nominal":
-            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-        elif feedback_type == "warning":
-            print(
-                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
-            )
-        elif feedback_type == "error":
-            print(Fore.RED + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
-
-
-def _find_pypirc_file(filename: str = ".pypirc") -> None:
-    """Function to iterate over paths in the PATH environment variable to find a file.
-
-     Designed to find a .pypirc file starting with the current working directory.
-     If identified will update the config.pypirc variable, so it can be used elsewhere.
-
-    Args:
-        filename:       filename to find.
-    """
-    system_path = os.getenv("PATH")
-    if system_path is not None:
-        path_directories = [os.getcwd()]
-        path_directories.extend(system_path.split(os.pathsep))
-        for directory in path_directories:
-            file_path = Path(directory) / filename
-            if file_path.exists():
-                logger.debug(
-                    "%s is present in the system's PATH at %s", filename, directory
-                )
-                config.pypirc = file_path
-                break
-    logger.debug("%s is not present in the system's PATH.", filename)
-
-
-def _rename_project_dir(old_name: str, new_name: str) -> None:
-    """Utility script to rename a directory.
-
-    The object being to rename a 'template' directory for the purpose of creating a
-    minimalist package for upload to PyPI.
-
-    Args:
-        old_name:       source name.
-        new_name:       dst name.
-
-    Raises:
-        FileNotFoundError
-    """
-    old_directory_path = Path(old_name)
-    new_directory_path = Path(new_name)
-    logger.debug("renaming project directory from %s to %s", old_name, new_name)
-    try:
-        old_directory_path.rename(new_directory_path)
-    except FileNotFoundError:
-        logger.error("directory %s cannot be found:", old_directory_path)
-        raise FileNotFoundError
-
-
-def _create_setup(new_project_name: str) -> None:
-    """Utility script to create a setup.py file.
-
-    The object being to create a setup.py file from a 'template' file for the purpose of
-    creating a minimalist package for upload to PyPI.
-
-    Args:
-        new_project_name:       name used to render the template.
-    """
-    template = Template(setup_text)
-    content = template.render(
-        PROJECT_NAME=new_project_name,
-        PACKAGE_VERSION=config.package_version,
-    )
-    setup_file = project_path.joinpath("setup.py")
-    with open(setup_file, mode="w", encoding="utf-8") as message:
-        logger.debug("creating new setup.py with the following: \n %s", content)
-        message.write(content)
-
-
-def _delete_director(items_to_delete: list[Path]) -> None:
-    """Utility function to delete files and directories.
-
-    Args:
-        items_to_delete:    A list of Path like objects to delete.
-    """
-    for item in items_to_delete:
-        if not item.exists():
-            logger.debug("trying to delete %s but it does not exist", item)
-            continue
-        if item.is_dir():
-            logger.debug("Deleting Directory: %s", item)
-            shutil.rmtree(item, ignore_errors=True)
-        else:
-            logger.debug("Deleting File: %s", item)
-            Path.unlink(item, missing_ok=True)
-
-
-def _run_command(
-    *arguments: str,
-    shell: bool = True,
-    capture_output: bool = False,
-    text: bool = True,
-    working_dir: Union[Path, str, None] = None,
-    project: Union[None, str] = None,
-) -> None:
-    """Utility designed to execute a command line utility.
-
-    Args:
-        arguments:  Comma separated strings- "utility", "arg1", "arg2", etc.
-        shell:      command executed by the shell or directly by the operating system.
-        cwd:        specifies the current working directory to use when starting
-                    the subprocess.
-                    e.g. "/home/user/mydir"
-        project:    the name of the project currently being tested
-    """
-    working_dir = os.getcwd() if working_dir is None else working_dir
-    try:
-        process = subprocess.Popen(
-            arguments,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            shell=shell,
-            text=True,
-            cwd=working_dir,
-        )
-        stdout, stderr = process.communicate()
-        if process.returncode != 0:
-            logger.error("Error running command: %s", arguments)
-            logger.error("stderr: %s", stderr)
-            if project is not None:
-                _cleanup(project)
-            return
-        logger.debug("%s", stdout)
-        return stdout
-    except Exception as e:
-        logger.error("Exception running command: %s", arguments)
-        logger.error(e)
-        if project is not None:
-            _cleanup(project)
-        return
-
-
-def _ping_project(project_name: str) -> bool:
-    """Determines if the URL to the project exists on PyPI.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Returns:
-        True:           If the URLs response code is 200
-        False:          If the URLs response code is not 200
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_project = "".join([config.pypi_project_url, project_name, "/"])
-    logger.debug("attempting to get url %s", url_project)
-    try:
-        project_ping = requests.get(url_project, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_ping.status_code == 200:
-        logger.debug("%s FOUND in the project area of PyPI", project_name)
-        return True
-    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
-    return False
-
-
-def _ping_json(project_name: str) -> str:
-    """Collects some details about the project if it exists.
-
-    Args:
-        project_name:   the name of the project to test.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-    """
-    url_json = "".join([config.pypi_json_url, project_name, "/json"])
-    logger.debug("attempting to get url %s", url_json)
-    try:
-        project_json_raw = requests.get(url_json, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    if project_json_raw.status_code == 200:
-        project_json = json.loads(project_json_raw.content)
-        result = "".join(
-            [
-                project_json["info"]["author"],
-                "\n",
-                project_json["info"]["author_email"],
-                "\n",
-                project_json["info"]["version"],
-                "\n",
-                project_json["info"]["summary"],
-            ]
-        )
-        return result
-    logger.debug("No response from JSON URL")
-    return ""
-
-
-def _build_dist() -> None:
-    """Builds the sdist and wheel of the minimalist project to upload to PyPI."""
-    logger.debug("Building the distribution... ")
-    builder = build.ProjectBuilder(project_path)
-    builder.build("wheel", project_path / "dist")
-    builder.build("sdist", project_path / "dist")
-
-
-def _upload_dist(project_name: str) -> None:
-    """Builds the twine command line to upload the minimalist project to PyPI.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Notes:
-        twine expects a filesystem path not Path object so use os.fspath()
-    """
-    logger.debug("Uploading the distribution... ")
-    dir_path = os.fspath(project_path / "dist" / "*")
-    pypirc_path = os.fspath(config.pypirc)  # type: ignore
-    _run_command(
-        sys.executable,
-        "-m",
-        "twine",
-        "upload",
-        "--config-file",
-        pypirc_path,
-        dir_path,
-        project=project_name,
-    )
-
-
-def _cleanup(project_name: str) -> None:
-    """Builds a manifest of artifacts to delete into a list of Path objects.
-
-    Args:
-        project_name:   the name of the project currently under test.
-    """
-    if config.no_cleanup is True:
-        return
-    _rename_project_dir(
-        project_path.joinpath(project_name),
-        project_path.joinpath(config.original_project_name),
-    )
-    build_artifacts = [
-        project_path / "build",
-        project_path / "dist",
-        project_path / "".join([project_name, ".egg-info"]),
-        project_path / "setup.py",
-    ]
-    logger.debug("cleaning build artifacts %s", build_artifacts)
-    _delete_director(build_artifacts)
-
-
-def _generate_pypi_index() -> None:
-    """Generates a list of projects in PyPI's simple index - writes results to a file.
-
-    Raises:
-        SystemExit:     If any requests.RequestException occurs.
-
-    Notes:
-        A potentially expensive operation as there are almost 500,000 projects to
-        process. Can take 2-3 seconds. Look to improve performance at a later date:
-        look at asyncio, asyncio.http etc.
-        An improvement is to automatically periodically run this in the background.
-    """
-    new_count = 0
-    pattern = re.compile(r">([\w\W]*?)<")
-    progress_bar = tqdm(total=config.project_count)
-    pypi_index = project_path / "pypi_index"
-    pypi_count = project_path / "project_count.pickle"
-    if pypi_index.exists():
-        Path.unlink(pypi_index, missing_ok=True)
-    try:
-        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=10)
-    except requests.RequestException as e:
-        logger.error("An error occurred: %s", e)
-        raise SystemExit("An error occurred with an HTTP request")
-    with pypi_index.open(mode="a") as file:
-        for line in index_object_raw.iter_lines():
-            line = str(line)
-            project_text = re.search(pattern, line)
-            if project_text is not None:
-                new_count += 1
-                progress_bar.update(1)
-                project = "".join([project_text.group(1), " \n"])
-                file.write(project)
-    progress_bar.close()
-    with open(pypi_count, "wb") as f:
-        pickle.dump(new_count, f)
-
-
-def _pypi_search_index(project_name: str) -> bool:
-    """Open the generated index file and search for the project name.
-
-    Args:
-        project_name:   the name of the project currently under test.
-
-    Returns:
-        True:           A match was found.
-        False:          A match was not found.
-    """
-    pypi_index = project_path / "pypi_index"
-    if not pypi_index.exists():
-        _generate_pypi_index()
-    with pypi_index.open(mode="r") as file:
-        projects = file.read()
-        if project_name in projects:
-            logger.debug("%s FOUND in the PyPI simple index", project_name)
-            return True
-        logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
-        return False
-
-
-def _pypi_search(
-    search_project: str,
-) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
-    """Performs a get request to PyPI's search API for the project name.
-
-    Args:
-        search_project:   the name of the project currently under test.
-
-    Returns:
-        match:          A list of projects matching name comprising:
-                            [project_name, version, released, description]
-        others:         A list of projects not matching but PyPI thinks are relevant.
-                            [project_name, version, released, description]
-        others_total:   A str representation of total projects found (minus matches).
-    """
-    pattern = re.compile(r">([\d,+]*?)<")
-    s = requests.Session()
-    projects_raw, match, others = [], [], []
-    params = {"q": {search_project}, "page": 1}
-    r = s.get(config.pypi_search_url, params=params)  # type: ignore
-    soup = BeautifulSoup(r.text, "html.parser")
-    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
-    for project_raw in projects_raw:
-        project_name = project_raw.select_one(
-            'span[class*="package-snippet__name"]'
-        ).text.strip()
-        version = project_raw.select_one(
-            'span[class*="package-snippet__version"]'
-        ).text.strip()
-        released_iso_8601 = project_raw.select_one(
-            'span[class*="package-snippet__created"]'
-        ).find("time")["datetime"]
-        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
-            "%Y-%m-%d"
-        )
-        description = project_raw.select_one(
-            'p[class*="package-snippet__description"]'
-        ).text.strip()
-        if project_name.lower() == search_project.lower():
-            match.append([project_name, version, released, description])
-        else:
-            others.append([project_name, version, released, description])
-
-    total_div_raw = soup.select(
-        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
-    )
-    total_raw = re.search(pattern, str(total_div_raw))
-    if total_raw is not None:
-        total_string = total_raw.group(1)
-        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
-        others_total = (
-            "".join([str(total), "+"])
-            if total == 10000
-            else (str(int(total) - len(match)))
-        )
-    else:
-        others_total = "0"
-    return match, others, others_total
-
-
-def _process_input_file(file: str) -> list[Union[str, Any]]:
-    """Processes the contents of the file to a list of strings.
-
-    Args:
-        file:           simple string for the file.
-
-    Raises:
-        SystemExit:     If the file is found to not exist.
-
-    Notes:
-        file contents should contain any number of space separated strings on any
-        number of lines.
-    """
-    file_path = Path(file)
-    if not file_path.exists():
-        raise SystemExit(f"The file {file} does not exist")
-    with file_path.open(mode="r") as f:
-        file_contents = f.read()
-        projects = file_contents.split()
-        return list(set(projects))
-
-
-def _write_output_file(file_name: str, results: dict) -> None:
-    """Write the results to a file
-
-    Args:
-        file_name:      Name of file to save as a simple string.
-        results:        Dictionary containing the test results e.g.
-                        {"pynball": [1, 1, 1]}
-    """
-    header_width = 83
-    truncation_width = 25
-    file_path = Path(file_name)
-    title = f"Results from pynamer PyPI utility\n"
-    title = "".join([title, "=" * header_width, "\n\n"])
-    title = "".join(
-        [
-            title,
-            "Test 1 - Basic url lookup on PyPI\n",
-            "Test 2 - Search of PyPIs simple index\n",
-            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
-        ]
-    )
-    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
-    header = "".join([header, "=" * header_width, "\n"])
-    projects_results: str = ""
-    for project in results:
-        project_name = (
-            project
-            if len(project) <= truncation_width
-            else project[: truncation_width - 3] + "..."
-        )
-        projects_results = "".join([projects_results, f"{project_name:30}"])
-        for test in results[project]:
-            test = "Found" if test == 1 else "Not Found"
-            projects_results = "".join([projects_results, f"{test:12}"])
-        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
-        projects_results = "".join([projects_results, f"{conclusion}"])
-        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
-    with file_path.open(mode="w") as f:
-        f.write(title)
-        f.write(header)
-        f.write(projects_results)
-
-
-def _final_analysis(pattern: list[int]) -> None:
-    """Displays a rich console table displaying the conclusion of the test results
-
-    Args:
-        pattern:    A list of the test results:
-                    1 - A 'negative' result, indicating the project has been found.
-                    0 - A 'positive' result, indicating the project was not found.
-    """
-    table = Table(show_header=True)
-    table.add_column("FINAL ANALYSIS", style="bold cyan")
-    if pattern == [0, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "It can only be found by searching the simple index which is not available "
-            "through the interface"
-        )
-    elif pattern == [1, 1, 0]:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row(
-            "A Gotcha!, whereby the package is not found even with PyPI's own search"
-            " facility.\n"
-            "However if appears in the simple index and can be displayed by simply"
-            " browsing "
-            "to the projects URL"
-        )
-    elif sum(pattern) >= 1:
-        table.add_row("[red]NOT AVAILABLE![/red]\n")
-        table.add_row("The package name was found in at least one place")
-    elif sum(pattern) == 0:
-        table.add_row("[green]AVAILABLE![/green]\n")
-        table.add_row("The package name was not found in any part of PyPI")
-
-    console = Console()
-    console.print(table)
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        prog="pynamer",
-        description="Determine if project name is available on pypi with the "
-        "option to 'register' it for future use if available",
-    )
-    parser.add_argument(
-        "projects",
-        nargs="*",
-        default="None",
-        help="Optional - one or more project names",
-    )
-    parser.add_argument(
-        "-r",
-        "--register",
-        action="store_true",
-        help="Register the name on PyPi if the name is available",
-    )
-    parser.add_argument(
-        "-d",
-        "--dryrun",
-        action="store_true",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "-f",
-        "--file",
-        default="None",
-        type=str,
-        help="File containing a list of projects to analyze",
-    )
-    parser.add_argument(
-        "-o",
-        "--output",
-        default="None",
-        type=str,
-        help="File to output the results to",
-    )
-    parser.add_argument(
-        "-n",
-        "--nocleanup",
-        action="store_true",
-        help=argparse.SUPPRESS,
-    )
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        help="output additional information",
-    )
-    parser.add_argument(
-        "-g",
-        "--generate",
-        action="store_true",
-        help="Generate a new PyPI simple index",
-    )
-
-    args = parser.parse_args()
-    logger.debug(" args: %s", args)
-
-    if args.generate is True:
-        _generate_pypi_index()
-
-    if args.projects == "None" and args.file == "None":
-        parser.print_help()
-        raise SystemExit("No projects to analyse")
-
-    project_list = []
-    test_results = []
-    aggregated_result = {}
-    _find_pypirc_file()
-    if args.nocleanup is True:
-        config.no_cleanup = True
-
-    # Gather the projects into one list
-    if args.projects != "None":
-        logger.debug("adding project names from command line %s", args.projects)
-        project_list.extend(list(set(args.projects)))
-        logger.debug("project_list = %s", project_list)
-    if args.file != "None":
-        logger.debug("adding project names from file %s", args.file)
-        project_list.extend(_process_input_file(args.file))
-        logger.debug("project_list = %s", project_list)
-    project_list.sort()
-
-    # Main loop
-    for new_project in project_list:
-        test_table = Table(title=f"Test Results for {new_project}", show_lines=True)
-        test_table.add_column("No.", style="bold yellow")
-        test_table.add_column("Test", style="bold cyan")
-        test_table.add_column("Result")
-        test_table.add_column("Details", style="bold cyan")
-
-        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
-        match_table.add_column("Package", style="bold yellow")
-        match_table.add_column("Version", style="bold green")
-        match_table.add_column("Released", style="bold yellow")
-        match_table.add_column("Description", style="bold cyan")
-
-        others_table = Table(
-            title="Other Close Matches or Related Projects (from page 1)"
-        )
-        others_table.add_column("Package", style="bold yellow")
-        others_table.add_column("Version", style="bold green")
-        others_table.add_column("Released", style="bold yellow")
-        others_table.add_column("Description", style="bold cyan")
-
-        # perform the tests
-        # Test 1
-        if _ping_project(new_project):
-            test_results.append(1)
-            json_data = _ping_json(new_project)
-            test_table.add_row(
-                "1", "Basic http get to project URL", "[red]FOUND[/red]", json_data
-            )
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "1", "Basic http get to project URL", "[green]NOT FOUND[/green]", ""
-            )
-
-        # Test 2
-        if _pypi_search_index(new_project):
-            test_results.append(1)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "[red]FOUND[/red]",
-                f"Searched {project_count} projects",
-            )
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "2",
-                "Check PyPI simple index",
-                "[green]NOT FOUND[/green]",
-                f"Searched {project_count} projects",
-            )
-
-        # Test 3
-        match, others, others_total = _pypi_search(new_project)
-        if match:
-            test_results.append(1)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "[red]FOUND[/red]",
-                f"Exact match found: {len(match)}, Others found: {others_total}",
-            )
-            for items in match:
-                match_table.add_row(items[0], items[1], items[2], items[3])
-        else:
-            test_results.append(0)
-            test_table.add_row(
-                "3",
-                "Check PyPI search",
-                "[green]NOT FOUND[/green]",
-                f"Exact match found: 0, Others found: {others_total}",
-            )
-
-        # Create Verbose Table
-        if others:
-            for items in others:
-                others_table.add_row(items[0], items[1], items[2], items[3])
-
-        # Display the Tables
-        console = Console()
-        console.print(test_table)
-        if match:
-            console.print(match_table)
-        if args.verbose and others:
-            console.print(others_table)
-        _final_analysis(test_results)
-
-        # build and upload
-        if (
-            test_results == [0, 0, 0]
-            and args.register is True
-            and config.pypirc is not None
-        ):
-            _rename_project_dir(
-                project_path.joinpath(config.original_project_name),
-                project_path.joinpath(new_project),
-            )
-            _create_setup(new_project)
-            _build_dist()
-            if args.dryrun is False:
-                _upload_dist(new_project)
-            else:
-                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
-            _cleanup(new_project)
-        elif config.pypirc is None:
-            _feedback(
-                ".pypirc file cannot be located ... wont attempt to 'register'",
-                "error",
-            )
-        elif sum(test_results) > 0 and args.register is True:
-            _feedback("Project already exists ... wont attempt to 'register'", "error")
-
-        aggregated_result[new_project] = test_results.copy()
-        test_results.clear()
-
-    if args.output != "None":
-        _write_output_file(args.output, aggregated_result)
-
-
-if __name__ == "__main__":
-    SystemExit(main())
+#!/usr/bin/env python3
+
+# Core Library modules
+import argparse
+import json
+import logging
+import os
+import pickle
+import re
+import shutil
+import string
+import subprocess
+import sys
+from datetime import datetime
+from pathlib import Path
+from typing import Any, Optional, Union
+
+# Third party modules
+import build
+import requests
+from bs4 import BeautifulSoup
+from colorama import Back, Fore, Style
+from jinja2 import Template
+from rich.console import Console
+from rich.table import Table
+from tqdm import tqdm
+
+# Local modules
+from . import project_count, project_path, setup_text
+
+logger = logging.getLogger()
+
+
+class Config:
+    """Configuration class"""
+
+    pypirc: Optional[Path] = None
+    original_project_name: str = "project_name"
+    no_cleanup: bool = False
+    project_count: int = 0
+    package_version: str = "0.0.0"
+    pypi_search_url: str = "https://pypi.org/search/"
+    pypi_project_url: str = "https://pypi.org/project/"
+    pypi_json_url: str = "https://pypi.org/pypi/"
+    pypi_simple_index_url: str = "https://pypi.org/simple/"
+    idlemode: int = 1 if "idlelib.run" in sys.modules else 0
+
+
+config = Config()
+config.project_count = project_count
+
+
+def _feedback(message: str, feedback_type: str) -> None:
+    """Generates a formatted messages appropriate to the message type.
+
+    Args:
+        message:        Text to be echoed.
+        feedback_type:  identifies type of message to display.
+    """
+    if feedback_type not in ["null", "nominal", "warning", "error"]:
+        return
+    if config.idlemode == 1:
+        print(message)
+    else:
+        if feedback_type == "null":
+            print(Fore.WHITE + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "nominal":
+            print(Fore.GREEN + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+        elif feedback_type == "warning":
+            print(
+                Fore.YELLOW + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL
+            )
+        elif feedback_type == "error":
+            print(Fore.RED + Back.BLACK + Style.BRIGHT + f"{message}" + Style.RESET_ALL)
+
+
+def _find_pypirc_file(filename: str = ".pypirc") -> None:
+    """Function to iterate over paths in the PATH environment variable to find a file.
+
+     Designed to find a .pypirc file starting with the current working directory.
+     If identified will update the config.pypirc variable, so it can be used elsewhere.
+
+    Args:
+        filename:       filename to find.
+    """
+    system_path = os.getenv("PATH")
+    if system_path is not None:
+        path_directories = [os.getcwd()]
+        path_directories.extend(system_path.split(os.pathsep))
+        for directory in path_directories:
+            file_path = Path(directory) / filename
+            if file_path.exists():
+                logger.debug(
+                    "%s is present in the system's PATH at %s", filename, directory
+                )
+                config.pypirc = file_path
+                break
+    logger.debug("%s is not present in the system's PATH.", filename)
+
+
+def _rename_project_dir(old_name: str, new_name: str) -> None:
+    """Utility script to rename a directory.
+
+    The object being to rename a 'template' directory for the purpose of creating a
+    minimalist package for upload to PyPI.
+
+    Args:
+        old_name:       source name.
+        new_name:       dst name.
+
+    Raises:
+        FileNotFoundError
+    """
+    old_directory_path = Path(old_name)
+    new_directory_path = Path(new_name)
+    logger.debug("renaming project directory from %s to %s", old_name, new_name)
+    try:
+        old_directory_path.rename(new_directory_path)
+    except FileNotFoundError:
+        logger.error("directory %s cannot be found:", old_directory_path)
+        raise FileNotFoundError
+
+
+def _create_setup(new_project_name: str) -> None:
+    """Utility script to create a setup.py file.
+
+    The object being to create a setup.py file from a 'template' file for the purpose of
+    creating a minimalist package for upload to PyPI.
+
+    Args:
+        new_project_name:       name used to render the template.
+    """
+    template = Template(setup_text)
+    content = template.render(
+        PROJECT_NAME=new_project_name,
+        PACKAGE_VERSION=config.package_version,
+    )
+    setup_file = project_path.joinpath("setup.py")
+    with open(setup_file, mode="w", encoding="utf-8") as message:
+        logger.debug("creating new setup.py with the following: \n %s", content)
+        message.write(content)
+
+
+def _delete_director(items_to_delete: list[Path]) -> None:
+    """Utility function to delete files and directories.
+
+    Args:
+        items_to_delete:    A list of Path like objects to delete.
+    """
+    for item in items_to_delete:
+        if not item.exists():
+            logger.debug("trying to delete %s but it does not exist", item)
+            continue
+        if item.is_dir():
+            logger.debug("Deleting Directory: %s", item)
+            shutil.rmtree(item, ignore_errors=True)
+        else:
+            logger.debug("Deleting File: %s", item)
+            Path.unlink(item, missing_ok=True)
+
+
+def _run_command(
+    *arguments: str,
+    shell: bool = True,
+    working_dir: Union[Path, str, None] = None,
+    project: Union[None, str] = None,
+) -> None:  # pragma: no cover
+    """Utility designed to execute a command line utility.
+
+    Args:
+        arguments:  Comma separated strings- "utility", "arg1", "arg2", etc.
+        shell:      command executed by the shell or directly by the operating system.
+        cwd:        specifies the current working directory to use when starting
+                    the subprocess.
+                    e.g. "/home/user/mydir"
+        project:    the name of the project currently being tested
+    """
+    working_dir = os.getcwd() if working_dir is None else working_dir
+    try:
+        process = subprocess.Popen(
+            arguments,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            shell=shell,
+            text=True,
+            cwd=working_dir,
+        )
+        stdout, stderr = process.communicate()
+        if process.returncode != 0:
+            logger.error("Error running command: %s", arguments)
+            logger.error("stderr: %s", stderr)
+            if project is not None:
+                _cleanup(project)
+            return
+        logger.debug("%s", stdout)
+        return
+    except Exception as e:
+        logger.error("Exception running command: %s", arguments)
+        logger.error(e)
+        if project is not None:
+            _cleanup(project)
+        return
+
+
+def _is_valid_package_name(project_name: str) -> bool:
+    """Function does a basic check of project name validity.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the name passes the basic check
+        False:          If the name fails the basic check
+
+
+    """
+    pattern = r"^[a-z][_a-z0-9]*$"
+    if re.match(pattern, project_name) is not None:
+        return True
+    else:
+        return False
+
+
+def _ping_project(project_name: str) -> bool:
+    """Determines if the URL to the project exists in PyPIs project area.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Returns:
+        True:           If the URLs response code is 200
+        False:          If the URLs response code is not 200
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_project = "".join([config.pypi_project_url, project_name, "/"])
+    logger.debug("attempting to get url %s", url_project)
+    try:
+        project_ping = requests.get(url_project, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_ping.status_code == 200:
+        logger.debug("%s FOUND in the project area of PyPI", project_name)
+        return True
+    logger.debug("%s NOT FOUND in the project area of PyPI", project_name)
+    return False
+
+
+def _ping_json(project_name: str) -> str:
+    """Collects some details about the project if it exists.
+
+    Args:
+        project_name:   the name of the project to test.
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+    """
+    url_json = "".join([config.pypi_json_url, project_name, "/json"])
+    logger.debug("attempting to get url %s", url_json)
+    try:
+        project_json_raw = requests.get(url_json, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    if project_json_raw.status_code == 200:
+        project_json = json.loads(project_json_raw.content)
+        result = "".join(
+            [
+                project_json["info"]["author"],
+                "\n",
+                project_json["info"]["author_email"],
+                "\n",
+                project_json["info"]["version"],
+                "\n",
+                project_json["info"]["summary"],
+            ]
+        )
+        return result
+    logger.debug("No response from JSON URL")
+    return ""
+
+
+def _build_dist() -> None:
+    """Builds the sdist and wheel of the minimalist project to upload to PyPI."""
+    logger.debug("Building the distribution... ")
+    builder = build.ProjectBuilder(project_path)
+    builder.build("wheel", project_path / "dist")
+    builder.build("sdist", project_path / "dist")
+
+
+def _upload_dist(project_name: str) -> None:
+    """Builds the twine command line to upload the minimalist project to PyPI.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Notes:
+        twine expects a filesystem path not Path object so use os.fspath()
+    """
+    logger.debug("Uploading the distribution... ")
+    dir_path = os.fspath(project_path / "dist" / "*")
+    pypirc_path = os.fspath(config.pypirc)  # type: ignore
+    _run_command(
+        sys.executable,
+        "-m",
+        "twine",
+        "upload",
+        "--config-file",
+        pypirc_path,
+        dir_path,
+        project=project_name,
+    )
+
+
+def _cleanup(project_name: str) -> None:
+    """Builds a manifest of artifacts to delete into a list of Path objects.
+
+    Args:
+        project_name:   the name of the project currently under test.
+    """
+    if config.no_cleanup is True:
+        return
+    _rename_project_dir(
+        project_path.joinpath(project_name),
+        project_path.joinpath(config.original_project_name),
+    )
+    build_artifacts = [
+        project_path / "build",
+        project_path / "dist",
+        project_path / "".join([project_name, ".egg-info"]),
+        project_path / "setup.py",
+    ]
+    logger.debug("cleaning build artifacts %s", build_artifacts)
+    _delete_director(build_artifacts)
+
+
+def _generate_pypi_index() -> None:
+    """Generates a list of projects in PyPI's simple index - writes results to a file.
+
+    Raises:
+        SystemExit:     If any requests.RequestException occurs.
+
+    Notes:
+        A potentially expensive operation as there are almost 500,000 projects to
+        process. Can take 2-3 seconds. Look to improve performance at a later date:
+        look at asyncio, asyncio.http etc.
+        An improvement is to automatically periodically run this in the background.
+    """
+    new_count = 0
+    pattern = re.compile(r">([\w\W]*?)<")
+    progress_bar = tqdm(total=config.project_count)
+    pypi_index = project_path / "pypi_index"
+    pypi_count = project_path / "project_count.pickle"
+    if pypi_index.exists():
+        Path.unlink(pypi_index, missing_ok=True)
+    try:
+        index_object_raw = requests.get(config.pypi_simple_index_url, timeout=10)
+    except requests.RequestException as e:
+        logger.error("An error occurred: %s", e)
+        raise SystemExit("An error occurred with an HTTP request")
+    with pypi_index.open(mode="a") as file:
+        for line in index_object_raw.iter_lines():
+            line = str(line)
+            project_text = re.search(pattern, line)
+            if project_text is not None:
+                new_count += 1
+                progress_bar.update(1)
+                project = "".join([project_text.group(1), " \n"])
+                file.write(project)
+    progress_bar.close()
+    with open(pypi_count, "wb") as f:
+        pickle.dump(new_count, f)
+
+
+def _pypi_search_index(project_name: str) -> bool:
+    """Open the generated index file and search for the project name.
+
+    Args:
+        project_name:   the name of the project currently under test.
+
+    Returns:
+        True:           A match was found.
+        False:          A match was not found.
+    """
+    pypi_index = project_path / "pypi_index"
+    if not pypi_index.exists():
+        _generate_pypi_index()
+    with pypi_index.open(mode="r") as file:
+        projects = file.read()
+        if project_name in projects:
+            logger.debug("%s FOUND in the PyPI simple index", project_name)
+            return True
+        logger.debug("%s NOT FOUND in the PyPI simple index", project_name)
+        return False
+
+
+def _pypi_search(
+    search_project: str,
+) -> tuple[list[list[Union[str, Any]]], list[list[Union[str, Any]]], str]:
+    """Performs a get request to PyPI's search API for the project name.
+
+    Args:
+        search_project:   The name of the project currently under test.
+
+    Returns:
+        match:          A list of projects matching name comprising:
+                            [project_name, version, released, description]
+        others:         A list of projects not matching but PyPI thinks are relevant.
+                            [project_name, version, released, description]
+        others_total:   A str representation of total projects found (minus matches).
+    """
+    pattern = re.compile(r">([\d,+]*?)<")
+    s = requests.Session()
+    projects_raw, match, others = [], [], []
+    params = {"q": {search_project}, "page": 1}
+    r = s.get(config.pypi_search_url, params=params)  # type: ignore
+    soup = BeautifulSoup(r.text, "html.parser")
+    projects_raw.extend(soup.select('a[class*="package-snippet"]'))
+    for project_raw in projects_raw:
+        project_name = project_raw.select_one(
+            'span[class*="package-snippet__name"]'
+        ).text.strip()
+        version = project_raw.select_one(
+            'span[class*="package-snippet__version"]'
+        ).text.strip()
+        released_iso_8601 = project_raw.select_one(
+            'span[class*="package-snippet__created"]'
+        ).find("time")["datetime"]
+        released = datetime.strptime(released_iso_8601, "%Y-%m-%dT%H:%M:%S%z").strftime(
+            "%Y-%m-%d"
+        )
+        description = project_raw.select_one(
+            'p[class*="package-snippet__description"]'
+        ).text.strip()
+        if project_name.lower() == search_project.lower():
+            match.append([project_name, version, released, description])
+        else:
+            others.append([project_name, version, released, description])
+
+    total_div_raw = soup.select(
+        'div[class="split-layout split-layout--table split-layout--wrap-on-tablet"]'
+    )
+    total_raw = re.search(pattern, str(total_div_raw))
+    if total_raw is not None:
+        total_string = total_raw.group(1)
+        total = int(total_string.translate(str.maketrans("", "", string.punctuation)))
+        others_total = (
+            "".join([str(total), "+"])
+            if total == 10000
+            else (str(int(total) - len(match)))
+        )
+    else:
+        others_total = "0"
+    return match, others, others_total
+
+
+def _process_input_file(file: str) -> list[Union[str, Any]]:
+    """Processes the contents of the file to a list of strings.
+
+    Args:
+        file:           simple string for the file.
+
+    Raises:
+        SystemExit:     If the file is found to not exist.
+
+    Notes:
+        file contents should contain any number of space separated strings on any
+        number of lines.
+    """
+    file_path = Path(file)
+    try:
+        with file_path.open(mode="r") as f:
+            file_contents = f.read()
+            projects = file_contents.split()
+            return list(set(projects))
+    except FileNotFoundError:
+        raise SystemExit(f"The file {file} does not exist")  # pragma: no cover
+    except PermissionError:
+        raise SystemExit(f"Permission denied to file: {file}")  # pragma: no cover
+    except IsADirectoryError:
+        raise SystemExit(f"{file} is a directory not a file")  # pragma: no cover
+    except OSError:
+        raise SystemExit(
+            f"A general IO error has occurred opening file: {file}"
+        )  # pragma: no cover
+    except Exception as e:
+        raise SystemExit("An error occurred:", str(e))  # pragma: no cover
+
+
+def _write_output_file(file_name: str, results: dict) -> None:
+    """Write the results to a file
+
+    Args:
+        file_name:      Name of file to save as a simple string.
+        results:        Dictionary containing the test results e.g.
+                        {"pynball": [1, 1, 1]}
+    """
+    header_width = 83
+    truncation_width = 25
+    file_path = Path(file_name)
+    title = f"Results from pynamer PyPI utility\n"
+    title = "".join([title, "=" * header_width, "\n\n"])
+    title = "".join(
+        [
+            title,
+            "Test 1 - Basic url lookup on PyPI\n",
+            "Test 2 - Search of PyPIs simple index\n",
+            "Test 3 - Search using an request to PyPIs search 'API'\n\n",
+        ]
+    )
+    header = f"{'Project':30}{'Test1':12}{'Test2':12}{'Test3':12}{'Conclusion'}\n"
+    header = "".join([header, "=" * header_width, "\n"])
+    projects_results: str = ""
+    for project in results:
+        project_name = (
+            project
+            if len(project) <= truncation_width
+            else project[: truncation_width - 3] + "..."
+        )
+        projects_results = "".join([projects_results, f"{project_name:30}"])
+        for test in results[project]:
+            test = "Found" if test == 1 else "Not Found"
+            projects_results = "".join([projects_results, f"{test:12}"])
+        conclusion = "Not Available" if sum(results[project]) > 0 else "Available"
+        projects_results = "".join([projects_results, f"{conclusion}"])
+        projects_results = "".join([projects_results, "\n", "-" * header_width, "\n"])
+
+    final_output_text = "".join([title, header, projects_results])
+
+    try:  # pragma: no cover
+        with file_path.open(mode="w") as f:
+            f.write(final_output_text)
+    except PermissionError:
+        raise SystemExit(
+            f"Permission denied to file: {file_path.open}"
+        )  # pragma: no cover
+    except FileExistsError:
+        raise SystemExit(f"File {file_path.open} already exists")  # pragma: no cover
+    except IsADirectoryError:
+        raise SystemExit(
+            f"{file_path.open} is a directory not a file"
+        )  # pragma: no cover
+    except OSError:
+        raise SystemExit("General IO error has occurred")  # pragma: no cover
+    except Exception as e:
+        raise SystemExit("An error occurred:", str(e))  # pragma: no cover
+
+
+def _final_analysis(pattern: list[int]) -> None:
+    """Displays a rich console table displaying the conclusion of the test results
+
+    Args:
+        pattern:    A list of the test results:
+                    1 - A 'negative' result, indicating the project has been found.
+                    0 - A 'positive' result, indicating the project was not found.
+    """
+    table = Table(show_header=True)
+    table.add_column("FINAL ANALYSIS", style="bold cyan")
+    if pattern == [0, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "It can only be found by searching the simple index which is not available "
+            "through the interface"
+        )
+    elif pattern == [1, 1, 0]:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row(
+            "A Gotcha!, whereby the package is not found even with PyPI's own search"
+            " facility.\n"
+            "However if appears in the simple index and can be displayed by simply"
+            " browsing "
+            "to the projects URL"
+        )
+    elif sum(pattern) >= 1:
+        table.add_row("[red]NOT AVAILABLE![/red]\n")
+        table.add_row("The package name was found in at least one place")
+    elif sum(pattern) == 0:
+        table.add_row("[green]AVAILABLE![/green]\n")
+        table.add_row("The package name was not found in any part of PyPI")
+
+    console = Console()
+    console.print(table)
+
+
+def _parse_args(args: list) -> argparse.Namespace:
+    """Function to return the ArgumentParser object created from all the args.
+
+    Args:
+        args:   A list of arguments from the commandline
+                e.g. ['pynball', '-v', '-g']
+    """
+    parser = argparse.ArgumentParser(
+        prog="pynamer",
+        description="Determine if project name is available on pypi with the "
+        "option to 'register' it for future use if available",
+    )
+    parser.add_argument(
+        "projects",
+        nargs="*",
+        default="None",
+        help="Optional - one or more project names",
+    )
+    parser.add_argument(
+        "-r",
+        "--register",
+        action="store_true",
+        help="Register the name on PyPi if the name is available",
+    )
+    parser.add_argument(
+        "-d",
+        "--dryrun",
+        action="store_true",
+        help=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-f",
+        "--file",
+        default="None",
+        type=str,
+        help="File containing a list of projects to analyze",
+    )
+    parser.add_argument(
+        "-o",
+        "--output",
+        default="None",
+        type=str,
+        help="File to output the results to",
+    )
+    parser.add_argument(
+        "-n",
+        "--nocleanup",
+        action="store_true",
+        help=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="output additional information",
+    )
+    parser.add_argument(
+        "-g",
+        "--generate",
+        action="store_true",
+        help="Generate a new PyPI simple index",
+    )
+    return parser.parse_args(args)
+
+
+def main():  # pragma: no cover
+    args = _parse_args(sys.argv[1:])
+    logger.debug(" args: %s", args)
+
+    if args.generate is True:
+        _generate_pypi_index()
+
+    if args.projects == "None" and args.file == "None":
+        raise SystemExit("No projects to analyse. Use '--help' to display help")
+
+    project_list = []
+    test_results = []
+    aggregated_result = {}
+    _find_pypirc_file()
+    if args.nocleanup is True:
+        config.no_cleanup = True
+
+    # Gather the projects into one list
+    if args.projects != "None":
+        logger.debug("adding project names from command line %s", args.projects)
+        project_list.extend(list(set(args.projects)))
+        logger.debug("project_list = %s", project_list)
+    if args.file != "None":
+        logger.debug("adding project names from file %s", args.file)
+        project_list.extend(_process_input_file(args.file))
+        logger.debug("project_list = %s", project_list)
+    project_list.sort()
+
+    # Main loop
+    for new_project in project_list:
+        if not _is_valid_package_name(new_project):
+            _feedback(f"{new_project} is not a valid package name", "error")
+            continue
+
+        test_table = Table(title=f"Test Results for {new_project}", show_lines=True)
+        test_table.add_column("No.", style="bold yellow")
+        test_table.add_column("Test", style="bold cyan")
+        test_table.add_column("Result")
+        test_table.add_column("Details", style="bold cyan")
+
+        match_table = Table(title=f"PyPI Search: Exact Match {new_project}")
+        match_table.add_column("Package", style="bold yellow")
+        match_table.add_column("Version", style="bold green")
+        match_table.add_column("Released", style="bold yellow")
+        match_table.add_column("Description", style="bold cyan")
+
+        others_table = Table(
+            title="Other Close Matches or Related Projects (from page 1)"
+        )
+        others_table.add_column("Package", style="bold yellow")
+        others_table.add_column("Version", style="bold green")
+        others_table.add_column("Released", style="bold yellow")
+        others_table.add_column("Description", style="bold cyan")
+
+        # perform the tests
+        # Test 1
+        if _ping_project(new_project):
+            test_results.append(1)
+            json_data = _ping_json(new_project)
+            test_table.add_row(
+                "1", "Basic http get to project URL", "[red]FOUND[/red]", json_data
+            )
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "1", "Basic http get to project URL", "[green]NOT FOUND[/green]", ""
+            )
+
+        # Test 2
+        if _pypi_search_index(new_project):
+            test_results.append(1)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "[red]FOUND[/red]",
+                f"Searched {project_count} projects",
+            )
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "2",
+                "Check PyPI simple index",
+                "[green]NOT FOUND[/green]",
+                f"Searched {project_count} projects",
+            )
+
+        # Test 3
+        match, others, others_total = _pypi_search(new_project)
+        if match:
+            test_results.append(1)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "[red]FOUND[/red]",
+                f"Exact match found: {len(match)}, Others found: {others_total}",
+            )
+            for items in match:
+                match_table.add_row(items[0], items[1], items[2], items[3])
+        else:
+            test_results.append(0)
+            test_table.add_row(
+                "3",
+                "Check PyPI search",
+                "[green]NOT FOUND[/green]",
+                f"Exact match found: 0, Others found: {others_total}",
+            )
+
+        # Create Verbose Table
+        if others:
+            for items in others:
+                others_table.add_row(items[0], items[1], items[2], items[3])
+
+        # Display the Tables
+        console = Console()
+        console.print(test_table)
+        if match:
+            console.print(match_table)
+        if args.verbose and others:
+            console.print(others_table)
+        _final_analysis(test_results)
+
+        # build and upload
+        if (
+            test_results == [0, 0, 0]
+            and args.register is True
+            and config.pypirc is not None
+        ):
+            _rename_project_dir(
+                project_path.joinpath(config.original_project_name),
+                project_path.joinpath(new_project),
+            )
+            _create_setup(new_project)
+            _build_dist()
+            if args.dryrun is False:
+                _upload_dist(new_project)
+            else:
+                _feedback("Dryrun .... bypassing upload to PyPI..", "warning")
+            _cleanup(new_project)
+        elif config.pypirc is None:
+            _feedback(
+                ".pypirc file cannot be located ... wont attempt to 'register'",
+                "error",
+            )
+        elif sum(test_results) > 0 and args.register is True:
+            _feedback("Project already exists ... wont attempt to 'register'", "error")
+
+        aggregated_result[new_project] = test_results.copy()
+        test_results.clear()
+
+    if args.output != "None":
+        _write_output_file(args.output, aggregated_result)
+
+
+if __name__ == "__main__":
+    SystemExit(main())
```

### Comparing `pynamer-0.5.7/src/pynamer.egg-info/PKG-INFO` & `pynamer-1.0.0/src/pynamer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: pynamer
-Version: 0.5.7
+Version: 1.0.0
 Summary: Utility to find an available package name on the PyPI repository and register it
 Home-page: https://github.com/Stephen-RA-King/pynamer
 Download-URL: https://github.com/Stephen-RA-King/pynamer/archive/refs/heads/main.zip
 Author: Stephen R A King
 Author-email: sking.github@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: sking.github@gmail.com
 License: MIT
 Keywords: utility
 Platform: Any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
-# pynamer
-
 _**Utility to find an available package name on the PyPI repository and optionally 'register' it.**_
 
 [![PyPI][pypi-image]][pypi-url]
 [![Downloads][downloads-image]][downloads-url]
 [![Status][status-image]][pypi-url]
 [![Python Version][python-version-image]][pypi-url]
 [![Format][format-image]][pypi-url]
@@ -88,15 +86,15 @@
 
 pip leaps to the rescue with its search utility... or does it?
 
 ```python
 pip search zaphod
 ```
 
-```commandline
+```bash
 ERROR: XMLRPC request failed [code: -32500]
 RuntimeError: PyPI no longer supports 'pip search' (or XML-RPC search).
 Please use https://pypi.org/search (via a browser) instead.
 See https://warehouse.pypa.io/api-reference/xml-rpc.html#deprecated-methods for more information.
 ```
 
 A quick search will show the internet replete with articles explaining the situation:
@@ -112,16 +110,16 @@
 So, I go ahead and code my new project, along with all the test files, documentation and meta data.
 I diligently debug and commit and push to git and github so I have a history.
 
 Finally the project is good enough to release and publish as an installable package on PyPI.
 
 Here goes....
 
-```commandline
-python -m twine upload --config-file .pypirc dist/*
+```bash
+~ $ python -m twine upload --config-file .pypirc dist/*
 Uploading distributions to https://upload.pypi.org/legacy/
 Uploading zaphod-0.0.0-py3-none-any.whl
 100% ---------------------------------------- 3.8/3.8 kB • 00:00 • ?
 WARNING  Error during upload. Retry with the --verbose option for more details.
 ERROR    HTTPError: 403 Forbidden from https://upload.pypi.org/legacy/
          The user 'stephenking' isn't allowed to upload to project 'zaphod'. See https://pypi.org/help/#project-name for more information.
 ```
@@ -176,31 +174,31 @@
 repository = https://upload.pypi.org/legacy/
 username = __token__
 password = your_API_token_here
 ```
 
 ### Installation
 
-```sh
+```bash
 ~ $ pipx install pynamer
 ```
 
 ### Basic Usage
 
 #### A package name that is not available
 
-```commandline
+```bash
 ~ $ pynamer pynball
 ```
 
 ![](assets/usage_pynball.png)
 
 #### A package name that is available
 
-```commandline
+```bash
 ~ $ pynamer allitnil
 ```
 
 ![](assets/usage_available.png)
 
 Holy smoke batman! You've managed to identify a unique name.
 
@@ -212,19 +210,19 @@
 
 # Usage
 
 ---
 
 Display the help menu with the -h argument
 
-```commandline
+```bash
 ~ $ pynamer -h
 ```
 
-```commandline
+```bash
 usage: pynamer [-h] [-r] [-f FILE] [-o OUTPUT] [-v] [-g] [projects ...]
 
 Determine if project name is available on pypi with the option to 'register' it for future use if available
 
 positional arguments:
   projects              Optional - one or more project names
 
@@ -238,15 +236,15 @@
   -g, --generate        Generate a new PyPI simple index
 ```
 
 ## Specifying multiple names
 
 You can specify as many names as you like from the command line e.g.
 
-```commandline
+```bash
 ~ $ pynamer ganymede europa callisto
 ```
 
 ## Using an input file
 
 You can use the -f argument to specify a file containing the a names of projects to analyze.
 You specify a space separated sequence of as many names as you like on as many lines as you like. e.g.
@@ -256,29 +254,29 @@
 ```file
 ganymede europa
 IO callisto
 ```
 
 Then specify the -f argument
 
-```commandline
+```bash
 ~ $ pynamer -f projects
 ```
 
 You can use the input file with names from the command line. The names will be aggregated. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda metis -f projects
 ```
 
 ## Saving the results to a file
 
 You can specify a file to write the result to by using the -o argument. e.g.
 
-```commandline
+```bash
 ~ $ pynamer ersa pandia leda -o results
 ```
 
 This will write a file e.g.
 
 results
 
@@ -300,27 +298,27 @@
 
 ## Register the name with PyPI
 
 You can optionally 'register' the name on PyPI by using the -r argument.
 If the project name is found to be available and you have a valid 'pypirc' file is found, a minimalistic project will be built and uploaded to
 to PyPI.
 
-```commandline
+```bash
 ~ $ pynamer agrajag -r
 ```
 
 ![](assets/usage_register.png)
 
 ## Verbose output
 
 ith the -v argument you can display the first page of all other project matched by PyPIs search API - ordered by relevance.
 The algorithm that PyPI uses to select these in unknown but seems to be a mixture of names and other
 projects written by the same author.
 
-```commandline
+```bash
 ~ $ pynamer pynamer -v
 ```
 
 ![](assets/usage_verbose.png)
 
 ## Regenerate the PyPI simple Repository Index
 
@@ -332,58 +330,78 @@
 
 The PyPI Simple Index is used by a variety of tools and libraries to download and install packages from PyPI. For example, the pip package manager, which is used to install and manage Python packages, uses the PyPI Simple Index to find packages.
 
 The PyPI Simple Index is updated every few hours
 
 Using the -r argument can be used to regenerate the local file contents.
 
-```commandline
+```bash
 ~ $ pynamer -g
 ```
 
 ![](assets/usage_generate.png)
 
 See planned future improvements
 
 ## The Oddities
 
 The reason I wrote this application in the first place.
 
-```commandline
+```bash
 ~ $ pynamer zaphod
 ```
 
 ![](assets/usage_zaphod.png)
 
 Even worse ...
 
-```commandline
+```bash
 ~ $ pynamer zem
 ```
 
 ![](assets/usage_zem.png)
 
-## Planned Future improvements
+## Limitations
 
--   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
--   Filter out invalid PyPI package names at the start
+There will be occasions where all the tests pass, the name appears to be available but the upload to PyPI still fails.
+This can be several reasons for this:
+
+-   You are trying to use an internally "reserved" keyword for PyPI.
+-   The name you are using is too similar to an existing project name and you get the following error message:
+
+```bash
+...
+Error during upload. Retry with the --verbose option for more details.
+HTTPError: 400 Bad Request from https://test.pypi.org/legacy/
+The name 'yourpackage' is too similar to an existing project. See https://test.pypi.org/help/#project-name for more information-
+```
+
+Using a name similar to to an existing package name is a security issue.
+
+Malicious players will try to create project names that are frequently mistyped for large popular projects, thereby facilitating installation of a malicious project.
+e.g. replacing "L" / "l" with the number 1 or "o" / "O" with 0. The Software utilized by PyPI can be found at GitHub: [warehouse](https://github.com/pypi/warehouse).
 
 ## Documentation
 
 ---
 
 [**Read the Docs**](https://pynamer.readthedocs.io/en/latest/)
 
 -   [**Example Usage**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Credits**](https://pynamer.readthedocs.io/en/latest/example.html)
 -   [**Changelog**](https://pynamer.readthedocs.io/en/latest/changelog.html)
 -   [**API Reference**](https://pynamer.readthedocs.io/en/latest/autoapi/index.html)
 
 [**Wiki**](https://github.com/Stephen-RA-King/pynamer/wiki)
 
+## Planned Future improvements
+
+-   Improve performance of the regeneration of the PyPI simple Repository Index, so this can be run in the background automatically.
+-   Filter out invalid PyPI package names at the start
+
 ## Meta
 
 ---
 
 [![](assets/linkedin.png)](https://www.linkedin.com/in/sr-king)
 [![](assets/github.png)](https://github.com/Stephen-RA-King)
 [![](assets/pypi.png)](https://pypi.org/project/pynamer)
@@ -424,15 +442,15 @@
 [isort-image]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
 [isort-url]: https://github.com/pycqa/isort/
 [lgtm-alerts-image]: https://img.shields.io/lgtm/alerts/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-alerts-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/alerts/
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynamer.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynamer/context:python
 [license-image]: https://img.shields.io/pypi/l/pynamer
-[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/license
+[license-url]: https://github.com/Stephen-RA-King/pynamer/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynamer/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynamer/main
 [pypi-url]: https://pypi.org/project/pynamer/
```

### Comparing `pynamer-0.5.7/src/pynamer.egg-info/SOURCES.txt` & `pynamer-1.0.0/src/pynamer.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 src/pynamer/README.md
 src/pynamer/__init__.py
+src/pynamer/project_count.pickle
 src/pynamer/pynamer.py
 src/pynamer/setup.txt
 src/pynamer.egg-info/PKG-INFO
 src/pynamer.egg-info/SOURCES.txt
 src/pynamer.egg-info/dependency_links.txt
 src/pynamer.egg-info/entry_points.txt
 src/pynamer.egg-info/requires.txt
 src/pynamer.egg-info/top_level.txt
 src/pynamer/project_name/__init__.py
+tests/test_args.py
 tests/test_build_dist.py
 tests/test_cleanup.py
 tests/test_create_setup_file.py
 tests/test_defaults.py
 tests/test_delete_director.py
 tests/test_feedback.py
 tests/test_final_analysis.py
 tests/test_find_pypirc_file.py
 tests/test_generate_pypi_index.py
+tests/test_is_valid_package_name.py
 tests/test_main TBC.py
 tests/test_ping_json.py
 tests/test_ping_project.py
 tests/test_process_input_file.py
 tests/test_pypi_search.py
 tests/test_pypi_search_index.py
 tests/test_rename_project_dir.py
 tests/test_run_command TBD.py
-tests/test_upload_dist TBD.py
+tests/test_upload_dist.py
 tests/test_write_output_file.py
```

### Comparing `pynamer-0.5.7/tests/test_build_dist.py` & `pynamer-1.0.0/tests/test_build_dist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-import shutil
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-setup_text = """#!/usr/bin/env python3
-
-# Third party modules
-from setuptools import setup
-
-setup(name='pynamer',
-      version='0.0.0',
-      description='place holder',
-      url='http://github.com/SK/pynamer',
-      author='sking',
-      author_email='flyingcircus@example.com',
-      license='MIT',
-      packages=['pynamer'],
-      zip_safe=False)"""
-
-
-@pytest.fixture()
-def pre_build_dist(monkeypatch):
-    project_dir = BASE_DIR / "pynamer"
-    project_dir.mkdir()
-    project_init_file = BASE_DIR / "pynamer" / "__init__.py"
-    project_init_file.touch()
-    pypirc_file = BASE_DIR / ".pypirc"
-    pypirc_file.touch()
-    setup_py = BASE_DIR / "setup.py"
-    setup_py.touch()
-    setup_py.write_text(setup_text)
-    readme_file = BASE_DIR / "README.md"
-    readme_file.touch()
-    readme_file.write_text("pynamer")
-    build = BASE_DIR / "build"
-    dist = BASE_DIR / "dist"
-    egg = BASE_DIR / "pynamer.egg-info"
-
-    yield
-
-    manifest = [
-        project_dir,
-        pypirc_file,
-        setup_py,
-        readme_file,
-        build,
-        dist,
-        egg,
-    ]
-    for item in manifest:
-        if item.exists():
-            if item.is_dir():
-                shutil.rmtree(item)
-            elif item.is_file():
-                item.unlink()
-
-
-def test_build_dist(pre_build_dist, project_path_mock):
-    pynamer._build_dist()
-    assert (BASE_DIR / "build").exists()
-    assert (BASE_DIR / "dist").exists()
-    assert (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
-    assert (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
-    assert (BASE_DIR / "pynamer.egg-info").exists()
+#!/usr/bin/env python3
+# Core Library modules
+import shutil
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+setup_text = """#!/usr/bin/env python3
+
+# Third party modules
+from setuptools import setup
+
+setup(name='pynamer',
+      version='0.0.0',
+      description='place holder',
+      url='http://github.com/SK/pynamer',
+      author='sking',
+      author_email='flyingcircus@example.com',
+      license='MIT',
+      packages=['pynamer'],
+      zip_safe=False)"""
+
+
+@pytest.fixture()
+def pre_build_dist(monkeypatch):
+    project_dir = BASE_DIR / "pynamer"
+    project_dir.mkdir()
+    project_init_file = BASE_DIR / "pynamer" / "__init__.py"
+    project_init_file.touch()
+    pypirc_file = BASE_DIR / ".pypirc"
+    pypirc_file.touch()
+    setup_py = BASE_DIR / "setup.py"
+    setup_py.touch()
+    setup_py.write_text(setup_text)
+    readme_file = BASE_DIR / "README.md"
+    readme_file.touch()
+    readme_file.write_text("pynamer")
+    build = BASE_DIR / "build"
+    dist = BASE_DIR / "dist"
+    egg = BASE_DIR / "pynamer.egg-info"
+
+    yield
+
+    manifest = [
+        project_dir,
+        pypirc_file,
+        setup_py,
+        readme_file,
+        build,
+        dist,
+        egg,
+    ]
+    for item in manifest:
+        if item.exists():
+            if item.is_dir():
+                shutil.rmtree(item)
+            elif item.is_file():
+                item.unlink()
+
+
+@pytest.mark.slow
+def test_build_dist(pre_build_dist, project_path_mock):
+    pynamer._build_dist()
+    assert (BASE_DIR / "build").exists()
+    assert (BASE_DIR / "dist").exists()
+    assert (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
+    assert (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
+    assert (BASE_DIR / "pynamer.egg-info").exists()
```

### Comparing `pynamer-0.5.7/tests/test_cleanup.py` & `pynamer-1.0.0/tests/test_cleanup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-#!/usr/bin/env python3
-# Core Library modules
-import pickle
-import shutil
-from pathlib import Path
-
-# Third party modules
-import pytest
-import requests
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-@pytest.fixture()
-def pre_build_cleanup(monkeypatch):
-    project_dir = BASE_DIR / "pynamer"
-    project_dir.mkdir()
-    build_dir = BASE_DIR / "build"
-    build_dir.mkdir()
-    dist_dir = BASE_DIR / "dist"
-    dist_dir.mkdir()
-    egg_dir = BASE_DIR / "pynamer.egg-info"
-    egg_dir.mkdir()
-    setup_py = BASE_DIR / "setup.py"
-    setup_py.touch()
-
-    yield
-
-    if (BASE_DIR / "project_name").exists():
-        shutil.rmtree(BASE_DIR / "project_name")
-
-
-def test_cleanup(pre_build_cleanup, project_path_mock):
-    pynamer._cleanup("pynamer")
-    assert not (BASE_DIR / "build").exists()
-    assert not (BASE_DIR / "dist").exists()
-    assert not (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
-    assert not (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
-    assert not (BASE_DIR / "pynamer.egg-info").exists()
+#!/usr/bin/env python3
+# Core Library modules
+import shutil
+from pathlib import Path
+
+# Third party modules
+import pytest
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+@pytest.fixture()
+def pre_cleanup(monkeypatch):
+    project_dir = BASE_DIR / "pynamer"
+    project_dir.mkdir()
+    build_dir = BASE_DIR / "build"
+    build_dir.mkdir()
+    dist_dir = BASE_DIR / "dist"
+    dist_dir.mkdir()
+    egg_dir = BASE_DIR / "pynamer.egg-info"
+    egg_dir.mkdir()
+    setup_py = BASE_DIR / "setup.py"
+    setup_py.touch()
+
+    yield
+
+    if (BASE_DIR / "project_name").exists():
+        shutil.rmtree(BASE_DIR / "project_name")
+
+
+def test_cleanup(pre_cleanup, project_path_mock):
+    pynamer._cleanup("pynamer")
+    assert not (BASE_DIR / "build").exists()
+    assert not (BASE_DIR / "dist").exists()
+    assert not (BASE_DIR / "dist" / "pynamer-0.0.0.tar.gz").exists()
+    assert not (BASE_DIR / "dist" / "pynamer-0.0.0-py3-none-any.whl").exists()
+    assert not (BASE_DIR / "pynamer.egg-info").exists()
```

### Comparing `pynamer-0.5.7/tests/test_create_setup_file.py` & `pynamer-1.0.0/tests/test_create_setup_file.py`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.7/tests/test_defaults.py` & `pynamer-1.0.0/tests/test_defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 #!/usr/bin/env python3
 # Core Library modules
-import pickle
 import platform
 from pathlib import Path
 
-# Third party modules
-import pytest
-
 # First party modules
 from pynamer import pynamer
 
-operating_system = platform.system()
+OS = platform.system()
 BASE_DIR = Path(__file__).parents[0]
 
 
 def test_project_path():
-    if operating_system == "Windows":
+    if OS == "Windows":
         assert str(pynamer.project_path).endswith("pynamer\\src\\pynamer")
     else:
         assert str(pynamer.project_path).endswith("pynamer/src/pynamer")
 
 
 def test_project_count(project_path_mock):
-    assert pynamer.project_count == 452490
+    assert pynamer.project_count >= 452490
 
 
 def test_setup_text():
     assert (
         pynamer.setup_text
         == """#!/usr/bin/env python3
```

### Comparing `pynamer-0.5.7/tests/test_feedback.py` & `pynamer-1.0.0/tests/test_feedback.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-#!/usr/bin/env python3
-# Core Library modules
-
-# Third party modules
-import pytest
-from colorama import Back, Fore, Style
-
-# First party modules
-from pynamer import pynamer
-
-
-@pytest.mark.parametrize(
-    "message, message_type, result",
-    [
-        ("null", "null", f"{Fore.WHITE}{Style.BRIGHT}null{Style.RESET_ALL}\n"),
-        ("nominal", "nominal", f"{Fore.GREEN}{Style.BRIGHT}nominal{Style.RESET_ALL}\n"),
-        (
-            "warning",
-            "warning",
-            f"{Fore.YELLOW}{Back.BLACK}{Style.BRIGHT}warning{Style.RESET_ALL}\n",
-        ),
-        (
-            "error",
-            "error",
-            f"{Fore.RED}{Back.BLACK}{Style.BRIGHT}error{Style.RESET_ALL}\n",
-        ),
-        ("error", "critical", ""),
-    ],
-)
-def test_feedback(message, message_type, result, capfd):
-    """Pytest test to assert mark parametrize pytest feature."""
-    pynamer._feedback(message, message_type)
-    captured = capfd.readouterr()
-    assert captured.out == result
-
-
-def test_idlemode(capfd):
-    assert pynamer.config.idlemode == 0
-    pynamer.config.idlemode = 1
-    pynamer._feedback("warning", "warning")
-    captured = capfd.readouterr()
-    assert captured.out == "warning\n"
-    pynamer.config.idlemode = 0
+#!/usr/bin/env python3
+# Core Library modules
+
+# Third party modules
+import pytest
+from colorama import Back, Fore, Style
+
+# First party modules
+from pynamer import pynamer
+
+
+@pytest.mark.parametrize(
+    "message, message_type, result",
+    [
+        ("null", "null", f"{Fore.WHITE}{Style.BRIGHT}null{Style.RESET_ALL}\n"),
+        ("nominal", "nominal", f"{Fore.GREEN}{Style.BRIGHT}nominal{Style.RESET_ALL}\n"),
+        (
+            "warning",
+            "warning",
+            f"{Fore.YELLOW}{Back.BLACK}{Style.BRIGHT}warning{Style.RESET_ALL}\n",
+        ),
+        (
+            "error",
+            "error",
+            f"{Fore.RED}{Back.BLACK}{Style.BRIGHT}error{Style.RESET_ALL}\n",
+        ),
+        ("error", "critical", ""),
+    ],
+)
+def test_feedback(message, message_type, result, capfd):
+    """Pytest test to assert mark parametrize pytest feature."""
+    pynamer._feedback(message, message_type)
+    captured = capfd.readouterr()
+    assert captured.out == result
+
+
+def test_feedback_idlemode(capfd):
+    assert pynamer.config.idlemode == 0
+    pynamer.config.idlemode = 1
+    pynamer._feedback("warning", "warning")
+    captured = capfd.readouterr()
+    assert captured.out == "warning\n"
+    pynamer.config.idlemode = 0
```

### Comparing `pynamer-0.5.7/tests/test_final_analysis.py` & `pynamer-1.0.0/tests/test_final_analysis.py`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.7/tests/test_rename_project_dir.py` & `pynamer-1.0.0/tests/test_rename_project_dir.py`

 * *Files identical despite different names*

### Comparing `pynamer-0.5.7/tests/test_write_output_file.py` & `pynamer-1.0.0/tests/test_write_output_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#!/usr/bin/env python3
-# Core Library modules
-from pathlib import Path
-
-# First party modules
-from pynamer import pynamer
-
-BASE_DIR = Path(__file__).parents[0]
-
-
-def test_pypi_search_index(monkeypatch):
-    expected_results_file = BASE_DIR / "resources" / "output_file"
-    output_file = BASE_DIR / "output_file"
-    result_dict = {"pyball": [1, 1, 1]}
-    pynamer._write_output_file(str(output_file), result_dict)
-
-    with open(expected_results_file) as f:
-        expected_text = f.read()
-    with open(output_file) as f:
-        result_text = f.read()
-
-    assert result_text == expected_text
-
-    output_file.unlink()
+#!/usr/bin/env python3
+# Core Library modules
+from pathlib import Path
+
+# First party modules
+from pynamer import pynamer
+
+BASE_DIR = Path(__file__).parents[0]
+
+
+def test_write_output_file(monkeypatch):
+    expected_results_file = BASE_DIR / "resources" / "output_file"
+    output_file = BASE_DIR / "output_file"
+    result_dict = {"pyball": [1, 1, 1]}
+    pynamer._write_output_file(str(output_file), result_dict)
+
+    with open(expected_results_file) as f:
+        expected_text = f.read()
+    with open(output_file) as f:
+        result_text = f.read()
+
+    assert result_text == expected_text
+
+    output_file.unlink()
```

