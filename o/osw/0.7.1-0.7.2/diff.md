# Comparing `tmp/osw-0.7.1.tar.gz` & `tmp/osw-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osw-0.7.1.tar", last modified: Fri May 12 05:52:52 2023, max compression
+gzip compressed data, was "osw-0.7.2.tar", last modified: Fri May 12 05:53:13 2023, max compression
```

## Comparing `osw-0.7.1.tar` & `osw-0.7.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.459142 osw-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 05:52:15.000000 osw-0.7.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.415141 osw-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.427142 osw-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-12 05:52:15.000000 osw-0.7.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 05:52:15.000000 osw-0.7.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-12 05:52:15.000000 osw-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 05:52:15.000000 osw-0.7.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:15.000000 osw-0.7.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-12 05:52:15.000000 osw-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-12 05:52:15.000000 osw-0.7.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 05:52:15.000000 osw-0.7.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-12 05:52:15.000000 osw-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-12 05:52:15.000000 osw-0.7.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-12 05:52:15.000000 osw-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-05-12 05:52:15.000000 osw-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:52:52.459142 osw-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-12 05:52:15.000000 osw-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:15.000000 osw-0.7.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.431141 osw-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 05:52:15.000000 osw-0.7.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.435141 osw-0.7.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 05:52:15.000000 osw-0.7.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 05:52:15.000000 osw-0.7.1/docs/auth.md
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 05:52:15.000000 osw-0.7.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 05:52:15.000000 osw-0.7.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-12 05:52:15.000000 osw-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 05:52:15.000000 osw-0.7.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 05:52:15.000000 osw-0.7.1/docs/controller.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 05:52:15.000000 osw-0.7.1/docs/dev.md
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-12 05:52:15.000000 osw-0.7.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 05:52:15.000000 osw-0.7.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 05:52:15.000000 osw-0.7.1/docs/model.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 05:52:15.000000 osw-0.7.1/docs/osw.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 05:52:15.000000 osw-0.7.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-12 05:52:15.000000 osw-0.7.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:15.000000 osw-0.7.1/docs/tools.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.439142 osw-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 05:52:15.000000 osw-0.7.1/examples/accounts.pwd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-12 05:52:15.000000 osw-0.7.1/examples/controller_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 05:52:15.000000 osw-0.7.1/examples/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-12 05:52:15.000000 osw-0.7.1/examples/create_page_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.439142 osw-0.7.1/examples/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-12 05:52:15.000000 osw-0.7.1/examples/data_processing/local_jsonpath_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 05:52:15.000000 osw-0.7.1/examples/database_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-12 05:52:15.000000 osw-0.7.1/examples/entity_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-12 05:52:15.000000 osw-0.7.1/examples/load_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-12 05:52:15.000000 osw-0.7.1/examples/local_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-12 05:52:15.000000 osw-0.7.1/examples/ontology_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-12 05:52:15.000000 osw-0.7.1/examples/page_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 05:52:15.000000 osw-0.7.1/examples/register_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 05:52:15.000000 osw-0.7.1/examples/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 05:52:15.000000 osw-0.7.1/examples/store_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 05:52:15.000000 osw-0.7.1/examples/update_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 05:52:15.000000 osw-0.7.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.419141 osw-0.7.1/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.439142 osw-0.7.1/nb/quantities/
--rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/Quantities.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.443142 osw-0.7.1/nb/quantities/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/broader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/buildDictionaryTest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/httpRequest.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/idea.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/querys.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-05-12 05:52:15.000000 osw-0.7.1/nb/quantities/archive/searchRunaways.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.447142 osw-0.7.1/nb/translations/
--rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-05-12 05:52:15.000000 osw-0.7.1/nb/translations/DeeplTranslate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-12 05:52:15.000000 osw-0.7.1/nb/translations/JsObjectToJson.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 05:52:15.000000 osw-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 05:52:52.463142 osw-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-12 05:52:15.000000 osw-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.419141 osw-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.447142 osw-0.7.1/src/osw/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.455141 osw-0.7.1/src/osw/controller/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/controller/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/controller/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.455141 osw-0.7.1/src/osw/model/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/model/page_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/model/static.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/sparql_client_smw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-05-12 05:52:15.000000 osw-0.7.1/src/osw/wtsite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.451141 osw-0.7.1/src/osw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 05:52:52.000000 osw-0.7.1/src/osw.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.459142 osw-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-12 05:52:15.000000 osw-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 05:52:15.000000 osw-0.7.1/tests/controller_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:52:52.459142 osw-0.7.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-12 05:52:15.000000 osw-0.7.1/tests/integration/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 05:52:15.000000 osw-0.7.1/tests/integration/login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-12 05:52:15.000000 osw-0.7.1/tests/integration/store_and_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-12 05:52:15.000000 osw-0.7.1/tests/sparql_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-12 05:52:15.000000 osw-0.7.1/tests/test_credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-12 05:52:15.000000 osw-0.7.1/tests/test_osl.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 05:52:15.000000 osw-0.7.1/tests/test_wiki_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-12 05:52:15.000000 osw-0.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-12 05:52:40.000000 osw-0.7.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-12 05:52:40.000000 osw-0.7.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-12 05:52:40.000000 osw-0.7.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-12 05:52:40.000000 osw-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-12 05:52:40.000000 osw-0.7.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:40.000000 osw-0.7.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-12 05:52:40.000000 osw-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-12 05:52:40.000000 osw-0.7.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-12 05:52:40.000000 osw-0.7.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-12 05:52:40.000000 osw-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-12 05:52:40.000000 osw-0.7.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    13425 2023-05-12 05:52:40.000000 osw-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32387 2023-05-12 05:52:40.000000 osw-0.7.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:53:13.970792 osw-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-12 05:52:40.000000 osw-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:40.000000 osw-0.7.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 05:52:40.000000 osw-0.7.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 05:52:40.000000 osw-0.7.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-12 05:52:40.000000 osw-0.7.2/docs/auth.md
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-12 05:52:40.000000 osw-0.7.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 05:52:40.000000 osw-0.7.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-12 05:52:40.000000 osw-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 05:52:40.000000 osw-0.7.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-12 05:52:40.000000 osw-0.7.2/docs/controller.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 05:52:40.000000 osw-0.7.2/docs/dev.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-12 05:52:40.000000 osw-0.7.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-12 05:52:40.000000 osw-0.7.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 05:52:40.000000 osw-0.7.2/docs/model.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 05:52:40.000000 osw-0.7.2/docs/osw.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-12 05:52:40.000000 osw-0.7.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-12 05:52:40.000000 osw-0.7.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 05:52:40.000000 osw-0.7.2/docs/tools.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-12 05:52:40.000000 osw-0.7.2/examples/accounts.pwd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-12 05:52:40.000000 osw-0.7.2/examples/controller_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 05:52:40.000000 osw-0.7.2/examples/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-12 05:52:40.000000 osw-0.7.2/examples/create_page_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/examples/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-12 05:52:40.000000 osw-0.7.2/examples/data_processing/local_jsonpath_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-12 05:52:40.000000 osw-0.7.2/examples/database_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-12 05:52:40.000000 osw-0.7.2/examples/entity_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-12 05:52:40.000000 osw-0.7.2/examples/load_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-05-12 05:52:40.000000 osw-0.7.2/examples/local_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-12 05:52:40.000000 osw-0.7.2/examples/ontology_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-05-12 05:52:40.000000 osw-0.7.2/examples/page_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-12 05:52:40.000000 osw-0.7.2/examples/register_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-12 05:52:40.000000 osw-0.7.2/examples/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-12 05:52:40.000000 osw-0.7.2/examples/store_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 05:52:40.000000 osw-0.7.2/examples/update_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 05:52:40.000000 osw-0.7.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.962792 osw-0.7.2/nb/quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)   123529 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/Quantities.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/nb/quantities/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107607 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/broader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59112 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/buildDictionaryTest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   152865 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/httpRequest.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/idea.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/querys.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31162 2023-05-12 05:52:40.000000 osw-0.7.2/nb/quantities/archive/searchRunaways.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/nb/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)   404547 2023-05-12 05:52:40.000000 osw-0.7.2/nb/translations/DeeplTranslate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-12 05:52:40.000000 osw-0.7.2/nb/translations/JsObjectToJson.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-12 05:52:40.000000 osw-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-12 05:53:13.970792 osw-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-12 05:52:40.000000 osw-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.958792 osw-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/controller/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/src/osw/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/page_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/model/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/sparql_client_smw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37470 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20859 2023-05-12 05:52:40.000000 osw-0.7.2/src/osw/wtsite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.966792 osw-0.7.2/src/osw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 05:53:13.000000 osw-0.7.2/src/osw.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-12 05:52:40.000000 osw-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-12 05:52:40.000000 osw-0.7.2/tests/controller_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 05:53:13.970792 osw-0.7.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-12 05:52:40.000000 osw-0.7.2/tests/integration/store_and_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-12 05:52:40.000000 osw-0.7.2/tests/sparql_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_osl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 05:52:40.000000 osw-0.7.2/tests/test_wiki_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-12 05:52:40.000000 osw-0.7.2/tox.ini
```

### Comparing `osw-0.7.1/.coveragerc` & `osw-0.7.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/.github/workflows/ci.yml` & `osw-0.7.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/.github/workflows/docs.yml` & `osw-0.7.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/.gitignore` & `osw-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/.pre-commit-config.yaml` & `osw-0.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/CHANGELOG.md` & `osw-0.7.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/CONTRIBUTING.md` & `osw-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/LICENSE.txt` & `osw-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/PKG-INFO` & `osw-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.7.1/README.md` & `osw-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/docs/Makefile` & `osw-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/docs/conf.py` & `osw-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/docs/index.md` & `osw-0.7.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/controller_logic.py` & `osw-0.7.2/examples/controller_logic.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/create_page_package.py` & `osw-0.7.2/examples/create_page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/data_processing/local_jsonpath_queries.py` & `osw-0.7.2/examples/data_processing/local_jsonpath_queries.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/database_access.py` & `osw-0.7.2/examples/database_access.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/entity_manipulation.py` & `osw-0.7.2/examples/entity_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/load_entity.py` & `osw-0.7.2/examples/load_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/local_editing.py` & `osw-0.7.2/examples/local_editing.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/ontology_import.py` & `osw-0.7.2/examples/ontology_import.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/page_manipulation.py` & `osw-0.7.2/examples/page_manipulation.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/register_model.py` & `osw-0.7.2/examples/register_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/settings.json` & `osw-0.7.2/examples/settings.json`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/store_entity.py` & `osw-0.7.2/examples/store_entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/examples/update_local_model.py` & `osw-0.7.2/examples/update_local_model.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/Quantities.ipynb` & `osw-0.7.2/nb/quantities/Quantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb` & `osw-0.7.2/nb/quantities/archive/Onto2Wiki_qudtQuantities.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/broader.ipynb` & `osw-0.7.2/nb/quantities/archive/broader.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/buildDictionaryTest.ipynb` & `osw-0.7.2/nb/quantities/archive/buildDictionaryTest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/httpRequest.ipynb` & `osw-0.7.2/nb/quantities/archive/httpRequest.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/idea.ipynb` & `osw-0.7.2/nb/quantities/archive/idea.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/querys.ipynb` & `osw-0.7.2/nb/quantities/archive/querys.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/quantities/archive/searchRunaways.ipynb` & `osw-0.7.2/nb/quantities/archive/searchRunaways.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/translations/DeeplTranslate.ipynb` & `osw-0.7.2/nb/translations/DeeplTranslate.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/nb/translations/JsObjectToJson.ipynb` & `osw-0.7.2/nb/translations/JsObjectToJson.ipynb`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/setup.cfg` & `osw-0.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/setup.py` & `osw-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/auth.py` & `osw-0.7.2/src/osw/auth.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/controller/database.py` & `osw-0.7.2/src/osw/controller/database.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/core.py` & `osw-0.7.2/src/osw/core.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/model/entity.py` & `osw-0.7.2/src/osw/model/entity.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/model/page_package.py` & `osw-0.7.2/src/osw/model/page_package.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/model/static.py` & `osw-0.7.2/src/osw/model/static.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/sparql_client_smw.py` & `osw-0.7.2/src/osw/sparql_client_smw.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/wiki_tools.py` & `osw-0.7.2/src/osw/wiki_tools.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/src/osw/wtsite.py` & `osw-0.7.2/src/osw/wtsite.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,24 +205,34 @@
                 skip_slot_suffix_for_main=config.skip_slot_suffix_for_main,
             )
         else:
             dump_config.target_dir = config.content_path
             dump_config.skip_slot_suffix_for_main = config.skip_slot_suffix_for_main
 
         bundle = config.bundle  # type: package.PagePackageBundle
