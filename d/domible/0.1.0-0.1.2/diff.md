# Comparing `tmp/domible-0.1.0.tar.gz` & `tmp/domible-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domible-0.1.0.tar", max compression
+gzip compressed data, was "domible-0.1.2.tar", max compression
```

## Comparing `domible-0.1.0.tar` & `domible-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,24 @@
--rw-r--r--   0        0        0     1092 2023-03-11 03:03:13.785121 domible-0.1.0/LICENSE
--rw-r--r--   0        0        0     2723 2023-04-29 00:54:27.568533 domible-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3104 2023-05-08 23:08:02.712458 domible-0.1.0/README.md
--rw-r--r--   0        0        0      158 2023-04-29 01:07:39.203375 domible-0.1.0/src/dicli/__init__.py
--rw-r--r--   0        0        0      129 2023-04-29 01:00:21.616611 domible-0.1.0/src/dicli/__main__.py
--rw-r--r--   0        0        0    10917 2023-05-06 00:23:31.795415 domible-0.1.0/src/dicli/main.py
--rw-r--r--   0        0        0   253343 2023-05-02 02:58:08.016495 domible-0.1.0/src/dicli/mdn_anchor.html
--rw-r--r--   0        0        0   166180 2023-05-03 21:02:17.488872 domible-0.1.0/src/dicli/mdn_area.html
--rw-r--r--   0        0        0     8567 2023-05-06 00:23:31.795415 domible-0.1.0/src/dicli/mdnElements.py
--rw-r--r--   0        0        0      115 2023-04-25 00:46:53.366854 domible-0.1.0/src/distarter/__init__.py
--rw-r--r--   0        0        0      153 2023-04-24 23:42:47.951581 domible-0.1.0/src/distarter/__main__.py
--rw-r--r--   0        0        0     1352 2023-05-03 23:37:48.759482 domible-0.1.0/src/distarter/main.py
--rw-r--r--   0        0        0      261 2023-04-10 20:09:30.576579 domible-0.1.0/src/domible/__init__.py
--rw-r--r--   0        0        0      153 2023-04-30 22:41:17.650214 domible-0.1.0/src/domible/builders/__init__.py
--rw-r--r--   0        0        0     9135 2023-05-05 23:32:51.362410 domible-0.1.0/src/domible/builders/tableBuilder.py
--rw-r--r--   0        0        0      551 2023-05-03 23:04:16.474331 domible-0.1.0/src/domible/elements/__init__.py
--rw-r--r--   0        0        0     9001 2023-05-03 23:45:41.986174 domible-0.1.0/src/domible/elements/baseElements.py
--rw-r--r--   0        0        0     1238 2023-04-08 01:20:10.358705 domible-0.1.0/src/domible/elements/inline.py
--rw-r--r--   0        0        0     3006 2023-04-08 01:20:10.359712 domible-0.1.0/src/domible/elements/lists.py
--rw-r--r--   0        0        0     2025 2023-05-03 22:36:18.440953 domible-0.1.0/src/domible/elements/meta.py
--rw-r--r--   0        0        0     3058 2023-05-05 23:56:06.508419 domible-0.1.0/src/domible/elements/roots.py
--rw-r--r--   0        0        0     5129 2023-04-18 03:29:41.301704 domible-0.1.0/src/domible/elements/tables.py
--rw-r--r--   0        0        0      149 2023-04-30 22:45:08.280439 domible-0.1.0/src/domible/starterDocuments/__init__.py
--rw-r--r--   0        0        0      882 2023-05-05 23:58:20.728253 domible-0.1.0/src/domible/starterDocuments/basicDocuments.py
--rw-r--r--   0        0        0      544 2023-04-10 22:06:28.199360 domible-0.1.0/src/domible/utils.py
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 domible-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-03-11 03:03:13.785121 domible-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2808 2023-05-11 22:44:16.876613 domible-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3104 2023-05-08 23:08:02.712458 domible-0.1.2/README.md
+-rw-r--r--   0        0        0      334 2023-05-11 22:39:35.224699 domible-0.1.2/src/dicli/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-29 01:00:21.616611 domible-0.1.2/src/dicli/__main__.py
+-rw-r--r--   0        0        0    10917 2023-05-06 00:23:31.795415 domible-0.1.2/src/dicli/main.py
+-rw-r--r--   0        0        0     8851 2023-05-11 21:08:44.343819 domible-0.1.2/src/dicli/mdnElements.py
+-rw-r--r--   0        0        0      291 2023-05-11 22:38:34.344692 domible-0.1.2/src/distarter/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-24 23:42:47.951581 domible-0.1.2/src/distarter/__main__.py
+-rw-r--r--   0        0        0     1352 2023-05-03 23:37:48.759482 domible-0.1.2/src/distarter/main.py
+-rw-r--r--   0        0        0      261 2023-04-10 20:09:30.576579 domible-0.1.2/src/domible/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-30 22:41:17.650214 domible-0.1.2/src/domible/builders/__init__.py
+-rw-r--r--   0        0        0     9135 2023-05-05 23:32:51.362410 domible-0.1.2/src/domible/builders/tableBuilder.py
+-rw-r--r--   0        0        0      551 2023-05-03 23:04:16.474331 domible-0.1.2/src/domible/elements/__init__.py
+-rw-r--r--   0        0        0     9001 2023-05-03 23:45:41.986174 domible-0.1.2/src/domible/elements/baseElements.py
+-rw-r--r--   0        0        0     1238 2023-04-08 01:20:10.358705 domible-0.1.2/src/domible/elements/inline.py
+-rw-r--r--   0        0        0     3006 2023-04-08 01:20:10.359712 domible-0.1.2/src/domible/elements/lists.py
+-rw-r--r--   0        0        0     2025 2023-05-03 22:36:18.440953 domible-0.1.2/src/domible/elements/meta.py
+-rw-r--r--   0        0        0     3058 2023-05-05 23:56:06.508419 domible-0.1.2/src/domible/elements/roots.py
+-rw-r--r--   0        0        0     5129 2023-04-18 03:29:41.301704 domible-0.1.2/src/domible/elements/tables.py
+-rw-r--r--   0        0        0      149 2023-04-30 22:45:08.280439 domible-0.1.2/src/domible/starterDocuments/__init__.py
+-rw-r--r--   0        0        0      882 2023-05-05 23:58:20.728253 domible-0.1.2/src/domible/starterDocuments/basicDocuments.py
+-rw-r--r--   0        0        0      544 2023-04-10 22:06:28.199360 domible-0.1.2/src/domible/utils.py
+-rw-r--r--   0        0        0     3976 1970-01-01 00:00:00.000000 domible-0.1.2/PKG-INFO
```

### Comparing `domible-0.1.0/LICENSE` & `domible-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/pyproject.toml` & `domible-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domible"
-version = "0.1.0"
+version = "0.1.2"
 description = "python classes to create accessible HTML elements and documents "
 authors = ["Joel Dodson <joeldodson@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/joeldodson/domible"
 repository = "https://github.com/joeldodson/domible"
 keywords = ["html", "accessibility", "a11y", "web development", "frontend", "server side rendering", "SSR"]
@@ -16,31 +16,33 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = {version = "^4.11.2", optional = true}
 typer = {version = "^0.7.0", optional = true}
 jsonloggeriso8601datetime = {version = "^1.0.3", optional = true}
+requests = {version = "^2.30.0", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 beautifulsoup4 = "^4.11.2"
 jsonloggeriso8601datetime = "^1.0.3"
 pytest-reportlog = "^0.2.1"
 myst-nb = {version = "^0.17.2", python = "^3.9"}
 sphinx-autoapi = "^2.1.0"
 sphinx-rtd-theme = "^1.2.0"
 install = "^1.3.5"
 ruff = "^0.0.263"
+requests = "^2.30.0"
 
 [tool.poetry.extras]
-dicli = ["beautifulsoup4", "typer", "jsonloggeriso8601datetime"]
+dicli = ["beautifulsoup4", "typer", "jsonloggeriso8601datetime", "requests"]
 
 [tool.poetry.scripts]
 distarter = "distarter:run"
 dicli = { callable = "dicli:run", extras = ["dicli"] }
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version" # version location
```

### Comparing `domible-0.1.0/README.md` & `domible-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/dicli/main.py` & `domible-0.1.2/src/dicli/main.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/dicli/mdnElements.py` & `domible-0.1.2/src/dicli/mdnElements.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,25 +68,31 @@
         return False
     else:
         return True
 
 
 def getElementSummary(soup: BSoup) -> Dict:
     """
-    find the summary in the document,
+    find and return the summary in the document,
 
     NOTE: this method hard codes knowledge of the format of the document.
-    e.g., the summary is the first paragraph after the only heading 1,
+    consider the first paragraph after the main element opening tag,
+    and all its sibling paragraphs, to be the summary.
     """
-    summary = soup.find("h1").next_sibling.find("p")
-    if summary:
-        sv = summary.decode()
-    else:
-        sv = f"no summary?  that's odd.  Please open an issue at the {DomibleIssuesPage}"
-    return {"Summary": sv}
+    summary = ""
+    try:
+        p0 = soup.find("main").find("p")
+        summary = p0.decode()
+        for el in p0.next_siblings:
+            if el.name and el.name == 'p': summary += el.decode()
+            elif el.name: break
+    except Exception:
+        logger.exception("exception while getting summary")
+        summary = f"no summary?  that's odd.  Please open an issue at the {DomibleIssuesPage}"
+    return {"Summary": summary}
 
 
 def getElementSpecificationReference(soup: BSoup) -> Dict:
     """
     The element specification is in a table with a single column and two rows.
     The first row is a <thead> with a <th> with the word "Specification"
     The second row is the specification link in a <td> in a <tbody>
```

### Comparing `domible-0.1.0/src/distarter/main.py` & `domible-0.1.2/src/distarter/main.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/builders/tableBuilder.py` & `domible-0.1.2/src/domible/builders/tableBuilder.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/__init__.py` & `domible-0.1.2/src/domible/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/baseElements.py` & `domible-0.1.2/src/domible/elements/baseElements.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/inline.py` & `domible-0.1.2/src/domible/elements/inline.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/lists.py` & `domible-0.1.2/src/domible/elements/lists.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/meta.py` & `domible-0.1.2/src/domible/elements/meta.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/roots.py` & `domible-0.1.2/src/domible/elements/roots.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/elements/tables.py` & `domible-0.1.2/src/domible/elements/tables.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/starterDocuments/basicDocuments.py` & `domible-0.1.2/src/domible/starterDocuments/basicDocuments.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/src/domible/utils.py` & `domible-0.1.2/src/domible/utils.py`

 * *Files identical despite different names*

### Comparing `domible-0.1.0/PKG-INFO` & `domible-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: domible
-Version: 0.1.0
+Version: 0.1.2
 Summary: python classes to create accessible HTML elements and documents 
 Home-page: https://github.com/joeldodson/domible
 License: MIT
 Keywords: html,accessibility,a11y,web development,frontend,server side rendering,SSR
 Author: Joel Dodson
 Author-email: joeldodson@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dicli
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) ; extra == "dicli"
 Requires-Dist: jsonloggeriso8601datetime (>=1.0.3,<2.0.0) ; extra == "dicli"
+Requires-Dist: requests (>=2.30.0,<3.0.0) ; extra == "dicli"
 Requires-Dist: typer (>=0.7.0,<0.8.0) ; extra == "dicli"
 Project-URL: Repository, https://github.com/joeldodson/domible
 Description-Content-Type: text/markdown
 
 # domible
 
 Domible is a set of Python classes used to generate HTML documents and elements of arbitrary complexity.
```

