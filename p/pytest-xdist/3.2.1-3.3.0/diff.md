# Comparing `tmp/pytest-xdist-3.2.1.tar.gz` & `tmp/pytest-xdist-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-xdist-3.2.1.tar", last modified: Sun Mar 12 15:09:27 2023, max compression
+gzip compressed data, was "pytest-xdist-3.3.0.tar", last modified: Fri May 12 20:41:30 2023, max compression
```

## Comparing `pytest-xdist-3.2.1.tar` & `pytest-xdist-3.3.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.893345 pytest-xdist-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    32690 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-12 15:09:27.893345 pytest-xdist-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/changelog/_template.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/crash.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/distribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/how-it-works.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/how-to.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/known-limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/remote.rst
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/docs/subprocess.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/boxed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/example/loadscope/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/example/loadscope/epsilon/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/epsilon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.885345 pytest-xdist-3.2.1/example/loadscope/test/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/test/test_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/test/test_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/test/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/test/test_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/example/loadscope/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-12 15:09:27.893345 pytest-xdist-3.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.881345 pytest-xdist-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.889345 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/pytest_xdist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.889345 pytest-xdist-3.2.1/src/xdist/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-12 15:09:27.000000 pytest-xdist-3.2.1/src/xdist/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17367 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/dsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/looponfail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/newhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.889345 pytest-xdist-3.2.1/src/xdist/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/each.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/loadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/loadgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/loadscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/scheduler/worksteal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/src/xdist/workermanage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 15:09:27.893345 pytest-xdist-3.2.1/testing/
--rw-r--r--   0 runner    (1001) docker     (123)    51290 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/acceptance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_dsession.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_looponfail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_newhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/test_workermanage.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/testing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-12 15:09:12.000000 pytest-xdist-3.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    32910 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/changelog/_template.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/crash.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/how-it-works.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/how-to.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/known-limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/remote.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/docs/subprocess.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/boxed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/epsilon/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/epsilon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.262263 pytest-xdist-3.3.0/example/loadscope/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/test/test_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/example/loadscope/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.258262 pytest-xdist-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/pytest_xdist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/xdist/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-12 20:41:30.000000 pytest-xdist-3.3.0/src/xdist/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/dsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.266263 pytest-xdist-3.3.0/src/xdist/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/each.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14207 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/loadscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/scheduler/worksteal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/src/xdist/workermanage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:41:30.270263 pytest-xdist-3.3.0/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)    51523 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/acceptance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21498 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_dsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_looponfail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_newhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/test_workermanage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/testing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-12 20:41:10.000000 pytest-xdist-3.3.0/tox.ini
```

### Comparing `pytest-xdist-3.2.1/CHANGELOG.rst` & `pytest-xdist-3.3.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+pytest-xdist 3.3.0 (2023-05-12)
+===============================
+
+Features
+--------
+
+- `#555 <https://github.com/pytest-dev/pytest-xdist/issues/555>`_: Improved progress output when collecting nodes to be less verbose.
+
+
 pytest-xdist 3.2.1 (2023-03-12)
 ===============================
 
 Bug Fixes
 ---------
 
 - `#884 <https://github.com/pytest-dev/pytest-xdist/issues/884>`_: Fixed hang in ``worksteal`` scheduler.
```

### Comparing `pytest-xdist-3.2.1/LICENSE` & `pytest-xdist-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/PKG-INFO` & `pytest-xdist-3.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist
-Version: 3.2.1
+Version: 3.3.0
 Summary: pytest xdist plugin for distributed testing, most importantly across multiple CPUs
 Home-page: https://github.com/pytest-dev/pytest-xdist
 Author: holger krekel and contributors
 Author-email: pytest-dev@python.org,holger@merlinux.eu
 License: MIT
 Project-URL: Documentation, https://pytest-xdist.readthedocs.io/en/latest
 Project-URL: Changelog, https://pytest-xdist.readthedocs.io/en/latest/changelog.html
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: psutil
 Provides-Extra: setproctitle
 License-File: LICENSE
 
 ============
 pytest-xdist
