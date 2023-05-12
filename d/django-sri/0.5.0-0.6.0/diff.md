# Comparing `tmp/django-sri-0.5.0.tar.gz` & `tmp/django-sri-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sri-0.5.0.tar", last modified: Mon Sep  5 08:11:50 2022, max compression
+gzip compressed data, was "django-sri-0.6.0.tar", last modified: Fri May 12 15:12:39 2023, max compression
```

## Comparing `django-sri-0.5.0.tar` & `django-sri-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:50.727301 django-sri-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-05 08:11:42.000000 django-sri-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-09-05 08:11:50.727301 django-sri-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-09-05 08:11:42.000000 django-sri-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:50.727301 django-sri-0.5.0/django_sri.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-09-05 08:11:50.000000 django-sri-0.5.0/django_sri.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-09-05 08:11:50.000000 django-sri-0.5.0/django_sri.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 08:11:50.000000 django-sri-0.5.0/django_sri.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-05 08:11:50.000000 django-sri-0.5.0/django_sri.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-09-05 08:11:50.000000 django-sri-0.5.0/django_sri.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-05 08:11:50.731301 django-sri-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-09-05 08:11:42.000000 django-sri-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:50.727301 django-sri-0.5.0/sri/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/hashers.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/integrity.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:50.727301 django-sri-0.5.0/sri/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/templatetags/sri.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-09-05 08:11:42.000000 django-sri-0.5.0/sri/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:39.276816 django-sri-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-12 15:12:27.000000 django-sri-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-12 15:12:39.276816 django-sri-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-12 15:12:27.000000 django-sri-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:39.276816 django-sri-0.6.0/django_sri.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-12 15:12:39.000000 django-sri-0.6.0/django_sri.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-12 15:12:39.000000 django-sri-0.6.0/django_sri.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:39.000000 django-sri-0.6.0/django_sri.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 15:12:39.000000 django-sri-0.6.0/django_sri.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 15:12:39.000000 django-sri-0.6.0/django_sri.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 15:12:27.000000 django-sri-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-12 15:12:39.276816 django-sri-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:12:27.000000 django-sri-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:39.276816 django-sri-0.6.0/sri/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/hashers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:39.276816 django-sri-0.6.0/sri/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/templatetags/sri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-12 15:12:27.000000 django-sri-0.6.0/sri/utils.py
```

### Comparing `django-sri-0.5.0/LICENSE` & `django-sri-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sri-0.5.0/PKG-INFO` & `django-sri-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sri
-Version: 0.5.0
+Version: 0.6.0
 Summary: Subresource Integrity for Django
 Home-page: https://github.com/RealOrangeOne/django-sri
 Author: Jake Howard
 License: BSD
 Description: # Django SRI
         
         ![CI](https://github.com/RealOrangeOne/django-sri/workflows/CI/badge.svg)
@@ -40,24 +40,35 @@
         {% sri_static "index.css" %} <!-- Will output "<link rel='stylesheet' href='/static/index.css' integrity='sha256-...'/>" -->
         ```
         
         For performance, the hashes of files are caches in Django's [caching framework](https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys are the hash of the file path in the specified algorithm in hex. Caches are stored for as long as `DEFAULT_TIMEOUT` is set to.
         
         #### Algorithms
         
-        The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional argument to the `sri` template tag (or the specific ones):
+        The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional `algorithm` argument to the `sri` template tag (or the specific ones):
         
         ```html
         {% load sri %}
         
-        {% sri_static "index.js" "sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
+        {% sri_static "index.js" algorithm="sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
         ```
         
         The default algorithm can be changed by setting `SRI_ALGORITHM` to the required algorithm.
         
+        #### Additional attributes
+        
+        To add additional attributes to the output tag (such as `async` / `defer`), specify them as additional arguments to the template tag:
+        
+        ```html
+        {% load sri %}
+        
+        {% sri_static "index.js" 'defer' 'async'%}
+        {% sri_static "index.woff2" preload as="font" %}
+        ```
+        
         #### Just the integrity value
         
         To retrieve just the integrity hash (the contents of the `integrity` attribute), you can use the `{% sri_integrity_static %}` tag, which supports the same arguments as the other tags.
         
         ```html
         {% load sri %}
         
@@ -67,14 +78,16 @@
         #### Supported Files
         
         For automatic tag output, the following files are supported:
         
         - `.js`
         - `.css`
         
+        Unknown extensions will emit a `link` tag with the URL as the `href` attribute.
+        
         `sri_integrity_static` is unaffected by this limitation.
         
         ### API
         
         ```python
         from pathlib import Path
         from sri import calculate_integrity, calculate_integrity_of_static, Algorithm
@@ -91,20 +104,25 @@
         
         When using a manifest `STATICFILES_STORAGE`, `django-sri` will automatically retrieve the hashed and post-processed file as opposed to the original.
         
 Keywords: django subresource integrity sri
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-sri Version: 0.5.0 Summary: Subresource
+Metadata-Version: 2.1 Name: django-sri Version: 0.6.0 Summary: Subresource
 Integrity for Django Home-page: https://github.com/RealOrangeOne/django-sri
 Author: Jake Howard License: BSD Description: # Django SRI ![CI](https://
 github.com/RealOrangeOne/django-sri/workflows/CI/badge.svg) ![PyPI](https://
 img.shields.io/pypi/v/django-sri.svg) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/django-sri.svg) ![PyPI - Status](https://
 img.shields.io/pypi/status/django-sri.svg) ![PyPI - License](https://
 img.shields.io/pypi/l/django-sri.svg) [Subresource Integrity](https://
@@ -15,36 +15,43 @@
 sri %} {% sri_static "index.js" %}  {% sri_static "index.css" %}  ``` For
 performance, the hashes of files are caches in Django's [caching framework]
 (https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use
 the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys
 are the hash of the file path in the specified algorithm in hex. Caches are
 stored for as long as `DEFAULT_TIMEOUT` is set to. #### Algorithms The SRI
 standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256
-is used. To override this, supply an additional argument to the `sri` template
-tag (or the specific ones): ```html {% load sri %} {% sri_static "index.js"
-"sha512" %}  ``` The default algorithm can be changed by setting
-`SRI_ALGORITHM` to the required algorithm. #### Just the integrity value To
-retrieve just the integrity hash (the contents of the `integrity` attribute),
-you can use the `{% sri_integrity_static %}` tag, which supports the same
-arguments as the other tags. ```html {% load sri %} {% sri_integrity_static
-"index.js" "sha512" %}  ``` #### Supported Files For automatic tag output, the
-following files are supported: - `.js` - `.css` `sri_integrity_static` is
-unaffected by this limitation. ### API ```python from pathlib import Path from
-sri import calculate_integrity, calculate_integrity_of_static, Algorithm
+is used. To override this, supply an additional `algorithm` argument to the
+`sri` template tag (or the specific ones): ```html {% load sri %} {% sri_static
+"index.js" algorithm="sha512" %}  ``` The default algorithm can be changed by
+setting `SRI_ALGORITHM` to the required algorithm. #### Additional attributes
+To add additional attributes to the output tag (such as `async` / `defer`),
+specify them as additional arguments to the template tag: ```html {% load sri
+%} {% sri_static "index.js" 'defer' 'async'%} {% sri_static "index.woff2"
+preload as="font" %} ``` #### Just the integrity value To retrieve just the
+integrity hash (the contents of the `integrity` attribute), you can use the `{%
+sri_integrity_static %}` tag, which supports the same arguments as the other
+tags. ```html {% load sri %} {% sri_integrity_static "index.js" "sha512" %}
+``` #### Supported Files For automatic tag output, the following files are
+supported: - `.js` - `.css` Unknown extensions will emit a `link` tag with the
+URL as the `href` attribute. `sri_integrity_static` is unaffected by this
+limitation. ### API ```python from pathlib import Path from sri import
+calculate_integrity, calculate_integrity_of_static, Algorithm
 calculate_integrity(Path("/path/to/myfile.txt")) # "sha256-..."
 calculate_integrity_of_static("index.js") # "sha256-..."
 calculate_integrity_of_static("index.js", Algorithm.SHA512) # "sha512-..." ```
 ### _"Does this work with [whitenoise](https://whitenoise.evans.io/en/stable/
 ) or alike?"_ Yes. `django-sri` outputs the static file URL in the same way the
 builtin `static` template tag does. This means the correct cachebusted URLs are
 output. When using a manifest `STATICFILES_STORAGE`, `django-sri` will
 automatically retrieve the hashed and post-processed file as opposed to the
 original. Keywords: django subresource integrity sri Platform: UNKNOWN
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software
-Development Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Software Development Classifier:
+Typing :: Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `django-sri-0.5.0/README.md` & `django-sri-0.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -33,24 +33,35 @@
 {% sri_static "index.css" %} <!-- Will output "<link rel='stylesheet' href='/static/index.css' integrity='sha256-...'/>" -->
 ```
 
 For performance, the hashes of files are caches in Django's [caching framework](https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys are the hash of the file path in the specified algorithm in hex. Caches are stored for as long as `DEFAULT_TIMEOUT` is set to.
 
 #### Algorithms
 
-The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional argument to the `sri` template tag (or the specific ones):
+The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional `algorithm` argument to the `sri` template tag (or the specific ones):
 
 ```html
 {% load sri %}
 
-{% sri_static "index.js" "sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
+{% sri_static "index.js" algorithm="sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
 ```
 
 The default algorithm can be changed by setting `SRI_ALGORITHM` to the required algorithm.
 
+#### Additional attributes
+
+To add additional attributes to the output tag (such as `async` / `defer`), specify them as additional arguments to the template tag:
+
+```html
+{% load sri %}
+
+{% sri_static "index.js" 'defer' 'async'%}
+{% sri_static "index.woff2" preload as="font" %}
+```
+
 #### Just the integrity value
 
 To retrieve just the integrity hash (the contents of the `integrity` attribute), you can use the `{% sri_integrity_static %}` tag, which supports the same arguments as the other tags.
 
 ```html
 {% load sri %}
 
@@ -60,14 +71,16 @@
 #### Supported Files
 
 For automatic tag output, the following files are supported:
 
 - `.js`
 - `.css`
 
+Unknown extensions will emit a `link` tag with the URL as the `href` attribute.
+
 `sri_integrity_static` is unaffected by this limitation.
 
 ### API
 
 ```python
 from pathlib import Path
 from sri import calculate_integrity, calculate_integrity_of_static, Algorithm
```

#### html2text {}

```diff
@@ -12,25 +12,30 @@
 sri %} {% sri_static "index.js" %}  {% sri_static "index.css" %}  ``` For
 performance, the hashes of files are caches in Django's [caching framework]
 (https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use
 the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys
 are the hash of the file path in the specified algorithm in hex. Caches are
 stored for as long as `DEFAULT_TIMEOUT` is set to. #### Algorithms The SRI
 standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256
-is used. To override this, supply an additional argument to the `sri` template
-tag (or the specific ones): ```html {% load sri %} {% sri_static "index.js"
-"sha512" %}  ``` The default algorithm can be changed by setting
-`SRI_ALGORITHM` to the required algorithm. #### Just the integrity value To
-retrieve just the integrity hash (the contents of the `integrity` attribute),
-you can use the `{% sri_integrity_static %}` tag, which supports the same
-arguments as the other tags. ```html {% load sri %} {% sri_integrity_static
-"index.js" "sha512" %}  ``` #### Supported Files For automatic tag output, the
-following files are supported: - `.js` - `.css` `sri_integrity_static` is
-unaffected by this limitation. ### API ```python from pathlib import Path from
-sri import calculate_integrity, calculate_integrity_of_static, Algorithm
+is used. To override this, supply an additional `algorithm` argument to the
+`sri` template tag (or the specific ones): ```html {% load sri %} {% sri_static
+"index.js" algorithm="sha512" %}  ``` The default algorithm can be changed by
+setting `SRI_ALGORITHM` to the required algorithm. #### Additional attributes
+To add additional attributes to the output tag (such as `async` / `defer`),
+specify them as additional arguments to the template tag: ```html {% load sri
+%} {% sri_static "index.js" 'defer' 'async'%} {% sri_static "index.woff2"
+preload as="font" %} ``` #### Just the integrity value To retrieve just the
+integrity hash (the contents of the `integrity` attribute), you can use the `{%
+sri_integrity_static %}` tag, which supports the same arguments as the other
+tags. ```html {% load sri %} {% sri_integrity_static "index.js" "sha512" %}
+``` #### Supported Files For automatic tag output, the following files are
+supported: - `.js` - `.css` Unknown extensions will emit a `link` tag with the
+URL as the `href` attribute. `sri_integrity_static` is unaffected by this
+limitation. ### API ```python from pathlib import Path from sri import
+calculate_integrity, calculate_integrity_of_static, Algorithm
 calculate_integrity(Path("/path/to/myfile.txt")) # "sha256-..."
 calculate_integrity_of_static("index.js") # "sha256-..."
 calculate_integrity_of_static("index.js", Algorithm.SHA512) # "sha512-..." ```
 ### _"Does this work with [whitenoise](https://whitenoise.evans.io/en/stable/
 ) or alike?"_ Yes. `django-sri` outputs the static file URL in the same way the
 builtin `static` template tag does. This means the correct cachebusted URLs are
 output. When using a manifest `STATICFILES_STORAGE`, `django-sri` will
```

### Comparing `django-sri-0.5.0/django_sri.egg-info/PKG-INFO` & `django-sri-0.6.0/django_sri.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sri
-Version: 0.5.0
+Version: 0.6.0
 Summary: Subresource Integrity for Django
 Home-page: https://github.com/RealOrangeOne/django-sri
 Author: Jake Howard
 License: BSD
 Description: # Django SRI
         
         ![CI](https://github.com/RealOrangeOne/django-sri/workflows/CI/badge.svg)
@@ -40,24 +40,35 @@
         {% sri_static "index.css" %} <!-- Will output "<link rel='stylesheet' href='/static/index.css' integrity='sha256-...'/>" -->
         ```
         
         For performance, the hashes of files are caches in Django's [caching framework](https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys are the hash of the file path in the specified algorithm in hex. Caches are stored for as long as `DEFAULT_TIMEOUT` is set to.
         
         #### Algorithms
         
-        The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional argument to the `sri` template tag (or the specific ones):
+        The SRI standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256 is used. To override this, supply an additional `algorithm` argument to the `sri` template tag (or the specific ones):
         
         ```html
         {% load sri %}
         
-        {% sri_static "index.js" "sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
+        {% sri_static "index.js" algorithm="sha512" %} <!-- Will output "<script src='/static/index.js' integrity='sha512-...'></script>" -->
         ```
         
         The default algorithm can be changed by setting `SRI_ALGORITHM` to the required algorithm.
         
+        #### Additional attributes
+        
+        To add additional attributes to the output tag (such as `async` / `defer`), specify them as additional arguments to the template tag:
+        
+        ```html
+        {% load sri %}
+        
+        {% sri_static "index.js" 'defer' 'async'%}
+        {% sri_static "index.woff2" preload as="font" %}
+        ```
+        
         #### Just the integrity value
         
         To retrieve just the integrity hash (the contents of the `integrity` attribute), you can use the `{% sri_integrity_static %}` tag, which supports the same arguments as the other tags.
         
         ```html
         {% load sri %}
         
@@ -67,14 +78,16 @@
         #### Supported Files
         
         For automatic tag output, the following files are supported:
         
         - `.js`
         - `.css`
         
+        Unknown extensions will emit a `link` tag with the URL as the `href` attribute.
+        
         `sri_integrity_static` is unaffected by this limitation.
         
         ### API
         
         ```python
         from pathlib import Path
         from sri import calculate_integrity, calculate_integrity_of_static, Algorithm
@@ -91,20 +104,25 @@
         
         When using a manifest `STATICFILES_STORAGE`, `django-sri` will automatically retrieve the hashed and post-processed file as opposed to the original.
         
 Keywords: django subresource integrity sri
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-sri Version: 0.5.0 Summary: Subresource
+Metadata-Version: 2.1 Name: django-sri Version: 0.6.0 Summary: Subresource
 Integrity for Django Home-page: https://github.com/RealOrangeOne/django-sri
 Author: Jake Howard License: BSD Description: # Django SRI ![CI](https://
 github.com/RealOrangeOne/django-sri/workflows/CI/badge.svg) ![PyPI](https://
 img.shields.io/pypi/v/django-sri.svg) ![PyPI - Python Version](https://
 img.shields.io/pypi/pyversions/django-sri.svg) ![PyPI - Status](https://
 img.shields.io/pypi/status/django-sri.svg) ![PyPI - License](https://
 img.shields.io/pypi/l/django-sri.svg) [Subresource Integrity](https://
@@ -15,36 +15,43 @@
 sri %} {% sri_static "index.js" %}  {% sri_static "index.css" %}  ``` For
 performance, the hashes of files are caches in Django's [caching framework]
 (https://docs.djangoproject.com/en/dev/topics/cache/). It will attempt to use
 the "sri" cache, but fall back to "default" if it doesn't exist. The cache keys
 are the hash of the file path in the specified algorithm in hex. Caches are
 stored for as long as `DEFAULT_TIMEOUT` is set to. #### Algorithms The SRI
 standard supports 3 algorithms: sha256, sha384 and sha512. By default, SHA256
-is used. To override this, supply an additional argument to the `sri` template
-tag (or the specific ones): ```html {% load sri %} {% sri_static "index.js"
-"sha512" %}  ``` The default algorithm can be changed by setting
-`SRI_ALGORITHM` to the required algorithm. #### Just the integrity value To
-retrieve just the integrity hash (the contents of the `integrity` attribute),
-you can use the `{% sri_integrity_static %}` tag, which supports the same
-arguments as the other tags. ```html {% load sri %} {% sri_integrity_static
-"index.js" "sha512" %}  ``` #### Supported Files For automatic tag output, the
-following files are supported: - `.js` - `.css` `sri_integrity_static` is
-unaffected by this limitation. ### API ```python from pathlib import Path from
-sri import calculate_integrity, calculate_integrity_of_static, Algorithm
+is used. To override this, supply an additional `algorithm` argument to the
+`sri` template tag (or the specific ones): ```html {% load sri %} {% sri_static
+"index.js" algorithm="sha512" %}  ``` The default algorithm can be changed by
+setting `SRI_ALGORITHM` to the required algorithm. #### Additional attributes
+To add additional attributes to the output tag (such as `async` / `defer`),
+specify them as additional arguments to the template tag: ```html {% load sri
+%} {% sri_static "index.js" 'defer' 'async'%} {% sri_static "index.woff2"
+preload as="font" %} ``` #### Just the integrity value To retrieve just the
+integrity hash (the contents of the `integrity` attribute), you can use the `{%
+sri_integrity_static %}` tag, which supports the same arguments as the other
+tags. ```html {% load sri %} {% sri_integrity_static "index.js" "sha512" %}
+``` #### Supported Files For automatic tag output, the following files are
+supported: - `.js` - `.css` Unknown extensions will emit a `link` tag with the
+URL as the `href` attribute. `sri_integrity_static` is unaffected by this
+limitation. ### API ```python from pathlib import Path from sri import
+calculate_integrity, calculate_integrity_of_static, Algorithm
 calculate_integrity(Path("/path/to/myfile.txt")) # "sha256-..."
 calculate_integrity_of_static("index.js") # "sha256-..."
 calculate_integrity_of_static("index.js", Algorithm.SHA512) # "sha512-..." ```
 ### _"Does this work with [whitenoise](https://whitenoise.evans.io/en/stable/
 ) or alike?"_ Yes. `django-sri` outputs the static file URL in the same way the
 builtin `static` template tag does. This means the correct cachebusted URLs are
 output. When using a manifest `STATICFILES_STORAGE`, `django-sri` will
 automatically retrieve the hashed and post-processed file as opposed to the
 original. Keywords: django subresource integrity sri Platform: UNKNOWN
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software
-Development Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Software Development Classifier:
+Typing :: Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `django-sri-0.5.0/setup.py` & `django-sri-0.6.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="django-sri",
-    version="0.5.0",
+    version="0.6.0",
     url="https://github.com/RealOrangeOne/django-sri",
     author="Jake Howard",
     description="Subresource Integrity for Django",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="BSD",
     packages=find_packages(include=["sri*"]),
     package_data={"sri": ["py.typed"]},
     install_requires=["Django>=3.2"],
     python_requires=">=3.8",
     keywords="django subresource integrity sri",
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
 )
```

### Comparing `django-sri-0.5.0/sri/hashers.py` & `django-sri-0.6.0/sri/hashers.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 
 HASHERS = {
     Algorithm.SHA256: hashlib.sha256,
     Algorithm.SHA384: hashlib.sha384,
     Algorithm.SHA512: hashlib.sha512,
 }
 
+READ_BUFFER_SIZE = 65536  # 64k
+
 
 def calculate_hash(path: Path, algorithm: Algorithm) -> str:
     cache = get_cache()
     cache_key = get_cache_key(path, algorithm)
     file_hash = cache.get(cache_key)
     if file_hash is None:
         # Cache miss, do the calculation
         hasher = HASHERS[algorithm]()
         with path.open("rb") as f:
             while True:
-                data = f.read(hasher.block_size)
+                data = f.read(READ_BUFFER_SIZE)
                 if not data:
                     break
                 hasher.update(data)
         file_hash = base64.b64encode(hasher.digest()).decode()
         cache.set(cache_key, file_hash)
     return file_hash
```

### Comparing `django-sri-0.5.0/sri/utils.py` & `django-sri-0.6.0/sri/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+import logging
 import os
 from pathlib import Path
 
 from django.contrib.staticfiles.finders import find as find_static_file
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.core.cache import DEFAULT_CACHE_ALIAS, caches
 from django.core.cache.backends.base import InvalidCacheBackendError
 
+logger = logging.getLogger(__name__)
+
 
 def get_static_path(path: str) -> Path:
     """
     Resolves a path commonly passed to `{% static %}` into a filesystem path
     """
 
     if hasattr(staticfiles_storage, "stored_name"):
         path = staticfiles_storage.stored_name(path)
-        collected_file_path = staticfiles_storage.path(path)
-        if os.path.exists(collected_file_path):
-            return Path(collected_file_path)
 
+    collected_file_path = staticfiles_storage.path(path)
+    if os.path.exists(collected_file_path):
+        return Path(collected_file_path)
+
+    logger.debug("File not found in staticfiles_storage - checking source files")
     source_static_file_path = find_static_file(path)
     if source_static_file_path is not None:
         return Path(source_static_file_path)
 
     raise FileNotFoundError(path)
```

