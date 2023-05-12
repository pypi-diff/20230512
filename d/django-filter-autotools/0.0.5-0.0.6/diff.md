# Comparing `tmp/django-filter-autotools-0.0.5.tar.gz` & `tmp/django-filter-autotools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-filter-autotools-0.0.5.tar", last modified: Tue May  2 09:36:06 2023, max compression
+gzip compressed data, was "dist/django-filter-autotools-0.0.6.tar", last modified: Fri May 12 10:08:36 2023, max compression
```

## Comparing `django-filter-autotools-0.0.5.tar` & `django-filter-autotools-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      816 2023-05-02 09:32:26.000000 django-filter-autotools-0.0.5/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5095 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filter_autotools.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.5/LICENSE
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4528 2023-05-02 09:31:40.000000 django-filter-autotools-0.0.5/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/django_filters_autotools/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7459 2023-05-02 09:31:25.000000 django-filter-autotools-0.0.5/django_filters_autotools/mixins.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.5/django_filters_autotools/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5095 2023-05-02 09:36:06.000000 django-filter-autotools-0.0.5/PKG-INFO
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      831 2023-05-12 10:06:28.000000 django-filter-autotools-0.0.6/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      332 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       20 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       25 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5694 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filter_autotools.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-05-01 17:39:21.000000 django-filter-autotools-0.0.6/LICENSE
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5112 2023-05-12 10:04:50.000000 django-filter-autotools-0.0.6/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/django_filters_autotools/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7459 2023-05-02 09:31:25.000000 django-filter-autotools-0.0.6/django_filters_autotools/mixins.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-01 17:40:18.000000 django-filter-autotools-0.0.6/django_filters_autotools/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5694 2023-05-12 10:08:36.000000 django-filter-autotools-0.0.6/PKG-INFO
```

### Comparing `django-filter-autotools-0.0.5/setup.py` & `django-filter-autotools-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="django-filter-autotools", 
-    version="0.0.5", 
+    version="0.0.6", 
     description=(
-        "Provides some mixins which allow automatic generation of filtersets with"
-        "a list of lookups, including new lookups not registered into Django."
+        "Provides some mixins which allow automatic generation of django-filter "
+        "filtersets with a list of lookups, including new lookups not registered into Django."
     ),
     author="Carlos Pastor",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(), 
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `django-filter-autotools-0.0.5/django_filter_autotools.egg-info/PKG-INFO` & `django-filter-autotools-0.0.6/django_filter_autotools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.5
-Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
+Version: 0.0.6
+Summary: Provides some mixins which allow automatic generation of django-filter filtersets with a list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 ```
 
 `MyFilterSet` will automatically generate filters for all these lookups for any field included in `fields` if `fields` is an array. In the case that `fields` is a dictionary, defaults will be generated for any key having `None` as value.
 
 
 ## PseudoLookupsMixin
 
-We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, and adding "exclusion" filters:
+We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, adding "exclusion" filters (not) and adding "conjoined" filters (and for m2m):
 
 ```python
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
 
@@ -66,33 +66,39 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
 `PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
-* `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
+* `filter_class`: filter class to be used for this lookup. If not specified or set to None, the one chosen django-filter for the `behaves_like` lookup will be used. Note that these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
 * `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
-Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
+Override the `filter_for_pseudolookup` class method on the FilterSet if you need to choose different filter classes depending on both the field type and the lookup.
 
 
 ## Integrating everything into DRF by default
 
-Complete example making available several lookups by default for all fields of type `CharField`:
+Complete example making available several lookups by default for all fields of type `CharField`, and conjoined filters for all fields of type `ManyToManyField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
 from django.db import models
 from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
@@ -117,19 +123,26 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
-        models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.CharField:        [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.ManyToManyField:  [ 'exact', 'exact_all' ],
     }
 
     
 class MyFilterBackend(filters.DjangoFilterBackend):
     filterset_base = MyFilterSet
 ```
```

### Comparing `django-filter-autotools-0.0.5/LICENSE` & `django-filter-autotools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.5/README.md` & `django-filter-autotools-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ```
 
 `MyFilterSet` will automatically generate filters for all these lookups for any field included in `fields` if `fields` is an array. In the case that `fields` is a dictionary, defaults will be generated for any key having `None` as value.
 
 
 ## PseudoLookupsMixin
 
-We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, and adding "exclusion" filters:
+We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, adding "exclusion" filters (not) and adding "conjoined" filters (and for m2m):
 
 ```python
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
 
