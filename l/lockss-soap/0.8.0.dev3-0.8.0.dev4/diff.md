# Comparing `tmp/lockss_soap-0.8.0.dev3.tar.gz` & `tmp/lockss_soap-0.8.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockss_soap-0.8.0.dev3.tar", max compression
+gzip compressed data, was "lockss_soap-0.8.0.dev4.tar", max compression
```

## Comparing `lockss_soap-0.8.0.dev3.tar` & `lockss_soap-0.8.0.dev4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2084 2023-05-11 16:22:26.475340 lockss_soap-0.8.0.dev3/CHANGELOG.rst
--rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_soap-0.8.0.dev3/LICENSE
--rw-r--r--   0        0        0     3165 2023-05-02 07:01:49.696347 lockss_soap-0.8.0.dev3/README.rst
--rw-r--r--   0        0        0     1090 2023-05-11 22:28:34.429792 lockss_soap-0.8.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     4174 2023-05-11 22:28:48.806471 lockss_soap-0.8.0.dev3/src/lockss/soap/__init__.py
--rw-r--r--   0        0        0    31684 2023-05-03 04:37:57.799706 lockss_soap-0.8.0.dev3/src/lockss/soap/cli.py
--rw-r--r--   0        0        0    20866 2023-05-11 20:30:39.806045 lockss_soap-0.8.0.dev3/src/lockss/soap/daemon_status_service.py
--rw-r--r--   0        0        0    11798 2023-05-11 22:28:15.863111 lockss_soap-0.8.0.dev3/src/lockss/soap/util.py
--rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 lockss_soap-0.8.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     2084 2023-05-11 16:22:26.475340 lockss_soap-0.8.0.dev4/CHANGELOG.rst
+-rw-r--r--   0        0        0     1506 2023-03-07 22:41:03.875719 lockss_soap-0.8.0.dev4/LICENSE
+-rw-r--r--   0        0        0     3165 2023-05-02 07:01:49.696347 lockss_soap-0.8.0.dev4/README.rst
+-rw-r--r--   0        0        0     1090 2023-05-12 16:45:22.577672 lockss_soap-0.8.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     4174 2023-05-12 16:45:14.201001 lockss_soap-0.8.0.dev4/src/lockss/soap/__init__.py
+-rw-r--r--   0        0        0    32056 2023-05-12 16:43:42.587615 lockss_soap-0.8.0.dev4/src/lockss/soap/cli.py
+-rw-r--r--   0        0        0    19921 2023-05-12 00:49:56.561767 lockss_soap-0.8.0.dev4/src/lockss/soap/daemon_status_service.py
+-rw-r--r--   0        0        0    12108 2023-05-12 16:36:26.113957 lockss_soap-0.8.0.dev4/src/lockss/soap/util.py
+-rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 lockss_soap-0.8.0.dev4/PKG-INFO
```

### Comparing `lockss_soap-0.8.0.dev3/CHANGELOG.rst` & `lockss_soap-0.8.0.dev4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `lockss_soap-0.8.0.dev3/LICENSE` & `lockss_soap-0.8.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `lockss_soap-0.8.0.dev3/README.rst` & `lockss_soap-0.8.0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `lockss_soap-0.8.0.dev3/pyproject.toml` & `lockss_soap-0.8.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lockss-soap"
-version = "0.8.0-dev3"
+version = "0.8.0-dev4"
 description = "Library and command line tools to interact with legacy LOCKSS SOAP interfaces"
 license = "BSD-3-Clause"
 authors = [
     "Thib Guicherd-Callin <thib@cs.stanford.edu>"
 ]
 readme = "README.rst"
 homepage = "https://www.lockss.org/"
```