```

### Comparing `pytest-xdist-3.2.1/README.rst` & `pytest-xdist-3.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/RELEASING.rst` & `pytest-xdist-3.3.0/RELEASING.rst`

 * *Files 13% similar despite different names*

```diff
@@ -28,18 +28,12 @@
 
     $ pip install tox
 
 #. Update the necessary files with::
 
     $ tox -e release -- X.Y.Z
 
-#. Commit and push the branch for review.
+#. Commit and push the branch to ``upstream`` and open a PR.
 
-#. Once PR is **green** and **approved**, create and push a tag::
+#. Once the PR is **green** and **approved**, start the ``deploy`` workflow manually from the branch ``release-VERSION``, passing ``VERSION`` as parameter.
 
-    $ export VERSION=X.Y.Z
-    $ git tag v$VERSION release-$VERSION
-    $ git push git@github.com:pytest-dev/pytest-xdist.git v$VERSION
-
-That will build the package and publish it on ``PyPI`` automatically.
-
-#. Merge the release PR to `master`.
+#. Merge the release PR to ``master``.
```

### Comparing `pytest-xdist-3.2.1/changelog/_template.rst` & `pytest-xdist-3.3.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/conf.py` & `pytest-xdist-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/distribution.rst` & `pytest-xdist-3.3.0/docs/distribution.rst`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
   when crashed (set to zero to disable this feature).
 
 The test distribution algorithm is configured with the ``--dist`` command-line option:
 
 .. _distribution modes:
 
 * ``--dist load`` **(default)**: Sends pending tests to any worker that is
-  available, without any guaranteed order.
+  available, without any guaranteed order. Scheduling can be fine-tuned with
+  the `--maxschedchunk` option, see output of `pytest --help`.
 
 * ``--dist loadscope``: Tests are grouped by **module** for *test functions*
   and by **class** for *test methods*. Groups are distributed to available
   workers as whole units. This guarantees that all tests in a group run in the
   same process. This can be useful if you have expensive module-level or
   class-level fixtures. Grouping by class takes priority over grouping by
   module.
```

### Comparing `pytest-xdist-3.2.1/docs/how-it-works.rst` & `pytest-xdist-3.3.0/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/how-to.rst` & `pytest-xdist-3.3.0/docs/how-to.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/index.rst` & `pytest-xdist-3.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/known-limitations.rst` & `pytest-xdist-3.3.0/docs/known-limitations.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/remote.rst` & `pytest-xdist-3.3.0/docs/remote.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/docs/subprocess.rst` & `pytest-xdist-3.3.0/docs/subprocess.rst`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/example/boxed.txt` & `pytest-xdist-3.3.0/example/boxed.txt`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/example/loadscope/test/test_alpha.py` & `pytest-xdist-3.3.0/example/loadscope/test/test_alpha.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/example/loadscope/test/test_beta.py` & `pytest-xdist-3.3.0/example/loadscope/test/test_beta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/example/loadscope/test/test_delta.py` & `pytest-xdist-3.3.0/example/loadscope/test/test_delta.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/example/loadscope/test/test_gamma.py` & `pytest-xdist-3.3.0/example/loadscope/test/test_gamma.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/pyproject.toml` & `pytest-xdist-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/setup.cfg` & `pytest-xdist-3.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [metadata]
 name = pytest-xdist
 description = pytest xdist plugin for distributed testing, most importantly across multiple CPUs
 long_description = file: README.rst
+long_description_content_type = text/x-rst
 license = MIT
 author = holger krekel and contributors
 author_email = pytest-dev@python.org,holger@merlinux.eu
 url = https://github.com/pytest-dev/pytest-xdist
 platforms = 
 	linux
 	osx