@@ -50,33 +50,39 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
 `PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
-* `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
+* `filter_class`: filter class to be used for this lookup. If not specified or set to None, the one chosen django-filter for the `behaves_like` lookup will be used. Note that these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
 * `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
-Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
+Override the `filter_for_pseudolookup` class method on the FilterSet if you need to choose different filter classes depending on both the field type and the lookup.
 
 
 ## Integrating everything into DRF by default
 
-Complete example making available several lookups by default for all fields of type `CharField`:
+Complete example making available several lookups by default for all fields of type `CharField`, and conjoined filters for all fields of type `ManyToManyField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
 from django.db import models
 from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
@@ -101,19 +107,26 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
-        models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.CharField:        [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.ManyToManyField:  [ 'exact', 'exact_all' ],
     }
 
     
 class MyFilterBackend(filters.DjangoFilterBackend):
     filterset_base = MyFilterSet
 ```
```

### Comparing `django-filter-autotools-0.0.5/django_filters_autotools/mixins.py` & `django-filter-autotools-0.0.6/django_filters_autotools/mixins.py`

 * *Files identical despite different names*

### Comparing `django-filter-autotools-0.0.5/PKG-INFO` & `django-filter-autotools-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-filter-autotools
-Version: 0.0.5
-Summary: Provides some mixins which allow automatic generation of filtersets witha list of lookups, including new lookups not registered into Django.
+Version: 0.0.6
+Summary: Provides some mixins which allow automatic generation of django-filter filtersets with a list of lookups, including new lookups not registered into Django.
 Home-page: UNKNOWN
 Author: Carlos Pastor
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -40,15 +40,15 @@
 ```
 
 `MyFilterSet` will automatically generate filters for all these lookups for any field included in `fields` if `fields` is an array. In the case that `fields` is a dictionary, defaults will be generated for any key having `None` as value.
 
 
 ## PseudoLookupsMixin
 
-We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, and adding "exclusion" filters:
+We can use this mixin to patch the FilterSet filter creation algorithm to understand some lookups which are not registered into Django. Two common scenarios are checking whether a string is empty, adding "exclusion" filters (not) and adding "conjoined" filters (and for m2m):
 
 ```python
 class EmptyStringFilter(filters.BooleanFilter):
     def filter(self, qs, value):
         if value in EMPTY_VALUES:
             return qs
 
@@ -66,33 +66,39 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 ```
 
 Under the hood this works by replacing the lookup with the one specified in the `behaves_like` key, running the filter creation algorithm and then patching the filters if necessary. This way any transformer or any extra lookups registered into Django will also be available.
 
 `PSEUDO_LOOKUPS` is a dictionary whose keys are the new lookups to be supported and the values are dictionary with the following keys:
 
 * `behaves_like`: should be a lookup registered in Django with similar semantics.
-* `filter_class`: filter class to be used for this lookup. If not specified or None, the one chosen django-filters for the `behaves_like` lookup will be used. Note these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
+* `filter_class`: filter class to be used for this lookup. If not specified or set to None, the one chosen django-filter for the `behaves_like` lookup will be used. Note that these may be fine-tuned by overriding the `FILTER_FOR_DBFIELD_DEFAULTS` dictionary.
 * `replace_with`: if present the filter class is patched so that its `__init__` method replaces the new lookup with this value.
 * `extra`: if present the object returned from applying this function to the field will be merged into the filter class kwargs.
 
-Note that more fine-tuning by overriding the `filter_for_pseudolookup` class method (for example, choosing the filter class based on the field type).
+Override the `filter_for_pseudolookup` class method on the FilterSet if you need to choose different filter classes depending on both the field type and the lookup.
 
 
 ## Integrating everything into DRF by default
 
-Complete example making available several lookups by default for all fields of type `CharField`:
+Complete example making available several lookups by default for all fields of type `CharField`, and conjoined filters for all fields of type `ManyToManyField`:
 
 filters.py:
 ```python
 from django_filters import rest_framework as filters
 from django.db import models
 from django.core.validators import EMPTY_VALUES
 from django_filters_autotools.mixins import *
@@ -117,19 +123,26 @@
             'filter_class': EmptyStringFilter,
         },
         'not_icontains': {
             'behaves_like': 'icontains',
             'filter_class': None,
             'replace_with': 'icontains',
             'extra': lambda f: {'exclude': True}
+        },
+        'exact_all': {
+            'behaves_like': 'exact',
+            'filter_class': None,
+            'replace_with': 'exact',
+            'extra': lambda f: {'conjoined': True}
         }
     }
 
     DEFAULT_LOOKUPS = {
-        models.CharField:      [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.CharField:        [ 'exact', 'icontains', 'isempty', 'not_icontains' ],
+        models.ManyToManyField:  [ 'exact', 'exact_all' ],
     }
 
     
 class MyFilterBackend(filters.DjangoFilterBackend):
     filterset_base = MyFilterSet
 ```
```

