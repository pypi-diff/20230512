# Comparing `tmp/infrasonar-0.1.8.tar.gz` & `tmp/infrasonar-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrasonar-0.1.8.tar", last modified: Wed May 10 18:56:00 2023, max compression
+gzip compressed data, was "infrasonar-0.1.9.tar", last modified: Fri May 12 08:38:54 2023, max compression
```

## Comparing `infrasonar-0.1.8.tar` & `infrasonar-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.714298 infrasonar-0.1.8/.github/
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 infrasonar-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/.github/workflows/
--rw-rw-r--   0 joente    (1000) joente    (1000)      690 2023-02-23 15:19:16.000000 infrasonar-0.1.8/.github/workflows/ci.yml
--rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 infrasonar-0.1.8/.gitignore
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 infrasonar-0.1.8/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-10 18:56:00.718298 infrasonar-0.1.8/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     2413 2023-02-27 08:16:16.000000 infrasonar-0.1.8/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/bin/
--rwxrwxr-x   0 joente    (1000) joente    (1000)    40006 2023-05-10 18:49:43.000000 infrasonar-0.1.8/bin/infrasonar
--rw-rw-r--   0 joente    (1000) joente    (1000)      269 2022-12-29 15:38:21.000000 infrasonar-0.1.8/example.yaml
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-10 18:56:00.718298 infrasonar-0.1.8/infrasonar.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      355 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       39 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-10 18:56:00.000000 infrasonar-0.1.8/infrasonar.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       39 2022-12-29 15:47:18.000000 infrasonar-0.1.8/requirements.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-10 18:56:00.722298 infrasonar-0.1.8/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1707 2023-05-10 18:49:52.000000 infrasonar-0.1.8/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.718755 infrasonar-0.1.9/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.714755 infrasonar-0.1.9/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.718755 infrasonar-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 infrasonar-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 infrasonar-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.718755 infrasonar-0.1.9/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      690 2023-02-23 15:19:16.000000 infrasonar-0.1.9/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1203 2019-07-16 19:49:06.000000 infrasonar-0.1.9/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2020-01-31 09:24:30.000000 infrasonar-0.1.9/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-12 08:38:54.718755 infrasonar-0.1.9/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2413 2023-02-27 08:16:16.000000 infrasonar-0.1.9/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.718755 infrasonar-0.1.9/bin/
+-rwxrwxr-x   0 joente    (1000) joente    (1000)    38643 2023-05-12 08:37:48.000000 infrasonar-0.1.9/bin/infrasonar
+-rw-rw-r--   0 joente    (1000) joente    (1000)      269 2022-12-29 15:38:21.000000 infrasonar-0.1.9/example.yaml
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-12 08:38:54.718755 infrasonar-0.1.9/infrasonar.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3089 2023-05-12 08:38:54.000000 infrasonar-0.1.9/infrasonar.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      355 2023-05-12 08:38:54.000000 infrasonar-0.1.9/infrasonar.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-12 08:38:54.000000 infrasonar-0.1.9/infrasonar.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       39 2023-05-12 08:38:54.000000 infrasonar-0.1.9/infrasonar.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-12 08:38:54.000000 infrasonar-0.1.9/infrasonar.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       39 2022-12-29 15:47:18.000000 infrasonar-0.1.9/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-12 08:38:54.718755 infrasonar-0.1.9/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1707 2023-05-12 08:37:53.000000 infrasonar-0.1.9/setup.py
```

### Comparing `infrasonar-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `infrasonar-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `infrasonar-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/.github/workflows/ci.yml` & `infrasonar-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/.gitignore` & `infrasonar-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/LICENSE` & `infrasonar-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/PKG-INFO` & `infrasonar-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrasonar
-Version: 0.1.8
+Version: 0.1.9
 Summary: InfraSonar Toolkit
 Home-page: https://github.com/infrasonar/toolkit
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: infrasonar monitoring toolkit util
 Platform: UNKNOWN
