# Comparing `tmp/model-porter-4.1.0.tar.gz` & `tmp/model-porter-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-porter-4.1.0.tar", last modified: Wed May 10 15:57:14 2023, max compression
+gzip compressed data, was "model-porter-4.1.1.tar", last modified: Fri May 12 16:37:19 2023, max compression
```

## Comparing `model-porter-4.1.0.tar` & `model-porter-4.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.308954 model-porter-4.1.0/
--rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 model-porter-4.1.0/AUTHORS.txt
--rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 model-porter-4.1.0/LICENSE.txt
--rw-r--r--   0 work       (505) staff       (20)      329 2022-11-21 19:45:21.000000 model-porter-4.1.0/MANIFEST.in
--rw-r--r--   0 work       (505) staff       (20)     1217 2023-05-10 15:57:14.309097 model-porter-4.1.0/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)      551 2023-05-10 15:56:27.000000 model-porter-4.1.0/README.md
--rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 model-porter-4.1.0/pyproject.toml
--rw-r--r--   0 work       (505) staff       (20)      810 2023-05-10 15:57:14.310741 model-porter-4.1.0/setup.cfg
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.295227 model-porter-4.1.0/src/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.300863 model-porter-4.1.0/src/model_porter/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-10-15 14:54:46.000000 model-porter-4.1.0/src/model_porter/__init__.py
--rw-r--r--   0 work       (505) staff       (20)      338 2022-10-24 22:38:02.000000 model-porter-4.1.0/src/model_porter/admin_urls.py
--rw-r--r--   0 work       (505) staff       (20)      949 2022-10-17 11:27:41.000000 model-porter-4.1.0/src/model_porter/apps.py
--rw-r--r--   0 work       (505) staff       (20)     3000 2023-01-29 19:02:56.000000 model-porter-4.1.0/src/model_porter/config.py
--rw-r--r--   0 work       (505) staff       (20)      560 2022-10-17 16:26:32.000000 model-porter-4.1.0/src/model_porter/files.py
--rw-r--r--   0 work       (505) staff       (20)     2059 2022-10-17 17:03:35.000000 model-porter-4.1.0/src/model_porter/forms.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.306131 model-porter-4.1.0/src/model_porter/management/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 20:04:24.000000 model-porter-4.1.0/src/model_porter/management/__init__.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.306653 model-porter-4.1.0/src/model_porter/management/commands/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 20:04:31.000000 model-porter-4.1.0/src/model_porter/management/commands/__init__.py
--rw-r--r--   0 work       (505) staff       (20)      609 2022-10-17 20:15:10.000000 model-porter-4.1.0/src/model_porter/management/commands/pack_repository.py
--rw-r--r--   0 work       (505) staff       (20)     4676 2023-04-01 13:55:08.000000 model-porter-4.1.0/src/model_porter/model_porter.py
--rw-r--r--   0 work       (505) staff       (20)    30548 2023-04-01 13:23:25.000000 model-porter-4.1.0/src/model_porter/repository.py
--rw-r--r--   0 work       (505) staff       (20)     6778 2022-10-21 21:25:53.000000 model-porter-4.1.0/src/model_porter/serialisation.py
--rw-r--r--   0 work       (505) staff       (20)      765 2022-10-17 16:23:07.000000 model-porter-4.1.0/src/model_porter/storage.py
--rw-r--r--   0 work       (505) staff       (20)      286 2022-11-21 14:18:54.000000 model-porter-4.1.0/src/model_porter/support_mixin.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.295735 model-porter-4.1.0/src/model_porter/templates/
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.307842 model-porter-4.1.0/src/model_porter/templates/model_porter/
--rw-r--r--   0 work       (505) staff       (20)     1080 2022-10-17 16:37:36.000000 model-porter-4.1.0/src/model_porter/templates/model_porter/choose_import_file.html
--rw-r--r--   0 work       (505) staff       (20)     2184 2022-10-18 09:58:31.000000 model-porter-4.1.0/src/model_porter/templates/model_porter/confirm_import.html
--rw-r--r--   0 work       (505) staff       (20)     1100 2022-10-17 16:00:39.000000 model-porter-4.1.0/src/model_porter/templates/model_porter/dashboard.html
--rw-r--r--   0 work       (505) staff       (20)     1465 2022-10-17 16:17:42.000000 model-porter-4.1.0/src/model_porter/templates/model_porter/import_summary.html
--rw-r--r--   0 work       (505) staff       (20)      556 2022-10-17 15:12:05.000000 model-porter-4.1.0/src/model_porter/utilities.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.308701 model-porter-4.1.0/src/model_porter/views/
--rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 11:32:14.000000 model-porter-4.1.0/src/model_porter/views/__init__.py
--rw-r--r--   0 work       (505) staff       (20)     5279 2023-02-05 12:56:14.000000 model-porter-4.1.0/src/model_porter/views/actions.py
--rw-r--r--   0 work       (505) staff       (20)     1036 2022-10-18 09:28:59.000000 model-porter-4.1.0/src/model_porter/views/dashboard.py
--rw-r--r--   0 work       (505) staff       (20)      771 2023-02-16 20:58:44.000000 model-porter-4.1.0/src/model_porter/wagtail_hooks.py
-drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-10 15:57:14.305813 model-porter-4.1.0/src/model_porter.egg-info/
--rw-r--r--   0 work       (505) staff       (20)     1217 2023-05-10 15:57:14.000000 model-porter-4.1.0/src/model_porter.egg-info/PKG-INFO
--rw-r--r--   0 work       (505) staff       (20)     1181 2023-05-10 15:57:14.000000 model-porter-4.1.0/src/model_porter.egg-info/SOURCES.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-10 15:57:14.000000 model-porter-4.1.0/src/model_porter.egg-info/dependency_links.txt
--rw-r--r--   0 work       (505) staff       (20)       17 2023-05-10 15:57:14.000000 model-porter-4.1.0/src/model_porter.egg-info/requires.txt
--rw-r--r--   0 work       (505) staff       (20)       13 2023-05-10 15:57:14.000000 model-porter-4.1.0/src/model_porter.egg-info/top_level.txt
--rw-r--r--   0 work       (505) staff       (20)        1 2023-05-10 15:57:13.000000 model-porter-4.1.0/src/model_porter.egg-info/zip-safe
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.984748 model-porter-4.1.1/
+-rw-r--r--   0 work       (505) staff       (20)       19 2022-03-13 22:55:00.000000 model-porter-4.1.1/AUTHORS.txt
+-rw-r--r--   0 work       (505) staff       (20)     1525 2023-05-10 12:24:52.000000 model-porter-4.1.1/LICENSE.txt
+-rw-r--r--   0 work       (505) staff       (20)      329 2022-11-21 19:45:21.000000 model-porter-4.1.1/MANIFEST.in
+-rw-r--r--   0 work       (505) staff       (20)     1217 2023-05-12 16:37:19.984933 model-porter-4.1.1/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)      551 2023-05-10 15:56:27.000000 model-porter-4.1.1/README.md
+-rw-r--r--   0 work       (505) staff       (20)      100 2021-02-16 17:38:13.000000 model-porter-4.1.1/pyproject.toml
+-rw-r--r--   0 work       (505) staff       (20)      810 2023-05-12 16:37:19.986461 model-porter-4.1.1/setup.cfg
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.776637 model-porter-4.1.1/src/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.895816 model-porter-4.1.1/src/model_porter/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-10-15 14:54:46.000000 model-porter-4.1.1/src/model_porter/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      338 2022-10-24 22:38:02.000000 model-porter-4.1.1/src/model_porter/admin_urls.py
+-rw-r--r--   0 work       (505) staff       (20)      949 2022-10-17 11:27:41.000000 model-porter-4.1.1/src/model_porter/apps.py
+-rw-r--r--   0 work       (505) staff       (20)     3000 2023-01-29 19:02:56.000000 model-porter-4.1.1/src/model_porter/config.py
+-rw-r--r--   0 work       (505) staff       (20)      560 2022-10-17 16:26:32.000000 model-porter-4.1.1/src/model_porter/files.py
+-rw-r--r--   0 work       (505) staff       (20)     2059 2022-10-17 17:03:35.000000 model-porter-4.1.1/src/model_porter/forms.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.906359 model-porter-4.1.1/src/model_porter/management/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 20:04:24.000000 model-porter-4.1.1/src/model_porter/management/__init__.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.926811 model-porter-4.1.1/src/model_porter/management/commands/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 20:04:31.000000 model-porter-4.1.1/src/model_porter/management/commands/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)      609 2022-10-17 20:15:10.000000 model-porter-4.1.1/src/model_porter/management/commands/pack_repository.py
+-rw-r--r--   0 work       (505) staff       (20)     4676 2023-04-01 13:55:08.000000 model-porter-4.1.1/src/model_porter/model_porter.py
+-rw-r--r--   0 work       (505) staff       (20)    30552 2023-05-12 14:38:28.000000 model-porter-4.1.1/src/model_porter/repository.py
+-rw-r--r--   0 work       (505) staff       (20)     6781 2023-05-12 16:37:08.000000 model-porter-4.1.1/src/model_porter/serialisation.py
+-rw-r--r--   0 work       (505) staff       (20)      765 2022-10-17 16:23:07.000000 model-porter-4.1.1/src/model_porter/storage.py
+-rw-r--r--   0 work       (505) staff       (20)      286 2022-11-21 14:18:54.000000 model-porter-4.1.1/src/model_porter/support_mixin.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.777531 model-porter-4.1.1/src/model_porter/templates/
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.952587 model-porter-4.1.1/src/model_porter/templates/model_porter/
+-rw-r--r--   0 work       (505) staff       (20)     1080 2022-10-17 16:37:36.000000 model-porter-4.1.1/src/model_porter/templates/model_porter/choose_import_file.html
+-rw-r--r--   0 work       (505) staff       (20)     2184 2022-10-18 09:58:31.000000 model-porter-4.1.1/src/model_porter/templates/model_porter/confirm_import.html
+-rw-r--r--   0 work       (505) staff       (20)     1100 2022-10-17 16:00:39.000000 model-porter-4.1.1/src/model_porter/templates/model_porter/dashboard.html
+-rw-r--r--   0 work       (505) staff       (20)     1465 2022-10-17 16:17:42.000000 model-porter-4.1.1/src/model_porter/templates/model_porter/import_summary.html
+-rw-r--r--   0 work       (505) staff       (20)      556 2022-10-17 15:12:05.000000 model-porter-4.1.1/src/model_porter/utilities.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.984298 model-porter-4.1.1/src/model_porter/views/
+-rw-r--r--   0 work       (505) staff       (20)        0 2022-10-17 11:32:14.000000 model-porter-4.1.1/src/model_porter/views/__init__.py
+-rw-r--r--   0 work       (505) staff       (20)     5279 2023-02-05 12:56:14.000000 model-porter-4.1.1/src/model_porter/views/actions.py
+-rw-r--r--   0 work       (505) staff       (20)     1036 2022-10-18 09:28:59.000000 model-porter-4.1.1/src/model_porter/views/dashboard.py
+-rw-r--r--   0 work       (505) staff       (20)      771 2023-02-16 20:58:44.000000 model-porter-4.1.1/src/model_porter/wagtail_hooks.py
+drwxr-xr-x   0 work       (505) staff       (20)        0 2023-05-12 16:37:19.905914 model-porter-4.1.1/src/model_porter.egg-info/
+-rw-r--r--   0 work       (505) staff       (20)     1217 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/PKG-INFO
+-rw-r--r--   0 work       (505) staff       (20)     1181 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/SOURCES.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/dependency_links.txt
+-rw-r--r--   0 work       (505) staff       (20)       17 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/requires.txt
+-rw-r--r--   0 work       (505) staff       (20)       13 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/top_level.txt
+-rw-r--r--   0 work       (505) staff       (20)        1 2023-05-12 16:37:19.000000 model-porter-4.1.1/src/model_porter.egg-info/zip-safe
```

### Comparing `model-porter-4.1.0/LICENSE.txt` & `model-porter-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/PKG-INFO` & `model-porter-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-porter
-Version: 4.1.0
+Version: 4.1.1
 Summary: Portable serialisation of Django models.
 Home-page: https://github.com/high-dimensional/model-porter
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `model-porter-4.1.0/README.md` & `model-porter-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/setup.cfg` & `model-porter-4.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = model-porter
-version = 4.1.0
+version = 4.1.1
 url = https://github.com/high-dimensional/model-porter
 author = High Dimensional Neurology Group, UCL
 author_email = pypi@highdimensional.net
 description = Portable serialisation of Django models.
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD-3-Clause
```

