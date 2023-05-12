# Comparing `tmp/ar_ex_sys_worker-1.6.20-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16230 bytes, number of entries: 11
+Zip file size: 16247 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
--rw-rw-rw-  2.0 fat    27414 b- defN 23-Apr-28 12:31 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19883 b- defN 23-Apr-25 07:19 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    27520 b- defN 23-May-11 09:20 ar_external_sys_worker/main.py
+-rw-rw-rw-  2.0 fat    19933 b- defN 23-May-11 09:20 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-Apr-28 12:31 ar_ex_sys_worker-1.6.20.dist-info/RECORD
-11 files, 62173 bytes uncompressed, 14514 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-11 09:22 ar_ex_sys_worker-1.6.21.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-May-11 09:22 ar_ex_sys_worker-1.6.21.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-11 09:22 ar_ex_sys_worker-1.6.21.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-11 09:22 ar_ex_sys_worker-1.6.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-May-11 09:22 ar_ex_sys_worker-1.6.21.dist-info/RECORD
+11 files, 62329 bytes uncompressed, 14531 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.20.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.21.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.20.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.21.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.20.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.21.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.20.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.21.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.20.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/main.py

```diff
@@ -149,16 +149,16 @@
         self.asu_polygon_name = None
         self.get_platform_url = self.get_full_endpoint("/extapi/v2/platform")
 
     def format_file_before_logging(self, data):
         data = json.loads(data)
         return str(data).replace("'", '"')
 
-    def send_unsend_acts(self):
-        data = self.get_unsend_acts()
+    def send_unsend_acts(self, record_id=None, limit=None):
+        data = self.get_unsend_acts(record_id=record_id, limit=limit)
         if not data:
             return {'error': 'no acts to send'}
         for act in data:
             response = self.send_data(act)
             asu_act_id = response.json()['id']
             photo_in = self.get_photo_path(act['ex_id'], 1)
             photo_out = self.get_photo_path(act['ex_id'], 2)
@@ -349,15 +349,14 @@
         self.act_id_from_response = 'act_id'
         if mutex:
             self.mutex = mutex
 
     def format_file_before_logging(self, data):
         data = json.loads(data)
         data.pop('photos')
-        print(data)
         return str(data).replace("'", '"')
 
     def format_alerts(self, alerts):
         if not alerts:
             return []
         res = alerts.split('&&')
         return res[:-1]
@@ -437,15 +436,16 @@
                         "kpp": act['client_kpp']},
             "trash_cat": act['trash_cat'],
             "trash_type": act['trash_type'],
             "operator_comments": {'gross_comm': act['gross_comm'],
                                     'tare_comm': act['tare_comm'],
                                     'add_comm': act['add_comm'],
                                     'changing_comm': act['changing_comm'],
-                                    'closing_comm': act['closing_comm']},
+                                    'closing_comm': act['closing_comm'],
+                                    'single_comm': act['single']},
             "photos": self.get_photos(act['ex_id']),
             "containers_plan": act['containers_plan'],
             'containers_fact': act['containers_fact'],
             "route_num": act["route_num"],
             'platform_type': act['pol_object'],
             "act_number": {'number': act['act_number'],
                            'package': act['package_name']},
```

## ar_external_sys_worker/mixins.py

```diff
@@ -390,14 +390,15 @@
                   "r.tara as tare, r.cargo, r.time_in, r.time_out, " \
                   "carrier_cji.inn as carrier_inn, carrier_cji.kpp as carrier_kpp," \
                   "client_cji.inn as client_inn, client_cji.kpp as client_kpp," \
                   "tc.name as trash_cat, " \
                   "tt.name as trash_type, oc.gross as gross_comm," \
                   "oc.tare as tare_comm, oc.additional as add_comm, " \
                   "oc.changing as changing_comm, oc.closing as closing_comm," \
+                  "oc.single as single_comm, " \
                   "dro.owner as polygon_id, ai.number as rfid, rri.route_num," \
                   "rri.containers_plan, rri.containers_fact, ra.alerts," \
                   "pol_objects.name as pol_object," \
                   "aprm.number as act_number, acts_packages.name as package_name " \
                   "FROM records r " \
                   "INNER JOIN clients carriers ON (r.carrier=carriers.id) " \
                   "INNER JOIN clients ON (r.client_id=clients.id) " \
```

## Comparing `ar_ex_sys_worker-1.6.20.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.21.dist-info/LICENSE`

 * *Files identical despite different names*

