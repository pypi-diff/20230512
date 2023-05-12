# Comparing `tmp/devolo_plc_api-1.3.0.tar.gz` & `tmp/devolo_plc_api-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devolo_plc_api-1.3.0.tar", last modified: Thu Apr 13 13:15:23 2023, max compression
+gzip compressed data, was "devolo_plc_api-1.3.1.tar", last modified: Fri May 12 13:38:19 2023, max compression
```

## Comparing `devolo_plc_api-1.3.0.tar` & `devolo_plc_api-1.3.1.tar`

### file list

```diff
@@ -1,101 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/convert_todos_to_issues.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/clients/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/device_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/exceptions/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.229554 devolo_plc_api-1.3.0/devolo_plc_api/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/devolo_plc_api/zeroconf/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/devolo_plc_api/zeroconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.225554 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 13:15:23.000000 devolo_plc_api-1.3.0/devolo_plc_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/docs/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/example_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/example_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4250 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/script/stubgen.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.233554 devolo_plc_api-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/device_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/plcnet_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/fixtures/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/mock_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/mocks/mock_zeroconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:15:23.237554 devolo_plc_api-1.3.0/tests/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/stubs/zeroconf.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_data.json
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_deviceapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_plcnetapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-13 13:15:02.000000 devolo_plc_api-1.3.0/tests/test_profobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/convert_todos_to_issues.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/clients/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/device_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/exceptions/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/devolo_plc_api/zeroconf/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/devolo_plc_api/zeroconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.834818 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44988 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 13:38:19.000000 devolo_plc_api-1.3.1/devolo_plc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/example_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/example_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4419 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/scripts/stubgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/device_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/fixtures/plcnet_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.838818 devolo_plc_api-1.3.1/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/mocks/zeroconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:38:19.842818 devolo_plc_api-1.3.1/tests/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/snapshots/test_device.ambr
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_deviceapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-05-12 13:38:03.000000 devolo_plc_api-1.3.1/tests/test_plcnetapi.py
```

### Comparing `devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `devolo_plc_api-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/.github/workflows/pythonpackage.yml` & `devolo_plc_api-1.3.1/.github/workflows/pythonpackage.yml`

 * *Files 6% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 jobs:
 
   format:
     name: Check formatting
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --no-binary=mypy mypy
     - name: Check formatting
       uses: pre-commit/action@v3.0.0
 
   lint:
     name: Lint
     runs-on: ubuntu-latest
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: "3.8"
     - name: Lint with ruff
       run: |
         python -m pip install --upgrade pip
         python -m pip install ruff
-        ruff check --format=github devolo_plc_api script
+        ruff check --format=github devolo_plc_api scripts
         ruff check --format=github --exit-zero tests
     - name: Lint with mypy
       run: |
         python -m pip install mypy types-protobuf
         mypy devolo_plc_api
         mypy tests || true
 
@@ -47,17 +47,17 @@
     name: Test with Python ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: ${{ matrix.python-version }}
         check-latest: true
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -e .[test]
@@ -72,17 +72,17 @@
 
   coverage:
     name: Upload coverage
     runs-on: ubuntu-latest
     needs: test
     steps:
     - name: Checkout sources
-      uses: actions/checkout@v3.5.0
+      uses: actions/checkout@v3.5.2
     - name: Set up Python
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: "3.8"
     - name: Download coverage
       uses: actions/download-artifact@v3.0.2
       with:
         name: coverage
     - name: Coveralls
```

### Comparing `devolo_plc_api-1.3.0/.github/workflows/pythonpublish.yml` & `devolo_plc_api-1.3.1/.github/workflows/pythonpublish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3.5.0
+    - uses: actions/checkout@v3.5.2
     - name: Set up Python
-      uses: actions/setup-python@v4.5.0
+      uses: actions/setup-python@v4.6.0
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install --upgrade build twine
     - name: Build and publish
```

### Comparing `devolo_plc_api-1.3.0/.gitignore` & `devolo_plc_api-1.3.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -121,19 +121,22 @@
 /site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
+# ruff
+.ruff_cache/
+
 # Pyre type checker
 .pyre/
 
 ### VisualStudioCode ###