### Comparing `model-porter-4.1.0/src/model_porter/apps.py` & `model-porter-4.1.1/src/model_porter/apps.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/config.py` & `model-porter-4.1.1/src/model_porter/config.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/files.py` & `model-porter-4.1.1/src/model_porter/files.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/forms.py` & `model-porter-4.1.1/src/model_porter/forms.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/management/commands/pack_repository.py` & `model-porter-4.1.1/src/model_porter/management/commands/pack_repository.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/model_porter.py` & `model-porter-4.1.1/src/model_porter/model_porter.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/repository.py` & `model-porter-4.1.1/src/model_porter/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import csv
 import io
 import tarfile
 import re
 import sys
 import importlib
 
-from collections import Sequence
+from collections.abc import Sequence
 from typing import Optional
 
 from django.apps import apps
 from django.utils.functional import cached_property
 from django.core.files.base import ContentFile
 from django.db.models.manager import Manager
```

### Comparing `model-porter-4.1.0/src/model_porter/serialisation.py` & `model-porter-4.1.1/src/model_porter/serialisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import types
-from collections import Sequence
+from collections.abc import Sequence
 
 __all__ = ['Serialisable', 'unpack_attribute_values', 'copy_list', 'copy_dict'] # noqa
 
 
-
 class copy_dict(dict):
     pass
 
 
 class copy_list(list):
     pass