```

### Comparing `pytest-xdist-3.2.1/src/pytest_xdist.egg-info/PKG-INFO` & `pytest-xdist-3.3.0/src/pytest_xdist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xdist
-Version: 3.2.1
+Version: 3.3.0
 Summary: pytest xdist plugin for distributed testing, most importantly across multiple CPUs
 Home-page: https://github.com/pytest-dev/pytest-xdist
 Author: holger krekel and contributors
 Author-email: pytest-dev@python.org,holger@merlinux.eu
 License: MIT
 Project-URL: Documentation, https://pytest-xdist.readthedocs.io/en/latest
 Project-URL: Changelog, https://pytest-xdist.readthedocs.io/en/latest/changelog.html
@@ -28,14 +28,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 Provides-Extra: testing
 Provides-Extra: psutil
 Provides-Extra: setproctitle
 License-File: LICENSE
 
 ============
 pytest-xdist
```

### Comparing `pytest-xdist-3.2.1/src/pytest_xdist.egg-info/SOURCES.txt` & `pytest-xdist-3.3.0/src/pytest_xdist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/_path.py` & `pytest-xdist-3.3.0/src/xdist/_path.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/dsession.py` & `pytest-xdist-3.3.0/src/xdist/dsession.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from __future__ import annotations
+import sys
+from enum import Enum, auto
+from typing import Sequence
+
 import pytest
 
 from xdist.remote import Producer
 from xdist.workermanage import NodeManager
 from xdist.scheduler import (
     EachScheduling,
     LoadScheduling,
@@ -247,22 +252,24 @@
             return
         self.config.hook.pytest_xdist_node_collection_finished(node=node, ids=ids)
         # tell session which items were effectively collected otherwise
         # the controller node will finish the session with EXIT_NOTESTSCOLLECTED
         self._session.testscollected = len(ids)
         self.sched.add_node_collection(node, ids)
         if self.terminal:
-            self.trdist.setstatus(node.gateway.spec, "[%d]" % (len(ids)))
+            self.trdist.setstatus(
+                node.gateway.spec, WorkerStatus.CollectionDone, tests_collected=len(ids)
+            )
         if self.sched.collection_is_completed:
             if self.terminal and not self.sched.has_pending:
                 self.trdist.ensure_show_status()
                 self.terminal.write_line("")
                 if self.config.option.verbose > 0:
                     self.terminal.write_line(
-                        "scheduling tests via %s" % (self.sched.__class__.__name__)
+                        f"scheduling tests via {self.sched.__class__.__name__}"
                     )
             self.sched.schedule()
 
     def worker_logstart(self, node, nodeid, location):
         """Emitted when a node calls the pytest_runtest_logstart hook."""
         self.config.hook.pytest_runtest_logstart(nodeid=nodeid, location=location)
 
@@ -341,15 +348,15 @@
             self.config.hook.pytest_collectreport(report=rep)
             self._handlefailures(rep)
 
     def _handlefailures(self, rep):
         if rep.failed:
             self.countfailures += 1
             if self.maxfail and self.countfailures >= self.maxfail:
-                self.shouldstop = "stopping after %d failures" % (self.countfailures)
+                self.shouldstop = f"stopping after {self.countfailures} failures"
 
     def triggershutdown(self):
         self.log("triggering shutdown")
         self.shuttingdown = True
         for node in self.sched.nodes:
             node.shutdown()
 
@@ -368,82 +375,105 @@
             crashitem=nodeid,
             report=rep,
             sched=self.sched,
         )
         self.config.hook.pytest_runtest_logreport(report=rep)
 
 
+class WorkerStatus(Enum):
+    """Status of each worker during creation/collection."""
+
+    # Worker spec has just been created.
+    Created = auto()
+
+    # Worker has been initialized.
+    Initialized = auto()
+
+    # Worker is now ready for collection.
+    ReadyForCollection = auto()
+
+    # Worker has finished collection.
+    CollectionDone = auto()
+
+
 class TerminalDistReporter:
-    def __init__(self, config):
+    def __init__(self, config) -> None:
         self.config = config
         self.tr = config.pluginmanager.getplugin("terminalreporter")
-        self._status = {}
+        self._status: dict[str, tuple[WorkerStatus, int]] = {}
         self._lastlen = 0
         self._isatty = getattr(self.tr, "isatty", self.tr.hasmarkup)
 
