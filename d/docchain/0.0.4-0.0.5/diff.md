# Comparing `tmp/docchain-0.0.4.tar.gz` & `tmp/docchain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docchain-0.0.4.tar", max compression
+gzip compressed data, was "docchain-0.0.5.tar", max compression
```

## Comparing `docchain-0.0.4.tar` & `docchain-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     1056 2023-04-30 12:46:59.618177 docchain-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/__init__.py
--rw-r--r--   0        0        0      758 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/documents.py
--rw-r--r--   0        0        0       51 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/__init__.py
--rw-r--r--   0        0        0     1905 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/base.py
--rw-r--r--   0        0        0     3446 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/pydantic.py
--rw-r--r--   0        0        0     2648 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/generators/text.py
--rw-r--r--   0        0        0        0 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/models/__init__.py
--rw-r--r--   0        0        0      155 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/models/gpt.py
--rw-r--r--   0        0        0     1707 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/output_parsers/json_schema.py
--rw-r--r--   0        0        0     1023 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/settings.py
--rw-r--r--   0        0        0     2044 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/specs.py
--rw-r--r--   0        0        0      574 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/__init__.py
--rw-r--r--   0        0        0      730 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/base.py
--rw-r--r--   0        0        0      921 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/collect_openai_stats.py
--rw-r--r--   0        0        0      394 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/steps/save_document.py
--rw-r--r--   0        0        0      288 2023-04-30 12:46:59.618177 docchain-0.0.4/docchain/utils.py
--rw-r--r--   0        0        0      605 2023-04-30 12:46:59.618177 docchain-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 docchain-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1139 2023-05-12 01:15:32.853173 docchain-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/__init__.py
+-rw-r--r--   0        0        0      284 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/__init__.py
+-rw-r--r--   0        0        0     1724 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/base.py
+-rw-r--r--   0        0        0      867 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/json_schema.py
+-rw-r--r--   0        0        0      953 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/pydantic.py
+-rw-r--r--   0        0        0      746 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/text.py
+-rw-r--r--   0        0        0      855 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/blocks/ui_schema.py
+-rw-r--r--   0        0        0     1023 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/documents.py
+-rw-r--r--   0        0        0       51 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/exceptions.py
+-rw-r--r--   0        0        0     4141 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/generator.py
+-rw-r--r--   0        0        0      817 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/middleware/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/middleware/base.py
+-rw-r--r--   0        0        0      963 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/middleware/collect_openai_stats.py
+-rw-r--r--   0        0        0      423 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/middleware/save_document.py
+-rw-r--r--   0        0        0        0 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/models/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/models/gpt.py
+-rw-r--r--   0        0        0      154 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1706 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/output_parsers/json_schema.py
+-rw-r--r--   0        0        0      879 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/output_parsers/ui_schema.py
+-rw-r--r--   0        0        0     1508 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/settings.py
+-rw-r--r--   0        0        0      592 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/specs.py
+-rw-r--r--   0        0        0      288 2023-05-12 01:15:32.853173 docchain-0.0.5/docchain/utils.py
+-rw-r--r--   0        0        0      647 2023-05-12 01:15:32.857173 docchain-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 docchain-0.0.5/PKG-INFO
```

### Comparing `docchain-0.0.4/docchain/output_parsers/json_schema.py` & `docchain-0.0.5/docchain/output_parsers/json_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import re
 
 import jsonschema
 from jsonschema import Draft202012Validator
-
 from langchain.schema import BaseOutputParser, OutputParserException
 
-
 FORMAT_INSTRUCTIONS = (
     "Give me result as json schema draft 2020-12. Use camel case for fields names. "
     "Be as concise as possible, use short names, reuse names where possible. "
     "Do not omit anything or use ..."
 )
 
 
@@ -52,8 +50,8 @@
         return json_object
 
     def get_format_instructions(self) -> str:
         return FORMAT_INSTRUCTIONS
 
     @property
     def _type(self) -> str:
-        return "jsonschema"
+        return "json_schema"
```

### Comparing `docchain-0.0.4/docchain/steps/base.py` & `docchain-0.0.5/docchain/middleware/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-from ..generators.base import BaseDocumentGenerator
 from ..documents import Document
 from ..specs import Spec
 
 