+        added_titles = []  # keep track of added pages, prevent duplicates
+
         if config.name not in bundle.packages:
             print(f"Error: package {config.name} does not exist in bundle")
             return
         if not bundle.packages[config.name].pages:
             bundle.packages[config.name].pages = []
         for title in config.titles:
+            if title in added_titles:
+                continue  # prevent duplicates
+            else:
+                added_titles.append(title)
             page = self.get_WtPage(title)
             bundle.packages[config.name].pages.append(page.dump(dump_config))
             if config.include_files:
                 for file in page._page.images():
+                    if file.name in added_titles:
+                        continue  # prevent duplicates
+                    else:
+                        added_titles.append(file.name)
                     file_page = self.get_WtPage(file.name)
                     bundle.packages[config.name].pages.append(
                         file_page.dump(dump_config)
                     )
 
         content = bundle.json(exclude_none=True, indent=4)
         # This will create the JSON (e.g., package.json) with the PagePackageConfig,
@@ -259,15 +269,15 @@
                 self._content, array_mode="only_multiple"
             )
             # multi content revisions
             rev = wtSite._site.api(
                 "query",
                 prop="revisions",
                 titles=title,
-                rvprop="ids|timestamp|flags|comment|user|content|contentmodel|roles|slotsize",
+                rvprop="ids|timestamp|flags|comment|user|content|contentmodel|roles|slotsize|slotsha1",
                 rvslots="*",
                 rvlimit="1",
                 format="json",
             )
             for page_id in rev["query"]["pages"]:
                 page = rev["query"]["pages"][page_id]
                 if page["title"] == title:
@@ -275,14 +285,15 @@
                         self._current_revision = revision
                         for slot_key in revision["slots"]:
                             self._slots[slot_key] = revision["slots"][slot_key]["*"]
                             self._content_model[slot_key] = revision["slots"][slot_key][
                                 "contentmodel"
                             ]
                             self._slots_changed[slot_key] = False
+                            # self._slots_sha1[slot_key] = revision["slots"][slot_key]["*"]
                             if self._content_model[slot_key] == "json":
                                 self._slots[slot_key] = json.loads(
                                     self._slots[slot_key]
                                 )
                     # todo: set content for slots not in revision["slots"] (use
                     #  SLOTS) --> create empty slots
```

### Comparing `osw-0.7.1/src/osw.egg-info/PKG-INFO` & `osw-0.7.2/src/osw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python toolset for data processing, queries, wikicode generation and page manipulation
 Home-page: https://github.com/OpenSemanticLab/osw-python
 Author: "Simon Stier"
 Author-email: simon.stier@isc.fraunhofer.de
 License: AGPL-3.0-or-later
 Project-URL: Documentation, https://opensemanticlab.github.io/osw-python/
 Project-URL: Source, https://github.com/OpenSemanticLab/osw-python
```

### Comparing `osw-0.7.1/src/osw.egg-info/SOURCES.txt` & `osw-0.7.2/src/osw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/conftest.py` & `osw-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/controller_mixin.py` & `osw-0.7.2/tests/controller_mixin.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/integration/db_test.py` & `osw-0.7.2/tests/integration/db_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/integration/store_and_load_test.py` & `osw-0.7.2/tests/integration/store_and_load_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/sparql_client_test.py` & `osw-0.7.2/tests/sparql_client_test.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tests/test_credential_manager.py` & `osw-0.7.2/tests/test_credential_manager.py`

 * *Files identical despite different names*

### Comparing `osw-0.7.1/tox.ini` & `osw-0.7.2/tox.ini`

 * *Files identical despite different names*