-    def write_line(self, msg):
+    def write_line(self, msg: str) -> None:
         self.tr.write_line(msg)
 
-    def ensure_show_status(self):
+    def ensure_show_status(self) -> None:
         if not self._isatty:
             self.write_line(self.getstatus())
 
-    def setstatus(self, spec, status, show=True):
-        self._status[spec.id] = status
+    def setstatus(
+        self, spec, status: WorkerStatus, *, tests_collected: int, show: bool = True
+    ) -> None:
+        self._status[spec.id] = (status, tests_collected)
         if show and self._isatty:
             self.rewrite(self.getstatus())
 
-    def getstatus(self):
+    def getstatus(self) -> str:
         if self.config.option.verbose >= 0:
-            parts = [f"{spec.id} {self._status[spec.id]}" for spec in self._specs]
-            return " / ".join(parts)
-        else:
-            return "bringing up nodes..."
+            line = get_workers_status_line(list(self._status.values()))
+            if line:
+                return line
+
+        return "bringing up nodes..."
 
     def rewrite(self, line, newline=False):
         pline = line + " " * max(self._lastlen - len(line), 0)
         if newline:
             self._lastlen = 0
             pline += "\n"
         else:
             self._lastlen = len(line)
         self.tr.rewrite(pline, bold=True)
 
     @pytest.hookimpl
-    def pytest_xdist_setupnodes(self, specs):
+    def pytest_xdist_setupnodes(self, specs) -> None:
         self._specs = specs
         for spec in specs:
-            self.setstatus(spec, "I", show=False)
-        self.setstatus(spec, "I", show=True)
+            self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=False)
+        self.setstatus(spec, WorkerStatus.Created, tests_collected=0, show=True)
         self.ensure_show_status()
 
     @pytest.hookimpl
-    def pytest_xdist_newgateway(self, gateway):
-        if self.config.option.verbose > 0:
-            rinfo = gateway._rinfo()
+    def pytest_xdist_newgateway(self, gateway) -> None:
+        rinfo = gateway._rinfo()
+        is_local = rinfo.executable == sys.executable
+        if self.config.option.verbose > 0 and not is_local:
             version = "%s.%s.%s" % rinfo.version_info[:3]
             self.rewrite(
                 "[%s] %s Python %s cwd: %s"
                 % (gateway.id, rinfo.platform, version, rinfo.cwd),
                 newline=True,
             )
-        self.setstatus(gateway.spec, "C")
+        self.setstatus(gateway.spec, WorkerStatus.Initialized, tests_collected=0)
 
     @pytest.hookimpl
-    def pytest_testnodeready(self, node):
-        if self.config.option.verbose > 0:
-            d = node.workerinfo
+    def pytest_testnodeready(self, node) -> None:
+        d = node.workerinfo
+        is_local = d.get("executable") == sys.executable
+        if self.config.option.verbose > 0 and not is_local:
             infoline = "[{}] Python {}".format(
                 d["id"], d["version"].replace("\n", " -- ")
             )
             self.rewrite(infoline, newline=True)
-        self.setstatus(node.gateway.spec, "ok")
+        self.setstatus(
+            node.gateway.spec, WorkerStatus.ReadyForCollection, tests_collected=0
+        )
 
     @pytest.hookimpl