-.vscode/*
+.vscode/
 
 ### VisualStudioCode Patch ###
 # Ignore all local history of files
 .history
 
 ### PyCharm ###
 .idea
```

### Comparing `devolo_plc_api-1.3.0/.pre-commit-config.yaml` & `devolo_plc_api-1.3.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -17,11 +17,11 @@
     rev: 'v0.12.1'
     hooks:
       - id: validate-pyproject
 -   repo: local
     hooks:
         - id: stubgen
           name: check API stub files
-          entry: script/stubgen.py
+          entry: scripts/stubgen.py
           description: check if stub files of the APIs are up-to-date
           language: script
           types: [python]
```

### Comparing `devolo_plc_api-1.3.0/LICENSE` & `devolo_plc_api-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/PKG-INFO` & `devolo_plc_api-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo_plc_api
-Version: 1.3.0
+Version: 1.3.1
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.3.0/README.md` & `devolo_plc_api-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/clients/protobuf.py` & `devolo_plc_api-1.3.1/devolo_plc_api/clients/protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DigestAuth,
     HTTPStatusError,
     ReadTimeout,
     RemoteProtocolError,
     Response,
 )
 
-from devolo_plc_api.exceptions.device import DevicePasswordProtected, DeviceUnavailable
+from devolo_plc_api.exceptions import DevicePasswordProtected, DeviceUnavailable
 
 TIMEOUT = 10.0
 
 
 class Protobuf(ABC):
     """Google Protobuf client as ground work."""
 
@@ -41,16 +41,15 @@
         self._user: str
         self._version: str
 
     def __getattr__(self, attr: str) -> Callable[..., Any]:
         """Catch attempts to call methods synchronously."""
 
         def method(*args: Any, **kwargs: Any) -> Any:
-            loop = asyncio.get_event_loop()
-            return loop.run_until_complete(getattr(self, async_method)(*args, **kwargs))
+            return asyncio.run(getattr(self, async_method)(*args, **kwargs))
 
         async_method = f"async_{attr}"
         if hasattr(self.__class__, async_method):
             return method
         raise AttributeError(f"{self.__class__.__name__} object has no attribute {attr}")  # noqa: EM102, TRY003
 
     @property
```

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Representation of your devolo device."""
 from __future__ import annotations
 
 import asyncio
 import logging
 from contextlib import suppress
 from datetime import date
-from ipaddress import ip_address
+from ipaddress import ip_address, ip_network
 from struct import unpack_from
 from types import TracebackType
+from typing import cast
 
 from httpx import AsyncClient
+from ifaddr import get_adapters
 from zeroconf import DNSQuestionType, ServiceInfo, ServiceStateChange, Zeroconf
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from .device_api import SERVICE_TYPE as DEVICEAPI, DeviceApi
-from .exceptions.device import DeviceNotFound
+from .exceptions import DeviceNotFound
 from .plcnet_api import DEVICES_WITHOUT_PLCNET, SERVICE_TYPE as PLCNETAPI, PlcNetApi
 from .zeroconf import ZeroconfServiceInfo
 
 
-class Device:  # pylint: disable=too-many-instance-attributes
+class Device:
     """
     Representing object for your devolo PLC device. It stores all properties and functionalities discovered during setup.
 
     :param ip: IP address of the device to communicate with.
     :param plcnetapi: Reuse externally gathered data for the plcnet API
     :param deviceapi: Reuse externally gathered data for the device API
     :param zeroconf_instance: Zeroconf instance to be potentially reused.
@@ -44,24 +46,25 @@
         self.technology = ""
         self.serial_number = "0"
 
         self.device: DeviceApi | None = None
         self.plcnet: PlcNetApi | None = None
 
         self._background_tasks: set[asyncio.Task] = set()
-        self._browser: dict[str, AsyncServiceBrowser] = {}
+        self._browser: AsyncServiceBrowser | None
         self._connected = False
         self._info: dict[str, ZeroconfServiceInfo] = {PLCNETAPI: ZeroconfServiceInfo(), DEVICEAPI: ZeroconfServiceInfo()}
         self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._multicast = False
         self._password = ""
         self._session_instance: AsyncClient | None = None
         self._zeroconf_instance = zeroconf_instance
-        logging.captureWarnings(True)
+        logging.captureWarnings(capture=True)
 
+        self._loop: asyncio.AbstractEventLoop
         self._session: AsyncClient
         self._zeroconf: AsyncZeroconf
 
     def __del__(self) -> None:
         """Warn user, if the connection was not properly closed."""
         if self._connected and self._session_instance is None:
             self._logger.warning("Please disconnect properly from the device.")
@@ -118,127 +121,148 @@
         Connect to a device asynchronous.
 
         :param: session_instance: Session client instance to be potentially reused.
         """
         self._session_instance = session_instance
         self._session = self._session_instance or AsyncClient()
         if not self._zeroconf_instance:
-            self._zeroconf = AsyncZeroconf()
+            self._zeroconf = AsyncZeroconf(interfaces=await self._get_relevant_interfaces())
         elif isinstance(self._zeroconf_instance, Zeroconf):
             self._zeroconf = AsyncZeroconf(zc=self._zeroconf_instance)
         else:
             self._zeroconf = self._zeroconf_instance
-        await asyncio.gather(self._get_device_info(), self._get_plcnet_info())
+        await self._get_zeroconf_info()
+        if not self._info[DEVICEAPI].properties and not self._info[PLCNETAPI].properties:
+            await self._retry_zeroconf_info()
         if not self.device and not self.plcnet:
             raise DeviceNotFound(self.ip)
         self._connected = True
 
     def connect(self) -> None:
         """Connect to a device synchronous."""
-        loop = asyncio.new_event_loop()
-        loop.run_until_complete(self.async_connect())
+        self._loop = asyncio.get_event_loop()
+        self._loop.run_until_complete(self.async_connect())
 
     async def async_disconnect(self) -> None:
         """Disconnect from a device asynchronous."""
         if self._connected:
-            for browser in self._browser.values():
-                await browser.async_cancel()
+            if self._browser:
+                await self._browser.async_cancel()
             if not self._zeroconf_instance:
                 await self._zeroconf.async_close()
             if not self._session_instance:
                 await self._session.aclose()
             self._connected = False
 
     def disconnect(self) -> None:
         """Disconnect from a device synchronous."""
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(self.async_disconnect())
-        loop.close()
+        self._loop.run_until_complete(self.async_disconnect())
+
+    async def _get_relevant_interfaces(self) -> list[str]:
+        """Get the IP address of the relevant interface to reduce traffic."""
+        interface: list[str] = []
+        for adapter in get_adapters():
+            interface.extend(
+                cast(str, ip.ip)
+                for ip in adapter.ips
+                if ip.is_IPv4 and ip_address(self.ip) in ip_network(f"{ip.ip}/{ip.network_prefix}", strict=False)
+            )
+            interface.extend(
+                cast(str, ip.ip[0])
+                for ip in adapter.ips
+                if ip.is_IPv6 and ip_address(self.ip) in ip_network(f"{ip.ip[0]}/{ip.network_prefix}", strict=False)
+            )
+        return interface
 
     async def _get_device_info(self) -> None:
         """Get information from the devolo Device API."""
         service_type = DEVICEAPI
-        await self._get_zeroconf_info(service_type=service_type)
-        if not self._info[service_type].properties:
-            await self._retry_zeroconf_info(service_type=service_type)
         if self._info[service_type].properties:
             self.mt_number = self._info[service_type].properties.get("MT", "0")
             self.product = self._info[service_type].properties.get("Product", "")
             self.serial_number = self._info[service_type].properties["SN"]
-            self.device = DeviceApi(ip=self.ip, session=self._session, info=self._info[service_type])
+            self.device = DeviceApi(
+                ip=str(ip_address(self._info[service_type].address)),
+                session=self._session,
+                info=self._info[service_type],
+            )
             self.device.password = self.password
 
     async def _get_plcnet_info(self) -> None:
         """Get information from the devolo PlcNet API."""
         service_type = PLCNETAPI
-        if self.mt_number in DEVICES_WITHOUT_PLCNET:
-            return
-        await self._get_zeroconf_info(service_type=service_type)
-        if not self._info[service_type].properties and self.mt_number not in DEVICES_WITHOUT_PLCNET:
-            await self._retry_zeroconf_info(service_type=service_type)
         if self._info[service_type].properties:
             self.mac = self._info[service_type].properties["PlcMacAddress"]
             self.technology = self._info[service_type].properties.get("PlcTechnology", "")
-            self.plcnet = PlcNetApi(ip=self.ip, session=self._session, info=self._info[service_type])
+            self.plcnet = PlcNetApi(
+                ip=str(ip_address(self._info[service_type].address)),
+                session=self._session,
+                info=self._info[service_type],
+            )
             self.plcnet.password = self.password
 
-    async def _get_zeroconf_info(self, service_type: str) -> None:
+    async def _get_zeroconf_info(self) -> None:
         """Browse for the desired mDNS service types and query them."""
-        self._logger.debug("Browsing for %s", service_type)
+        service_types = [DEVICEAPI, PLCNETAPI]
         counter = 0
+        self._logger.debug("Browsing for %s", service_types)
         addr = None if self._multicast else self.ip
         question_type = DNSQuestionType.QM if self._multicast else DNSQuestionType.QU
-        self._browser[service_type] = AsyncServiceBrowser(
+        self._browser = AsyncServiceBrowser(
             zeroconf=self._zeroconf.zeroconf,
-            type_=service_type,
+            type_=service_types,
             handlers=[self._state_change],
             addr=addr,
             question_type=question_type,
         )
-        while not self._info[service_type].properties and counter < self.MDNS_TIMEOUT:
+        while (
+            not self._info[DEVICEAPI].properties
+            or not self._info[PLCNETAPI].properties
+            and self.mt_number not in DEVICES_WITHOUT_PLCNET
+        ) and counter < self.MDNS_TIMEOUT:
             counter += 1
             await asyncio.sleep(0.01)
 
-    async def _retry_zeroconf_info(self, service_type: str) -> None:
+    async def _retry_zeroconf_info(self) -> None:
         """Retry getting the zeroconf info using multicast."""
-        self._logger.debug(
-            "Having trouble getting %s via unicast messages. Switching to multicast for this device.", service_type
-        )
+        self._logger.debug("Having trouble getting results via unicast messages. Switching to multicast for this device.")
         self._multicast = True
-        await self._get_zeroconf_info(service_type=service_type)
+        await self._get_zeroconf_info()
 
     def _state_change(self, zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange) -> None:
         """Evaluate the query result."""
         if state_change == ServiceStateChange.Removed:
             return
         task = asyncio.create_task(self._get_service_info(zeroconf, service_type, name))
         self._background_tasks.add(task)
         task.add_done_callback(self._background_tasks.remove)
 
     async def _get_service_info(self, zeroconf: Zeroconf, service_type: str, name: str) -> None:
         """Get service information, if IP matches."""
         service_info = AsyncServiceInfo(service_type, name)
         question_type = DNSQuestionType.QM if self._multicast else DNSQuestionType.QU
+        update = {
+            DEVICEAPI: self._get_device_info,
+            PLCNETAPI: self._get_plcnet_info,
+        }
         with suppress(RuntimeError):
             await service_info.async_request(zeroconf, timeout=1000, question_type=question_type)
 
-        if not service_info.addresses or str(ip_address(service_info.addresses[0])) != self.ip:
+        if not service_info.addresses or self.ip not in service_info.parsed_addresses():
             return  # No need to continue, if there are no relevant service information
 
         self._logger.debug("Updating service info of %s for %s", service_type, service_info.server_key)
         if info := self.info_from_service(service_info):
             self._info[service_type] = info
+            await update[service_type]()
 
     @staticmethod
     def info_from_service(service_info: ServiceInfo) -> ZeroconfServiceInfo | None:
         """Return prepared info from mDNS entries."""
         properties = {}
-        if not service_info.addresses:
-            return None  # No need to continue, if there is no IP address to contact the device
-
         total_length = len(service_info.text)
         offset = 0
         while offset < total_length:
             (parsed_length,) = unpack_from("!B", service_info.text, offset)
             key_value = service_info.text[offset + 1 : offset + 1 + parsed_length].decode("UTF-8").split("=")
             properties[key_value[0]] = key_value[1]
             offset += parsed_length + 1
```

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/__init__.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import functools
 from typing import TYPE_CHECKING, Callable, TypeVar
 
 from httpx import AsyncClient
 
 from devolo_plc_api.clients import Protobuf
-from devolo_plc_api.exceptions.feature import FeatureNotSupported
+from devolo_plc_api.exceptions import FeatureNotSupported
 from devolo_plc_api.zeroconf import ZeroconfServiceInfo
 
 from .factoryreset_pb2 import FactoryResetStart
 from .ledsettings_pb2 import LedSettingsGet, LedSettingsSet, LedSettingsSetResponse
 from .multiap_pb2 import WifiMultiApGetResponse
 from .restart_pb2 import RestartResponse, UptimeGetResponse
 from .support_pb2 import SupportInfoDump, SupportInfoDumpResponse
```

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/deviceapi.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/deviceapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/factoryreset_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/factoryreset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/ledsettings_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/ledsettings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/multiap_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/multiap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/restart_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/restart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/support_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/updatefirmware_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/updatefirmware_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/device_api/wifinetwork_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/device_api/wifinetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/exceptions/device.py` & `devolo_plc_api-1.3.1/devolo_plc_api/exceptions/device.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/network/__init__.py` & `devolo_plc_api-1.3.1/devolo_plc_api/network/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 """Discover devices in your network."""
 from __future__ import annotations
 
 import asyncio
 import time
 from ipaddress import ip_address
+from typing import Any, cast
 
+from ifaddr import get_adapters
 from zeroconf import DNSQuestionType, ServiceBrowser, ServiceStateChange, Zeroconf
 
 from devolo_plc_api.device import Device
 from devolo_plc_api.device_api import SERVICE_TYPE
 
 
-async def async_discover_network() -> dict[str, Device]:
+async def async_discover_network(timeout: float = 3) -> dict[str, Device]:
     """
     Discover all devices that expose the devolo device API via mDNS asynchronous.
 
     :return: Devices accessible via serial number.
     """
     devices: dict[str, Device] = {}
 
     def add(zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange) -> None:
         """React on state changes."""
-        _add(devices, zeroconf, service_type, name, state_change)
+        _add(zeroconf, service_type, name, state_change, devices=devices, timeout=timeout)
 
-    browser = ServiceBrowser(Zeroconf(), SERVICE_TYPE, [add], question_type=DNSQuestionType.QM)
-    await asyncio.sleep(3)
+    browser = ServiceBrowser(Zeroconf(interfaces=_interfaces()), SERVICE_TYPE, [add], question_type=DNSQuestionType.QM)
+    await asyncio.sleep(timeout)
     browser.cancel()
     return devices
 
 
-def discover_network() -> dict[str, Device]:
+def discover_network(timeout: float = 3) -> dict[str, Device]:
     """
     Discover devices that expose the devolo device API via mDNS synchronous.
 
     :return: Devices accessible via serial number.
     """
     devices: dict[str, Device] = {}
 
     def add(zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange) -> None:
         """React on state changes."""
-        _add(devices, zeroconf, service_type, name, state_change)
+        _add(zeroconf, service_type, name, state_change, devices=devices, timeout=timeout)
 
-    browser = ServiceBrowser(Zeroconf(), SERVICE_TYPE, [add], question_type=DNSQuestionType.QM)
-    time.sleep(3)
+    browser = ServiceBrowser(Zeroconf(interfaces=_interfaces()), SERVICE_TYPE, [add], question_type=DNSQuestionType.QM)
+    time.sleep(timeout)
     browser.cancel()
     return devices
 
 
-def _add(
-    devices: dict[str, Device], zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange
-) -> None:
+def _add(zeroconf: Zeroconf, service_type: str, name: str, state_change: ServiceStateChange, **kwargs: Any) -> None:
     """Create a device object to each matching device."""
     if state_change is not ServiceStateChange.Added:
         return
 
-    if (service_info := zeroconf.get_service_info(service_type, name)) is None:
+    if (service_info := zeroconf.get_service_info(service_type, name, timeout=kwargs["timeout"] * 1000)) is None:
         return
 
     info = Device.info_from_service(service_info)
     if info is None or info.properties["MT"] in ("2600", "2601"):
         return  # Don't react on devolo Home Control central units
 
+    devices: dict[str, Device] = kwargs["devices"]
     devices[info.properties["SN"]] = Device(ip=str(ip_address(info.address)), zeroconf_instance=zeroconf)
+
+
+def _interfaces() -> list[str]:
+    """Get IP addresses not being localhost."""
+    interface: list[str] = []
+    for adapter in get_adapters():
+        interface.extend(cast(str, ip.ip) for ip in adapter.ips if ip.is_IPv4 and ip.ip != "127.0.0.1")
+        interface.extend(cast(str, ip.ip[0]) for ip in adapter.ips if ip.is_IPv6 and ip.ip[0] != "::1")
+    return interface
```

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/__init__.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/__init__.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/getnetworkoverview_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/identifydevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/pairdevice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/plcnetapi.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/plcnetapi.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi` & `devolo_plc_api-1.3.1/devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api.egg-info/PKG-INFO` & `devolo_plc_api-1.3.1/devolo_plc_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devolo-plc-api
-Version: 1.3.0
+Version: 1.3.1
 Summary: devolo PLC devices in Python
 Author-email: Markus Bong <m.bong@famabo.de>, Guido Schmitz <guido.schmitz@fedaix.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `devolo_plc_api-1.3.0/devolo_plc_api.egg-info/SOURCES.txt` & `devolo_plc_api-1.3.1/devolo_plc_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,27 +55,21 @@
 devolo_plc_api/plcnet_api/plcnetapi.pyi
 devolo_plc_api/plcnet_api/setuserdevicename_pb2.py
 devolo_plc_api/plcnet_api/setuserdevicename_pb2.pyi
 devolo_plc_api/zeroconf/__init__.py
 docs/CHANGELOG.md
 docs/CODE_OF_CONDUCT.md
 docs/CONTRIBUTING.md
-script/stubgen.py
+scripts/stubgen.py
 tests/__init__.py
 tests/conftest.py
 tests/test_data.json
 tests/test_device.py
 tests/test_deviceapi.py
 tests/test_network.py
 tests/test_plcnetapi.py
-tests/test_profobuf.py
 tests/fixtures/__init__.py
-tests/fixtures/device.py
 tests/fixtures/device_api.py
 tests/fixtures/plcnet_api.py
-tests/fixtures/protobuf.py
 tests/mocks/__init__.py
-tests/mocks/mock_device.py
-tests/mocks/mock_zeroconf.py
-tests/stubs/__init__.py
-tests/stubs/protobuf.py
-tests/stubs/zeroconf.py
+tests/mocks/zeroconf.py
+tests/snapshots/test_device.ambr
```

### Comparing `devolo_plc_api-1.3.0/docs/CHANGELOG.md` & `devolo_plc_api-1.3.1/docs/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [v1.3.1] - 2023/05/12
+
+### Fixed
+
+- Reduce zeroconf traffic
+
 ## [v1.3.0] - 2023/04/13
 
 ### Added
 
 - Get MultiAP information from the device
 
 ### Fixed
```

### Comparing `devolo_plc_api-1.3.0/docs/CODE_OF_CONDUCT.md` & `devolo_plc_api-1.3.1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/docs/CONTRIBUTING.md` & `devolo_plc_api-1.3.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/example_async.py` & `devolo_plc_api-1.3.1/example_async.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/example_sync.py` & `devolo_plc_api-1.3.1/example_sync.py`

 * *Files identical despite different names*

### Comparing `devolo_plc_api-1.3.0/pyproject.toml` & `devolo_plc_api-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 description = "devolo PLC devices in Python"
 dependencies = [
+    "ifaddr>=0.1.7",
     "httpx>=0.21.0",
-    "protobuf",
+    "protobuf>=4.22.0",
     "zeroconf>=0.32.0",
 ]
 dynamic = [
     "version",
 ]
 license = { file = "LICENSE" }
 name = "devolo_plc_api"
@@ -34,14 +35,15 @@
 ]
 test = [
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-httpx>=0.18.0",
     "typing-extensions",
+    "syrupy",
 ]
 
 [tool.black]
 line-length = 127
 force-exclude = '.*_pb2\.py|.*\.pyi'
 
 [tool.isort]
@@ -56,24 +58,24 @@
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.ruff]
 exclude = ["*_pb2.py", "*.pyi"]
-ignore = ["ANN101", "ANN401", "COM812", "D203", "D205", "D212", "FBT", "N818", "TCH"]
+ignore = ["ANN101", "ANN401", "COM812", "D203", "D205", "D212", "FBT001", "N818", "TCH"]
 line-length = 127
 select = ["ALL"]
 target-version = "py38"
 
 [tool.ruff.isort]
 combine-as-imports = true
 forced-separate = ["tests"]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["ANN201", "ARG", "PLR2004", "PT004", "PT012", "S", "SLF001"]
-"script/*" = ["INP001"]
+"scripts/*" = ["INP001"]
 
 [tool.setuptools]
 packages = { find = {exclude=["docs*", "script*", "tests*"]} }
 
 [tool.setuptools_scm]
```

### Comparing `devolo_plc_api-1.3.0/script/stubgen.py` & `devolo_plc_api-1.3.1/scripts/stubgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,26 +25,29 @@
 """
 '''
 
 
 class ApiStubGenerator(StubGenerator):
     """Generate stub text from a mypy AST."""
 
-    def get_str_type_of_node(self, rvalue: Expression, can_infer_optional: bool = False, can_be_any: bool = True) -> str:
+    def get_str_type_of_node(self, rvalue: Expression, *, can_infer_optional: bool = False, can_be_any: bool = True) -> str:
         """Get type of node as string."""
         if isinstance(rvalue, ConditionalExpr):
-            if_type = self.get_str_type_of_node(rvalue.if_expr, can_infer_optional, False)
-            else_type = self.get_str_type_of_node(rvalue.else_expr, can_infer_optional, False)
+            if_type = self.get_str_type_of_node(rvalue.if_expr, can_infer_optional=can_infer_optional, can_be_any=False)
+            else_type = self.get_str_type_of_node(rvalue.else_expr, can_infer_optional=can_infer_optional, can_be_any=False)
             if if_type and else_type and if_type != else_type:
                 return f"{if_type} | {else_type}"
             return if_type or else_type or "Any" if can_be_any else ""
         if isinstance(rvalue, ListExpr):
-            list_item_type = {self.get_str_type_of_node(item, can_infer_optional, can_be_any) for item in rvalue.items}
+            list_item_type = {
+                self.get_str_type_of_node(item, can_infer_optional=can_infer_optional, can_be_any=can_be_any)
+                for item in rvalue.items
+            }
             return f"list[{' | '.join(list_item_type)}]"
-        return super().get_str_type_of_node(rvalue, can_infer_optional, can_be_any)
+        return super().get_str_type_of_node(rvalue, can_infer_optional=can_infer_optional, can_be_any=can_be_any)
 
     def add_sync(self) -> None:
         """Add sync methods."""
         output = copy(self._output)
         for i in range(len(output)):
             if "async" in output[i]:
                 self.add(output[i].replace("async_", "").replace("async ", ""))
```

### Comparing `devolo_plc_api-1.3.0/tests/__init__.py` & `devolo_plc_api-1.3.1/tests/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 """Unittests for devolo_plc_api."""
 from __future__ import annotations
 
 import json
-import pathlib
 from dataclasses import dataclass
+from enum import Enum
+from pathlib import Path
+
+from syrupy.extensions.amber import AmberSnapshotExtension
+from syrupy.location import PyTestLocation
 
 from devolo_plc_api.device_api import SERVICE_TYPE as DEVICE_API
 from devolo_plc_api.plcnet_api import SERVICE_TYPE as PLCNET_API
 from devolo_plc_api.zeroconf import ZeroconfServiceInfo
 
 
+class DeviceType(Enum):
+    """Different device types."""
+
+    REPEATER = 1
+    PLC = 2
+
+
+class DifferentDirectoryExtension(AmberSnapshotExtension):
+    """Extention for Syrupy to change the directory in which snapshots are stored."""
+
+    @classmethod
+    def dirname(cls: type[DifferentDirectoryExtension], *, test_location: PyTestLocation) -> str:
+        """Store snapshots in `snapshots`rather than `__snapshots__`."""
+        return str(Path(test_location.filepath).parent.joinpath("snapshots"))
+
+
 @dataclass
 class TestData:
     """Test data for a devolo device."""
 
     __test__ = False
 
     ip: str
@@ -24,15 +44,15 @@
 
     device_info: dict[str, ZeroconfServiceInfo]
     """Zeroconf info a device delivers."""
 
 
 def load_test_data():
     """Load test data from file."""
-    file = pathlib.Path(__file__).parent / "test_data.json"
+    file = Path(__file__).parent / "test_data.json"
     with file.open("r") as handler:
         data = json.load(handler)
     device_info = {
         DEVICE_API: ZeroconfServiceInfo(hostname=data["hostname"], **data["device_info"][DEVICE_API]),
         PLCNET_API: ZeroconfServiceInfo(**data["device_info"][PLCNET_API]),
     }
     return TestData(ip=data["ip"], hostname=data["hostname"], device_info=device_info)
```

### Comparing `devolo_plc_api-1.3.0/tests/conftest.py` & `devolo_plc_api-1.3.1/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,82 @@
 """Test configuration."""
 from __future__ import annotations
 
-import asyncio
-from typing import Generator
-from unittest.mock import AsyncMock, patch
+from collections import OrderedDict
+from functools import partial
+from typing import AsyncGenerator, Generator
+from unittest.mock import AsyncMock, Mock, patch
 
 import pytest
+import pytest_asyncio
+from ifaddr import IP, Adapter
+from syrupy.assertion import SnapshotAssertion
 
-from . import TestData, load_test_data
-from .mocks.mock_zeroconf import MockServiceBrowser
+from devolo_plc_api import Device
+
+from . import DeviceType, DifferentDirectoryExtension, TestData, load_test_data
+from .mocks.zeroconf import MockAsyncServiceInfo, MockServiceBrowser
 
 pytest_plugins = [
-    "tests.fixtures.device",
     "tests.fixtures.device_api",
     "tests.fixtures.plcnet_api",
-    "tests.fixtures.protobuf",
 ]
 
 
-def pytest_configure(config: pytest.Config):
-    """Configure pytest."""
-    config.addinivalue_line("markers", "allow_sleep: mark tests that are allowed to sleep")
-
-
 @pytest.fixture(scope="session")
 def test_data() -> TestData:
     """Load test data."""
     return load_test_data()
 
 
-@pytest.fixture(name="sleep", autouse=True)
-def patch_sleep(request: pytest.FixtureRequest) -> Generator[AsyncMock | None, None, None]:
+@pytest.fixture()
+def block_communication() -> Generator[None, None, None]:
+    """Block external communication."""
+    adapter = OrderedDict()
+    adapter["eth0"] = Adapter(name="eth0", nice_name="eth0", ips=[IP("192.0.2.100", network_prefix=24, nice_name="eth0")])
+    with patch("devolo_plc_api.device.get_adapters", return_value=adapter.values()), patch(
+        "devolo_plc_api.device.AsyncZeroconf", AsyncMock
+    ), patch("devolo_plc_api.device.AsyncServiceInfo", MockAsyncServiceInfo):
+        yield
+
+
+@pytest_asyncio.fixture()
+async def http_client() -> AsyncGenerator[None, None]:
+    """Patch HTTP client."""
+    with patch("devolo_plc_api.device.AsyncClient", autospec=True):
+        yield
+
+
+@pytest.fixture()
+def mock_device(test_data: TestData) -> Device:
+    """Generate a device from test data."""
+    return Device(ip=test_data.ip)
+
+
+@pytest.fixture()
+def mock_info_from_service() -> Generator[Mock, None, None]:
+    """Patch reading info from mDNS entries."""
+    with patch("devolo_plc_api.device.Device.info_from_service") as ifs:
+        yield ifs
+
+
+@pytest.fixture(name="sleep")
+def patch_sleep() -> Generator[AsyncMock, None, None]:
     """Don't sleep anywhere except if marked as allowed."""
-    if "allow_sleep" not in request.keywords:
-        with patch("time.sleep"), patch("asyncio.sleep") as sleep:
-            yield sleep
-    else:
-        yield None
+    with patch("time.sleep"), patch("asyncio.sleep") as sleep:
+        yield sleep
 
 
 @pytest.fixture()
-def block_communication() -> Generator[None, None, None]:
-    """Block external communication."""
-    with patch("devolo_plc_api.device.AsyncZeroconf", AsyncMock), patch("devolo_plc_api.device.AsyncClient", AsyncMock), patch(
-        "devolo_plc_api.device.AsyncServiceBrowser", MockServiceBrowser
-    ), patch("devolo_plc_api.device.AsyncServiceInfo"), patch("devolo_plc_api.network.Zeroconf"), patch(
-        "devolo_plc_api.network.ServiceBrowser", MockServiceBrowser
+def service_browser(device_type: DeviceType) -> Generator[None, None, None]:
+    """Patch mDNS service browser."""
+    service_browser = partial(MockServiceBrowser, device_type=device_type)
+    with patch("devolo_plc_api.device.AsyncServiceBrowser", service_browser), patch(
+        "devolo_plc_api.network.ServiceBrowser", service_browser
     ):
         yield
 
 
 @pytest.fixture()
-def event_loop() -> Generator[asyncio.events.AbstractEventLoop, None, None]:
-    """Handle the event loop in tests."""
-    loop = asyncio.new_event_loop()
-    yield loop
-    if loop.is_running():
-        to_cancel = asyncio.tasks.all_tasks(loop)
-        for task in to_cancel:
-            task.cancel()
-        loop.run_until_complete(asyncio.tasks.gather(*to_cancel, return_exceptions=True))
-        loop.close()
+def snapshot(snapshot: SnapshotAssertion) -> SnapshotAssertion:
+    """Return snapshot assertion fixture with nicer path."""
+    return snapshot.use_extension(DifferentDirectoryExtension)
```

### Comparing `devolo_plc_api-1.3.0/tests/fixtures/device_api.py` & `devolo_plc_api-1.3.1/tests/fixtures/device_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Fixtures for device API tests."""
 from __future__ import annotations
 
 from secrets import randbelow
-from typing import AsyncGenerator, Generator
-from unittest.mock import patch
+from typing import AsyncGenerator
 
 import pytest
 import pytest_asyncio
 from httpx import AsyncClient
 
 from devolo_plc_api.device_api import (
     SERVICE_TYPE,
@@ -26,21 +25,14 @@
 async def device_api(test_data: TestData, feature: str) -> AsyncGenerator[DeviceApi, None]:
     """Yield a prepared DeviceApi object."""
     test_data.device_info[SERVICE_TYPE].properties["Features"] = feature
     async with AsyncClient() as client:
         yield DeviceApi(test_data.ip, client, test_data.device_info[SERVICE_TYPE])
 
 
-@pytest.fixture()
-def mock_device_api() -> Generator[None, None, None]:
-    """Mock a DeviceApi object."""
-    with patch("devolo_plc_api.device_api.deviceapi.DeviceApi"):
-        yield
-
-
 @pytest.fixture(scope="session")
 def connected_station() -> ConnectedStationInfo:
     """Generate a mocked answer of a connected wifi station."""
     station = ConnectedStationInfo()
     station.mac_address = "aa:bb:cc:dd:ee:ff"
     return station
```

### Comparing `devolo_plc_api-1.3.0/tests/fixtures/plcnet_api.py` & `devolo_plc_api-1.3.1/tests/fixtures/plcnet_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Fixtures for plcnet API tests."""
-from typing import AsyncGenerator, Generator
-from unittest.mock import patch
+from typing import AsyncGenerator
 
 import pytest
 import pytest_asyncio
 from httpx import AsyncClient
 
 from devolo_plc_api.plcnet_api import SERVICE_TYPE, LogicalNetwork, PlcNetApi
 
@@ -15,17 +14,10 @@
 async def plcnet_api(test_data: TestData) -> AsyncGenerator[PlcNetApi, None]:
     """Yield a prepared PlcNetApi object."""
     async with AsyncClient() as client:
         yield PlcNetApi(test_data.ip, client, test_data.device_info[SERVICE_TYPE])
 
 
 @pytest.fixture()
-def mock_plcnet_api() -> Generator[None, None, None]:
-    """Mock a PlcNetApi object."""
-    with patch("devolo_plc_api.plcnet_api.plcnetapi.PlcNetApi"):
-        yield
-
-
-@pytest.fixture()
 def network() -> LogicalNetwork:
     """Mock a PLC network."""
     return LogicalNetwork(devices=[], data_rates=[])
```

### Comparing `devolo_plc_api-1.3.0/tests/test_data.json` & `devolo_plc_api-1.3.1/tests/test_data.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9717881944444443%*

 * *Differences: {"'device_info'": "{'_dvl-deviceapi._tcp.local.': {'properties': {'MT': '3046'}, 'address': "*

 * *                  "'192.0.2.1'}, '_dvl-plcnetapi._tcp.local.': {'address': '192.0.2.1'}}"}*

```diff
@@ -1,23 +1,25 @@
 {
     "device_info": {
         "_dvl-deviceapi._tcp.local.": {
+            "address": "192.0.2.1",
             "port": 80,
             "properties": {
                 "Features": "wifi1",
                 "FirmwareDate": "2020-06-29",
                 "FirmwareVersion": "5.5.1",
-                "MT": "2730",
+                "MT": "3046",
                 "Path": "1234567890abcdef",
                 "Product": "dLAN pro 1200+ WiFi ac",
                 "SN": "1234567890123456",
                 "Version": "v0"
             }
         },
         "_dvl-plcnetapi._tcp.local.": {
+            "address": "192.0.2.1",
             "port": 80,
             "properties": {
                 "Path": "1234567890abcdef",
                 "PlcMacAddress": "AABBCCDDEEFF",
                 "PlcTechnology": "hpav",
                 "Version": "v0"
             }
```

### Comparing `devolo_plc_api-1.3.0/tests/test_deviceapi.py` & `devolo_plc_api-1.3.1/tests/test_deviceapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """Test communicating with a the device API."""
 from __future__ import annotations
 
+from http import HTTPStatus
+
 import pytest
+from httpx import ConnectTimeout
 from pytest_httpx import HTTPXMock
 
+from devolo_plc_api import Device
 from devolo_plc_api.device_api import ConnectedStationInfo, DeviceApi, NeighborAPInfo, RepeatedAPInfo, SupportInfoItem
 from devolo_plc_api.device_api.factoryreset_pb2 import FactoryResetStart
 from devolo_plc_api.device_api.ledsettings_pb2 import LedSettingsGet, LedSettingsSetResponse
 from devolo_plc_api.device_api.multiap_pb2 import WifiMultiApGetResponse
 from devolo_plc_api.device_api.restart_pb2 import RestartResponse, UptimeGetResponse
 from devolo_plc_api.device_api.support_pb2 import SupportInfoDump, SupportInfoDumpResponse
 from devolo_plc_api.device_api.updatefirmware_pb2 import UpdateFirmwareCheck, UpdateFirmwareStart
@@ -17,15 +21,17 @@
     WifiGuestAccessSetResponse,
     WifiNeighborAPsGet,
     WifiRepeatedAPsGet,
     WifiRepeaterWpsClonePbcStart,
     WifiResult,
     WifiWpsPbcStart,
 )
-from devolo_plc_api.exceptions.feature import FeatureNotSupported
+from devolo_plc_api.exceptions import DevicePasswordProtected, DeviceUnavailable, FeatureNotSupported
+
+from . import DeviceType
 
 
 class TestDeviceApi:
     """Test devolo_plc_api.device_api.deviceapi.DeviceApi class."""
 
     @pytest.mark.parametrize("feature", ["[]"])
     def test_unsupported_feature(self, device_api: DeviceApi):
@@ -35,14 +41,35 @@
 
     @pytest.mark.parametrize("feature", [""])
     def test_feature(self, device_api: DeviceApi):
         """Test list of default features."""
         assert device_api.features == ["reset", "update", "led", "intmtg"]
 
     @pytest.mark.asyncio()
+    @pytest.mark.parametrize("device_type", [DeviceType.PLC])
+    @pytest.mark.usefixtures("block_communication", "service_browser")
+    async def test_wrong_password_type(self, httpx_mock: HTTPXMock, mock_device: Device):
+        """Test using different password hash if original password failed."""
+        await mock_device.async_connect()
+        assert mock_device.device
+        mock_device.password = "password"
+
+        httpx_mock.add_response(status_code=HTTPStatus.UNAUTHORIZED)
+        with pytest.raises(DevicePasswordProtected):
+            await mock_device.device.async_get_wifi_connected_station()
+            assert mock_device.device.password == "5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8"
+
+        httpx_mock.add_response(status_code=HTTPStatus.UNAUTHORIZED)
+        with pytest.raises(DevicePasswordProtected):
+            await mock_device.device.async_get_wifi_connected_station()
+            assert mock_device.device.password == "113459eb7bb31bddee85ade5230d6ad5d8b2fb52879e00a84ff6ae1067a210d3"
+
+        await mock_device.async_disconnect()
+
+    @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["led"])
     async def test_async_get_led_setting(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test getting LED settings asynchronously."""
         led_setting_get = LedSettingsGet(state=LedSettingsGet.LED_ON)
         httpx_mock.add_response(content=led_setting_get.SerializeToString())
         assert await device_api.async_get_led_setting()
 
@@ -55,22 +82,22 @@
 
     @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["led"])
     async def test_async_set_led_setting(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting LED settings asynchronously."""
         led_setting_set = LedSettingsSetResponse()
         httpx_mock.add_response(content=led_setting_set.SerializeToString())
-        assert await device_api.async_set_led_setting(True)
+        assert await device_api.async_set_led_setting(enable=True)
 
     @pytest.mark.parametrize("feature", ["led"])
     def test_set_led_setting(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting LED settings synchronously."""
         led_setting_set = LedSettingsSetResponse()
         httpx_mock.add_response(content=led_setting_set.SerializeToString())
-        assert device_api.set_led_setting(True)
+        assert device_api.set_led_setting(enable=True)
 
     @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["multiap"])
     async def test_async_get_wifi_multi_ap(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting LED settings asynchronously."""
         multi_ap_details = WifiMultiApGetResponse(enabled=True)
         httpx_mock.add_response(content=multi_ap_details.SerializeToString())
@@ -252,22 +279,22 @@
 
     @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["wifi1"])
     async def test_async_set_wifi_guest_access(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting wifi guest access status asynchronously."""
         wifi_guest_access_set = WifiGuestAccessSetResponse(result=WifiResult.WIFI_SUCCESS)
         httpx_mock.add_response(content=wifi_guest_access_set.SerializeToString())
-        assert await device_api.async_set_wifi_guest_access(True)
+        assert await device_api.async_set_wifi_guest_access(enable=True)
 
     @pytest.mark.parametrize("feature", ["wifi1"])
     def test_set_wifi_guest_access(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test setting wifi guest access status synchronously."""
         wifi_guest_access_set = WifiGuestAccessSetResponse(result=WifiResult.WIFI_SUCCESS)
         httpx_mock.add_response(content=wifi_guest_access_set.SerializeToString())
-        assert device_api.set_wifi_guest_access(True)
+        assert device_api.set_wifi_guest_access(enable=True)
 
     @pytest.mark.asyncio()
     @pytest.mark.parametrize("feature", ["wifi1"])
     async def test_async_get_wifi_neighbor_access_points(
         self, device_api: DeviceApi, httpx_mock: HTTPXMock, neighbor_ap: NeighborAPInfo
     ):
         """Test getting neighboring wifi access points asynchronously."""
@@ -294,7 +321,28 @@
 
     @pytest.mark.parametrize("feature", ["wifi1"])
     def test_start_wps(self, device_api: DeviceApi, httpx_mock: HTTPXMock):
         """Test starting WPS synchronously."""
         wps = WifiWpsPbcStart(result=WifiResult.WIFI_SUCCESS)
         httpx_mock.add_response(content=wps.SerializeToString())
         assert device_api.start_wps()
+
+    @pytest.mark.asyncio()
+    @pytest.mark.parametrize("device_type", [DeviceType.PLC])
+    @pytest.mark.usefixtures("block_communication", "service_browser")
+    async def test_device_unavailable(self, httpx_mock: HTTPXMock, mock_device: Device):
+        """Test device being unavailable."""
+        await mock_device.async_connect()
+        assert mock_device.device
+        httpx_mock.add_exception(ConnectTimeout(""))
+        with pytest.raises(DeviceUnavailable):
+            await mock_device.device.async_get_wifi_connected_station()
+
+    @pytest.mark.asyncio()
+    @pytest.mark.parametrize("device_type", [DeviceType.PLC])
+    @pytest.mark.usefixtures("block_communication", "service_browser")
+    async def test_attribute_error(self, mock_device: Device):
+        """Test raising on calling not existing method."""
+        await mock_device.async_connect()
+        assert mock_device.device
+        with pytest.raises(AttributeError):
+            mock_device.device.test()
```

