# Comparing `tmp/custodian-2023.5.12.tar.gz` & `tmp/custodian-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodian-2023.5.12.tar", last modified: Fri May 12 15:31:24 2023, max compression
+gzip compressed data, was "custodian-2023.5.7.tar", last modified: Sun May  7 20:41:37 2023, max compression
```

## Comparing `custodian-2023.5.12.tar` & `custodian-2023.5.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 15:26:37.000000 custodian-2023.5.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 15:26:37.000000 custodian-2023.5.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-12 15:31:24.358600 custodian-2023.5.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-12 15:26:37.000000 custodian-2023.5.12/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.350599 custodian-2023.5.12/custodian/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.354600 custodian-2023.5.12/custodian/ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/ansible/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/ansible/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.354600 custodian-2023.5.12/custodian/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/converge_geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/converge_kpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/cstdn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/run_nwchem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cli/run_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.354600 custodian-2023.5.12/custodian/cp2k/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/cp2k/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    36611 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.354600 custodian-2023.5.12/custodian/feff/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/feff/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/feff/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/feff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/custodian/lobster/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/lobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/lobster/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/lobster/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/custodian/nwchem/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/nwchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/nwchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/nwchem/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/custodian/qchem/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/qchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/qchem/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/qchem/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/custodian/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/tests/test_custodian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.358600 custodian-2023.5.12/custodian/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76174 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/vasp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/vasp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38518 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-12 15:26:37.000000 custodian-2023.5.12/custodian/vasp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:24.354600 custodian-2023.5.12/custodian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 15:31:24.000000 custodian-2023.5.12/custodian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-12 15:26:37.000000 custodian-2023.5.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-12 15:26:37.000000 custodian-2023.5.12/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-12 15:26:37.000000 custodian-2023.5.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-12 15:31:24.362599 custodian-2023.5.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-12 15:26:37.000000 custodian-2023.5.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 20:37:45.000000 custodian-2023.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-07 20:37:45.000000 custodian-2023.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.788636 custodian-2023.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-07 20:37:45.000000 custodian-2023.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.780636 custodian-2023.5.7/custodian/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/ansible/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4538 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/converge_kpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/cstdn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_nwchem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12410 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cli/run_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44267 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/cp2k/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36593 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/feff/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/feff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/lobster/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/lobster/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/nwchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/nwchem/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian/qchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/qchem/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/tests/test_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.788636 custodian-2023.5.7/custodian/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76156 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38518 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-07 20:37:45.000000 custodian-2023.5.7/custodian/vasp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:41:37.784636 custodian-2023.5.7/custodian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 20:41:37.000000 custodian-2023.5.7/custodian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 20:37:45.000000 custodian-2023.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 20:37:45.000000 custodian-2023.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-07 20:41:37.788636 custodian-2023.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-07 20:37:45.000000 custodian-2023.5.7/setup.py
```

### Comparing `custodian-2023.5.12/LICENSE` & `custodian-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/PKG-INFO` & `custodian-2023.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.5.12
+Version: 2023.5.7
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.5.12/README.rst` & `custodian-2023.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/ansible/actions.py` & `custodian-2023.5.7/custodian/ansible/actions.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/ansible/interpreter.py` & `custodian-2023.5.7/custodian/ansible/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cli/converge_geometry.py` & `custodian-2023.5.7/custodian/cli/converge_geometry.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cli/converge_kpoints.py` & `custodian-2023.5.7/custodian/cli/converge_kpoints.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cli/cstdn.py` & `custodian-2023.5.7/custodian/cli/cstdn.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cli/run_nwchem.py` & `custodian-2023.5.7/custodian/cli/run_nwchem.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cli/run_vasp.py` & `custodian-2023.5.7/custodian/cli/run_vasp.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cp2k/handlers.py` & `custodian-2023.5.7/custodian/cp2k/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cp2k/interpreter.py` & `custodian-2023.5.7/custodian/cp2k/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cp2k/jobs.py` & `custodian-2023.5.7/custodian/cp2k/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cp2k/utils.py` & `custodian-2023.5.7/custodian/cp2k/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/cp2k/validators.py` & `custodian-2023.5.7/custodian/cp2k/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/custodian.py` & `custodian-2023.5.7/custodian/custodian.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         monitor_freq=30,
         skip_over_errors=False,
         scratch_dir=None,
         gzipped_output=False,
         checkpoint=False,
         terminate_func=None,
         terminate_on_nonzero_returncode=True,
-        **kwargs,
     ):
         """
         Initializes a Custodian from a list of jobs and error handlers.
 
         Args:
             handlers ([ErrorHandler]): Error handlers. In order of priority of
                 fixing.
```

### Comparing `custodian-2023.5.12/custodian/feff/handlers.py` & `custodian-2023.5.7/custodian/feff/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/feff/interpreter.py` & `custodian-2023.5.7/custodian/feff/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/feff/jobs.py` & `custodian-2023.5.7/custodian/feff/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/lobster/handlers.py` & `custodian-2023.5.7/custodian/lobster/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/lobster/jobs.py` & `custodian-2023.5.7/custodian/lobster/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/nwchem/handlers.py` & `custodian-2023.5.7/custodian/nwchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/nwchem/jobs.py` & `custodian-2023.5.7/custodian/nwchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/qchem/handlers.py` & `custodian-2023.5.7/custodian/qchem/handlers.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/qchem/jobs.py` & `custodian-2023.5.7/custodian/qchem/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/qchem/utils.py` & `custodian-2023.5.7/custodian/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/tests/test_custodian.py` & `custodian-2023.5.7/custodian/tests/test_custodian.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/utils.py` & `custodian-2023.5.7/custodian/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/vasp/handlers.py` & `custodian-2023.5.7/custodian/vasp/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,14 @@
     }
 
     def __init__(
         self,
         output_filename="vasp.out",
         errors_subset_to_catch=None,
         vtst_fixes=False,
-        **kwargs,
     ):
         """
         Initializes the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
```

### Comparing `custodian-2023.5.12/custodian/vasp/interpreter.py` & `custodian-2023.5.7/custodian/vasp/interpreter.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/vasp/jobs.py` & `custodian-2023.5.7/custodian/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian/vasp/validators.py` & `custodian-2023.5.7/custodian/vasp/validators.py`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/custodian.egg-info/PKG-INFO` & `custodian-2023.5.7/custodian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2023.5.12
+Version: 2023.5.7
 Summary: A simple JIT job management framework in Python.
 Home-page: https://github.com/materialsproject/custodian
 Author: Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau
 Author-email: ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 License: MIT
 Keywords: jit,just-in-time,job,management,vasp
```

### Comparing `custodian-2023.5.12/custodian.egg-info/SOURCES.txt` & `custodian-2023.5.7/custodian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/setup.cfg` & `custodian-2023.5.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `custodian-2023.5.12/setup.py` & `custodian-2023.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_desc = f.read()
     ind = long_desc.find("\n")
     long_desc = long_desc[ind + 1 :]
 
 setup(
     name="custodian",
     packages=find_packages(),
-    version="2023.5.12",
+    version="2023.5.7",
     install_requires=["monty>=2.0.6", "ruamel.yaml>=0.15.6", "sentry-sdk>=0.8.0"],
     extras_require={"vasp, nwchem, qchem": ["pymatgen>=2019.8.23"]},
     package_data={},
     author="Shyue Ping Ong, William Davidson Richards, Stephen Dacek, Xiaohui Qu, Matthew Horton, Samuel M. Blau",
     author_email="ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     url="https://github.com/materialsproject/custodian",
```

