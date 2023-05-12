# Comparing `tmp/atsphinx-og-article-0.1.1.tar.gz` & `tmp/atsphinx-og-article-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atsphinx-og-article-0.1.1.tar", last modified: Tue May  9 18:37:39 2023, max compression
+gzip compressed data, was "atsphinx-og-article-0.2.0.tar", last modified: Fri May 12 00:38:19 2023, max compression
```

## Comparing `atsphinx-og-article-0.1.1.tar` & `atsphinx-og-article-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      517 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.editorconfig
--rw-r--r--   0        0        0     3338 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.gitignore
--rw-r--r--   0        0        0      543 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      444 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/.readthedocs.yml
--rw-r--r--   0        0        0      395 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/CHANGES.rst
--rw-r--r--   0        0        0     9161 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/LICENSE
--rw-r--r--   0        0        0     1718 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/README.rst
--rw-r--r--   0        0        0      634 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/Makefile
--rw-r--r--   0        0        0       14 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/_static/.gitignore
--rw-r--r--   0        0        0       14 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/_templates/.gitignore
--rw-r--r--   0        0        0      914 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/conf.py
--rw-r--r--   0        0        0     1875 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/docs/make.bat
--rw-r--r--   0        0        0     1130 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      364 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/setup.cfg
--rw-r--r--   0        0        0      919 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/__init__.py
--rw-r--r--   0        0        0     2021 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/models.py
--rw-r--r--   0        0        0     1233 2023-05-09 18:37:36.312377 atsphinx-og-article-0.1.1/src/atsphinx/og_article/processors.py
--rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 atsphinx-og-article-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      517 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     3338 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/.gitignore
+-rw-r--r--   0        0        0      543 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      444 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0      536 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1718 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/README.rst
+-rw-r--r--   0        0        0      634 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       14 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0        0        0       14 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/_templates/.gitignore
+-rw-r--r--   0        0        0      914 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     2041 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     1130 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      364 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      919 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/src/atsphinx/og_article/__init__.py
+-rw-r--r--   0        0        0     2661 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/src/atsphinx/og_article/models.py
+-rw-r--r--   0        0        0     1471 2023-05-12 00:38:16.344664 atsphinx-og-article-0.2.0/src/atsphinx/og_article/processors.py
+-rw-r--r--   0        0        0     2869 1970-01-01 00:00:00.000000 atsphinx-og-article-0.2.0/PKG-INFO
```

### Comparing `atsphinx-og-article-0.1.1/.editorconfig` & `atsphinx-og-article-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/.gitignore` & `atsphinx-og-article-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/.pre-commit-config.yaml` & `atsphinx-og-article-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/LICENSE` & `atsphinx-og-article-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/README.rst` & `atsphinx-og-article-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/docs/Makefile` & `atsphinx-og-article-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/docs/conf.py` & `atsphinx-og-article-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/docs/index.rst` & `atsphinx-og-article-0.2.0/docs/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 This renders only ``article:**`` meta tags.
 For full functional as OpenGraph, install :pypi:`sphinxext-opengraph` too.
 
 Installation
 ============
 
-.. todo:: This is scheduled method.
-
 This is registered on PyPI.
 You can install ``pip`` command.
 
 .. code-block:: console
 
    pip install atsphinx-og-article
 
@@ -61,14 +59,20 @@
 
    ``published_time`` and ``modified_time`` accept any format that dateutil can parse.
    When it is parsing attribute, datetime object has timezone always.
 
    These are complement by mutually. If one is not set, use another value automately.
    If neither not set, these are set build datetime.
 
+   .. rst:directive:option:: tags
+      :type: string
+
+      Comma separated list for tags of article.
+      When this is set, extension generates ``article:tag`` properties per values separated comma.
+
 Configuration
 =============
 
 .. confval:: og_article_timezone
 
    :Type: ``str | None``
    :Default: ``None``
```

### Comparing `atsphinx-og-article-0.1.1/docs/make.bat` & `atsphinx-og-article-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/pyproject.toml` & `atsphinx-og-article-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atsphinx-og-article-0.1.1/src/atsphinx/og_article/__init__.py` & `atsphinx-og-article-0.2.0/src/atsphinx/og_article/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Support article tpye's properties of Open Graph for Sphinx."""
 
 from docutils import nodes
 from sphinx.application import Sphinx
 
 from . import models, processors
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 
 def skip_node(self, node: models.og_article):
     """Minimum function to skip when builder visit it."""
     raise nodes.SkipNode()
```

### Comparing `atsphinx-og-article-0.1.1/src/atsphinx/og_article/processors.py` & `atsphinx-og-article-0.2.0/src/atsphinx/og_article/processors.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,9 +38,20 @@
             "meta",
             {
                 "property": "article:modified_time",
                 "content": node["modified_time"].isoformat(timespec="seconds"),
             },
         ),
     ]
+    # Append tag properties
+    metatags += [
+        ET.Element(
+            "meta",
+            {
+                "property": "article:tag",
+                "content": tag,
+            },
+        )
+        for tag in node["tags"]
+    ]
     metatags = b"\n".join([ET.tostring(e) for e in metatags])
     context["metatags"] += f"\n{metatags}"
```

### Comparing `atsphinx-og-article-0.1.1/PKG-INFO` & `atsphinx-og-article-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atsphinx-og-article
-Version: 0.1.1
+Version: 0.2.0
 Summary: Support article tpye's properties of Open Graph for Sphinx.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
```