```

### Comparing `model-porter-4.1.0/src/model_porter/storage.py` & `model-porter-4.1.1/src/model_porter/storage.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/templates/model_porter/choose_import_file.html` & `model-porter-4.1.1/src/model_porter/templates/model_porter/choose_import_file.html`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/templates/model_porter/confirm_import.html` & `model-porter-4.1.1/src/model_porter/templates/model_porter/confirm_import.html`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/templates/model_porter/dashboard.html` & `model-porter-4.1.1/src/model_porter/templates/model_porter/dashboard.html`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/templates/model_porter/import_summary.html` & `model-porter-4.1.1/src/model_porter/templates/model_porter/import_summary.html`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/utilities.py` & `model-porter-4.1.1/src/model_porter/utilities.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/views/actions.py` & `model-porter-4.1.1/src/model_porter/views/actions.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/views/dashboard.py` & `model-porter-4.1.1/src/model_porter/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter/wagtail_hooks.py` & `model-porter-4.1.1/src/model_porter/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `model-porter-4.1.0/src/model_porter.egg-info/PKG-INFO` & `model-porter-4.1.1/src/model_porter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-porter
-Version: 4.1.0
+Version: 4.1.1
 Summary: Portable serialisation of Django models.
 Home-page: https://github.com/high-dimensional/model-porter
 Author: High Dimensional Neurology Group, UCL
 Author-email: pypi@highdimensional.net
 License: BSD-3-Clause
 Platform: any
 Classifier: Framework :: Django
```

### Comparing `model-porter-4.1.0/src/model_porter.egg-info/SOURCES.txt` & `model-porter-4.1.1/src/model_porter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

