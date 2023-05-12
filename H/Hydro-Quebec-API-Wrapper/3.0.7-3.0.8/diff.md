# Comparing `tmp/Hydro-Quebec-API-Wrapper-3.0.7.tar.gz` & `tmp/Hydro-Quebec-API-Wrapper-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hydro-Quebec-API-Wrapper-3.0.7.tar", last modified: Mon May  1 01:18:35 2023, max compression
+gzip compressed data, was "Hydro-Quebec-API-Wrapper-3.0.8.tar", last modified: Fri May 12 12:57:49 2023, max compression
```

## Comparing `Hydro-Quebec-API-Wrapper-3.0.7.tar` & `Hydro-Quebec-API-Wrapper-3.0.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1859 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11000 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7459 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2560 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-01 01:18:35.000000 Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7459 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/config.default.yaml
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/conflict_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/
--rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/custom.css
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/
--rw-rw-rw-   0 root         (0) root         (0)   348837 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/description-des-codes-interruption.pdf
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.contract.rst
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.hydro_api.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.cpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.dpc.rst
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.rst
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.types.rst
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/docs/source/todo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/examples/
--rwxrwxrwx   0 root         (0) root         (0)     2216 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/examples/hydro.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/account.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/consts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15445 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/common.py
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4940 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_residential.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/outage.py
--rw-rw-rw-   0 root         (0) root         (0)     6165 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/customer.py
--rw-rw-rw-   0 root         (0) root         (0)    15470 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/diagnostic.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    29216 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.339125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)    15695 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     6700 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/peak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     8860 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/peak.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     1136 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/timerange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/account.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/common.py
--rw-rw-rw-   0 root         (0) root         (0)     5928 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/consump.py
--rw-rw-rw-   0 root         (0) root         (0)     1656 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/contract.py
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dpc.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/outage.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/webuser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/logo/
--rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo-128.png
--rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2646 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/renovate.json
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 01:18:35.343125 Hydro-Quebec-API-Wrapper-3.0.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    17588 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_common.py
--rw-rw-rw-   0 root         (0) root         (0)     2591 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d.py
--rw-rw-rw-   0 root         (0) root         (0)     8496 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d_cpc.py
--rw-rw-rw-   0 root         (0) root         (0)     6711 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dpc.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dt.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m.py
--rw-rw-rw-   0 root         (0) root         (0)     3247 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m_gdp.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/test_basic.py
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/test_timerange.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tests/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2023-05-01 01:18:26.000000 Hydro-Quebec-API-Wrapper-3.0.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.370082 Hydro-Quebec-API-Wrapper-3.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1859 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11000 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7459 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 12:57:49.000000 Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7459 2023-05-12 12:57:49.370082 Hydro-Quebec-API-Wrapper-3.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/config.default.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/conflict_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      770 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/external/
+-rw-rw-rw-   0 root         (0) root         (0)   348837 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/external/description-des-codes-interruption.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.contract.rst
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.hydro_api.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.peak.cpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.peak.dpc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.peak.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.types.rst
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/docs/source/todo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.362082 Hydro-Quebec-API-Wrapper-3.0.8/examples/
+-rwxrwxrwx   0 root         (0) root         (0)     2216 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/examples/hydro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/consts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15445 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_residential.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)     6165 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)    15470 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/diagnostic.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    29216 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)    15695 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6700 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/peak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     8860 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/peak.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     1136 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/timerange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3695 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/account.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     5928 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/consump.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3889 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/outage.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/webuser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.366082 Hydro-Quebec-API-Wrapper-3.0.8/logo/
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/logo/hydroqc-logo-128.png
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/logo/hydroqc-logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2646 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/renovate.json
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-12 12:57:49.370082 Hydro-Quebec-API-Wrapper-3.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:57:49.370082 Hydro-Quebec-API-Wrapper-3.0.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    17588 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2591 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_d.py
+-rw-rw-rw-   0 root         (0) root         (0)     8496 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_d_cpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6711 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_dpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_dt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_m.py
+-rw-rw-rw-   0 root         (0) root         (0)     3247 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_m_gdp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/test_basic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/test_timerange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tests/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2023-05-12 12:57:38.000000 Hydro-Quebec-API-Wrapper-3.0.8/tox.ini
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/.gitignore` & `Hydro-Quebec-API-Wrapper-3.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/.gitlab-ci.yml` & `Hydro-Quebec-API-Wrapper-3.0.8/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/.pre-commit-config.yaml` & `Hydro-Quebec-API-Wrapper-3.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/.pylintrc` & `Hydro-Quebec-API-Wrapper-3.0.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO` & `Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.0.7
+Version: 3.0.8
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt` & `Hydro-Quebec-API-Wrapper-3.0.8/Hydro_Quebec_API_Wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/LICENSE` & `Hydro-Quebec-API-Wrapper-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/PKG-INFO` & `Hydro-Quebec-API-Wrapper-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hydro-Quebec-API-Wrapper
-Version: 3.0.7
+Version: 3.0.8
 Summary: A wrapper library to access hydro quebec API and more
 Home-page: https://hydroqc.ca
 Author-email: Hydroqc Team <info@hydroqc.ca>
 License: LGPL-3.0-or-later
 Project-URL: Source Code, https://gitlab.com/hydroqc/hydroqc
 Project-URL: Bug Reports, https://gitlab.com/hydroqc/hydroqc/-/issues
 Project-URL: Home-page, https://hydroqc.ca
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/README.md` & `Hydro-Quebec-API-Wrapper-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/config.default.yaml` & `Hydro-Quebec-API-Wrapper-3.0.8/config.default.yaml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/Makefile` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/make.bat` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo-128.png` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/_static/hydroqc-logo.svg` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/_static/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/conf.py` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/external/description-des-codes-interruption.pdf` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/external/description-des-codes-interruption.pdf`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.contract.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.contract.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.hydro_api.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.hydro_api.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.cpc.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.peak.cpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.peak.dpc.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.peak.dpc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/docs/source/reference/hydroqc.types.rst` & `Hydro-Quebec-API-Wrapper-3.0.8/docs/source/reference/hydroqc.types.rst`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/examples/hydro.py` & `Hydro-Quebec-API-Wrapper-3.0.8/examples/hydro.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/account.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/account.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/__init__.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/__init__.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/common.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_d.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_d_cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_d_cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_dt.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_dt.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_m.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_m_gdp.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_m_gdp.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/contract_residential.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/contract_residential.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/contract/outage.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/contract/outage.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/customer.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/customer.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/diagnostic.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/diagnostic.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/cache.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/cache.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/client.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/client.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/hydro_api/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/hydro_api/consts.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/logger.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/logger.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/consts.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/handler.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/handler.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/cpc/peak.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/cpc/peak.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/consts.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/consts.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/handler.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/handler.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/peak/dpc/peak.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/peak/dpc/peak.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/timerange.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/timerange.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/__init__.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/__init__.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/account.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/account.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/common.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/consump.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/consump.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/contract.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/contract.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/types/outage.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/types/outage.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     travaux_securitaire = 63
     manoeuvre_securitaire = 64
     manoeuvre = 65
     securite_public = 66
     interruption_demande_client = 76
     reforcement_de_reseau = 68
     programme_special = 69