### Comparing `lockss_soap-0.8.0.dev3/src/lockss/soap/__init__.py` & `lockss_soap-0.8.0.dev4/src/lockss/soap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = '0.8.0-dev3'
+__version__ = '0.8.0-dev4'
 
 __copyright__ = '''
 Copyright (c) 2000-2023, Board of Trustees of Leland Stanford Jr. University
 '''.strip()
 
 __license__ = __copyright__ + '\n\n' + '''
 Redistribution and use in source and binary forms, with or without
```

### Comparing `lockss_soap-0.8.0.dev3/src/lockss/soap/cli.py` & `lockss_soap-0.8.0.dev4/src/lockss/soap/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,32 +248,34 @@
                 data[(*t, field)] = AU_STATUS[field][1](r)
         _do(lockss.soap.daemon_status_service.get_au_status,
             [(node_object, auid) for auid in auids for node_object in node_objects],
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
+        headers = [] if self._get_skip_headers() else ['AUID', *[f'{node_object}\n{AU_STATUS[field][0]}' for node_object, field in itertools.product(node_objects, fields)]]
         print(tabulate.tabulate([[auid, *[data.get((node_object, auid, field)) for node_object, field in itertools.product(node_objects, fields)]] for auid in sorted(auids)],
-                                headers=['AUID', *[f'{node_object}\n{AU_STATUS[field][0]}' for node_object, field in itertools.product(node_objects, fields)]],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
     def _get_au_urls(self):
         node_objects = [lockss.soap.node(node_ref, self._get_username(), self._get_password()) for node_ref in self._get_nodes()]
         auids = self._get_auids()
         data = dict()
         def __result_func(t, r):
             data[t] = r
         _do(lockss.soap.daemon_status_service.get_au_urls,
             [(node_object, auid) for auid in auids for node_object in node_objects],
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
+        headers = [] if self._get_skip_headers() else ['AUID', *[node_object for node_object in node_objects]]
         print(tabulate.tabulate([[auid, *['\n'.join(data.get((node_object, auid), [])) for node_object in node_objects]] for auid in sorted(auids)],
-                                headers=['AUID', *[node_object for node_object in node_objects]],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
     def _get_auids(self):
         if self._auids is None:
             self._auids = list()
             self._auids.extend(self._args.auid)
             for path in self._args.auids:
@@ -293,16 +295,17 @@
         _do(lockss.soap.daemon_status_service.get_auids,
             itertools.product(node_objects),
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
         names = self._args.names
+        headers = [] if self._get_skip_headers() else [*(['AUID', 'AU Name'] if names else ['AUID']), *[node_object for node_object in node_objects]]
         print(tabulate.tabulate([[*([auid, name] if names else [auid]), *[data.get((node_object, auid), False) for node_object in node_objects]] for auid, name in sorted(all_auids.items())],
-                                headers=[*(['AUID', 'AU Name'] if names else ['AUID']), *[node_object for node_object in node_objects]],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
     def _get_platform_configuration(self):
         node_objects = [lockss.soap.node(node_ref, self._get_username(), self._get_password()) for node_ref in self._get_nodes()]
         fields = self._args.select if self._args.select and len(self._args.select) > 0 else PLATFORM_CONFIGURATION.keys()
         data = dict()
         def __result_func(t, r):
@@ -310,16 +313,17 @@
                 data[(*t, field)] = PLATFORM_CONFIGURATION[field][1](r)
         _do(lockss.soap.daemon_status_service.get_platform_configuration,
             itertools.product(node_objects),
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
+        headers = [] if self._get_skip_headers() else ['Field', *[node_object.get_url() for node_object in node_objects]]
         print(tabulate.tabulate([[PLATFORM_CONFIGURATION[field][0], *[data.get((node_object, field)) for node_object in node_objects]] for field in fields],
-                                headers=['Field', *[node_object.get_url() for node_object in node_objects]],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
     def _handle_exception(self, tup, exc):
         if self._args.verbose:
             traceback.print_exception(exc)
         else:
             print(f'error on {tup}: {exc}', file=sys.stderr)
@@ -332,16 +336,17 @@
             data[t[0]] = r
         _do(lockss.soap.daemon_status_service.is_daemon_ready,
             itertools.product(node_objects),
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
+        headers = [] if self._get_skip_headers() else ['Node', 'Ready']
         print(tabulate.tabulate([[node_object, data.get(node_object)] for node_object in node_objects],
-                                headers=['Node', 'Ready'],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
     def _make_option_names(self, container):
         container.add_argument('--names',
                                action='store_true',
                                help='also output AU names')
 
@@ -506,14 +511,15 @@
                     data[(t[0], auid, field)] = query_mapping[field][1](row)
         _do(target,
             [(node_object, select_auid_first, where) for node_object in node_objects],
             __result_func,
             self._handle_exception,
             not self._args.process_pool,
             self._args.pool_size)
+        headers = [] if self._get_skip_headers() else ['AUID', *[f'{node_object}\n{query_mapping[field][0]}' for node_object, field in itertools.product(node_objects, requested_fields)]]
         print(tabulate.tabulate([[auid, *[data.get((node_object, auid, field)) for node_object, field in itertools.product(node_objects, requested_fields)]] for auid in sorted(all_auids)],
-                                headers=['AUID', *[f'{node_object}\n{query_mapping[field][0]}' for node_object, field in itertools.product(node_objects, requested_fields)]],
+                                headers=headers,
                                 tablefmt=self._args.output_format))
 
 
 def daemon_status_service():
     DaemonStatusServiceCli().run()
```

### Comparing `lockss_soap-0.8.0.dev3/src/lockss/soap/daemon_status_service.py` & `lockss_soap-0.8.0.dev4/src/lockss/soap/daemon_status_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -450,49 +450,39 @@
     with attributes among these:
 
     *  ``activeRepairCount`` (numeric)
     *  ``activeRepairs``, a list of records with these attributes:
        *  ``peerId`` (string)
        *  ``url`` (string)
     *  ``additionalInfo`` (string)
+    *  ``agreedUrlCount`` (numeric)
+    *  ``agreedUrls`` (list of strings)
+    *  ``auId`` (string)
+    *  ``auName`` (string)
+    *  ``bytesHashedCount`` (numeric)
+    *  ``bytesReadCount`` (numeric)
+    *  ``completedRepairCount`` (numeric)
+    *  ``completedRepairs``, a list of records with these attributes:
+       *  ``peerId`` (string)
+       *  ``url`` (string)
+    *  ``deadline`` (numeric)
+    *  ``disagreedUrlCount`` (numeric)
+    *  ``disagreedUrls`` (list of strings)
+    *  ``duration`` (numeric)
+    *  ``endTime`` (numeric)
+    *  ``errorDetail`` (string)
+    *  ``errorUrls``, a list of records with these attributes:
+       *  ``entry``, a record with these attributes:
+          *  ``key`` (string)
+          *  ``value`` (string)
+    *  ``hashErrorCount`` (numeric)
+    *  ``noQuorumUrlCount`` (numeric)
+    *  ``noQuorumUrls`` (list of strings)
+    *  ``participantCount`` (numeric)
 
-<xs:element maxOccurs="unbounded" minOccurs="0" name="activeRepairs" nillable="true" type="tns:repairWsResult"/>
-<xs:element minOccurs="0" name="additionalInfo" type="xs:string"/>
-<xs:element minOccurs="0" name="agreedUrlCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="agreedUrls" nillable="true" type="xs:string"/>
-<xs:element minOccurs="0" name="auId" type="xs:string"/>
-<xs:element minOccurs="0" name="auName" type="xs:string"/>
-<xs:element minOccurs="0" name="bytesHashedCount" type="xs:long"/>
-<xs:element minOccurs="0" name="bytesReadCount" type="xs:long"/>
-<xs:element minOccurs="0" name="completedRepairCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="completedRepairs" nillable="true" type="tns:repairWsResult"/>
-<xs:element minOccurs="0" name="deadline" type="xs:long"/>
-<xs:element minOccurs="0" name="disagreedUrlCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="disagreedUrls" nillable="true" type="xs:string"/>
-<xs:element minOccurs="0" name="duration" type="xs:long"/>
-<xs:element minOccurs="0" name="endTime" type="xs:long"/>
-<xs:element minOccurs="0" name="errorDetail" type="xs:string"/>
-<xs:element name="errorUrls">
-<xs:complexType>
-<xs:sequence>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="entry">
-<xs:complexType>
-<xs:sequence>
-<xs:element minOccurs="0" name="key" type="xs:string"/>
-<xs:element minOccurs="0" name="value" type="xs:string"/>
-</xs:sequence>
-</xs:complexType>
-</xs:element>
-</xs:sequence>
-</xs:complexType>
-</xs:element>
-<xs:element minOccurs="0" name="hashErrorCount" type="xs:int"/>
-<xs:element minOccurs="0" name="noQuorumUrlCount" type="xs:int"/>
-<xs:element maxOccurs="unbounded" minOccurs="0" name="noQuorumUrls" nillable="true" type="xs:string"/>
-<xs:element minOccurs="0" name="participantCount" type="xs:int"/>
 <xs:element maxOccurs="unbounded" minOccurs="0" name="participants" nillable="true" type="tns:participantWsResult"/>
 <xs:element minOccurs="0" name="percentAgreement" type="xs:float"/>
 <xs:element minOccurs="0" name="pollKey" type="xs:string"/>
 <xs:element minOccurs="0" name="pollStatus" type="xs:string"/>
 <xs:element minOccurs="0" name="pollVariant" type="xs:string"/>
 <xs:element minOccurs="0" name="quorum" type="xs:int"/>
 <xs:element minOccurs="0" name="remainingTime" type="xs:long"/>
```

### Comparing `lockss_soap-0.8.0.dev3/src/lockss/soap/util.py` & `lockss_soap-0.8.0.dev4/src/lockss/soap/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,33 +185,42 @@
         return self._nodes
 
     def _get_password(self):
         if not self._args.password:
             self._args.password = getpass.getpass('UI password: ')
         return self._args.password
 
+    def _get_skip_headers(self):
+        return self._args.skip_headers
+
     def _get_username(self):
         if not self._args.username:
             self._args.username = getpass.getpass('UI username: ')
         return self._args.username
 
+    def _get_verbose(self):
+        return self._args.verbose
+
     def _license(self):
         print(lockss.soap.__license__)
 
     def _make_option_debug_cli(self, container):
         container.add_argument('--debug-cli',
                                action='store_true',
                                help='print the result of parsing command line arguments')
 
     def _make_option_output_format(self, container):
-        container.add_argument('--output-format',
+        container.add_argument('--output-format', '-f',
                                metavar='FMT',
                                choices=tabulate.tabulate_formats,
                                default='simple',
                                help='set tabular output format to %(metavar)s (default: %(default)s; choices: %(choices)s)')
+        container.add_argument('--skip-headers',
+                               action='store_true',
+                               help='skip tabular output headers')
 
     def _make_option_verbose(self, container):
         container.add_argument('--verbose', '-v',
                                action='store_true',
                                help='print verbose error messages')
 
     def _make_options_job_pool(self, container):
```

### Comparing `lockss_soap-0.8.0.dev3/PKG-INFO` & `lockss_soap-0.8.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockss-soap
-Version: 0.8.0.dev3
+Version: 0.8.0.dev4
 Summary: Library and command line tools to interact with legacy LOCKSS SOAP interfaces
 Home-page: https://www.lockss.org/
 License: BSD-3-Clause
 Author: Thib Guicherd-Callin
 Author-email: thib@cs.stanford.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

