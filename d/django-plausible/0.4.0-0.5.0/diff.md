# Comparing `tmp/django-plausible-0.4.0.tar.gz` & `tmp/django-plausible-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plausible-0.4.0.tar", last modified: Sat Oct 29 14:28:49 2022, max compression
+gzip compressed data, was "django-plausible-0.5.0.tar", last modified: Fri May 12 15:20:03 2023, max compression
```

## Comparing `django-plausible-0.4.0.tar` & `django-plausible-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.350203 django-plausible-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-10-29 14:28:42.000000 django-plausible-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-10-29 14:28:49.350203 django-plausible-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-10-29 14:28:42.000000 django-plausible-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.346202 django-plausible-0.4.0/django_plausible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-10-29 14:28:49.000000 django-plausible-0.4.0/django_plausible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-10-29 14:28:49.000000 django-plausible-0.4.0/django_plausible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-29 14:28:49.000000 django-plausible-0.4.0/django_plausible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-29 14:28:49.000000 django-plausible-0.4.0/django_plausible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-29 14:28:49.000000 django-plausible-0.4.0/django_plausible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.346202 django-plausible-0.4.0/plausible/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.346202 django-plausible-0.4.0/plausible/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.346202 django-plausible-0.4.0/plausible/contrib/wagtail/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.346202 django-plausible-0.4.0/plausible/contrib/wagtail/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.350203 django-plausible-0.4.0/plausible/contrib/wagtail/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/templatetags/plausible_wagtail.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/contrib/wagtail/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:49.350203 django-plausible-0.4.0/plausible/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/templatetags/plausible.py
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-10-29 14:28:42.000000 django-plausible-0.4.0/plausible/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-10-29 14:28:49.350203 django-plausible-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-10-29 14:28:42.000000 django-plausible-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-12 15:19:47.000000 django-plausible-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-12 15:20:03.021156 django-plausible-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-12 15:19:47.000000 django-plausible-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/django_plausible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-12 15:20:02.000000 django-plausible-0.5.0/django_plausible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-12 15:20:02.000000 django-plausible-0.5.0/django_plausible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:20:02.000000 django-plausible-0.5.0/django_plausible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 15:20:02.000000 django-plausible-0.5.0/django_plausible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 15:20:02.000000 django-plausible-0.5.0/django_plausible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/contrib/wagtail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/contrib/wagtail/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/contrib/wagtail/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/templatetags/plausible_wagtail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/contrib/wagtail/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:20:03.021156 django-plausible-0.5.0/plausible/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/templatetags/plausible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-12 15:19:47.000000 django-plausible-0.5.0/plausible/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 15:19:47.000000 django-plausible-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-12 15:20:03.025156 django-plausible-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-12 15:19:47.000000 django-plausible-0.5.0/setup.py
```

### Comparing `django-plausible-0.4.0/LICENSE` & `django-plausible-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/PKG-INFO` & `django-plausible-0.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,104 @@
 Metadata-Version: 2.1
 Name: django-plausible
-Version: 0.4.0
+Version: 0.5.0
 Summary:  Django module to provide easy Plausible integration, with Wagtail support
 Home-page: https://github.com/RealOrangeOne/django-plausible
 Author: Jake Howard
 License: BSD