+    travaux_vegetation = 77
 
 
 # TODO use strEnum on python 3.11
 class OutageCode(Enum):
     """Outage code enum."""
 
     # Unkonwn (not official HQ code)
@@ -96,14 +97,15 @@
 class OutageStatus(Enum):
     """Outage Status enum."""
 
     prevu = "P"
     commence = "C"
     reporte = "R"
     termine = "T"
+    non_confirme = "N"
 
 
 class OutageIdTyping(TypedDict, total=True):
     """Outage id json output format."""
 
     site: str
     typeObjet: str
```

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/hydroqc/webuser.py` & `Hydro-Quebec-API-Wrapper-3.0.8/hydroqc/webuser.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo-128.png` & `Hydro-Quebec-API-Wrapper-3.0.8/logo/hydroqc-logo-128.png`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/logo/hydroqc-logo.svg` & `Hydro-Quebec-API-Wrapper-3.0.8/logo/hydroqc-logo.svg`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/pyproject.toml` & `Hydro-Quebec-API-Wrapper-3.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/renovate.json` & `Hydro-Quebec-API-Wrapper-3.0.8/renovate.json`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_common.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_common.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_d.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_d_cpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_d_cpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dpc.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_dpc.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_dt.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_dt.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_m.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/subtest_contract_m_gdp.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/subtest_contract_m_gdp.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/test_basic.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/test_timerange.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/test_timerange.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tests/tools.py` & `Hydro-Quebec-API-Wrapper-3.0.8/tests/tools.py`

 * *Files identical despite different names*

### Comparing `Hydro-Quebec-API-Wrapper-3.0.7/tox.ini` & `Hydro-Quebec-API-Wrapper-3.0.8/tox.ini`

 * *Files identical despite different names*