```

### Comparing `infrasonar-0.1.8/README.md` & `infrasonar-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `infrasonar-0.1.8/bin/infrasonar` & `infrasonar-0.1.9/bin/infrasonar`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import yamlloader
 from aiohttp import ClientSession
 from collections import OrderedDict
 from dataclasses import dataclass
 from setproctitle import setproctitle
 from typing import Any, Optional, Dict, List, Tuple
 
-__version__ = '0.1.8'  # Update version in setup as well
+__version__ = '0.1.9'  # Update version in setup as well
 
 
 _labels_example = """
 Invalid "labels". Expecting something like:
 
 labels:
   dns: 1409
@@ -66,18 +66,19 @@
 
 _kinds = (
     'Asset',
     'APC',
     'Apple',
     'Azure',
     'Citrix',
-    'Dell',
     'DNS',
+    'Dell',
     'Docker',
     'Eaton',
+    'Email',
     'Firewall',
     'FreeBSD',
     'HP',
     'Linux',
     'NetApp',
     'PaloAlto',
     'PureStorage',
@@ -142,187 +143,115 @@
     'kind',
     'description',
     'mode',
     'labels',
     'collectors'
 }
 _collector_keys = set(['key', 'config'])
-
-_spaces = re.compile(r'\s+')
-_uri = re.compile(r'https?:\/\/.+')
 _extract_name = re.compile(r'\w+')
 
 
-def _test_use(o: Any, key: str, prop: str):
-    if not isinstance(o, str) or _spaces.search(o):
-        sys.exit(
-            f'Option "_use" ({key}) must be a string without '
-            'whitespace or null')
+def _test_bool(o: Any, key: str, prop: str):
+    if not isinstance(o, bool):
+        sys.exit(f'Option "{prop}" ({key}) must be a boolean value')
 
 
-def _test_name_servers(o: Any, key: str, prop: str):
-    if not isinstance(o, list) or \
-            not len(o) or \
-            not all([
-                isinstance(obj, str) and not _spaces.search(obj)
-                for obj in o]) or \
-            len(set(o)) != len(o):
-        sys.exit(
-            f'Option "nameServers" ({key}) is required and must be a list '
-            'with unique and at least one nameserver')
+def _test_int(o: Any, key: str, prop: str):
+    if not isinstance(o, int):
+        sys.exit(f'Option "{prop}" ({key}) must be a integer value')
 
 
-def _test_fqdn(o: Any, key: str, prop: str):
-    if not isinstance(o, str):
-        sys.exit(f'Option "fqdn" ({key}) must be a string or null')
+def _test_float(o: Any, key: str, prop: str):
+    if not isinstance(o, float):
+        sys.exit(f'Option "{prop}" ({key}) must be a floating point value')
 
 
-def _test_address(o: Any, key: str, prop: str):
-    if not isinstance(o, str) or _spaces.search(o):
-        sys.exit(
-            f'Option "address" ({key}) must be a string without '
-            'whitespace or null')
+def _test_string(o: Any, key: str, prop: str):
+    if not isinstance(o, str):
+        sys.exit(f'Option "{prop}" ({key}) must be a string value')
 
 
-def _test_interval(o: Any, key: str, prop: str):
-    if not isinstance(o, int) or not (1 <= o <= 9):
+def _test_listbool(o: Any, key: str, prop: str):
+    if not isinstance(o, list) or \
+            not all([isinstance(obj, bool) for obj in o]):
         sys.exit(
-            f'Option "interval" ({key}) must be an interger value '
-            'between 1 and 9')
+            f'Option "{prop}" ({key}) is required and must be '
+            'a list with boolean values')
 
 
-def _test_count(o: Any, key: str, prop: str):
-    if not isinstance(o, int) or not (1 <= o <= 9):
+def _test_listint(o: Any, key: str, prop: str):
+    if not isinstance(o, list) or \
+            not all([isinstance(obj, int) for obj in o]) or \
+            len(set(o)) != len(o):
         sys.exit(
-            f'Option "count" ({key}) must be an interger value '
-            'between 1 and 9')
+            f'Option "{prop}" ({key}) is required and must be '
+            'a list with unique interger values')
 
 
-def _test_timeout(o: Any, key: str, prop: str):
-    if not isinstance(o, (float, int)) or not (0.0 <= o <= 240.0):
+def _test_listfloat(o: Any, key: str, prop: str):
+    if not isinstance(o, list) or \
+            not all([isinstance(obj, float) for obj in o]) or \
+            len(set(o)) != len(o):
         sys.exit(
-            f'Option "timeout" ({key}) must be a float value '
-            'between 0.0 and 240.0')
+            f'Option "{prop}" ({key}) is required and must be '
+            'a list with unique floating point values')
 
 
-def _test_ports(o: Any, key: str, prop: str):
+def _test_liststring(o: Any, key: str, prop: str):
     if not isinstance(o, list) or \
-            not all([
-                isinstance(obj, int) and (0 < obj <= 65535)
-                for obj in o]) or \
+            not all([isinstance(obj, str) for obj in o]) or \
             len(set(o)) != len(o):
         sys.exit(
             f'Option "{prop}" ({key}) is required and must be '
-            'a list with unique port numbers')
-
+            'a list with unique string values')
 
-def _test_port(o: Any, key: str, prop: str):
-    if not isinstance(o, int) or not (0 < o <= 65535):
-        sys.exit(
-            f'Option "port" ({key}) must be an interger value '
-            'between 1 and 65535')
 
+_TYPE_MAP = {
+    'Bool': _test_bool,
+    'Int': _test_int,
+    'Float': _test_float,
+    'String': _test_string,
+    'ListBool': _test_listbool,
+    'ListInt': _test_listint,
+    'ListFloat': _test_listfloat,
+    'ListString': _test_liststring,
+}
 
-def _test_uri(o: Any, key: str, prop: str):
-    if not isinstance(o, str) or not _uri.match(o):
-        sys.exit(
-            f'Option "uri" ({key}) must be a valid URI')
 
+async def aget_collectors(api: str, token: str, container_id: int,
+                          verify_ssl: bool):
+    args = '?field=key&options=key,type,default'
 
-def _test_bool(o: Any, key: str, prop: str):
-    if not isinstance(o, bool):
-        sys.exit(f'Option "{prop}" ({key}) must be a boolean value')
+    url = _join(api, f'container/{container_id}/collectors{args}')
+    async with ClientSession(headers=_headers(token)) as session:
+        async with session.get(url, ssl=verify_ssl) as r:
+            if r.status != 200:
+                msg = await r.text()
+                raise Exception(f'{msg} (error code: {r.status})')
+            resp = await r.json()
+            return resp
 
 
-def _test_string(o: Any, key: str, prop: str):
-    if not isinstance(o, str):
-        sys.exit(f'Option "{prop}" ({key}) must be a string value')
+_collectors = {}
 
 
-_collectors = {
-    'dns': {
-        'nameServers': (_test_name_servers, []),
-        'fqdn': (_test_fqdn, ''),
-    },
-    'docker': None,
-    'eaton': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'esx': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'hpilo': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'hpprocurve': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'http': {
-        'uri': (_test_uri, ''),
-        'timeout': (_test_timeout, 10.0),
-        'verifySSL': (_test_bool, False),
-        'withPayload': (_test_bool, False),
-        'allowRedirects': (_test_bool, False),
-    },
-    'lastseen': None,
-    'mssql': {
-        'address': (_test_address, ''),
-        'port': (_test_port, 1433),
-        '_use': (_test_use, ''),
-    },
-    'netapp': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'ping': {
-        'address': (_test_address, ''),
-        'interval': (_test_interval, 1),
-        'count': (_test_count, 5),
-        'timeout': (_test_timeout, 10.0),
-    },
-    'platform': None,
-    'santricity': {
-        'address': (_test_address, ''),
-        'port': (_test_port, 8443),
-        'storageSystemId': (_test_string, '1'),
-        '_use': (_test_use, ''),
-    },
-    'snmp': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'synology': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'tcp': {
-        'address': (_test_address, ''),
-        'checkCertificatePorts': (
-            _test_ports,
-            [443, 995, 993, 465, 3389, 989, 990, 636, 5986]
-        ),
-        'checkPorts': (_test_ports, []),
-    },
-    'unifi': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'vcenter': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
-    },
-    'wmi': {
-        'address': (_test_address, ''),
-        '_use': (_test_use, ''),
+def _load_collectos(api: str, token: str, container_id: int,
+                    verify_ssl: bool):
+    """Returns {collectorkey: {option: [verify_func, default], ..}, ..}
+    """
+    global _collectors
+
+    data = asyncio.run(aget_collectors(api, token, container_id, verify_ssl))
+    _collectors = {
+        c['key']: {
+            o['key']: (_TYPE_MAP[o['type']], o['default'])
+            for o in c['options']
+        } if c['options'] else None
+        for c in data
     }
-}
 
 
 def check_collector(collector: dict, configs: dict,
                     allow_unknown_collectors: bool):
     too_much = set(collector.keys()) - _collector_keys
     if too_much:
         sys.exit(f'Unexpected key in collector: "{too_much.pop()}"')
@@ -367,16 +296,15 @@
             sys.exit(
                 f'Unexpected property in collector {key}: "{too_much.pop()}"')
         for k, tester in validate.items():
             func, dval = tester
             func(config.get(k, dval), key, k)
 
 
-def check_asset(asset: dict, labels: dict, configs: dict,
-                allow_unknown_collectors: bool, allow_unknown_kinds: bool):
+def check_asset(asset: dict, labels: dict, allow_unknown_kinds: bool):
     too_much = set(asset.keys()) - _asset_keys
     if too_much:
         sys.exit(f'Unexpected key in asset: "{too_much.pop()}"')
 
     asset_id = asset.get('id')
     if asset_id is not None and not isinstance(asset_id, int):
         sys.exit('Asset id must be an integer')
@@ -414,25 +342,28 @@
             sys.exit('Asset labels must be a list of strings')
 
         for idx, label in enumerate(asset_labels):
             if label not in labels:
                 sys.exit(f'Asset label "{label}" missing in labels')
             asset_labels[idx] = labels[label]
 
+
+def check_asset_collectors(asset: dict, configs: dict,
+                           allow_unknown_collectors: bool):
     collectors = asset.get('collectors')
     if collectors is not None:
         if not isinstance(collectors, list) or \
                 not all([isinstance(o, dict) for o in collectors]):
             sys.exit(_collectors_example)
         for collector in collectors:
             check_collector(collector, configs, allow_unknown_collectors)
 
 
 def sanity_check(data: dict, allow_unknown_collectors: bool,
-                 allow_unknown_kinds: bool):
+                 allow_unknown_kinds: bool, api: str, verify_ssl: bool):
     too_much = set(data.keys()) - _yaml_keys
     if too_much:
         sys.exit(f'Unexpected key in yaml: "{too_much.pop()}"')
 
     token = data.get('token')
     labels = data.get('labels')
     configs = data.get('configs')
@@ -458,34 +389,33 @@
         sys.exit(_configs_example)
 
     if not isinstance(assets, list) or \
             not all([isinstance(o, dict) for o in assets]):
         sys.exit(_assets_example)
 
     for asset in assets:
-        check_asset(
-            asset,
-            labels,
-            configs,
-            allow_unknown_collectors,
-            allow_unknown_kinds)
+        check_asset(asset, labels, allow_unknown_kinds)
 
     if token is None:
         try:
             ttype = 'container'
             if container_id:
                 if all(('id' in a for a in assets)):
                     ttype = 'user or container'
 
             data['token'] = getpass.getpass(f'Enter {ttype} token: ')
         except KeyboardInterrupt:
             sys.exit('Cancelled')
     elif not isinstance(token, str):
         sys.exit('token must be a string or null')
 
+    _load_collectos(api, data['token'], container_id, verify_ssl)
+    for asset in assets:
+        check_asset_collectors(asset, configs, allow_unknown_collectors)
+
 
 def collector_by_key(asset: dict, key: str):
     collectors = asset.get('collectors')
     if collectors:
         for c in collectors:
             if c['key'] == key:
                 return {
@@ -763,15 +693,20 @@
     except Exception as e:
         msg = str(e) or type(e).__name__
         sys.exit(msg)
 
     if not isinstance(data, dict):
         sys.exit('Expecting the yaml to conain a dict')
 
-    sanity_check(data, allow_unknown_collectors, allow_unknown_kinds)
+    sanity_check(
+        data,
+        allow_unknown_collectors,
+        allow_unknown_kinds,
+        api,
+        verify_ssl)
 
     labels = data.get('labels', {})
     container_id = data.get('container', 0)
     assets = data.get('assets')
     token = data['token']
     if assets:
         aa = ApplyAssets(
@@ -939,16 +874,17 @@
                 c['key'] = collector['key']
                 config = collector['config']
 
                 if not include_defaults and config:
                     control = _collectors.get(c['key'])
                     if control is not None:
                         for k in tuple(config.keys()):
-                            if config[k] == control[k][1]:
-                                del config[k]
+                            if k in control:
+                                if config[k] == control[k][1]:
+                                    del config[k]
                 if config:
                     c['config'] = config
                 cc.append(c)
             a['collectors'] = cc
         ordered.append(a)
 
     assets.clear()
@@ -985,14 +921,17 @@
             label, not_label))
         labels = {}
         if with_labels:
             label_ids = get_label_ids(assets)
             if label_ids:
                 labels = asyncio.run(async_get_labels(
                     api, token, verify_ssl, label_ids))
+
+        _load_collectos(api, token, container_id, verify_ssl)
+
         mod_assets_res(assets, labels, include_defaults)
 
         data = OrderedDict()
         data['container'] = container_id
         if labels:
             data['labels'] = labels
 
@@ -1030,20 +969,24 @@
 
     with_labels = 'labels' in fields
 
     try:
         assets = asyncio.run(aget_asset(
             api, token, asset_id, verify_ssl, fields))
         container_id = assets[0]['container']
+
         labels = {}
         if with_labels:
             label_ids = get_label_ids(assets)
             if label_ids:
                 labels = asyncio.run(async_get_labels(
                     api, token, verify_ssl, label_ids))
+
+        _load_collectos(api, token, container_id, verify_ssl)
+
         mod_assets_res(assets, labels, include_defaults)
 
         data = OrderedDict()
         data['container'] = container_id
         if labels:
             data['labels'] = labels
```

### Comparing `infrasonar-0.1.8/infrasonar.egg-info/PKG-INFO` & `infrasonar-0.1.9/infrasonar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infrasonar
-Version: 0.1.8
+Version: 0.1.9
 Summary: InfraSonar Toolkit
 Home-page: https://github.com/infrasonar/toolkit
 Author: Jeroen van der Heijden
 Author-email: jeroen@cesbit.com
 License: GPLv3
 Keywords: infrasonar monitoring toolkit util
 Platform: UNKNOWN
```

### Comparing `infrasonar-0.1.8/setup.py` & `infrasonar-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     with open('README.md', 'r') as f:
         long_description = f.read()
 except IOError:
     long_description = ''
 
 setup(
     name='infrasonar',
-    version='0.1.8',  # Update version in infrasonar as well
+    version='0.1.9',  # Update version in infrasonar as well
     description='InfraSonar Toolkit',
     url='https://github.com/infrasonar/toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jeroen van der Heijden',
     author_email='jeroen@cesbit.com',
     scripts=['bin/infrasonar'],
```