-    def pytest_testnodedown(self, node, error):
+    def pytest_testnodedown(self, node, error) -> None:
         if not error:
             return
         self.write_line(f"[{node.gateway.id}] node down: {error}")
 
 
 def get_default_max_worker_restart(config):
     """gets the default value of --max-worker-restart option if it is not provided.
@@ -453,7 +483,40 @@
     result = config.option.maxworkerrestart
     if result is not None:
         result = int(result)
     elif config.option.numprocesses:
         # if --max-worker-restart was not provided, use a reasonable default (#226)
         result = config.option.numprocesses * 4
     return result
+
+
+def get_workers_status_line(
+    status_and_items: Sequence[tuple[WorkerStatus, int]]
+) -> str:
+    """
+    Return the line to display during worker setup/collection based on the
+    status of the workers and number of tests collected for each.
+    """
+    statuses = [s for s, c in status_and_items]
+    total_workers = len(statuses)
+    workers_noun = "worker" if total_workers == 1 else "workers"
+    if status_and_items and all(s == WorkerStatus.CollectionDone for s in statuses):
+        # All workers collect the same number of items, so we grab
+        # the total number of items from the first worker.
+        first = status_and_items[0]
+        status, tests_collected = first
+        tests_noun = "item" if tests_collected == 1 else "items"
+        return f"{total_workers} {workers_noun} [{tests_collected} {tests_noun}]"
+    if WorkerStatus.CollectionDone in statuses:
+        done = sum(1 for s, c in status_and_items if c > 0)
+        return f"collecting: {done}/{total_workers} {workers_noun}"
+    if WorkerStatus.ReadyForCollection in statuses:
+        ready = statuses.count(WorkerStatus.ReadyForCollection)
+        return f"ready: {ready}/{total_workers} {workers_noun}"
+    if WorkerStatus.Initialized in statuses:
+        initialized = statuses.count(WorkerStatus.Initialized)
+        return f"initialized: {initialized}/{total_workers} {workers_noun}"
+    if WorkerStatus.Created in statuses:
+        created = statuses.count(WorkerStatus.Created)
+        return f"created: {created}/{total_workers} {workers_noun}"
+
+    return ""
```

### Comparing `pytest-xdist-3.2.1/src/xdist/looponfail.py` & `pytest-xdist-3.3.0/src/xdist/looponfail.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/newhooks.py` & `pytest-xdist-3.3.0/src/xdist/newhooks.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/plugin.py` & `pytest-xdist-3.3.0/src/xdist/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
         type=int,
         help=(
             "Maximum number of tests scheduled in one step for --dist=load. "
             "Setting it to 1 will force pytest to send tests to workers one by "
             "one - might be useful for a small number of slow tests. "
             "Larger numbers will allow the scheduler to submit consecutive "
             "chunks of tests to workers - allows reusing fixtures. "
+            "Due to implementation reasons, at least 2 tests are scheduled per "
+            "worker at the start. Only later tests can be scheduled one by one. "
             "Unlimited if not set."
         ),
     )
 
     parser.addini(
         "rsyncdirs",
         "list of (relative) paths to be rsynced for remote distributed testing.",
```

### Comparing `pytest-xdist-3.2.1/src/xdist/remote.py` & `pytest-xdist-3.3.0/src/xdist/remote.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/report.py` & `pytest-xdist-3.3.0/src/xdist/report.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/each.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/each.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/load.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/load.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/loadfile.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/loadfile.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/loadgroup.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/loadgroup.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/loadscope.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/loadscope.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/scheduler/worksteal.py` & `pytest-xdist-3.3.0/src/xdist/scheduler/worksteal.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/src/xdist/workermanage.py` & `pytest-xdist-3.3.0/src/xdist/workermanage.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/acceptance_test.py` & `pytest-xdist-3.3.0/testing/acceptance_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,20 @@
                 def test_ok():
                     pass
                 def test_skip():
                     pytest.skip("hello")
             """
         )
         result = pytester.runpytest(p1, "-v", "-d", "--tx=popen", "--tx=popen")
