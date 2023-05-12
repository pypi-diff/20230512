# Comparing `tmp/marcflow-0.2.tar.gz` & `tmp/marcflow-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marcflow-0.2.tar", last modified: Mon Nov 21 00:27:00 2022, max compression
+gzip compressed data, was "marcflow-0.3.tar", last modified: Fri May 12 13:49:24 2023, max compression
```

## Comparing `marcflow-0.2.tar` & `marcflow-0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3077 2022-05-12 05:40:01.189318 marcflow-0.2/.gitignore
--rw-r--r--   0        0        0    35148 2022-05-12 05:40:56.020429 marcflow-0.2/LICENSE
--rw-r--r--   0        0        0     1357 2022-09-30 10:58:27.162130 marcflow-0.2/README.md
--rw-r--r--   0        0        0      145 2022-11-19 02:58:37.229181 marcflow-0.2/marcflow/__init__.py
--rw-r--r--   0        0        0    13870 2022-11-18 13:34:02.309200 marcflow-0.2/marcflow/marcflow.py
--rw-r--r--   0        0        0      596 2022-11-19 03:03:43.634413 marcflow-0.2/pyproject.toml
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 marcflow-0.2/PKG-INFO
+-rw-r--r--   0        0        0     3077 2022-05-12 05:40:01.189318 marcflow-0.3/.gitignore
+-rw-r--r--   0        0        0    35148 2022-05-12 05:40:56.020429 marcflow-0.3/LICENSE
+-rw-r--r--   0        0        0     1357 2022-09-30 10:58:27.162130 marcflow-0.3/README.md
+-rw-r--r--   0        0        0      145 2023-05-12 13:04:10.786872 marcflow-0.3/marcflow/__init__.py
+-rw-r--r--   0        0        0    13694 2023-04-11 05:27:25.337000 marcflow-0.3/marcflow/marcflow.py
+-rw-r--r--   0        0        0      596 2022-11-19 03:03:43.634413 marcflow-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 marcflow-0.3/PKG-INFO
```

### Comparing `marcflow-0.2/.gitignore` & `marcflow-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `marcflow-0.2/LICENSE` & `marcflow-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marcflow-0.2/README.md` & `marcflow-0.3/README.md`

 * *Files identical despite different names*

### Comparing `marcflow-0.2/marcflow/marcflow.py` & `marcflow-0.3/marcflow/marcflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,24 +82,22 @@
         except (AttributeError, UnicodeDecodeError):
             yield None
 
     def marcxml(self, source):
         if isinstance(source, str):
             source = StringIO(source)
         try:
-            namespaces = {n[0]: n[1] for _, n in Et.iterparse(
-                source, events=['start-ns'])}
             source.seek(0)
             if not (root := Et.parse(source).getroot()):
                 yield None
-            if any(root.tag == f'{{{n}}}record' for n in namespaces.values()):
-                yield self._parse_marcxml(root, namespaces)
+            if root.tag.endswith('record'):
+                yield self._parse_marcxml(root)
             else:
-                for record in root.iterfind('record', namespaces):
-                    yield self._parse_marcxml(record, namespaces)
+                for record in root.iterfind('{*}record'):
+                    yield self._parse_marcxml(record)
         except Et.ParseError:
             yield None
 
     def aleph(self, source):
         if isinstance(source, str):
             source = StringIO(source)
         try:
@@ -211,36 +209,36 @@
                 if len(sf) > 1:
                     if fh:
                         self._extract_field(tag + sf[:1], sf[1:], values)
                     if ch:
                         self._set_match(tag + ind + sf[:1], sf[1:])
         return self._get_result(values)
 
-    def _parse_marcxml(self, record, nss):
+    def _parse_marcxml(self, record):
         for condition in self._conditions:
             condition['match'] = []
         if not record:
             return None
         values = [[] for _ in range(len(self._fields))]
-        ldr = record.find('leader', nss)
-        if ldr and ldr.text:
+        ldr = record.find('{*}leader')
+        if ldr is not None and ldr.text:
             self._extract_field('LDR', ldr.text, values)
             self._set_match('LDR' + self._ANY * 3, ldr.text)
-        for cf in record.findall('controlfield', nss):
+        for cf in record.findall('{*}controlfield'):
             tag = cf.attrib.get('tag', None)
             if not tag or not cf.text:
                 continue
             if not self._is_hit(tag, self._tags['select']):
                 continue
             if tag != 'LDR' or (ldr and ldr.text != cf.text):
                 if self._is_hit(tag, self._tags['field']):
                     self._extract_field(tag, cf.text, values)
                 if self._is_hit(tag, self._tags['condition']):
                     self._set_match(tag + self._ANY * 3, cf.text)
-        for df in record.findall('datafield', nss):
+        for df in record.findall('{*}datafield'):
             if not (tag := df.attrib.get('tag', None)):
                 continue
             ind1 = df.attrib.get('ind1', ' ')
             ind2 = df.attrib.get('ind2', ' ')
             if len(tag + ind1 + ind2) != 5:
                 continue
             if not self._is_hit(tag, self._tags['select']):
```

### Comparing `marcflow-0.2/pyproject.toml` & `marcflow-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marcflow-0.2/PKG-INFO` & `marcflow-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marcflow
-Version: 0.2
+Version: 0.3
 Summary: A Python library for MARC data preprocessing
 Author: zhv
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