-Description: # django-plausible
-        
-        ![CI](https://github.com/RealOrangeOne/django-plausible/workflows/CI/badge.svg)
-        ![PyPI](https://img.shields.io/pypi/v/django-plausible.svg)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible.svg)
-        ![PyPI - Status](https://img.shields.io/pypi/status/django-plausible.svg)
-        ![PyPI - License](https://img.shields.io/pypi/l/django-plausible.svg)
-        
-        
-        Django module to provide easy [Plausible](https://plausible.io/) integration, with [Wagtail](https://wagtail.io/) support.
-        
-        ## Installation
-        
-        ```
-        pip install django-plausible
-        ```
-        
-        Then simply add `plausible` to `INSTALLED_APPS`.
-        
-        ## Usage
-        
-        `django-plausible` provides a `plausible` template tag, which can be used to output the required [script tag](https://plausible.io/docs/plausible-script) for Plausible.
-        
-        ```html
-        {% load plausible %}
-        
-        {% plausible %}
-        ```
-        
-        Will result in:
-        
-        ```html
-        <script defer data-domain="example.com" src="https://plausible.io/js/plausible.js"></script>
-        ```
-        
-        ### Configuration
-        
-        Configuration can be changed either in `settings.py`, or when calling the `plausible` template tag:
-        
-        - `PLAUSIBLE_DOMAIN`: The domain Plausible is running on (defaults to `plausible.io`)
-        - `PLAUSIBLE_SCRIPT_NAME`: The name of the script to use (defaults to `plausible.js`). See [script extensions](https://plausible.io/docs/script-extensions) for available options.
-        
-        These settings will affect all calls to the `plausible` template tag. To override it at call time, you can also pass them into the template tag:
-        
-        ```
-        {% plausible plausible_domain="my-plausible.com" script_name="plausible.hash.js" %}
-        ```
-        
-        By default, the domain (`data-domain`) used will be based on the request's hostname (using [`request.get_host()`](https://docs.djangoproject.com/en/dev/ref/request-response/#django.http.HttpRequest.get_host)). To override this, pass `site_domain` to the template tag.
-        
-        If the ["compat" script](https://plausible.io/docs/script-extensions#plausiblecompatjs) is used, `django-plausible` will automatically add the required `id` to the `script` tag. It is excluded by default to help hide Plausible's presence.
-        
-        ## Usage with Wagtail
-        
-        Additionally, `django-plausible` provides an (optional) deep integration with [Wagtail](https://wagtail.io), allowing configuration through the Wagtail admin. To enable this, additionally add `plausible.contrib.wagtail` to `INSTALLED_APPS`.
-        
-        Configuration is done through the "Plausible Analytics" [setting](https://docs.wagtail.io/en/stable/reference/contrib/settings.html#settings):
-        
-        - `site_domain`: the value for `data-domain`. If left blank (the default), the request's hostname will be used (as above), **not** the site hostname.
-        - `plausible_domain`: The domain Plausible is running on (as above)
-        - `script_name`: The name of the script to use (as above)
-        
-        To access the template tag, load `plausible_wagtail`, rather than `plausible`. The template tag itself is still `plausible`. Note that unlike the Django variant, the Wagtail template tag doesn't allow options to be passed.
-        
-        ```html
-        {% load plausible_wagtail %}
-        
-        {% plausible %}
-        ```
-        
 Keywords: django plausible wagtail analytics
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: wagtail
+License-File: LICENSE
+
+# django-plausible
+
+![CI](https://github.com/RealOrangeOne/django-plausible/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plausible.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plausible.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plausible.svg)
+
+
+Django module to provide easy [Plausible](https://plausible.io/) integration, with [Wagtail](https://wagtail.io/) support.
+
+## Installation
+
+```
+pip install django-plausible
+```
+
+Then simply add `plausible` to `INSTALLED_APPS`.
+
+## Usage
+
+`django-plausible` provides a `plausible` template tag, which can be used to output the required [script tag](https://plausible.io/docs/plausible-script) for Plausible.
+
+```html
+{% load plausible %}
+
+{% plausible %}
+```
+
+Will result in:
+
+```html
+<script defer data-domain="example.com" src="https://plausible.io/js/plausible.js"></script>
+```
+
+### Configuration
+
+Configuration can be changed either in `settings.py`, or when calling the `plausible` template tag:
+
+- `PLAUSIBLE_DOMAIN`: The domain Plausible is running on (defaults to `plausible.io`)
+- `PLAUSIBLE_SCRIPT_NAME`: The name of the script to use (defaults to `plausible.js`). See [script extensions](https://plausible.io/docs/script-extensions) for available options.
+
+These settings will affect all calls to the `plausible` template tag. To override it at call time, you can also pass them into the template tag:
+
+```
+{% plausible plausible_domain="my-plausible.com" script_name="plausible.hash.js" %}
+```
+
+By default, the domain (`data-domain`) used will be based on the request's hostname (using [`request.get_host()`](https://docs.djangoproject.com/en/dev/ref/request-response/#django.http.HttpRequest.get_host)). To override this, pass `site_domain` to the template tag.
+
+If the ["compat" script](https://plausible.io/docs/script-extensions#plausiblecompatjs) is used, `django-plausible` will automatically add the required `id` to the `script` tag. It is excluded by default to help hide Plausible's presence.
+
+## Usage with Wagtail
+
+Additionally, `django-plausible` provides an (optional) deep integration with [Wagtail](https://wagtail.io), allowing configuration through the Wagtail admin. To enable this, additionally add `plausible.contrib.wagtail` to `INSTALLED_APPS`.
+
+Configuration is done through the "Plausible Analytics" [setting](https://docs.wagtail.io/en/stable/reference/contrib/settings.html#settings):
+
+- `site_domain`: the value for `data-domain`. If left blank (the default), the request's hostname will be used (as above), **not** the site hostname.
+- `plausible_domain`: The domain Plausible is running on (as above)
+- `script_name`: The name of the script to use (as above)
+
+To access the template tag, load `plausible_wagtail`, rather than `plausible`. The template tag itself is still `plausible`. Note that unlike the Django variant, the Wagtail template tag doesn't allow options to be passed.
+
+```html
+{% load plausible_wagtail %}
+
+{% plausible %}
+```
```

#### html2text {}

```diff
@@ -1,22 +1,36 @@
-Metadata-Version: 2.1 Name: django-plausible Version: 0.4.0 Summary: Django
+Metadata-Version: 2.1 Name: django-plausible Version: 0.5.0 Summary: Django
 module to provide easy Plausible integration, with Wagtail support Home-page:
 https://github.com/RealOrangeOne/django-plausible Author: Jake Howard License:
-BSD Description: # django-plausible ![CI](https://github.com/RealOrangeOne/
-django-plausible/workflows/CI/badge.svg) ![PyPI](https://img.shields.io/pypi/v/
-django-plausible.svg) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/django-plausible.svg) ![PyPI - Status](https://img.shields.io/pypi/
-status/django-plausible.svg) ![PyPI - License](https://img.shields.io/pypi/l/
-django-plausible.svg) Django module to provide easy [Plausible](https://
-plausible.io/) integration, with [Wagtail](https://wagtail.io/) support. ##
-Installation ``` pip install django-plausible ``` Then simply add `plausible`
-to `INSTALLED_APPS`. ## Usage `django-plausible` provides a `plausible`
-template tag, which can be used to output the required [script tag](https://
-plausible.io/docs/plausible-script) for Plausible. ```html {% load plausible %}
-{% plausible %} ``` Will result in: ```html
+BSD Keywords: django plausible wagtail analytics Classifier: Environment :: Web
+Environment Classifier: Framework :: Wagtail Classifier: Framework :: Wagtail
+:: 4 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: BSD License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: wagtail
+License-File: LICENSE # django-plausible ![CI](https://github.com/
+RealOrangeOne/django-plausible/workflows/CI/badge.svg) ![PyPI](https://
+img.shields.io/pypi/v/django-plausible.svg) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/django-plausible.svg) ![PyPI - Status](https://
+img.shields.io/pypi/status/django-plausible.svg) ![PyPI - License](https://
+img.shields.io/pypi/l/django-plausible.svg) Django module to provide easy
+[Plausible](https://plausible.io/) integration, with [Wagtail](https://
+wagtail.io/) support. ## Installation ``` pip install django-plausible ``` Then
+simply add `plausible` to `INSTALLED_APPS`. ## Usage `django-plausible`
+provides a `plausible` template tag, which can be used to output the required
+[script tag](https://plausible.io/docs/plausible-script) for Plausible. ```html
+{% load plausible %} {% plausible %} ``` Will result in: ```html
  ``` ### Configuration Configuration can be changed either in `settings.py`, or
 when calling the `plausible` template tag: - `PLAUSIBLE_DOMAIN`: The domain
 Plausible is running on (defaults to `plausible.io`) - `PLAUSIBLE_SCRIPT_NAME`:
 The name of the script to use (defaults to `plausible.js`). See [script
 extensions](https://plausible.io/docs/script-extensions) for available options.
 These settings will affect all calls to the `plausible` template tag. To
 override it at call time, you can also pass them into the template tag: ``` {%
@@ -36,18 +50,8 @@
 stable/reference/contrib/settings.html#settings): - `site_domain`: the value
 for `data-domain`. If left blank (the default), the request's hostname will be
 used (as above), **not** the site hostname. - `plausible_domain`: The domain
 Plausible is running on (as above) - `script_name`: The name of the script to
 use (as above) To access the template tag, load `plausible_wagtail`, rather
 than `plausible`. The template tag itself is still `plausible`. Note that
 unlike the Django variant, the Wagtail template tag doesn't allow options to be
-passed. ```html {% load plausible_wagtail %} {% plausible %} ``` Keywords:
-django plausible wagtail analytics Platform: UNKNOWN Classifier: Environment ::
-Web Environment Classifier: Framework :: Django Classifier: Intended Audience
-:: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: wagtail
+passed. ```html {% load plausible_wagtail %} {% plausible %} ```
```

### Comparing `django-plausible-0.4.0/README.md` & `django-plausible-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/django_plausible.egg-info/PKG-INFO` & `django-plausible-0.5.0/django_plausible.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,104 @@
 Metadata-Version: 2.1
 Name: django-plausible
-Version: 0.4.0
+Version: 0.5.0
 Summary:  Django module to provide easy Plausible integration, with Wagtail support
 Home-page: https://github.com/RealOrangeOne/django-plausible
 Author: Jake Howard
 License: BSD
-Description: # django-plausible
-        
-        ![CI](https://github.com/RealOrangeOne/django-plausible/workflows/CI/badge.svg)
-        ![PyPI](https://img.shields.io/pypi/v/django-plausible.svg)
-        ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible.svg)
-        ![PyPI - Status](https://img.shields.io/pypi/status/django-plausible.svg)
-        ![PyPI - License](https://img.shields.io/pypi/l/django-plausible.svg)
-        
-        
-        Django module to provide easy [Plausible](https://plausible.io/) integration, with [Wagtail](https://wagtail.io/) support.
-        
-        ## Installation
-        
-        ```
-        pip install django-plausible
-        ```
-        
-        Then simply add `plausible` to `INSTALLED_APPS`.
-        
-        ## Usage
-        
-        `django-plausible` provides a `plausible` template tag, which can be used to output the required [script tag](https://plausible.io/docs/plausible-script) for Plausible.
-        
-        ```html
-        {% load plausible %}
-        
-        {% plausible %}
-        ```
-        
-        Will result in:
-        
-        ```html
-        <script defer data-domain="example.com" src="https://plausible.io/js/plausible.js"></script>
-        ```
-        
-        ### Configuration
-        
-        Configuration can be changed either in `settings.py`, or when calling the `plausible` template tag:
-        
-        - `PLAUSIBLE_DOMAIN`: The domain Plausible is running on (defaults to `plausible.io`)
-        - `PLAUSIBLE_SCRIPT_NAME`: The name of the script to use (defaults to `plausible.js`). See [script extensions](https://plausible.io/docs/script-extensions) for available options.
-        
-        These settings will affect all calls to the `plausible` template tag. To override it at call time, you can also pass them into the template tag:
-        
-        ```
-        {% plausible plausible_domain="my-plausible.com" script_name="plausible.hash.js" %}
-        ```
-        
-        By default, the domain (`data-domain`) used will be based on the request's hostname (using [`request.get_host()`](https://docs.djangoproject.com/en/dev/ref/request-response/#django.http.HttpRequest.get_host)). To override this, pass `site_domain` to the template tag.
-        
-        If the ["compat" script](https://plausible.io/docs/script-extensions#plausiblecompatjs) is used, `django-plausible` will automatically add the required `id` to the `script` tag. It is excluded by default to help hide Plausible's presence.
-        
-        ## Usage with Wagtail
-        
-        Additionally, `django-plausible` provides an (optional) deep integration with [Wagtail](https://wagtail.io), allowing configuration through the Wagtail admin. To enable this, additionally add `plausible.contrib.wagtail` to `INSTALLED_APPS`.
-        
-        Configuration is done through the "Plausible Analytics" [setting](https://docs.wagtail.io/en/stable/reference/contrib/settings.html#settings):
-        
-        - `site_domain`: the value for `data-domain`. If left blank (the default), the request's hostname will be used (as above), **not** the site hostname.
-        - `plausible_domain`: The domain Plausible is running on (as above)
-        - `script_name`: The name of the script to use (as above)
-        
-        To access the template tag, load `plausible_wagtail`, rather than `plausible`. The template tag itself is still `plausible`. Note that unlike the Django variant, the Wagtail template tag doesn't allow options to be passed.
-        
-        ```html
-        {% load plausible_wagtail %}
-        
-        {% plausible %}
-        ```
-        
 Keywords: django plausible wagtail analytics
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: wagtail
+License-File: LICENSE
+
+# django-plausible
+
+![CI](https://github.com/RealOrangeOne/django-plausible/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plausible.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plausible.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plausible.svg)
+
+
+Django module to provide easy [Plausible](https://plausible.io/) integration, with [Wagtail](https://wagtail.io/) support.
+
+## Installation
+
+```
+pip install django-plausible
+```
+
+Then simply add `plausible` to `INSTALLED_APPS`.
+
+## Usage
+
+`django-plausible` provides a `plausible` template tag, which can be used to output the required [script tag](https://plausible.io/docs/plausible-script) for Plausible.
+
+```html
+{% load plausible %}
+
+{% plausible %}
+```
+
+Will result in:
+
+```html
+<script defer data-domain="example.com" src="https://plausible.io/js/plausible.js"></script>
+```
+
+### Configuration
+
+Configuration can be changed either in `settings.py`, or when calling the `plausible` template tag:
+
+- `PLAUSIBLE_DOMAIN`: The domain Plausible is running on (defaults to `plausible.io`)
+- `PLAUSIBLE_SCRIPT_NAME`: The name of the script to use (defaults to `plausible.js`). See [script extensions](https://plausible.io/docs/script-extensions) for available options.
+
+These settings will affect all calls to the `plausible` template tag. To override it at call time, you can also pass them into the template tag:
+
+```
+{% plausible plausible_domain="my-plausible.com" script_name="plausible.hash.js" %}
+```
+
+By default, the domain (`data-domain`) used will be based on the request's hostname (using [`request.get_host()`](https://docs.djangoproject.com/en/dev/ref/request-response/#django.http.HttpRequest.get_host)). To override this, pass `site_domain` to the template tag.
+
+If the ["compat" script](https://plausible.io/docs/script-extensions#plausiblecompatjs) is used, `django-plausible` will automatically add the required `id` to the `script` tag. It is excluded by default to help hide Plausible's presence.
+
+## Usage with Wagtail
+
+Additionally, `django-plausible` provides an (optional) deep integration with [Wagtail](https://wagtail.io), allowing configuration through the Wagtail admin. To enable this, additionally add `plausible.contrib.wagtail` to `INSTALLED_APPS`.
+
+Configuration is done through the "Plausible Analytics" [setting](https://docs.wagtail.io/en/stable/reference/contrib/settings.html#settings):
+
+- `site_domain`: the value for `data-domain`. If left blank (the default), the request's hostname will be used (as above), **not** the site hostname.
+- `plausible_domain`: The domain Plausible is running on (as above)
+- `script_name`: The name of the script to use (as above)
+
+To access the template tag, load `plausible_wagtail`, rather than `plausible`. The template tag itself is still `plausible`. Note that unlike the Django variant, the Wagtail template tag doesn't allow options to be passed.
+
+```html
+{% load plausible_wagtail %}
+
+{% plausible %}
+```
```

#### html2text {}

```diff
@@ -1,22 +1,36 @@
-Metadata-Version: 2.1 Name: django-plausible Version: 0.4.0 Summary: Django
+Metadata-Version: 2.1 Name: django-plausible Version: 0.5.0 Summary: Django
 module to provide easy Plausible integration, with Wagtail support Home-page:
 https://github.com/RealOrangeOne/django-plausible Author: Jake Howard License:
-BSD Description: # django-plausible ![CI](https://github.com/RealOrangeOne/
-django-plausible/workflows/CI/badge.svg) ![PyPI](https://img.shields.io/pypi/v/
-django-plausible.svg) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/django-plausible.svg) ![PyPI - Status](https://img.shields.io/pypi/
-status/django-plausible.svg) ![PyPI - License](https://img.shields.io/pypi/l/
-django-plausible.svg) Django module to provide easy [Plausible](https://
-plausible.io/) integration, with [Wagtail](https://wagtail.io/) support. ##
-Installation ``` pip install django-plausible ``` Then simply add `plausible`
-to `INSTALLED_APPS`. ## Usage `django-plausible` provides a `plausible`
-template tag, which can be used to output the required [script tag](https://
-plausible.io/docs/plausible-script) for Plausible. ```html {% load plausible %}
-{% plausible %} ``` Will result in: ```html
+BSD Keywords: django plausible wagtail analytics Classifier: Environment :: Web
+Environment Classifier: Framework :: Wagtail Classifier: Framework :: Wagtail
+:: 4 Classifier: Framework :: Wagtail :: 5 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: BSD License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: wagtail
+License-File: LICENSE # django-plausible ![CI](https://github.com/
+RealOrangeOne/django-plausible/workflows/CI/badge.svg) ![PyPI](https://
+img.shields.io/pypi/v/django-plausible.svg) ![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/django-plausible.svg) ![PyPI - Status](https://
+img.shields.io/pypi/status/django-plausible.svg) ![PyPI - License](https://
+img.shields.io/pypi/l/django-plausible.svg) Django module to provide easy
+[Plausible](https://plausible.io/) integration, with [Wagtail](https://
+wagtail.io/) support. ## Installation ``` pip install django-plausible ``` Then
+simply add `plausible` to `INSTALLED_APPS`. ## Usage `django-plausible`
+provides a `plausible` template tag, which can be used to output the required
+[script tag](https://plausible.io/docs/plausible-script) for Plausible. ```html
+{% load plausible %} {% plausible %} ``` Will result in: ```html
  ``` ### Configuration Configuration can be changed either in `settings.py`, or
 when calling the `plausible` template tag: - `PLAUSIBLE_DOMAIN`: The domain
 Plausible is running on (defaults to `plausible.io`) - `PLAUSIBLE_SCRIPT_NAME`:
 The name of the script to use (defaults to `plausible.js`). See [script
 extensions](https://plausible.io/docs/script-extensions) for available options.
 These settings will affect all calls to the `plausible` template tag. To
 override it at call time, you can also pass them into the template tag: ``` {%
@@ -36,18 +50,8 @@
 stable/reference/contrib/settings.html#settings): - `site_domain`: the value
 for `data-domain`. If left blank (the default), the request's hostname will be
 used (as above), **not** the site hostname. - `plausible_domain`: The domain
 Plausible is running on (as above) - `script_name`: The name of the script to
 use (as above) To access the template tag, load `plausible_wagtail`, rather
 than `plausible`. The template tag itself is still `plausible`. Note that
 unlike the Django variant, the Wagtail template tag doesn't allow options to be
-passed. ```html {% load plausible_wagtail %} {% plausible %} ``` Keywords:
-django plausible wagtail analytics Platform: UNKNOWN Classifier: Environment ::
-Web Environment Classifier: Framework :: Django Classifier: Intended Audience
-:: Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: wagtail
+passed. ```html {% load plausible_wagtail %} {% plausible %} ```
```

### Comparing `django-plausible-0.4.0/django_plausible.egg-info/SOURCES.txt` & `django-plausible-0.5.0/django_plausible.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 django_plausible.egg-info/PKG-INFO
 django_plausible.egg-info/SOURCES.txt
 django_plausible.egg-info/dependency_links.txt
 django_plausible.egg-info/requires.txt
 django_plausible.egg-info/top_level.txt
```

### Comparing `django-plausible-0.4.0/plausible/contrib/wagtail/migrations/0001_initial.py` & `django-plausible-0.5.0/plausible/contrib/wagtail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/plausible/contrib/wagtail/templatetags/plausible_wagtail.py` & `django-plausible-0.5.0/plausible/contrib/wagtail/templatetags/plausible_wagtail.py`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/plausible/contrib/wagtail/validators.py` & `django-plausible-0.5.0/plausible/contrib/wagtail/validators.py`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/plausible/templatetags/plausible.py` & `django-plausible-0.5.0/plausible/templatetags/plausible.py`

 * *Files identical despite different names*

### Comparing `django-plausible-0.4.0/plausible/utils.py` & `django-plausible-0.5.0/plausible/utils.py`

 * *Files identical despite different names*