-        result.stdout.fnmatch_lines(["*1*Python*", "*2 failed, 1 passed, 1 skipped*"])
+        result.stdout.fnmatch_lines(
+            [
+                "created: 2/2 workers",
+                "*2 failed, 1 passed, 1 skipped*",
+            ]
+        )
         assert result.ret == 1
 
     def test_n1_fail_minus_x(self, pytester: pytest.Pytester) -> None:
         p1 = pytester.makepyfile(
             """
             def test_fail1():
                 assert 0
@@ -147,15 +152,20 @@
         pytester.makeini(
             """
             [pytest]
             addopts = --tx=3*popen
         """
         )
         result = pytester.runpytest(p1, "-d", "-v")
-        result.stdout.fnmatch_lines(["*2*Python*", "*2 failed, 1 passed, 1 skipped*"])
+        result.stdout.fnmatch_lines(
+            [
+                "created: 3/3 workers",
+                "*2 failed, 1 passed, 1 skipped*",
+            ]
+        )
         assert result.ret == 1
 
     def test_dist_tests_with_crash(self, pytester: pytest.Pytester) -> None:
         if not hasattr(os, "kill"):
             pytest.skip("no os.kill")
 
         p1 = pytester.makepyfile(
@@ -233,17 +243,14 @@
             "--rsyncdir=%(subdir)s" % locals(),
             "--tx=popen//chdir=%(dest)s" % locals(),
             p,
         )
         assert result.ret == 0
         result.stdout.fnmatch_lines(
             [
-                "*0* *cwd*",
-                # "RSyncStart: [G1]",
-                # "RSyncFinished: [G1]",
                 "*1 passed*",
             ]
         )
         result.stderr.fnmatch_lines(["--foobar=123 active! *"])
         assert dest.joinpath(subdir.name).is_dir()
 
     def test_data_exchange(self, pytester: pytest.Pytester) -> None:
@@ -272,15 +279,19 @@
                     terminalreporter._tw.sep('-',
                         'calculated result is %s' % calc_result)
         """
         )
         p1 = pytester.makepyfile("def test_func(): pass")
         result = pytester.runpytest("-v", p1, "-d", "--tx=popen")
         result.stdout.fnmatch_lines(
-            ["*0*Python*", "*calculated result is 49*", "*1 passed*"]
+            [
+                "created: 1/1 worker",
+                "*calculated result is 49*",
+                "*1 passed*",
+            ]
         )
         assert result.ret == 0
 
     def test_keyboardinterrupt_hooks_issue79(self, pytester: pytest.Pytester) -> None:
         pytester.makepyfile(
             __init__="",
             test_one="""
@@ -389,22 +400,22 @@
         args = ["-n1"]
         if verbosity:
             args.append(verbosity)
         result = pytester.runpytest(*args)
         out = result.stdout.str()
         if verbosity == "-v":
             assert "scheduling tests" in out
-            assert "gw" in out
+            assert "1 worker [1 item]" in out
         elif verbosity == "-q":
             assert "scheduling tests" not in out
             assert "gw" not in out
             assert "bringing up nodes..." in out
         else:
             assert "scheduling tests" not in out
-            assert "gw" in out
+            assert "1 worker [1 item]" in out
 
     def test_pass_skip_fail(self, pytester: pytest.Pytester) -> None:
         pytester.makepyfile(
             """
             import pytest
             def test_ok():
                 pass
@@ -1095,16 +1106,17 @@
             assert 1
     """
     )
     args = ["--color=yes", "-n2"]
     result = pytester.runpytest(*args)
     assert "test session starts" in result.stdout.str()
     assert "\x1b[1m" in result.stdout.str()
-    assert "gw0 [10] / gw1 [10]" in result.stdout.str()
-    assert "gw0 C / gw1 C" not in result.stdout.str()
+    assert "created: 2/2 workers" in result.stdout.str()
+    assert "2 workers [10 items]" in result.stdout.str()
+    assert "collecting:" not in result.stdout.str()
 
 
 def test_without_terminal_plugin(pytester, request) -> None:
     """
     No output when terminal plugin is disabled
     """
     pytester.makepyfile(
@@ -1550,16 +1562,16 @@
         assert 0
     """
     )
     result = testdir.runpytest(p1, "-n1")
     assert result.ret == 1
     result.stdout.fnmatch_lines(
         [
-            "gw0 I",
-            "gw0 [[]0[]]",
+            "created: 1/1 worker",
+            "1 worker [[]0 items[]]",
             "*_ ERROR collecting test_collection_crash.py _*",
             "E   assert 0",
             "*= 1 error in *",
         ]
     )