-class AbstractStep:
-    """
-    Abstract step implementation.
-    """
-
-    document_builder: BaseDocumentGenerator
-
+class AbstractMiddleware:
     def __init__(self, build_document: callable):
         self.build_document = build_document
 
     def __call__(self, spec: Spec):
         self.spec_pass(spec)
         document = self.build_document(spec)
         self.doc_pass(document)
```

### Comparing `docchain-0.0.4/docchain/steps/collect_openai_stats.py` & `docchain-0.0.5/docchain/middleware/collect_openai_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import json
-from ..settings import conf
-
 from logging import getLogger
 
-from docchain.specs import Spec
 from langchain.callbacks import get_openai_callback
 
+from docchain.specs import Spec
+
+from ..settings import conf
+
 logger = getLogger(__name__)
 
 
 def collect_openai_stats(build_document):
     def run(spec: Spec):
         with get_openai_callback() as cb:
             document = build_document(spec)
 
         if document.filename and conf.debug:
-            with open(f"{conf.workspace}/{document.filename}.stats", "w+") as file:
+            with conf.fs.open(
+                f"{conf.fs_workspace}/{document.filename}.stats", "w+"
+            ) as file:
                 stats = {
                     "total_tokens": cb.total_tokens,
                     "prompt_tokens": cb.prompt_tokens,
                     "completion_tokens": cb.completion_tokens,
                     "successful_requests": cb.successful_requests,
                     "total_cost": cb.total_cost,
                 }
```

### Comparing `docchain-0.0.4/pyproject.toml` & `docchain-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "docchain"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Artem Kolesnikov <tyomo4ka@gmail.com>"]
 readme = "README.md"
 packages = [{include = "docchain"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-langchain = "^0.0.153"
-openai = "^0.27.5"
-python-dotenv = "^1.0.0"
+langchain = "^0.0.158"
+openai = "^0.27.6"
 jsonschema = "^4.17.3"
+fsspec = "^2023.4.0"
+pydantic = "^1.10.7"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
+pytest-dotenv = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 datamodel-code-generator = "^0.18.0"
 bump2version = "^1.0.1"
 
 [tool.ruff]
```

### Comparing `docchain-0.0.4/PKG-INFO` & `docchain-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: docchain
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Artem Kolesnikov
 Author-email: tyomo4ka@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fsspec (>=2023.4.0,<2024.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
-Requires-Dist: langchain (>=0.0.153,<0.0.154)
-Requires-Dist: openai (>=0.27.5,<0.28.0)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: langchain (>=0.0.158,<0.0.159)
+Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
-# Doc Chain
+# DocChain
 
-This package can be used to generate complex structured documents from specification using LLMm
-models.
+This package can be used to generate complex structured documents from Specs using LLMm models.
 
-`Document` is an abstraction that represent generated data e.g. text in markdown or HTML,
-configuration in JSON, YAML or other formats, it could be Python objects or classes, or any other
-structure that can be generated by LLMs.
+`Document` is an abstraction that represent generated data, e.g. it could be any text data in
+markdown or HTML, configuration in JSON, YAML or other formats, Python objects or classes, or any
+other data that can be generated by LLMs.
 
-`Spec` contains document requirements that can vary depending on type of generated document, e.g.
-for YAML or JSON docs it could include JSON Schema definition.
+`Spec` contains document requirements. It holds general information about the generated document.
 
 `Section` is a composite part of a Document. Document itself is a Section. Such design allows
 inclusion of Documents inside another documents.
 
-`Generator` generates Document from the provided Spec. Each generator cna be configured with a list
+`Generator` generates Document from the provided Spec. Each generator can be configured with a list
 of steps that are executed before or after generation.
 
-`Step` is a callable that can modify Spec or generated Document. It could be thought as middleware
-in an HTTP framework and cna be used for variety of tasks.
+`Middleware` is a callable that can modify Spec or the generated Documents. It acts the same as
+middleware in an HTTP framework, it can be used for variety of tasks. E.g. transforming, formatting
+or linting generated document ot its parts.
 
 ## TODO
 
-- [ ] Implement checkpoints and resume generation from checkpoint on failure.
+- [ ] Store stats in an SQLite database.
+- [ ] Blocks for HTML, Markdown, Python, one line Python, templates.
+- [ ] Add middleware to plan steps.
```

