# Comparing `tmp/wikirate4py-1.1.6.tar.gz` & `tmp/wikirate4py-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikirate4py-1.1.6.tar", last modified: Thu Apr  6 10:00:15 2023, max compression
+gzip compressed data, was "wikirate4py-1.1.8.tar", last modified: Fri May 12 11:54:36 2023, max compression
```

## Comparing `wikirate4py-1.1.6.tar` & `wikirate4py-1.1.8.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:00:15.160251 wikirate4py-1.1.6/
--rw-rw-rw-   0        0        0    35823 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     3721 2023-04-06 10:00:15.160251 wikirate4py-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2485 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/README.rst
--rw-rw-rw-   0        0        0       87 2023-04-06 10:00:15.164273 wikirate4py-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2190 2023-04-06 09:58:29.000000 wikirate4py-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:00:15.143768 wikirate4py-1.1.6/wikirate4py/
--rw-rw-rw-   0        0        0     1124 2023-04-06 09:58:29.000000 wikirate4py-1.1.6/wikirate4py/__init__.py
--rw-rw-rw-   0        0        0    62018 2023-04-06 09:56:30.000000 wikirate4py-1.1.6/wikirate4py/api.py
--rw-rw-rw-   0        0        0      586 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/wikirate4py/cursor.py
--rw-rw-rw-   0        0        0     1675 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/wikirate4py/exceptions.py
--rw-rw-rw-   0        0        0      327 2023-04-06 09:40:13.000000 wikirate4py-1.1.6/wikirate4py/main.py
--rw-rw-rw-   0        0        0      541 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/wikirate4py/mixins.py
--rw-rw-rw-   0        0        0    18417 2023-04-05 10:25:18.000000 wikirate4py-1.1.6/wikirate4py/models.py
--rw-rw-rw-   0        0        0     2154 2023-04-04 16:58:48.000000 wikirate4py-1.1.6/wikirate4py/new_metrics.py
--rw-rw-rw-   0        0        0      859 2023-02-02 11:17:13.000000 wikirate4py-1.1.6/wikirate4py/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:00:15.160251 wikirate4py-1.1.6/wikirate4py.egg-info/
--rw-rw-rw-   0        0        0     3721 2023-04-06 10:00:15.000000 wikirate4py-1.1.6/wikirate4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-04-06 10:00:15.000000 wikirate4py-1.1.6/wikirate4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:00:15.000000 wikirate4py-1.1.6/wikirate4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-04-06 10:00:15.000000 wikirate4py-1.1.6/wikirate4py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-06 10:00:15.000000 wikirate4py-1.1.6/wikirate4py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-03 19:11:20.000000 wikirate4py-1.1.6/wikirate4py.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.413273 wikirate4py-1.1.8/
+-rw-rw-rw-   0        0        0    35823 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     3721 2023-05-12 11:54:36.413273 wikirate4py-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2485 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/README.rst
+-rw-rw-rw-   0        0        0       87 2023-05-12 11:54:36.414285 wikirate4py-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2190 2023-05-12 11:52:41.000000 wikirate4py-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.390906 wikirate4py-1.1.8/wikirate4py/
+-rw-rw-rw-   0        0        0     1124 2023-05-12 11:52:41.000000 wikirate4py-1.1.8/wikirate4py/__init__.py
+-rw-rw-rw-   0        0        0    62893 2023-05-12 11:41:45.000000 wikirate4py-1.1.8/wikirate4py/api.py
+-rw-rw-rw-   0        0        0      586 2023-05-12 11:40:36.000000 wikirate4py-1.1.8/wikirate4py/cursor.py
+-rw-rw-rw-   0        0        0     1675 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/exceptions.py
+-rw-rw-rw-   0        0        0     5953 2023-05-12 09:53:30.000000 wikirate4py-1.1.8/wikirate4py/main.py
+-rw-rw-rw-   0        0        0      541 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/mixins.py
+-rw-rw-rw-   0        0        0    18417 2023-04-05 10:25:18.000000 wikirate4py-1.1.8/wikirate4py/models.py
+-rw-rw-rw-   0        0        0     2210 2023-05-12 11:39:59.000000 wikirate4py-1.1.8/wikirate4py/msa_download_script.py
+-rw-rw-rw-   0        0        0     2154 2023-04-04 16:58:48.000000 wikirate4py-1.1.8/wikirate4py/new_metrics.py
+-rw-rw-rw-   0        0        0     5377 2023-05-10 06:47:11.000000 wikirate4py-1.1.8/wikirate4py/uk_assessed_statements.py
+-rw-rw-rw-   0        0        0      859 2023-02-02 11:17:13.000000 wikirate4py-1.1.8/wikirate4py/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-12 11:54:36.411764 wikirate4py-1.1.8/wikirate4py.egg-info/
+-rw-rw-rw-   0        0        0     3721 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-12 11:54:36.000000 wikirate4py-1.1.8/wikirate4py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-03 19:11:20.000000 wikirate4py-1.1.8/wikirate4py.egg-info/zip-safe
```

### Comparing `wikirate4py-1.1.6/LICENSE` & `wikirate4py-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/PKG-INFO` & `wikirate4py-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wikirate4py
-Version: 1.1.6
+Version: 1.1.8
 Summary: WikiRate for Python!
 Home-page: https://github.com/wikirate/wikirate4py
 Author: Vasiliki Gkatziaki
 Author-email: vasso@wikirate.org
 License: GPL-3.0
-Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.6.tar.gz
+Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz
 Project-URL: Documentation, https://wikirate4py.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/wikirate4py/wikirate4py/issues
 Project-URL: Source Code, https://github.com/wikirate4py/wikirate4py
 Keywords: wikirate library
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `wikirate4py-1.1.6/README.rst` & `wikirate4py-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/setup.py` & `wikirate4py-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       version=version,
       description='WikiRate for Python!',
       long_description=readme,
       url='https://github.com/wikirate/wikirate4py',
       author='Vasiliki Gkatziaki',
       author_email='vasso@wikirate.org',
       license='GPL-3.0',
-      download_url='https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.6.tar.gz',
+      download_url='https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz',
       packages=find_packages(exclude=["tests", "examples"]),
       install_requires=[
           "requests",
           "html2text",
           "pandas"
       ],
       project_urls={
```

### Comparing `wikirate4py-1.1.6/wikirate4py/__init__.py` & `wikirate4py-1.1.8/wikirate4py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # wikirate4py
 # Copyright 2021 Vasiliki Gkatziaki for WikiRate
 # See LICENSE for details.
 
 """
 wikirate4py WikiRate API library
 """
-__version__ = '1.1.6'
+__version__ = '1.1.8'
 __author__ = 'Vasiliki Gkatziaki'
 __license__ = 'GPL-3.0'
 
 from wikirate4py.api import API
 from wikirate4py.cursor import Cursor
 from wikirate4py.exceptions import (IllegalHttpMethod, WikiRate4PyException, HTTPException, BadRequestException,
                                     UnauthorizedException, ForbiddenException, NotFoundException,
```

### Comparing `wikirate4py-1.1.6/wikirate4py/api.py` & `wikirate4py-1.1.8/wikirate4py/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,34 @@
             :py:class:`List`\[:class:`~wikirate4py.models.Source`]
         """
         return self.get("/Sources.json", endpoint_params=('limit', 'offset'), filters=(
             'name', 'wikirate_title', 'wikirate_topic', 'report_type', 'year', 'wikirate_link', 'company_name'),
                         **kwargs)
 
     @objectify(Answer)
+    def get_answer_by(self, metric_designer, metric_name, company, year):
+        """get_answer(id)
+
+        Returns a metric answer given its numeric identifier.
+
+        Parameters
+        ----------
+        id
+            numeric identifier of the metric answer
+
+        Returns
+        -------
+            :py:class:`~wikirate4py.models.Company`
+        """
+        company = ('~' + company.__str__()) if isinstance(company, int) else company.__str__().replace(',', ' ').replace('.',
+                                                                                                        ' ').replace(
+            '/', ' ').replace('-', ' ').strip().replace(" ", "_")
+        return self.get("/{0}+{1}+{2}+{3}.json".format(metric_designer, metric_name, company, str(year)))
+
+    @objectify(Answer)
     def get_answer(self, id):
         """get_answer(id)
 
         Returns a metric answer given its numeric identifier.
 
         Parameters
         ----------
@@ -431,24 +451,24 @@
         Returns
         -------
             :py:class:`~wikirate4py.models.Company`
         """
         return self.get("/~{0}.json".format(id))
 
     @objectify(AnswerItem, True)
-    def get_answers_by_metric_id(self, metric_id, **kwargs):
-        """get_answers_by_metric_id(metric_id, *, offset, limit, year, status, company_group, country, company_id, value, value_from, value_to, \
-                       updated, updater, outliers, source, verification, project, bookmark)
+    def get_answers_by_id(self, identifier, **kwargs):
+        """get_answers_by_id(metric_id, *, offset, limit, year, status, company_group, country, company_id, value, value_from, value_to, \
+                       updated, updater, outliers, source, verification, project, bookmark, view)
 
-        Returns a list of WikiRate Answers
+        Returns a list of WikiRate Answers by id (it can be metric id, dataset id, company id or source id)
 
         Parameters
         ----------
-        metric_id
-            numeric metric identifier
+        id
+            numeric wikirate identifier
 
         offset
             default value 0, the (zero-based) offset of the first item in the collection to return
 
         limit
             default value 20, the maximum number of entries to return. If the value exceeds the maximum, then the maximum value will be used.
 
@@ -509,15 +529,15 @@
             - `bookmark`, restrict to answers you have bookmarked
             - `nobookmark`, restrict to answers you have not bookmarked
 
         Returns
         -------
         :py:class:`List`\[:class:`~wikirate4py.models.AnswerItem`]
         """
-        return self.get("/~{0}+Answer.json".format(metric_id), endpoint_params=('limit', 'offset'),
+        return self.get("/~{0}+Answer.json".format(identifier), endpoint_params=('limit', 'offset', 'view'),
                         filters=('year', 'status', 'company_group', 'country', 'value', 'value_from', 'value_to',
                                  'updated', 'company_id', 'company_name', 'dataset', 'updater', 'outliers', 'source',
                                  'verification', 'bookmark', 'published'),
                         **kwargs)
 
     @objectify(AnswerItem, True)
     def get_answers(self, metric_name, metric_designer, **kwargs):
@@ -1081,15 +1101,15 @@
 
         if isinstance(identifier, int):
             return self.post("/update/~{0}".format(identifier), params)
         else:
             return self.post("/update/{0}".format(
                 identifier.replace(',', ' ').replace('.', ' ').replace('/', ' ').replace('-', ' ').strip().replace(" ",
                                                                                                                    "_")),
-                             params)
+                params)
 
     @objectify(Answer)
     def add_research_metric_answer(self, **kwargs):
         """add_research_metric_answer(metric_designer, metric_name, company, year, value, source, *, comment)
 
         Creates and Returns a company given the company name and headquarters
 
@@ -1378,15 +1398,15 @@
         Returns
         -------
             :py:class:`~wikirate4py.models.Metric`
 
         """
         required_params = ['designer', 'name', 'metric_type', 'value_type']
         optional_params = (
-        'question', 'about', 'methodology', 'unit', 'topics', 'value_options', 'research_policy', 'report_type')
+            'question', 'about', 'methodology', 'unit', 'topics', 'value_options', 'research_policy', 'report_type')
 
         for k in required_params:
             if k not in kwargs:
                 raise WikiRate4PyException("""Invalid set of params! You need to define all the following params to create
                                 a new metric in WikiRate platform: """ + required_params.__str__())
 
         params = {
```

### Comparing `wikirate4py-1.1.6/wikirate4py/cursor.py` & `wikirate4py-1.1.8/wikirate4py/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 class Cursor(object):
 
     def __init__(self, method, per_page=20, **kwargs):
         self.method = method
         self.kwargs = kwargs
-        if per_page > 100:
-            self.per_page = 100
+        if per_page > 200:
+            self.per_page = 200
         else:
             self.per_page = per_page
 
         self.offset = 0
         self.limit = per_page
         self.items = None
```

### Comparing `wikirate4py-1.1.6/wikirate4py/exceptions.py` & `wikirate4py-1.1.8/wikirate4py/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/wikirate4py/mixins.py` & `wikirate4py-1.1.8/wikirate4py/mixins.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/wikirate4py/models.py` & `wikirate4py-1.1.8/wikirate4py/models.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/wikirate4py/new_metrics.py` & `wikirate4py-1.1.8/wikirate4py/new_metrics.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/wikirate4py/utils.py` & `wikirate4py-1.1.8/wikirate4py/utils.py`

 * *Files identical despite different names*

### Comparing `wikirate4py-1.1.6/wikirate4py.egg-info/PKG-INFO` & `wikirate4py-1.1.8/wikirate4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wikirate4py
-Version: 1.1.6
+Version: 1.1.8
 Summary: WikiRate for Python!
 Home-page: https://github.com/wikirate/wikirate4py
 Author: Vasiliki Gkatziaki
 Author-email: vasso@wikirate.org
 License: GPL-3.0
-Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.6.tar.gz
+Download-URL: https://github.com/wikirate/wikirate4py/archive/refs/tags/v1.1.8.tar.gz
 Project-URL: Documentation, https://wikirate4py.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/wikirate4py/wikirate4py/issues
 Project-URL: Source Code, https://github.com/wikirate4py/wikirate4py
 Keywords: wikirate library
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

