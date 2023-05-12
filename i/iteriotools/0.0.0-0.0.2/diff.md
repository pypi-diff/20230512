# Comparing `tmp/iteriotools-0.0.0.tar.gz` & `tmp/iteriotools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iteriotools-0.0.0.tar", last modified: Tue May  9 22:18:42 2023, max compression
+gzip compressed data, was "iteriotools-0.0.2.tar", last modified: Thu May 11 17:28:31 2023, max compression
```

## Comparing `iteriotools-0.0.0.tar` & `iteriotools-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:18:42.499030 iteriotools-0.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-09 22:18:26.000000 iteriotools-0.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4303 2023-05-09 22:18:26.000000 iteriotools-0.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-09 22:18:26.000000 iteriotools-0.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-09 22:18:26.000000 iteriotools-0.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-09 22:18:42.499030 iteriotools-0.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-09 22:18:26.000000 iteriotools-0.0.0/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    45324 2023-05-09 22:18:26.000000 iteriotools-0.0.0/Pipfile.lock
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:18:42.496280 iteriotools-0.0.0/iteriotools/
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-09 22:18:26.000000 iteriotools-0.0.0/iteriotools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:18:42.497197 iteriotools-0.0.0/iteriotools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-09 22:18:42.000000 iteriotools-0.0.0/iteriotools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-09 22:18:42.000000 iteriotools-0.0.0/iteriotools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 22:18:42.000000 iteriotools-0.0.0/iteriotools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-09 22:18:42.000000 iteriotools-0.0.0/iteriotools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1372 2023-05-09 22:18:26.000000 iteriotools-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 22:18:42.499030 iteriotools-0.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:18:42.498114 iteriotools-0.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 22:18:26.000000 iteriotools-0.0.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 22:18:42.499030 iteriotools-0.0.0/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 22:18:26.000000 iteriotools-0.0.0/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-09 22:18:26.000000 iteriotools-0.0.0/tests/unit/test_inbuffer.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-09 22:18:26.000000 iteriotools-0.0.0/tests/unit/test_raw_iter_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.057641 iteriotools-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-11 17:28:13.000000 iteriotools-0.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4303 2023-05-11 17:28:13.000000 iteriotools-0.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-11 17:28:13.000000 iteriotools-0.0.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-11 17:28:13.000000 iteriotools-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-05-11 17:28:31.056641 iteriotools-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-11 17:28:13.000000 iteriotools-0.0.2/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    45324 2023-05-11 17:28:13.000000 iteriotools-0.0.2/Pipfile.lock
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-05-11 17:28:13.000000 iteriotools-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.050640 iteriotools-0.0.2/example/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)     7127 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/Pipfile.lock
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.052641 iteriotools-0.0.2/example/project/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/project/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/project/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-05-11 17:28:13.000000 iteriotools-0.0.2/example/project/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.052641 iteriotools-0.0.2/iteriotools/
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-05-11 17:28:13.000000 iteriotools-0.0.2/iteriotools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.055641 iteriotools-0.0.2/iteriotools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-05-11 17:28:31.000000 iteriotools-0.0.2/iteriotools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-11 17:28:31.000000 iteriotools-0.0.2/iteriotools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 17:28:31.000000 iteriotools-0.0.2/iteriotools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 17:28:31.000000 iteriotools-0.0.2/iteriotools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-11 17:28:13.000000 iteriotools-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 17:28:31.057641 iteriotools-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.055641 iteriotools-0.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 17:28:13.000000 iteriotools-0.0.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 17:28:31.056641 iteriotools-0.0.2/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-11 17:28:13.000000 iteriotools-0.0.2/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-11 17:28:13.000000 iteriotools-0.0.2/tests/unit/test_inbuffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-11 17:28:13.000000 iteriotools-0.0.2/tests/unit/test_raw_iter_io.py
```

### Comparing `iteriotools-0.0.0/.gitlab-ci.yml` & `iteriotools-0.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iteriotools-0.0.0/.pre-commit-config.yaml` & `iteriotools-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iteriotools-0.0.0/LICENSE` & `iteriotools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iteriotools-0.0.0/Pipfile.lock` & `iteriotools-0.0.2/Pipfile.lock`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995291902071562%*

 * *Differences: {"'develop'": "{'simple-git-versioning': {'hashes': "*

 * *              "['sha256:508069a9ff85e963cd4ad4fc9ee82aefbecf79375f1416efb5cf3d7d4274a84c', "*

 * *              "'sha256:ebd923d5dc7f850725c19cc5a21802342a4efd85379fe8986422ce0979bc0e4f'], "*

 * *              "'version': '==0.0.29'}}"}*

```diff
@@ -690,19 +690,19 @@
                 "sha256:800efeda403b63879b0a5625f65a0021fd1ea61ed181954da0346372a7b2a341"
             ],
             "markers": "python_version < '4.0' and python_full_version >= '3.8.1'",
             "version": "==2.0.3"
         },
         "simple-git-versioning": {
             "hashes": [
-                "sha256:624206739ffed2c7ae7bf9879c2ac8b97ffa8444b1ba1cf1c70e16ca347472a6",
-                "sha256:7d0535efac545d9da5fda87bb2e7dcc9f3dda82caaa397e761459f3c333eb001"
+                "sha256:508069a9ff85e963cd4ad4fc9ee82aefbecf79375f1416efb5cf3d7d4274a84c",
+                "sha256:ebd923d5dc7f850725c19cc5a21802342a4efd85379fe8986422ce0979bc0e4f"
             ],
             "index": "pypi",
-            "version": "==0.0.27"
+            "version": "==0.0.29"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
```

### Comparing `iteriotools-0.0.0/iteriotools/__init__.py` & `iteriotools-0.0.2/iteriotools/__init__.py`

 * *Files identical despite different names*

### Comparing `iteriotools-0.0.0/pyproject.toml` & `iteriotools-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
+readme = "README.md"
 dynamic = ["dependencies", "version"]
 
 [project.urls]
+homepage = "https://gitlab.com/ypsah/iteriotools"
 repository = "https://gitlab.com/ypsah/iteriotools"
 
 [build-system]
 requires = ["setuptools>=63", "setuptools_scm[toml]>=6.2", "setuptools-pipfile"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
@@ -44,12 +46,16 @@
 
 [tool.isort]
 profile = "black"
 src_paths = ["iteriotools", "tests"]
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --cov=iteriotools --cov-branch --cov-fail-under=90"
+testpaths = ["iteriotools", "tests"]
 
 [tool.ruff]
 ignore = [
     "E501",  # line-length: black already covers this
 ]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["F401"]
```

### Comparing `iteriotools-0.0.0/tests/unit/test_inbuffer.py` & `iteriotools-0.0.2/tests/unit/test_inbuffer.py`

 * *Files identical despite different names*