```

### Comparing `pytest-xdist-3.2.1/testing/conftest.py` & `pytest-xdist-3.3.0/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/test_dsession.py` & `pytest-xdist-3.3.0/testing/test_dsession.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-from xdist.dsession import DSession, get_default_max_worker_restart
+from __future__ import annotations
+from xdist.dsession import (
+    DSession,
+    get_default_max_worker_restart,
+    get_workers_status_line,
+    WorkerStatus,
+)
 from xdist.report import report_collection_diff
 from xdist.scheduler import EachScheduling, LoadScheduling, WorkStealingScheduling
-from typing import Optional
+from typing import Sequence
 
 import pytest
 import execnet
 
 
 class MockGateway:
     def __init__(self) -> None:
@@ -469,15 +475,15 @@
     from_collection = to_collection = ["aaa", "bbb", "ccc"]
     assert report_collection_diff(from_collection, to_collection, 1, 2) is None
 
 
 def test_default_max_worker_restart() -> None:
     class config:
         class option:
-            maxworkerrestart: Optional[str] = None
+            maxworkerrestart: str | None = None
             numprocesses: int = 0
 
     assert get_default_max_worker_restart(config) is None
 
     config.option.numprocesses = 2
     assert get_default_max_worker_restart(config) == 8
 
@@ -523,7 +529,74 @@
         def test_2011_table(birth_year):
             pass
     """
     )
     reprec = pytester.inline_run("-n1")
     reprec.assertoutcome(passed=2)
     assert 0
+
+
+Created = WorkerStatus.Created
+Initialized = WorkerStatus.Initialized
+ReadyForCollection = WorkerStatus.ReadyForCollection
+CollectionDone = WorkerStatus.CollectionDone
+
+
+@pytest.mark.parametrize(
+    "status_and_items, expected",
+    [
+        (
+            [],
+            "",
+        ),
+        (
+            [(Created, 0)],
+            "created: 1/1 worker",
+        ),
+        (
+            [(Created, 0), (Created, 0)],
+            "created: 2/2 workers",
+        ),
+        (
+            [(Initialized, 0), (Created, 0)],
+            "initialized: 1/2 workers",
+        ),
+        (
+            [(Initialized, 0), (Initialized, 0)],
+            "initialized: 2/2 workers",
+        ),
+        (
+            [(ReadyForCollection, 0), (Created, 0)],
+            "ready: 1/2 workers",
+        ),
+        (
+            [(ReadyForCollection, 0), (ReadyForCollection, 0)],
+            "ready: 2/2 workers",
+        ),
+        (
+            [(CollectionDone, 12), (Created, 0)],
+            "collecting: 1/2 workers",
+        ),
+        (
+            [(CollectionDone, 12), (CollectionDone, 12)],
+            "2 workers [12 items]",
+        ),
+        (
+            [(CollectionDone, 1), (CollectionDone, 1)],
+            "2 workers [1 item]",
+        ),
+        (
+            [(CollectionDone, 1)],
+            "1 worker [1 item]",
+        ),
+        # Different number of tests collected will raise an error and should not happen in practice,
+        # but we test for it anyway.
+        (
+            [(CollectionDone, 1), (CollectionDone, 12)],
+            "2 workers [1 item]",
+        ),
+    ],
+)
+def test_get_workers_status_line(
+    status_and_items: Sequence[tuple[WorkerStatus, int]], expected: str
+) -> None:
+    assert get_workers_status_line(status_and_items) == expected
```

### Comparing `pytest-xdist-3.2.1/testing/test_looponfail.py` & `pytest-xdist-3.3.0/testing/test_looponfail.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/test_newhooks.py` & `pytest-xdist-3.3.0/testing/test_newhooks.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/test_plugin.py` & `pytest-xdist-3.3.0/testing/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/test_remote.py` & `pytest-xdist-3.3.0/testing/test_remote.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/testing/test_workermanage.py` & `pytest-xdist-3.3.0/testing/test_workermanage.py`

 * *Files identical despite different names*

### Comparing `pytest-xdist-3.2.1/tox.ini` & `pytest-xdist-3.3.0/tox.ini`

 * *Files identical despite different names*

