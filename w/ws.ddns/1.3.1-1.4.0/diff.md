# Comparing `tmp/ws.ddns-1.3.1.tar.gz` & `tmp/ws.ddns-1.4.0.tar.gz`

## Comparing `ws.ddns-1.3.1.tar` & `ws.ddns-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.coveragerc
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/CHANGES.txt
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/README.rst
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/config
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/changelog/.keep
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/src/ws/ddns/__init__.py
--rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/src/ws/ddns/update.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/src/ws/ddns/web.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/src/ws/ddns/tests/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/.gitignore
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ws_ddns-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.coveragerc
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/CHANGES.txt
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/README.rst
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/config
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/changelog/.keep
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/src/ws/ddns/__init__.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/src/ws/ddns/update.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/src/ws/ddns/web.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/src/ws/ddns/tests/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 ws.ddns-1.4.0/PKG-INFO
```

### Comparing `ws_ddns-1.3.1/CHANGES.txt` & `ws.ddns-1.4.0/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGES
 =======
 
 .. towncrier release notes start
 
+1.4.0 (2023-05-12)
+------------------
+
+Changes
++++++++
+
+- Fix config parsing after introducing totp secret parameter (totp)
+
+
 1.3.1 (2023-04-04)
 ------------------
 
 Changes
 +++++++
 
 - Switch from setup.py to pyproject.toml (wheel)
```

### Comparing `ws_ddns-1.3.1/README.rst` & `ws.ddns-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ws_ddns-1.3.1/src/ws/ddns/update.py` & `ws.ddns-1.4.0/src/ws/ddns/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
 
 class DNS(object):
 
     ZONE_INQUIRE = '0205'
     ZONE_UPDATE = '0202'
 
-    def __init__(self, url, username, password, context, totp_secret=None):
+    def __init__(self, url, username, password, context, **kw):
         self.url = url
         self.username = username
         self.password = password
         self.context = context
-        self.totp_secret = totp_secret
+        totp_secret = kw.get('totp_secret')
         if totp_secret is not None and pyotp is None:
             raise ValueError('Using totp_secret requires installing pytotp')
-        breakpoint()
+        self.totp_secret = totp_secret
 
     def post(self, xml):
         xml = serialize_xml(xml)
         log.debug('POST %s:\n%s', self.url, xml)
         response = requests.post(self.url, data=xml)
         return lxml.objectify.fromstring(response.text.encode('utf-8'))
 
@@ -66,15 +66,15 @@
         response = self.post(query)
         if not response.result.status.type == 'success':
             raise RuntimeError('Could not retrieve zone data: %s' %
                                response.result.status.find('text'))
         return response
 
     def update(self, hostname, ip):
-        parts = hostname.split('.', 1)
+        parts = hostname.split('.')
         host = '.'.join(parts[:-2])
         domain = '.'.join(parts[-2:])
 
         zone = self.get(domain).result.data.zone
 
         current = zone.xpath('//rr[name = "%s"]' % host)
         if not current:
```

### Comparing `ws_ddns-1.3.1/src/ws/ddns/web.py` & `ws.ddns-1.4.0/src/ws/ddns/web.py`

 * *Files identical despite different names*

### Comparing `ws_ddns-1.3.1/pyproject.toml` & `ws.ddns-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ws_ddns-1.3.1/PKG-INFO` & `ws.ddns-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws.ddns
-Version: 1.3.1
+Version: 1.4.0
 Summary: Update DNS settings using the Schlundtech XML-Gateway
 Project-URL: Repository, https://github.com/wosc/schlund-ddns
 Author-email: Wolfgang Schnerring <wosc@wosc.de>
 License:  BSD-3-Clause
 Requires-Python: >=3.7
 Requires-Dist: flask
 Requires-Dist: gocept-logging
@@ -90,14 +90,23 @@
 
 
 CHANGES
 =======
 
 .. towncrier release notes start
 
+1.4.0 (2023-05-12)
+------------------
+
+Changes
++++++++
+
+- Fix config parsing after introducing totp secret parameter (totp)
+
+
 1.3.1 (2023-04-04)
 ------------------
 
 Changes
 +++++++
 
 - Switch from setup.py to pyproject.toml (wheel)
```

