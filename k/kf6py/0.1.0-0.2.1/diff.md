# Comparing `tmp/kf6py-0.1.0.tar.gz` & `tmp/kf6py-0.2.1.tar.gz`

## Comparing `kf6py-0.1.0.tar` & `kf6py-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kf6py-0.1.0/src/kf6py/__init__.py
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 kf6py-0.1.0/src/kf6py/api.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 kf6py-0.1.0/tests/testing.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 kf6py-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kf6py-0.1.0/LICENSE
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 kf6py-0.1.0/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 kf6py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 kf6py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kf6py-0.2.1/src/kf6py/__init__.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 kf6py-0.2.1/src/kf6py/api.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 kf6py-0.2.1/tests/testing.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 kf6py-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 kf6py-0.2.1/LICENSE
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kf6py-0.2.1/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 kf6py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 kf6py-0.2.1/PKG-INFO
```

### Comparing `kf6py-0.1.0/src/kf6py/api.py` & `kf6py-0.2.1/src/kf6py/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,16 @@
         self.login_credential = {
             'userName': username,
             'password': password
         }
         self.KF_URL = url
         self.token = self._login()
         self.author_id = None
+        self.current_community = None
+        self.temp_data = []
 
     def _login(self) -> str:
         res = requests.post(f"{self.KF_URL}/auth/local", json = self.login_credential)
         if res.status_code != 200:
             raise Exception("Something is not right", res)
 
         return res.json()['token']
@@ -38,76 +40,96 @@
         # for simplicity just use this as a starting point, no need for all information for now.
         return [{
             'id': i['communityId'], 
             'title': i['_community']['title'], 
             'created': i['created']
             } for i in res.json()]
 
-    def get_contributions(self, community_id: str, *, filter: List[str]=None) -> List[Dict[str, Any]]:
+    def get_contributions(self, community_id: str):
         """
         get all the notes in the specified `community_id`. If you are only interested in a subset of notes, you 
         can pass in additional parameter `filter` with the target note ids.
         """
+
+        if self.current_community == community_id: # don't need to retieve again, already in memory
+            return
+
         body = {
             "query": {
                 "type": "Note",
                 "pagesize": "max",
                 "status": "active"
             }
         }
         headers = self._craft_header(True)
 
         res = requests.post(f"{self.KF_URL}/api/contributions/{community_id}/search", headers = headers, json = body)
-        response = [{
+        responses = {i["_id"]: {
                 "_id": i["_id"],
                 "_type": i["type"],
                 "authors": i["authors"],
                 "title": i["title"],
                 "text4search": i["text4search"],
                 "wordCount": i['wordCount'],
                 'status': i['status'],
                 'data': i['data']['body'],
+                'riseabove_view': i['data'].get('riseabove', {}).get('viewId', None),
                 'processed_text': BeautifulSoup(i['data']['body'], 'html').get_text().strip('\n').replace(u'\xa0', u' ')
-            } for i in res.json()]
-
-        if filter:
-            return [i for i in response if i["_id"] in filter]
-        else:
-            return response
+            } for i in res.json()}
+       
+        self.current_community = community_id
+        self.temp_data = responses
+        print("contributions has been saved in the memory")
 
-
-    def get_views(self, commuitny_id: str) -> List[Dict[str, Any]]:
+    def get_views(self, community_id: str) -> List[Dict[str, Any]]:
         """
         Get the view from a particular community
         """
-        res = requests.get(f"{self.KF_URL}/api/communities/{commuitny_id}/views", headers= self._craft_header())
+        res = requests.get(f"{self.KF_URL}/api/communities/{community_id}/views", headers= self._craft_header())
         # return res.json()
         return [{
             '_id': i['_id'],
             'title': i['title'],
             'created': i['created'],
             'modified': i['modified'],
             'type': i['type']
-        } for i in res.json() if i['status'] == 'active']
+            } for i in res.json() if i['status'] == 'active']
+
+    def get_notes_from_view(self, community_id: str, view_id: str) -> List[Any]:
+        if community_id != self.current_community:
+            self.get_contributions(community_id)
 
-    def get_notes_from_view(self, community_id: str, view_id: str) -> List[str]:
         body = {
             "query": {
                 "type": "contains",
                 "from": view_id,
                 "_to.type": "Note",
                 "_to.status": "active"
             },
         }
         res = requests.post(f"{self.KF_URL}/api/links/{community_id}/search", headers= self._craft_header(), json= body)
         if res.json(): 
             print("VIEW TITLE:", res.json()[0]["_from"]["title"])
 
+        riseaboves = []
         target_ids = [i['to'] for i in res.json()]
-        return self.get_contributions(community_id, filter= target_ids)
+        result = []
+        for i in target_ids:
+            data = self.temp_data[i]
+            result.append(data)
+            
+            riseabove_view = data['riseabove_view']
+            if riseabove_view:
+                riseaboves.append(riseabove_view)
+        
+        while riseaboves:
+            ra_view_id = riseaboves.pop(0)
+            result += self.get_notes_from_view(community_id, ra_view_id)
+
+        return result
     
     def create_contribution(self, community_id: str, view_id: str, title: str, content: str):
     
         res_authors = requests.get(f"{self.KF_URL}/api/authors/{community_id}/me", headers= self._craft_header())
         self.author_id = res_authors.json()["_id"]
         contribution = {
             'communityId': community_id,
```

### Comparing `kf6py-0.1.0/LICENSE` & `kf6py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kf6py-0.1.0/pyproject.toml` & `kf6py-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 [project]
 name = "kf6py"
 dependencies = [
     'requests >=2.28, <3',
     'beautifulsoup4 >=4, <5',
 ]
-version = "0.1.0"
+version = "0.2.1"
 
 authors = [
     { name="Jerrison Chang-Sundin", email="chunyen.cs@gmail.com"}
 ]
 
-description = "A small tools for calling APIs in Knowledge Forum"
+description = "A small tool for calling APIs in Knowledge Forum"
 
 readme = "README.md"
 requires-python = ">=3.7"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

