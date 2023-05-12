# Comparing `tmp/django-cors-headers-3.9.0.tar.gz` & `tmp/django_cors_headers-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cors-headers-3.9.0.tar", last modified: Tue Sep 28 13:56:44 2021, max compression
+gzip compressed data, was "django_cors_headers-4.0.0.tar", last modified: Fri May 12 09:21:48 2023, max compression
```

## Comparing `django-cors-headers-3.9.0.tar` & `django_cors_headers-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-09-28 13:56:44.267826 django-cors-headers-3.9.0/
--rw-r--r--   0 chainz     (501) staff       (20)     9983 2021-09-28 13:56:37.000000 django-cors-headers-3.9.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1116 2021-02-07 15:09:16.000000 django-cors-headers-3.9.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      255 2021-08-30 15:52:14.000000 django-cors-headers-3.9.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)    15445 2021-09-28 13:56:44.268011 django-cors-headers-3.9.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)    13858 2021-09-28 13:52:24.000000 django-cors-headers-3.9.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      636 2021-08-30 15:52:14.000000 django-cors-headers-3.9.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1844 2021-09-28 13:56:44.268920 django-cors-headers-3.9.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 15:09:16.000000 django-cors-headers-3.9.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-09-28 13:56:44.259714 django-cors-headers-3.9.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-09-28 13:56:44.265414 django-cors-headers-3.9.0/src/corsheaders/
--rw-r--r--   0 chainz     (501) staff       (20)      108 2021-02-07 15:09:16.000000 django-cors-headers-3.9.0/src/corsheaders/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)      312 2021-08-15 11:33:27.000000 django-cors-headers-3.9.0/src/corsheaders/apps.py
--rw-r--r--   0 chainz     (501) staff       (20)     5538 2021-08-15 11:33:27.000000 django-cors-headers-3.9.0/src/corsheaders/checks.py
--rw-r--r--   0 chainz     (501) staff       (20)     1941 2021-08-15 11:33:27.000000 django-cors-headers-3.9.0/src/corsheaders/conf.py
--rw-r--r--   0 chainz     (501) staff       (20)      258 2021-02-07 15:09:16.000000 django-cors-headers-3.9.0/src/corsheaders/defaults.py
--rw-r--r--   0 chainz     (501) staff       (20)     6746 2021-08-15 11:33:27.000000 django-cors-headers-3.9.0/src/corsheaders/middleware.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-15 11:33:27.000000 django-cors-headers-3.9.0/src/corsheaders/py.typed
--rw-r--r--   0 chainz     (501) staff       (20)      255 2021-02-07 15:09:16.000000 django-cors-headers-3.9.0/src/corsheaders/signals.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2021-09-28 13:56:44.267510 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)    15445 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      568 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       12 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       12 2021-09-28 13:56:44.000000 django-cors-headers-3.9.0/src/django_cors_headers.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-12 09:21:48.169854 django_cors_headers-4.0.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    12171 2023-05-12 09:21:44.000000 django_cors_headers-4.0.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1111 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    16571 2023-05-12 09:21:48.169950 django_cors_headers-4.0.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14941 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      500 2023-05-12 08:45:23.000000 django_cors_headers-4.0.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1880 2023-05-12 09:21:48.170310 django_cors_headers-4.0.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-12 09:21:48.159171 django_cors_headers-4.0.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-12 09:21:48.168546 django_cors_headers-4.0.0/src/corsheaders/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/src/corsheaders/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      378 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/src/corsheaders/apps.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5920 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/src/corsheaders/checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     2146 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/src/corsheaders/conf.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      273 2023-05-12 08:45:23.000000 django_cors_headers-4.0.0/src/corsheaders/defaults.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6122 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/src/corsheaders/middleware.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/src/corsheaders/py.typed
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      291 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/src/corsheaders/signals.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-12 09:21:48.169343 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    16571 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      626 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       12 2023-05-12 09:21:48.000000 django_cors_headers-4.0.0/src/django_cors_headers.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-05-12 09:21:48.169724 django_cors_headers-4.0.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     6000 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/tests/test_checks.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1553 2023-04-27 20:44:48.000000 django_cors_headers-4.0.0/tests/test_conf.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    17280 2023-05-12 09:12:46.000000 django_cors_headers-4.0.0/tests/test_middleware.py
```

### Comparing `django-cors-headers-3.9.0/HISTORY.rst` & `django_cors_headers-4.0.0/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,68 @@
-=======
-History
-=======
+=========
+Changelog
+=========
+
+4.0.0 (2023-05-12)
+------------------
+
+* Add ``CORS_ALLOW_PRIVATE_NETWORK_ACCESS`` setting, which enables support for the Local Network Access draft specification.
+
+  Thanks to Issac Kelly in `PR #745 <https://github.com/adamchainz/django-cors-headers/pull/745>`__ and jjurgens0 in `PR #833 <https://github.com/adamchainz/django-cors-headers/pull/833>`__.
+
+* Remove three headers from the default "accept list": ``accept-encoding``, ``dnt``, and ``origin``.
+  These are `Forbidden header names <https://developer.mozilla.org/en-US/docs/Glossary/Forbidden_header_name>`__, which means requests JavaScript can never set them.
+  Consequently, allowing them via CORS has no effect.
+
+  Thanks to jub0bs for the report in `Issue #842 <https://github.com/adamchainz/django-cors-headers/issues/842>`__.
+
+* Drop the ``CORS_REPLACE_HTTPS_REFERER`` setting and ``CorsPostCsrfMiddleware``.
+  Since Django 1.9, the ``CSRF_TRUSTED_ORIGINS`` setting has been the preferred solution to making CSRF checks pass for CORS requests.
+  The removed setting and middleware only existed as a workaround for Django versions before 1.9.
+
+* Add async support to the middleware, reducing overhead on async views.
+
+3.14.0 (2023-02-25)
+-------------------
+
+* Support Django 4.2.
+
+* Switch from ``urlparse()`` to ``urlsplit()`` for URL parsing, reducing the middleware runtime up to 5%.
+  This changes the type passed to ``origin_found_in_white_lists()``, so if you have subclassed the middleware to override this method, you should check it is compatible (it most likely is).
+
+  Thanks to Thibaut Decombe in `PR #793 <https://github.com/adamchainz/django-cors-headers/pull/793>`__.
+
+3.13.0 (2022-06-05)
+-------------------
+
+* Support Python 3.11.
+
+* Support Django 4.1.
+
+3.12.0 (2022-05-10)
+-------------------
+
+* Drop support for Django 2.2, 3.0, and 3.1.
+
+3.11.0 (2022-01-10)
+-------------------
+
+* Drop Python 3.6 support.
+
+3.10.1 (2021-12-05)
+-------------------
+
+* Prevent a crash when an invalid ``Origin`` header is sent.
+
+  Thanks to minusf for the report in `Issue #701 <https://github.com/adamchainz/django-cors-headers/issues/701>`__.
+
+3.10.0 (2021-10-05)
+-------------------
+
+* Support Python 3.10.
 
 3.9.0 (2021-09-28)
 ------------------
 
 * Support Django 4.0.
 
 3.8.0 (2021-08-15)
```

### Comparing `django-cors-headers-3.9.0/LICENSE` & `django_cors_headers-4.0.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2021 Otto Yiu (https://ottoyiu.com) and other contributors.
+Copyright (c) 2017 Otto Yiu (https://ottoyiu.com) and other contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-cors-headers-3.9.0/PKG-INFO` & `django_cors_headers-4.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
-Name: django-cors-headers
-Version: 3.9.0
+Name: django_cors_headers
+Version: 4.0.0
 Summary: django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 Home-page: https://github.com/adamchainz/django-cors-headers
 Author: Otto Yiu
 Author-email: otto@live.ca
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
-License: MIT License
-Project-URL: Changelog, https://github.com/adamchainz/django-cors-headers/blob/main/HISTORY.rst
+License: MIT
+Project-URL: Changelog, https://github.com/adamchainz/django-cors-headers/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: django,cors,middleware,rest,api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 django-cors-headers
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-cors-headers/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-cors-headers/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
-.. image:: https://img.shields.io/codecov/c/github/adamchainz/django-cors-headers/main?style=for-the-badge
-  :target: https://app.codecov.io/gh/adamchainz/django-cors-headers
+.. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
+  :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-cors-headers.svg?style=for-the-badge
     :target: https://pypi.org/project/django-cors-headers/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
     :target: https://github.com/psf/black
 
@@ -66,29 +67,30 @@
 important you understand the implications before adding the headers, since you
 could be unintentionally opening up your site's private data to others.
 
 Some good resources to read on the subject are:
 
 * Julia Evans' `introductory comic <https://drawings.jvns.ca/cors/>`__ and
   `educational quiz <https://questions.wizardzines.com/cors.html>`__.
-* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
+* Jake Archibald’s `How to win at CORS <https://jakearchibald.com/2021/cors/>`__
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
+* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.6 to 3.9 supported.
+Python 3.7 to 3.11 supported.
 
-Django 2.2 to 4.0 supported.
+Django 3.2 to 4.2 supported.
 
 ----
 
-**Are your tests slow?**
-Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
+**Want to work smarter and faster?**
+Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
 
 Setup
 -----
 
 Install from **pip**:
@@ -123,17 +125,14 @@
     ]
 
 ``CorsMiddleware`` should be placed as high as possible, especially before any
 middleware that can generate responses such as Django's ``CommonMiddleware`` or
 Whitenoise's ``WhiteNoiseMiddleware``. If it is not before, it will not be able
 to add the CORS headers to these responses.
 
-Also if you are using ``CORS_REPLACE_HTTPS_REFERER`` it should be placed before
-Django's ``CsrfViewMiddleware`` (see more below).
-
 About
 -----
 
 **django-cors-headers** was created in January 2013 by Otto Yiu. It went
 unmaintained from August 2015 and was forked in January 2016 to the package
 `django-cors-middleware <https://github.com/zestedesavoir/django-cors-middleware>`_
 by Laville Augustin at Zeste de Savoir.
@@ -160,244 +159,230 @@
 * ``CORS_ALLOWED_ORIGIN_REGEXES``
 * ``CORS_ALLOW_ALL_ORIGINS``
 
 ``CORS_ALLOWED_ORIGINS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A list of origins that are authorized to make cross-site HTTP requests.
+The origins in this setting will be allowed, and the requesting origin will be echoed back to the client in the |access-control-allow-origin header|__.
 Defaults to ``[]``.
 
-An Origin is defined by
-`the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_
-as a URI scheme + hostname + port, or one of the special values `'null'` or
-`'file://'`.
-Default ports (HTTPS = 443, HTTP = 80) are optional here.
-
-The special value `null` is sent by the browser in
-`"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__,
-such as when the client is running from a ``file://`` domain.
-The special value `file://` is sent accidentally by some versions of Chrome on
-Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
+.. |access-control-allow-origin header| replace:: ``access-control-allow-origin`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin
+
+An Origin is defined by `the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_ as a URI scheme + hostname + port, or one of the special values ``'null'`` or ``'file://'``.
+Default ports (HTTPS = 443, HTTP = 80) are optional.
+
+The special value ``null`` is sent by the browser in `"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__, such as when the client is running from a ``file://`` domain.
+The special value `file://` is sent accidentally by some versions of Chrome on Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
         "https://example.com",
         "https://sub.example.com",
         "http://localhost:8080",
         "http://127.0.0.1:9000",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works
-as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOWED_ORIGIN_REGEXES: Sequence[str | Pattern[str]]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of strings representing regexes that match Origins that are authorized
-to make cross-site HTTP requests. Defaults to ``[]``. Useful when
-``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number
-of subdomains.
+A list of strings representing regexes that match Origins that are authorized to make cross-site HTTP requests.
+Defaults to ``[]``.
+Useful when ``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number of subdomains.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGIN_REGEXES = [
         r"^https://\w+\.example\.com$",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOW_ALL_ORIGINS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, all origins will be allowed. Other settings restricting allowed
-origins will be ignored. Defaults to ``False``.
+If ``True``, all origins will be allowed.
+Other settings restricting allowed origins will be ignored.
+Defaults to ``False``.
 
-Setting this to ``True`` can be *dangerous*, as it allows any website to make
-cross-origin requests to yours. Generally you'll want to restrict the list of
-allowed origins with ``CORS_ALLOWED_ORIGINS`` or
-``CORS_ALLOWED_ORIGIN_REGEXES``.
+Setting this to ``True`` can be *dangerous*, as it allows any website to make cross-origin requests to yours.
+Generally you'll want to restrict the list of allowed origins with ``CORS_ALLOWED_ORIGINS`` or ``CORS_ALLOWED_ORIGIN_REGEXES``.
 
-Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still works as an alias, with the new name taking precedence.
 
 --------------
 
 The following are optional settings, for which the defaults probably suffice.
 
 ``CORS_URLS_REGEX: str | Pattern[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A regex which restricts the URL's for which the CORS headers will be sent.
-Defaults to ``r'^.*$'``, i.e. match all URL's. Useful when you only need CORS
-on a part of your site, e.g. an API at ``/api/``.
+Defaults to ``r'^.*$'``, i.e. match all URL's.
+Useful when you only need CORS on a part of your site, e.g. an API at ``/api/``.
 
 Example:
 
 .. code-block:: python
 
     CORS_URLS_REGEX = r"^/api/.*$"
 
 ``CORS_ALLOW_METHODS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of HTTP verbs that are allowed for the actual request. Defaults to:
+A list of HTTP verbs that are allowed for the actual request.
+Defaults to:
 
 .. code-block:: python
 
-    CORS_ALLOW_METHODS = [
+    CORS_ALLOW_METHODS = (
         "DELETE",
         "GET",
         "OPTIONS",
         "PATCH",
         "POST",
         "PUT",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_methods`` so you
-can just extend it with your custom methods. This allows you to keep up to date
-with any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_methods`` so you can just extend it with your custom methods.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_methods
 
-    CORS_ALLOW_METHODS = list(default_methods) + [
+    CORS_ALLOW_METHODS = (
+        *default_methods,
         "POKE",
-    ]
+    )
 
 ``CORS_ALLOW_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of non-standard HTTP headers that can be used when making the actual
-request. Defaults to:
+The list of non-standard HTTP headers that you permit in requests from the browser.
+Sets the |Access-Control-Allow-Headers header|__ in responses to `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__.
+Defaults to:
+
+.. |Access-Control-Allow-Headers header| replace:: ``Access-Control-Allow-Headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Headers
 
 .. code-block:: python
 
-    CORS_ALLOW_HEADERS = [
+    CORS_ALLOW_HEADERS = (
         "accept",
-        "accept-encoding",
         "authorization",
         "content-type",
-        "dnt",
-        "origin",
         "user-agent",
         "x-csrftoken",
         "x-requested-with",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_headers`` so you
-can extend it with your custom headers. This allows you to keep up to date with
-any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_headers`` so you can extend it with your custom headers.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_headers
 
-    CORS_ALLOW_HEADERS = list(default_headers) + [
+    CORS_ALLOW_HEADERS = (
+        *default_headers,
         "my-custom-header",
-    ]
+    )
 
 ``CORS_EXPOSE_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of HTTP headers that are to be exposed to the browser. Defaults to
-``[]``.
+The list of extra HTTP headers to expose to the browser, in addition to the default `safelisted headers <https://developer.mozilla.org/en-US/docs/Glossary/CORS-safelisted_response_header>`__.
+If non-empty, these are declared in the |access-control-expose-headers header|__.
+Defaults to ``[]``.
 
+.. |access-control-expose-headers header| replace:: ``access-control-expose-headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Expose-Headers
 
 ``CORS_PREFLIGHT_MAX_AGE: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The number of seconds a client/browser can cache the preflight response. If
-this is 0 (or any falsey value), no max age header will be sent. Defaults to
-``86400`` (one day).
-
-
-**Note:** A preflight request is an extra request that is made when making a
-"not-so-simple" request (e.g. ``Content-Type`` is not
-``application/x-www-form-urlencoded``) to determine what requests the server
-actually accepts. Read more about it in the
-`CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#Preflighted_requests>`_.
+The number of seconds the browser can cache the preflight response.
+This sets the |access-control-max-age header|__ in preflight responses.
+If this is 0 (or any falsey value), no max age header will be sent.
+Defaults to ``86400`` (one day).
+
+.. |access-control-max-age header| replace:: ``access-control-max-age`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Max-Age
+
+**Note:**
+Browsers send `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__ before certain “non-simple” requests, to check they will be allowed.
+Read more about it in the `CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#preflighted_requests>`_.
 
 ``CORS_ALLOW_CREDENTIALS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, cookies will be allowed to be included in cross-site HTTP
-requests. Defaults to ``False``.
+If ``True``, cookies will be allowed to be included in cross-site HTTP requests.
+This sets the |access-control-allow-credentials header|__ in preflight and normal responses.
+Defaults to ``False``.
+
+.. |access-control-allow-credentials header| replace:: ``Access-Control-Allow-Credentials`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/access-control-allow-credentials
 
-Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to
-``'Lax'`` by default, which will prevent Django's session cookie being sent
-cross-domain. Change it to ``None`` to bypass this security restriction.
+Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to ``'Lax'`` by default, which will prevent Django's session cookie being sent cross-domain.
+Change the setting to ``'None'`` if you need to bypass this security restriction.
 
-.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/stable/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+
+``CORS_ALLOW_PRIVATE_NETWORK: bool``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If ``True``, allow requests from sites on “public” IP to this server on a “private” IP.
+In such cases, browsers send an extra CORS header ``access-control-request-private-network``, for which ``OPTIONS`` responses must contain ``access-control-allow-private-network: true``.
+
+Refer to:
+
+* `Local Network Access <https://wicg.github.io/local-network-access/>`__, the W3C Community Draft specification.
+* `Private Network Access: introducing preflights <https://developer.chrome.com/blog/private-network-access-preflight/>`__, a blog post from the Google Chrome team.
 
 CSRF Integration
 ----------------
 
 Most sites will need to take advantage of the `Cross-Site Request Forgery
-protection <https://docs.djangoproject.com/en/3.0/ref/csrf/>`_ that Django
+protection <https://docs.djangoproject.com/en/stable/ref/csrf/>`_ that Django
 offers. CORS and CSRF are separate, and Django has no way of using your CORS
 configuration to exempt sites from the ``Referer`` checking that it does on
 secure requests. The way to do that is with its `CSRF_TRUSTED_ORIGINS setting
-<https://docs.djangoproject.com/en/3.0/ref/settings/#csrf-trusted-origins>`_.
+<https://docs.djangoproject.com/en/stable/ref/settings/#csrf-trusted-origins>`_.
 For example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
-        "http://read.only.com",
-        "http://change.allowed.com",
+        "https://read-only.example.com",
+        "https://read-and-write.example.com",
     ]
 
     CSRF_TRUSTED_ORIGINS = [
-        "change.allowed.com",
-    ]
-
-``CORS_REPLACE_HTTPS_REFERER: bool``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-``CSRF_TRUSTED_ORIGINS`` was introduced in Django 1.9, so users of earlier
-versions will need an alternate solution. If ``CORS_REPLACE_HTTPS_REFERER`` is
-``True``, ``CorsMiddleware`` will change the ``Referer`` header to something
-that will pass Django's CSRF checks whenever the CORS checks pass. Defaults to
-``False``.
-
-Note that unlike ``CSRF_TRUSTED_ORIGINS``, this setting does not allow you to
-distinguish between domains that are trusted to *read* resources by CORS and
-domains that are trusted to *change* resources by avoiding CSRF protection.
-
-With this feature enabled you should also add
-``corsheaders.middleware.CorsPostCsrfMiddleware`` after
-``django.middleware.csrf.CsrfViewMiddleware`` in your ``MIDDLEWARE_CLASSES`` to
-undo the ``Referer`` replacement:
-
-.. code-block:: python
-
-    MIDDLEWARE_CLASSES = [
-        ...,
-        "corsheaders.middleware.CorsMiddleware",
-        ...,
-        "django.middleware.csrf.CsrfViewMiddleware",
-        "corsheaders.middleware.CorsPostCsrfMiddleware",
-        ...,
+        "https://read-and-write.example.com",
     ]
 
 Signals
 -------
 
 If you have a use case that requires more than just the above configuration,
 you can attach code to check if a given request should be allowed. For example,
 this can be used to read the list of origins you allow from a model. Attach any
 number of handlers to the ``check_request_enabled``
-`Django signal <https://docs.djangoproject.com/en/3.0/ref/signals/>`_, which
+`Django signal <https://docs.djangoproject.com/en/stable/ref/signals/>`_, which
 provides the ``request`` argument (use ``**kwargs`` in your handler to protect
 against any future arguments being added). If any handler attached to the
 signal returns a truthy value, the request will be allowed.
 
 For example you might define a handler like this:
 
 .. code-block:: python
@@ -405,21 +390,21 @@
     # myapp/handlers.py
     from corsheaders.signals import check_request_enabled
 
     from myapp.models import MySite
 
 
     def cors_allow_mysites(sender, request, **kwargs):
-        return MySite.objects.filter(host=request.host).exists()
+        return MySite.objects.filter(host=request.headers["origin"]).exists()
 
 
     check_request_enabled.connect(cors_allow_mysites)
 
 Then connect it at app ready time using a `Django AppConfig
-<https://docs.djangoproject.com/en/3.0/ref/applications/>`_:
+<https://docs.djangoproject.com/en/stable/ref/applications/>`_:
 
 .. code-block:: python
 
     # myapp/__init__.py
 
     default_app_config = "myapp.apps.MyAppConfig"
 
@@ -454,9 +439,7 @@
 
 
     def cors_allow_api_to_everyone(sender, request, **kwargs):
         return request.path.startswith("/api/")
 
 
     check_request_enabled.connect(cors_allow_api_to_everyone)
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-cors-headers-3.9.0/README.rst` & `django_cors_headers-4.0.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ===================
 django-cors-headers
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-cors-headers/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-cors-headers/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
-.. image:: https://img.shields.io/codecov/c/github/adamchainz/django-cors-headers/main?style=for-the-badge
-  :target: https://app.codecov.io/gh/adamchainz/django-cors-headers
+.. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
+  :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-cors-headers.svg?style=for-the-badge
     :target: https://pypi.org/project/django-cors-headers/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
     :target: https://github.com/psf/black
 
@@ -29,29 +29,30 @@
 important you understand the implications before adding the headers, since you
 could be unintentionally opening up your site's private data to others.
 
 Some good resources to read on the subject are:
 
 * Julia Evans' `introductory comic <https://drawings.jvns.ca/cors/>`__ and
   `educational quiz <https://questions.wizardzines.com/cors.html>`__.
-* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
+* Jake Archibald’s `How to win at CORS <https://jakearchibald.com/2021/cors/>`__
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
+* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.6 to 3.9 supported.
+Python 3.7 to 3.11 supported.
 
-Django 2.2 to 4.0 supported.
+Django 3.2 to 4.2 supported.
 
 ----
 
-**Are your tests slow?**
-Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
+**Want to work smarter and faster?**
+Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
 
 Setup
 -----
 
 Install from **pip**:
@@ -86,17 +87,14 @@
     ]
 
 ``CorsMiddleware`` should be placed as high as possible, especially before any
 middleware that can generate responses such as Django's ``CommonMiddleware`` or
 Whitenoise's ``WhiteNoiseMiddleware``. If it is not before, it will not be able
 to add the CORS headers to these responses.
 
-Also if you are using ``CORS_REPLACE_HTTPS_REFERER`` it should be placed before
-Django's ``CsrfViewMiddleware`` (see more below).
-
 About
 -----
 
 **django-cors-headers** was created in January 2013 by Otto Yiu. It went
 unmaintained from August 2015 and was forked in January 2016 to the package
 `django-cors-middleware <https://github.com/zestedesavoir/django-cors-middleware>`_
 by Laville Augustin at Zeste de Savoir.
@@ -123,244 +121,230 @@
 * ``CORS_ALLOWED_ORIGIN_REGEXES``
 * ``CORS_ALLOW_ALL_ORIGINS``
 
 ``CORS_ALLOWED_ORIGINS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A list of origins that are authorized to make cross-site HTTP requests.
+The origins in this setting will be allowed, and the requesting origin will be echoed back to the client in the |access-control-allow-origin header|__.
 Defaults to ``[]``.
 
-An Origin is defined by
-`the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_
-as a URI scheme + hostname + port, or one of the special values `'null'` or
-`'file://'`.
-Default ports (HTTPS = 443, HTTP = 80) are optional here.
-
-The special value `null` is sent by the browser in
-`"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__,
-such as when the client is running from a ``file://`` domain.
-The special value `file://` is sent accidentally by some versions of Chrome on
-Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
+.. |access-control-allow-origin header| replace:: ``access-control-allow-origin`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin
+
+An Origin is defined by `the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_ as a URI scheme + hostname + port, or one of the special values ``'null'`` or ``'file://'``.
+Default ports (HTTPS = 443, HTTP = 80) are optional.
+
+The special value ``null`` is sent by the browser in `"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__, such as when the client is running from a ``file://`` domain.
+The special value `file://` is sent accidentally by some versions of Chrome on Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
         "https://example.com",
         "https://sub.example.com",
         "http://localhost:8080",
         "http://127.0.0.1:9000",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works
-as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOWED_ORIGIN_REGEXES: Sequence[str | Pattern[str]]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of strings representing regexes that match Origins that are authorized
-to make cross-site HTTP requests. Defaults to ``[]``. Useful when
-``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number
-of subdomains.
+A list of strings representing regexes that match Origins that are authorized to make cross-site HTTP requests.
+Defaults to ``[]``.
+Useful when ``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number of subdomains.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGIN_REGEXES = [
         r"^https://\w+\.example\.com$",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOW_ALL_ORIGINS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, all origins will be allowed. Other settings restricting allowed
-origins will be ignored. Defaults to ``False``.
+If ``True``, all origins will be allowed.
+Other settings restricting allowed origins will be ignored.
+Defaults to ``False``.
 
-Setting this to ``True`` can be *dangerous*, as it allows any website to make
-cross-origin requests to yours. Generally you'll want to restrict the list of
-allowed origins with ``CORS_ALLOWED_ORIGINS`` or
-``CORS_ALLOWED_ORIGIN_REGEXES``.
+Setting this to ``True`` can be *dangerous*, as it allows any website to make cross-origin requests to yours.
+Generally you'll want to restrict the list of allowed origins with ``CORS_ALLOWED_ORIGINS`` or ``CORS_ALLOWED_ORIGIN_REGEXES``.
 
-Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still works as an alias, with the new name taking precedence.
 
 --------------
 
 The following are optional settings, for which the defaults probably suffice.
 
 ``CORS_URLS_REGEX: str | Pattern[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A regex which restricts the URL's for which the CORS headers will be sent.
-Defaults to ``r'^.*$'``, i.e. match all URL's. Useful when you only need CORS
-on a part of your site, e.g. an API at ``/api/``.
+Defaults to ``r'^.*$'``, i.e. match all URL's.
+Useful when you only need CORS on a part of your site, e.g. an API at ``/api/``.
 
 Example:
 
 .. code-block:: python
 
     CORS_URLS_REGEX = r"^/api/.*$"
 
 ``CORS_ALLOW_METHODS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of HTTP verbs that are allowed for the actual request. Defaults to:
+A list of HTTP verbs that are allowed for the actual request.
+Defaults to:
 
 .. code-block:: python
 
-    CORS_ALLOW_METHODS = [
+    CORS_ALLOW_METHODS = (
         "DELETE",
         "GET",
         "OPTIONS",
         "PATCH",
         "POST",
         "PUT",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_methods`` so you
-can just extend it with your custom methods. This allows you to keep up to date
-with any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_methods`` so you can just extend it with your custom methods.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_methods
 
-    CORS_ALLOW_METHODS = list(default_methods) + [
+    CORS_ALLOW_METHODS = (
+        *default_methods,
         "POKE",
-    ]
+    )
 
 ``CORS_ALLOW_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of non-standard HTTP headers that can be used when making the actual
-request. Defaults to:
+The list of non-standard HTTP headers that you permit in requests from the browser.
+Sets the |Access-Control-Allow-Headers header|__ in responses to `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__.
+Defaults to:
+
+.. |Access-Control-Allow-Headers header| replace:: ``Access-Control-Allow-Headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Headers
 
 .. code-block:: python
 
-    CORS_ALLOW_HEADERS = [
+    CORS_ALLOW_HEADERS = (
         "accept",
-        "accept-encoding",
         "authorization",
         "content-type",
-        "dnt",
-        "origin",
         "user-agent",
         "x-csrftoken",
         "x-requested-with",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_headers`` so you
-can extend it with your custom headers. This allows you to keep up to date with
-any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_headers`` so you can extend it with your custom headers.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_headers
 
-    CORS_ALLOW_HEADERS = list(default_headers) + [
+    CORS_ALLOW_HEADERS = (
+        *default_headers,
         "my-custom-header",
-    ]
+    )
 
 ``CORS_EXPOSE_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of HTTP headers that are to be exposed to the browser. Defaults to
-``[]``.
+The list of extra HTTP headers to expose to the browser, in addition to the default `safelisted headers <https://developer.mozilla.org/en-US/docs/Glossary/CORS-safelisted_response_header>`__.
+If non-empty, these are declared in the |access-control-expose-headers header|__.
+Defaults to ``[]``.
 
+.. |access-control-expose-headers header| replace:: ``access-control-expose-headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Expose-Headers
 
 ``CORS_PREFLIGHT_MAX_AGE: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The number of seconds a client/browser can cache the preflight response. If
-this is 0 (or any falsey value), no max age header will be sent. Defaults to
-``86400`` (one day).
-
-
-**Note:** A preflight request is an extra request that is made when making a
-"not-so-simple" request (e.g. ``Content-Type`` is not
-``application/x-www-form-urlencoded``) to determine what requests the server
-actually accepts. Read more about it in the
-`CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#Preflighted_requests>`_.
+The number of seconds the browser can cache the preflight response.
+This sets the |access-control-max-age header|__ in preflight responses.
+If this is 0 (or any falsey value), no max age header will be sent.
+Defaults to ``86400`` (one day).
+
+.. |access-control-max-age header| replace:: ``access-control-max-age`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Max-Age
+
+**Note:**
+Browsers send `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__ before certain “non-simple” requests, to check they will be allowed.
+Read more about it in the `CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#preflighted_requests>`_.
 
 ``CORS_ALLOW_CREDENTIALS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, cookies will be allowed to be included in cross-site HTTP
-requests. Defaults to ``False``.
+If ``True``, cookies will be allowed to be included in cross-site HTTP requests.
+This sets the |access-control-allow-credentials header|__ in preflight and normal responses.
+Defaults to ``False``.
 
-Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to
-``'Lax'`` by default, which will prevent Django's session cookie being sent
-cross-domain. Change it to ``None`` to bypass this security restriction.
+.. |access-control-allow-credentials header| replace:: ``Access-Control-Allow-Credentials`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/access-control-allow-credentials
 
-.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to ``'Lax'`` by default, which will prevent Django's session cookie being sent cross-domain.
+Change the setting to ``'None'`` if you need to bypass this security restriction.
+
+.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/stable/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+
+``CORS_ALLOW_PRIVATE_NETWORK: bool``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If ``True``, allow requests from sites on “public” IP to this server on a “private” IP.
+In such cases, browsers send an extra CORS header ``access-control-request-private-network``, for which ``OPTIONS`` responses must contain ``access-control-allow-private-network: true``.
+
+Refer to:
+
+* `Local Network Access <https://wicg.github.io/local-network-access/>`__, the W3C Community Draft specification.
+* `Private Network Access: introducing preflights <https://developer.chrome.com/blog/private-network-access-preflight/>`__, a blog post from the Google Chrome team.
 
 CSRF Integration
 ----------------
 
 Most sites will need to take advantage of the `Cross-Site Request Forgery
-protection <https://docs.djangoproject.com/en/3.0/ref/csrf/>`_ that Django
+protection <https://docs.djangoproject.com/en/stable/ref/csrf/>`_ that Django
 offers. CORS and CSRF are separate, and Django has no way of using your CORS
 configuration to exempt sites from the ``Referer`` checking that it does on
 secure requests. The way to do that is with its `CSRF_TRUSTED_ORIGINS setting
-<https://docs.djangoproject.com/en/3.0/ref/settings/#csrf-trusted-origins>`_.
+<https://docs.djangoproject.com/en/stable/ref/settings/#csrf-trusted-origins>`_.
 For example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
-        "http://read.only.com",
-        "http://change.allowed.com",
+        "https://read-only.example.com",
+        "https://read-and-write.example.com",
     ]
 
     CSRF_TRUSTED_ORIGINS = [
-        "change.allowed.com",
-    ]
-
-``CORS_REPLACE_HTTPS_REFERER: bool``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-``CSRF_TRUSTED_ORIGINS`` was introduced in Django 1.9, so users of earlier
-versions will need an alternate solution. If ``CORS_REPLACE_HTTPS_REFERER`` is
-``True``, ``CorsMiddleware`` will change the ``Referer`` header to something
-that will pass Django's CSRF checks whenever the CORS checks pass. Defaults to
-``False``.
-
-Note that unlike ``CSRF_TRUSTED_ORIGINS``, this setting does not allow you to
-distinguish between domains that are trusted to *read* resources by CORS and
-domains that are trusted to *change* resources by avoiding CSRF protection.
-
-With this feature enabled you should also add
-``corsheaders.middleware.CorsPostCsrfMiddleware`` after
-``django.middleware.csrf.CsrfViewMiddleware`` in your ``MIDDLEWARE_CLASSES`` to
-undo the ``Referer`` replacement:
-
-.. code-block:: python
-
-    MIDDLEWARE_CLASSES = [
-        ...,
-        "corsheaders.middleware.CorsMiddleware",
-        ...,
-        "django.middleware.csrf.CsrfViewMiddleware",
-        "corsheaders.middleware.CorsPostCsrfMiddleware",
-        ...,
+        "https://read-and-write.example.com",
     ]
 
 Signals
 -------
 
 If you have a use case that requires more than just the above configuration,
 you can attach code to check if a given request should be allowed. For example,
 this can be used to read the list of origins you allow from a model. Attach any
 number of handlers to the ``check_request_enabled``
-`Django signal <https://docs.djangoproject.com/en/3.0/ref/signals/>`_, which
+`Django signal <https://docs.djangoproject.com/en/stable/ref/signals/>`_, which
 provides the ``request`` argument (use ``**kwargs`` in your handler to protect
 against any future arguments being added). If any handler attached to the
 signal returns a truthy value, the request will be allowed.
 
 For example you might define a handler like this:
 
 .. code-block:: python
@@ -368,21 +352,21 @@
     # myapp/handlers.py
     from corsheaders.signals import check_request_enabled
 
     from myapp.models import MySite
 
 
     def cors_allow_mysites(sender, request, **kwargs):
-        return MySite.objects.filter(host=request.host).exists()
+        return MySite.objects.filter(host=request.headers["origin"]).exists()
 
 
     check_request_enabled.connect(cors_allow_mysites)
 
 Then connect it at app ready time using a `Django AppConfig
-<https://docs.djangoproject.com/en/3.0/ref/applications/>`_:
+<https://docs.djangoproject.com/en/stable/ref/applications/>`_:
 
 .. code-block:: python
 
     # myapp/__init__.py
 
     default_app_config = "myapp.apps.MyAppConfig"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-cors-headers-3.9.0/setup.cfg` & `django_cors_headers-4.0.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,81 @@
 [metadata]
-name = django-cors-headers
-version = 3.9.0
+name = django_cors_headers
+version = 4.0.0
 description = django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 long_description = file: README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/adamchainz/django-cors-headers
 author = Otto Yiu
 author_email = otto@live.ca
 maintainer = Adam Johnson
 maintainer_email = me@adamj.eu
-url = https://github.com/adamchainz/django-cors-headers
-project_urls = 
-	Changelog = https://github.com/adamchainz/django-cors-headers/blob/main/HISTORY.rst
-	Twitter = https://twitter.com/adamchainz
-license = MIT License
-keywords = 
-	django
-	cors
-	middleware
-	rest
-	api
+license = MIT
+license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 2.2
-	Framework :: Django :: 3.0
-	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
+	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
+	Natural Language :: English
 	Operating System :: OS Independent
-	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Topic :: Software Development :: Libraries :: Application Frameworks
-	Topic :: Software Development :: Libraries :: Python Modules
-license_file = LICENSE
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: Implementation :: CPython
+	Typing :: Typed
+keywords = 
+	django
+	cors
+	middleware
+	rest
+	api
+project_urls = 
+	Changelog = https://github.com/adamchainz/django-cors-headers/blob/main/CHANGELOG.rst
+	Mastodon = https://fosstodon.org/@adamchainz
+	Twitter = https://twitter.com/adamchainz
 
 [options]
-package_dir = 
-	=src
 packages = find:
+install_requires = 
+	Django>=3.2
+python_requires = >=3.7
 include_package_data = True
-install_requires = Django>=2.2
-python_requires = >=3.6
+package_dir = 
+	=src
 zip_safe = False
 
 [options.packages.find]
 where = src
 
 [coverage:run]
 branch = True
-source = corsheaders
+parallel = True
+source = 
+	corsheaders
+	tests
 
 [coverage:paths]
 source = 
 	src
-	.tox/*/site-packages
+	.tox/**/site-packages
 
 [coverage:report]
 show_missing = True
 
 [flake8]
-max-line-length = 80
-select = E,F,W,B,B950,C,I,TYP
-ignore = E203,E501,W503
+max-line-length = 88
+extend-ignore = E203
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-cors-headers-3.9.0/src/corsheaders/checks.py` & `django_cors_headers-4.0.0/src/corsheaders/checks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from __future__ import annotations
+
 import re
 from collections.abc import Sequence
-from typing import Any, List, Tuple, Type, Union
-from urllib.parse import urlparse
+from typing import Any
+from urllib.parse import urlsplit
 
-from django.apps import AppConfig
 from django.conf import settings
+from django.core.checks import CheckMessage
 from django.core.checks import Error
 
 from corsheaders.conf import conf
 
 re_type = type(re.compile(""))
 
 
-def check_settings(app_configs: List[AppConfig], **kwargs: Any) -> List[Error]:
-    errors = []
+def check_settings(**kwargs: Any) -> list[CheckMessage]:
+    errors: list[CheckMessage] = []
 
     if not is_sequence(conf.CORS_ALLOW_HEADERS, str):
         errors.append(
             Error(
                 "CORS_ALLOW_HEADERS should be a sequence of strings.",
                 id="corsheaders.E001",
             )
@@ -32,14 +34,22 @@
         )
 
     if not isinstance(conf.CORS_ALLOW_CREDENTIALS, bool):
         errors.append(  # type: ignore [unreachable]
             Error("CORS_ALLOW_CREDENTIALS should be a bool.", id="corsheaders.E003")
         )
 
+    if not isinstance(conf.CORS_ALLOW_PRIVATE_NETWORK, bool):
+        errors.append(  # type: ignore [unreachable]
+            Error(
+                "CORS_ALLOW_PRIVATE_NETWORK should be a bool.",
+                id="corsheaders.E015",
+            )
+        )
+
     if (
         not isinstance(conf.CORS_PREFLIGHT_MAX_AGE, int)
         or conf.CORS_PREFLIGHT_MAX_AGE < 0
     ):
         errors.append(
             Error(
                 (
@@ -81,15 +91,15 @@
             # From files on Chrome on Android
             # https://bugs.chromium.org/p/chromium/issues/detail?id=991107
             "file://",
         )
         for origin in conf.CORS_ALLOWED_ORIGINS:
             if origin in special_origin_values:
                 continue
-            parsed = urlparse(origin)
+            parsed = urlsplit(origin)
             if parsed.scheme == "" or parsed.netloc == "":
                 errors.append(
                     Error(
                         "Origin {} in {} is missing scheme or netloc".format(
                             repr(origin), allowed_origins_alias
                         ),
                         id="corsheaders.E013",
@@ -98,15 +108,15 @@
                             + "example.com)."
                         ),
                     )
                 )
             else:
                 # Only do this check in this case because if the scheme is not
                 # provided, netloc ends up in path
-                for part in ("path", "params", "query", "fragment"):
+                for part in ("path", "query", "fragment"):
                     if getattr(parsed, part) != "":
                         errors.append(
                             Error(
                                 "Origin {} in {} should not have {}".format(
                                     repr(origin), allowed_origins_alias, part
                                 ),
                                 id="corsheaders.E014",
@@ -133,32 +143,36 @@
         )
 
     if not isinstance(conf.CORS_URLS_REGEX, (str, re_type)):
         errors.append(
             Error("CORS_URLS_REGEX should be a string or regex.", id="corsheaders.E009")
         )
 
-    if not isinstance(conf.CORS_REPLACE_HTTPS_REFERER, bool):
-        errors.append(  # type: ignore [unreachable]
-            Error("CORS_REPLACE_HTTPS_REFERER should be a bool.", id="corsheaders.E011")
-        )
-
     if hasattr(settings, "CORS_MODEL"):
         errors.append(
             Error(
                 (
                     "The CORS_MODEL setting has been removed - see "
                     + "django-cors-headers' HISTORY."
                 ),
                 id="corsheaders.E012",
             )
         )
 
+    if hasattr(settings, "CORS_REPLACE_HTTPS_REFERER"):
+        errors.append(
+            Error(
+                (
+                    "The CORS_REPLACE_HTTPS_REFERER setting has been removed"
+                    + " - see django-cors-headers' CHANGELOG."
+                ),
+                id="corsheaders.E013",
+            )
+        )
+
     return errors
 
 
-def is_sequence(
-    thing: Any, type_or_types: Union[Type[Any], Tuple[Type[Any], ...]]
-) -> bool:
+def is_sequence(thing: Any, type_or_types: type[Any] | tuple[type[Any], ...]) -> bool:
     return isinstance(thing, Sequence) and all(
         isinstance(x, type_or_types) for x in thing
     )
```

### Comparing `django-cors-headers-3.9.0/src/corsheaders/conf.py` & `django_cors_headers-4.0.0/src/corsheaders/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-from typing import List, Pattern, Sequence, Tuple, Union
+from __future__ import annotations
+
+from typing import cast
+from typing import List
+from typing import Pattern
+from typing import Sequence
+from typing import Tuple
+from typing import Union
 
 from django.conf import settings
 
+from corsheaders.defaults import default_headers
+from corsheaders.defaults import default_methods
+
 # Kept here for backwards compatibility
-from corsheaders.defaults import default_headers, default_methods
 
 
 class Settings:
     """
     Shadow Django's settings with a little logic
     """
 
@@ -20,48 +29,49 @@
         return getattr(settings, "CORS_ALLOW_METHODS", default_methods)
 
     @property
     def CORS_ALLOW_CREDENTIALS(self) -> bool:
         return getattr(settings, "CORS_ALLOW_CREDENTIALS", False)
 
     @property
+    def CORS_ALLOW_PRIVATE_NETWORK(self) -> bool:
+        return getattr(settings, "CORS_ALLOW_PRIVATE_NETWORK", False)
+
+    @property
     def CORS_PREFLIGHT_MAX_AGE(self) -> int:
         return getattr(settings, "CORS_PREFLIGHT_MAX_AGE", 86400)
 
     @property
     def CORS_ALLOW_ALL_ORIGINS(self) -> bool:
         return getattr(
             settings,
             "CORS_ALLOW_ALL_ORIGINS",
             getattr(settings, "CORS_ORIGIN_ALLOW_ALL", False),
         )
 
     @property
-    def CORS_ALLOWED_ORIGINS(self) -> Union[List[str], Tuple[str]]:
-        return getattr(
+    def CORS_ALLOWED_ORIGINS(self) -> list[str] | tuple[str]:
+        value = getattr(
             settings,
             "CORS_ALLOWED_ORIGINS",
             getattr(settings, "CORS_ORIGIN_WHITELIST", ()),
         )
+        return cast(Union[List[str], Tuple[str]], value)
 
     @property
-    def CORS_ALLOWED_ORIGIN_REGEXES(self) -> Sequence[Union[str, Pattern[str]]]:
+    def CORS_ALLOWED_ORIGIN_REGEXES(self) -> Sequence[str | Pattern[str]]:
         return getattr(
             settings,
             "CORS_ALLOWED_ORIGIN_REGEXES",
             getattr(settings, "CORS_ORIGIN_REGEX_WHITELIST", ()),
         )
 
     @property
     def CORS_EXPOSE_HEADERS(self) -> Sequence[str]:
         return getattr(settings, "CORS_EXPOSE_HEADERS", ())
 
     @property
-    def CORS_URLS_REGEX(self) -> Union[str, Pattern[str]]:
+    def CORS_URLS_REGEX(self) -> str | Pattern[str]:
         return getattr(settings, "CORS_URLS_REGEX", r"^.*$")
 
-    @property
-    def CORS_REPLACE_HTTPS_REFERER(self) -> bool:
-        return getattr(settings, "CORS_REPLACE_HTTPS_REFERER", False)
-
 
 conf = Settings()
```

### Comparing `django-cors-headers-3.9.0/src/corsheaders/middleware.py` & `django_cors_headers-4.0.0/src/corsheaders/middleware.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,142 +1,113 @@
-import re
-from typing import Any, Optional
-from urllib.parse import ParseResult, urlparse
+from __future__ import annotations
 
-from django.http import HttpRequest, HttpResponse
+import asyncio
+import re
+from typing import Awaitable
+from typing import Callable
+from urllib.parse import SplitResult
+from urllib.parse import urlsplit
+
+from django.http import HttpRequest
+from django.http import HttpResponse
+from django.http.response import HttpResponseBase
 from django.utils.cache import patch_vary_headers
-from django.utils.deprecation import MiddlewareMixin
 
 from corsheaders.conf import conf
 from corsheaders.signals import check_request_enabled
 
-ACCESS_CONTROL_ALLOW_ORIGIN = "Access-Control-Allow-Origin"
-ACCESS_CONTROL_EXPOSE_HEADERS = "Access-Control-Expose-Headers"
-ACCESS_CONTROL_ALLOW_CREDENTIALS = "Access-Control-Allow-Credentials"
-ACCESS_CONTROL_ALLOW_HEADERS = "Access-Control-Allow-Headers"
-ACCESS_CONTROL_ALLOW_METHODS = "Access-Control-Allow-Methods"
-ACCESS_CONTROL_MAX_AGE = "Access-Control-Max-Age"
+ACCESS_CONTROL_ALLOW_ORIGIN = "access-control-allow-origin"
+ACCESS_CONTROL_EXPOSE_HEADERS = "access-control-expose-headers"
+ACCESS_CONTROL_ALLOW_CREDENTIALS = "access-control-allow-credentials"
+ACCESS_CONTROL_ALLOW_HEADERS = "access-control-allow-headers"
+ACCESS_CONTROL_ALLOW_METHODS = "access-control-allow-methods"
+ACCESS_CONTROL_MAX_AGE = "access-control-max-age"
+ACCESS_CONTROL_REQUEST_PRIVATE_NETWORK = "access-control-request-private-network"
+ACCESS_CONTROL_ALLOW_PRIVATE_NETWORK = "access-control-allow-private-network"
 
 
-class CorsPostCsrfMiddleware(MiddlewareMixin):
-    def _https_referer_replace_reverse(self, request: HttpRequest) -> None:
-        """
-        Put the HTTP_REFERER back to its original value and delete the
-        temporary storage
-        """
-        if conf.CORS_REPLACE_HTTPS_REFERER and "ORIGINAL_HTTP_REFERER" in request.META:
-            http_referer = request.META["ORIGINAL_HTTP_REFERER"]
-            request.META["HTTP_REFERER"] = http_referer
-            del request.META["ORIGINAL_HTTP_REFERER"]
+class CorsMiddleware:
+    sync_capable = True
+    async_capable = True
 
-    def process_request(self, request: HttpRequest) -> None:
-        self._https_referer_replace_reverse(request)
-        return None
-
-    def process_view(
+    def __init__(
         self,
-        request: HttpRequest,
-        callback: Any,
-        callback_args: Any,
-        callback_kwargs: Any,
+        get_response: (
+            Callable[[HttpRequest], HttpResponseBase]
+            | Callable[[HttpRequest], Awaitable[HttpResponseBase]]
+        ),
     ) -> None:
-        self._https_referer_replace_reverse(request)
-        return None
+        self.get_response = get_response
+        if asyncio.iscoroutinefunction(self.get_response):
+            # Mark the class as async-capable, but do the actual switch
+            # inside __call__ to avoid swapping out dunder methods
+            self._is_coroutine = (
+                asyncio.coroutines._is_coroutine  # type: ignore [attr-defined]
+            )
+        else:
+            self._is_coroutine = None
 
+    def __call__(
+        self, request: HttpRequest
+    ) -> HttpResponseBase | Awaitable[HttpResponseBase]:
+        if self._is_coroutine:
+            return self.__acall__(request)
+        response: HttpResponseBase | None = self.check_preflight(request)
+        if response is None:
+            result = self.get_response(request)
+            assert isinstance(result, HttpResponseBase)
+            response = result
+        self.add_response_headers(request, response)
+        return response
 
-class CorsMiddleware(MiddlewareMixin):
-    def _https_referer_replace(self, request: HttpRequest) -> None:
+    async def __acall__(self, request: HttpRequest) -> HttpResponseBase:
+        response = self.check_preflight(request)
+        if response is None:
+            result = self.get_response(request)
+            assert not isinstance(result, HttpResponseBase)
+            response = await result
+        self.add_response_headers(request, response)
+        return response
+
+    def check_preflight(self, request: HttpRequest) -> HttpResponseBase | None:
         """
-        When https is enabled, django CSRF checking includes referer checking
-        which breaks when using CORS. This function updates the HTTP_REFERER
-        header to make sure it matches HTTP_HOST, provided that our cors logic
-        succeeds
+        Generate a response for CORS preflight requests.
         """
-        origin = request.META.get("HTTP_ORIGIN")
-
+        request._cors_enabled = self.is_enabled(request)  # type: ignore [attr-defined]
         if (
-            request.is_secure()
-            and origin
-            and "ORIGINAL_HTTP_REFERER" not in request.META
+            request._cors_enabled  # type: ignore [attr-defined]
+            and request.method == "OPTIONS"
+            and "access-control-request-method" in request.headers
         ):
-
-            url = urlparse(origin)
-            if (
-                not conf.CORS_ALLOW_ALL_ORIGINS
-                and not self.origin_found_in_white_lists(origin, url)
-            ):
-                return
-
-            try:
-                http_referer = request.META["HTTP_REFERER"]
-                http_host = "https://%s/" % request.META["HTTP_HOST"]
-                request.META = request.META.copy()
-                request.META["ORIGINAL_HTTP_REFERER"] = http_referer
-                request.META["HTTP_REFERER"] = http_host
-            except KeyError:
-                pass
-
-    def process_request(self, request: HttpRequest) -> Optional[HttpResponse]:
-        """
-        If CORS preflight header, then create an
-        empty body response (200 OK) and return it
-
-        Django won't bother calling any other request
-        view/exception middleware along with the requested view;
-        it will call any response middlewares
-        """
-        request._cors_enabled = self.is_enabled(request)
-        if request._cors_enabled:
-            if conf.CORS_REPLACE_HTTPS_REFERER:
-                self._https_referer_replace(request)
-
-            if (
-                request.method == "OPTIONS"
-                and "HTTP_ACCESS_CONTROL_REQUEST_METHOD" in request.META
-            ):
-                response = HttpResponse()
-                response["Content-Length"] = "0"
-                return response
-        return None
-
-    def process_view(
-        self,
-        request: HttpRequest,
-        callback: Any,
-        callback_args: Any,
-        callback_kwargs: Any,
-    ) -> None:
-        """
-        Do the referer replacement here as well
-        """
-        if request._cors_enabled and conf.CORS_REPLACE_HTTPS_REFERER:
-            self._https_referer_replace(request)
+            return HttpResponse(headers={"content-length": "0"})
         return None
 
-    def process_response(
-        self, request: HttpRequest, response: HttpResponse
-    ) -> HttpResponse:
+    def add_response_headers(
+        self, request: HttpRequest, response: HttpResponseBase
+    ) -> HttpResponseBase:
         """
         Add the respective CORS headers
         """
         enabled = getattr(request, "_cors_enabled", None)
         if enabled is None:
             enabled = self.is_enabled(request)
 
         if not enabled:
             return response
 
-        patch_vary_headers(response, ["Origin"])
+        patch_vary_headers(response, ("origin",))
 
-        origin = request.META.get("HTTP_ORIGIN")
+        origin = request.headers.get("origin")
         if not origin:
             return response
 
-        # todo: check hostname from db instead
-        url = urlparse(origin)
+        try:
+            url = urlsplit(origin)
+        except ValueError:
+            return response
 
         if conf.CORS_ALLOW_CREDENTIALS:
             response[ACCESS_CONTROL_ALLOW_CREDENTIALS] = "true"
 
         if (
             not conf.CORS_ALLOW_ALL_ORIGINS
             and not self.origin_found_in_white_lists(origin, url)
@@ -156,17 +127,23 @@
 
         if request.method == "OPTIONS":
             response[ACCESS_CONTROL_ALLOW_HEADERS] = ", ".join(conf.CORS_ALLOW_HEADERS)
             response[ACCESS_CONTROL_ALLOW_METHODS] = ", ".join(conf.CORS_ALLOW_METHODS)
             if conf.CORS_PREFLIGHT_MAX_AGE:
                 response[ACCESS_CONTROL_MAX_AGE] = str(conf.CORS_PREFLIGHT_MAX_AGE)
 
+        if (
+            conf.CORS_ALLOW_PRIVATE_NETWORK
+            and request.headers.get(ACCESS_CONTROL_REQUEST_PRIVATE_NETWORK) == "true"
+        ):
+            response[ACCESS_CONTROL_ALLOW_PRIVATE_NETWORK] = "true"
+
         return response
 
-    def origin_found_in_white_lists(self, origin: str, url: ParseResult) -> bool:
+    def origin_found_in_white_lists(self, origin: str, url: SplitResult) -> bool:
         return (
             (origin == "null" and origin in conf.CORS_ALLOWED_ORIGINS)
             or self._url_in_whitelist(url)
             or self.regex_domain_match(origin)
         )
 
     def regex_domain_match(self, origin: str) -> bool:
@@ -180,13 +157,13 @@
             re.match(conf.CORS_URLS_REGEX, request.path_info)
         ) or self.check_signal(request)
 
     def check_signal(self, request: HttpRequest) -> bool:
         signal_responses = check_request_enabled.send(sender=None, request=request)
         return any(return_value for function, return_value in signal_responses)
 
-    def _url_in_whitelist(self, url: ParseResult) -> bool:
-        origins = [urlparse(o) for o in conf.CORS_ALLOWED_ORIGINS]
+    def _url_in_whitelist(self, url: SplitResult) -> bool:
+        origins = [urlsplit(o) for o in conf.CORS_ALLOWED_ORIGINS]
         return any(
             origin.scheme == url.scheme and origin.netloc == url.netloc
             for origin in origins
         )
```

### Comparing `django-cors-headers-3.9.0/src/django_cors_headers.egg-info/PKG-INFO` & `django_cors_headers-4.0.0/src/django_cors_headers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: django-cors-headers
-Version: 3.9.0
+Version: 4.0.0
 Summary: django-cors-headers is a Django application for handling the server headers required for Cross-Origin Resource Sharing (CORS).
 Home-page: https://github.com/adamchainz/django-cors-headers
 Author: Otto Yiu
 Author-email: otto@live.ca
 Maintainer: Adam Johnson
 Maintainer-email: me@adamj.eu
-License: MIT License
-Project-URL: Changelog, https://github.com/adamchainz/django-cors-headers/blob/main/HISTORY.rst
+License: MIT
+Project-URL: Changelog, https://github.com/adamchainz/django-cors-headers/blob/main/CHANGELOG.rst
+Project-URL: Mastodon, https://fosstodon.org/@adamchainz
 Project-URL: Twitter, https://twitter.com/adamchainz
 Keywords: django,cors,middleware,rest,api
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 django-cors-headers
 ===================
 
-.. image:: https://img.shields.io/github/workflow/status/adamchainz/django-cors-headers/CI/main?style=for-the-badge
+.. image:: https://img.shields.io/github/actions/workflow/status/adamchainz/django-cors-headers/main.yml?branch=main&style=for-the-badge
    :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
-.. image:: https://img.shields.io/codecov/c/github/adamchainz/django-cors-headers/main?style=for-the-badge
-  :target: https://app.codecov.io/gh/adamchainz/django-cors-headers
+.. image:: https://img.shields.io/badge/Coverage-100%25-success?style=for-the-badge
+  :target: https://github.com/adamchainz/django-cors-headers/actions?workflow=CI
 
 .. image:: https://img.shields.io/pypi/v/django-cors-headers.svg?style=for-the-badge
     :target: https://pypi.org/project/django-cors-headers/
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
     :target: https://github.com/psf/black
 
@@ -66,29 +67,30 @@
 important you understand the implications before adding the headers, since you
 could be unintentionally opening up your site's private data to others.
 
 Some good resources to read on the subject are:
 
 * Julia Evans' `introductory comic <https://drawings.jvns.ca/cors/>`__ and
   `educational quiz <https://questions.wizardzines.com/cors.html>`__.
-* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
+* Jake Archibald’s `How to win at CORS <https://jakearchibald.com/2021/cors/>`__
 * The `MDN Article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS>`_
 * The `HTML5 Rocks Tutorial <https://www.html5rocks.com/en/tutorials/cors/>`_
+* The `Wikipedia Page <https://en.wikipedia.org/wiki/Cross-origin_resource_sharing>`_
 
 Requirements
 ------------
 
-Python 3.6 to 3.9 supported.
+Python 3.7 to 3.11 supported.
 
-Django 2.2 to 4.0 supported.
+Django 3.2 to 4.2 supported.
 
 ----
 
-**Are your tests slow?**
-Check out my book `Speed Up Your Django Tests <https://gumroad.com/l/suydt>`__ which covers loads of best practices so you can write faster, more accurate tests.
+**Want to work smarter and faster?**
+Check out my book `Boost Your Django DX <https://adamchainz.gumroad.com/l/byddx>`__ which covers many ways to improve your development experience.
 
 ----
 
 Setup
 -----
 
 Install from **pip**:
@@ -123,17 +125,14 @@
     ]
 
 ``CorsMiddleware`` should be placed as high as possible, especially before any
 middleware that can generate responses such as Django's ``CommonMiddleware`` or
 Whitenoise's ``WhiteNoiseMiddleware``. If it is not before, it will not be able
 to add the CORS headers to these responses.
 
-Also if you are using ``CORS_REPLACE_HTTPS_REFERER`` it should be placed before
-Django's ``CsrfViewMiddleware`` (see more below).
-
 About
 -----
 
 **django-cors-headers** was created in January 2013 by Otto Yiu. It went
 unmaintained from August 2015 and was forked in January 2016 to the package
 `django-cors-middleware <https://github.com/zestedesavoir/django-cors-middleware>`_
 by Laville Augustin at Zeste de Savoir.
@@ -160,244 +159,230 @@
 * ``CORS_ALLOWED_ORIGIN_REGEXES``
 * ``CORS_ALLOW_ALL_ORIGINS``
 
 ``CORS_ALLOWED_ORIGINS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A list of origins that are authorized to make cross-site HTTP requests.
+The origins in this setting will be allowed, and the requesting origin will be echoed back to the client in the |access-control-allow-origin header|__.
 Defaults to ``[]``.
 
-An Origin is defined by
-`the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_
-as a URI scheme + hostname + port, or one of the special values `'null'` or
-`'file://'`.
-Default ports (HTTPS = 443, HTTP = 80) are optional here.
-
-The special value `null` is sent by the browser in
-`"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__,
-such as when the client is running from a ``file://`` domain.
-The special value `file://` is sent accidentally by some versions of Chrome on
-Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
+.. |access-control-allow-origin header| replace:: ``access-control-allow-origin`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Origin
+
+An Origin is defined by `the CORS RFC Section 3.2 <https://tools.ietf.org/html/rfc6454#section-3.2>`_ as a URI scheme + hostname + port, or one of the special values ``'null'`` or ``'file://'``.
+Default ports (HTTPS = 443, HTTP = 80) are optional.
+
+The special value ``null`` is sent by the browser in `"privacy-sensitive contexts" <https://tools.ietf.org/html/rfc6454#section-6>`__, such as when the client is running from a ``file://`` domain.
+The special value `file://` is sent accidentally by some versions of Chrome on Android as per `this bug <https://bugs.chromium.org/p/chromium/issues/detail?id=991107>`__.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
         "https://example.com",
         "https://sub.example.com",
         "http://localhost:8080",
         "http://127.0.0.1:9000",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works
-as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOWED_ORIGIN_REGEXES: Sequence[str | Pattern[str]]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of strings representing regexes that match Origins that are authorized
-to make cross-site HTTP requests. Defaults to ``[]``. Useful when
-``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number
-of subdomains.
+A list of strings representing regexes that match Origins that are authorized to make cross-site HTTP requests.
+Defaults to ``[]``.
+Useful when ``CORS_ALLOWED_ORIGINS`` is impractical, such as when you have a large number of subdomains.
 
 Example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGIN_REGEXES = [
         r"^https://\w+\.example\.com$",
     ]
 
-Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_REGEX_WHITELIST``, which still works as an alias, with the new name taking precedence.
 
 ``CORS_ALLOW_ALL_ORIGINS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, all origins will be allowed. Other settings restricting allowed
-origins will be ignored. Defaults to ``False``.
+If ``True``, all origins will be allowed.
+Other settings restricting allowed origins will be ignored.
+Defaults to ``False``.
 
-Setting this to ``True`` can be *dangerous*, as it allows any website to make
-cross-origin requests to yours. Generally you'll want to restrict the list of
-allowed origins with ``CORS_ALLOWED_ORIGINS`` or
-``CORS_ALLOWED_ORIGIN_REGEXES``.
+Setting this to ``True`` can be *dangerous*, as it allows any website to make cross-origin requests to yours.
+Generally you'll want to restrict the list of allowed origins with ``CORS_ALLOWED_ORIGINS`` or ``CORS_ALLOWED_ORIGIN_REGEXES``.
 
-Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still
-works as an alias, with the new name taking precedence.
+Previously this setting was called ``CORS_ORIGIN_ALLOW_ALL``, which still works as an alias, with the new name taking precedence.
 
 --------------
 
 The following are optional settings, for which the defaults probably suffice.
 
 ``CORS_URLS_REGEX: str | Pattern[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A regex which restricts the URL's for which the CORS headers will be sent.
-Defaults to ``r'^.*$'``, i.e. match all URL's. Useful when you only need CORS
-on a part of your site, e.g. an API at ``/api/``.
+Defaults to ``r'^.*$'``, i.e. match all URL's.
+Useful when you only need CORS on a part of your site, e.g. an API at ``/api/``.
 
 Example:
 
 .. code-block:: python
 
     CORS_URLS_REGEX = r"^/api/.*$"
 
 ``CORS_ALLOW_METHODS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-A list of HTTP verbs that are allowed for the actual request. Defaults to:
+A list of HTTP verbs that are allowed for the actual request.
+Defaults to:
 
 .. code-block:: python
 
-    CORS_ALLOW_METHODS = [
+    CORS_ALLOW_METHODS = (
         "DELETE",
         "GET",
         "OPTIONS",
         "PATCH",
         "POST",
         "PUT",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_methods`` so you
-can just extend it with your custom methods. This allows you to keep up to date
-with any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_methods`` so you can just extend it with your custom methods.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_methods
 
-    CORS_ALLOW_METHODS = list(default_methods) + [
+    CORS_ALLOW_METHODS = (
+        *default_methods,
         "POKE",
-    ]
+    )
 
 ``CORS_ALLOW_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of non-standard HTTP headers that can be used when making the actual
-request. Defaults to:
+The list of non-standard HTTP headers that you permit in requests from the browser.
+Sets the |Access-Control-Allow-Headers header|__ in responses to `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__.
+Defaults to:
+
+.. |Access-Control-Allow-Headers header| replace:: ``Access-Control-Allow-Headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Allow-Headers
 
 .. code-block:: python
 
-    CORS_ALLOW_HEADERS = [
+    CORS_ALLOW_HEADERS = (
         "accept",
-        "accept-encoding",
         "authorization",
         "content-type",
-        "dnt",
-        "origin",
         "user-agent",
         "x-csrftoken",
         "x-requested-with",
-    ]
+    )
 
-The default can be imported as ``corsheaders.defaults.default_headers`` so you
-can extend it with your custom headers. This allows you to keep up to date with
-any future changes. For example:
+The default can be imported as ``corsheaders.defaults.default_headers`` so you can extend it with your custom headers.
+This allows you to keep up to date with any future changes.
+For example:
 
 .. code-block:: python
 
     from corsheaders.defaults import default_headers
 
-    CORS_ALLOW_HEADERS = list(default_headers) + [
+    CORS_ALLOW_HEADERS = (
+        *default_headers,
         "my-custom-header",
-    ]
+    )
 
 ``CORS_EXPOSE_HEADERS: Sequence[str]``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The list of HTTP headers that are to be exposed to the browser. Defaults to
-``[]``.
+The list of extra HTTP headers to expose to the browser, in addition to the default `safelisted headers <https://developer.mozilla.org/en-US/docs/Glossary/CORS-safelisted_response_header>`__.
+If non-empty, these are declared in the |access-control-expose-headers header|__.
+Defaults to ``[]``.
 
+.. |access-control-expose-headers header| replace:: ``access-control-expose-headers`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Expose-Headers
 
 ``CORS_PREFLIGHT_MAX_AGE: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The number of seconds a client/browser can cache the preflight response. If
-this is 0 (or any falsey value), no max age header will be sent. Defaults to
-``86400`` (one day).
-
-
-**Note:** A preflight request is an extra request that is made when making a
-"not-so-simple" request (e.g. ``Content-Type`` is not
-``application/x-www-form-urlencoded``) to determine what requests the server
-actually accepts. Read more about it in the
-`CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#Preflighted_requests>`_.
+The number of seconds the browser can cache the preflight response.
+This sets the |access-control-max-age header|__ in preflight responses.
+If this is 0 (or any falsey value), no max age header will be sent.
+Defaults to ``86400`` (one day).
+
+.. |access-control-max-age header| replace:: ``access-control-max-age`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Max-Age
+
+**Note:**
+Browsers send `preflight requests <https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request>`__ before certain “non-simple” requests, to check they will be allowed.
+Read more about it in the `CORS MDN article <https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#preflighted_requests>`_.
 
 ``CORS_ALLOW_CREDENTIALS: bool``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-If ``True``, cookies will be allowed to be included in cross-site HTTP
-requests. Defaults to ``False``.
+If ``True``, cookies will be allowed to be included in cross-site HTTP requests.
+This sets the |access-control-allow-credentials header|__ in preflight and normal responses.
+Defaults to ``False``.
+
+.. |access-control-allow-credentials header| replace:: ``Access-Control-Allow-Credentials`` header
+__ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/access-control-allow-credentials
 
-Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to
-``'Lax'`` by default, which will prevent Django's session cookie being sent
-cross-domain. Change it to ``None`` to bypass this security restriction.
+Note: in Django 2.1 the `SESSION_COOKIE_SAMESITE`_ setting was added, set to ``'Lax'`` by default, which will prevent Django's session cookie being sent cross-domain.
+Change the setting to ``'None'`` if you need to bypass this security restriction.
 
-.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+.. _SESSION_COOKIE_SAMESITE: https://docs.djangoproject.com/en/stable/ref/settings/#std:setting-SESSION_COOKIE_SAMESITE
+
+``CORS_ALLOW_PRIVATE_NETWORK: bool``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+If ``True``, allow requests from sites on “public” IP to this server on a “private” IP.
+In such cases, browsers send an extra CORS header ``access-control-request-private-network``, for which ``OPTIONS`` responses must contain ``access-control-allow-private-network: true``.
+
+Refer to:
+
+* `Local Network Access <https://wicg.github.io/local-network-access/>`__, the W3C Community Draft specification.
+* `Private Network Access: introducing preflights <https://developer.chrome.com/blog/private-network-access-preflight/>`__, a blog post from the Google Chrome team.
 
 CSRF Integration
 ----------------
 
 Most sites will need to take advantage of the `Cross-Site Request Forgery
-protection <https://docs.djangoproject.com/en/3.0/ref/csrf/>`_ that Django
+protection <https://docs.djangoproject.com/en/stable/ref/csrf/>`_ that Django
 offers. CORS and CSRF are separate, and Django has no way of using your CORS
 configuration to exempt sites from the ``Referer`` checking that it does on
 secure requests. The way to do that is with its `CSRF_TRUSTED_ORIGINS setting
-<https://docs.djangoproject.com/en/3.0/ref/settings/#csrf-trusted-origins>`_.
+<https://docs.djangoproject.com/en/stable/ref/settings/#csrf-trusted-origins>`_.
 For example:
 
 .. code-block:: python
 
     CORS_ALLOWED_ORIGINS = [
-        "http://read.only.com",
-        "http://change.allowed.com",
+        "https://read-only.example.com",
+        "https://read-and-write.example.com",
     ]
 
     CSRF_TRUSTED_ORIGINS = [
-        "change.allowed.com",
-    ]
-
-``CORS_REPLACE_HTTPS_REFERER: bool``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-``CSRF_TRUSTED_ORIGINS`` was introduced in Django 1.9, so users of earlier
-versions will need an alternate solution. If ``CORS_REPLACE_HTTPS_REFERER`` is
-``True``, ``CorsMiddleware`` will change the ``Referer`` header to something
-that will pass Django's CSRF checks whenever the CORS checks pass. Defaults to
-``False``.
-
-Note that unlike ``CSRF_TRUSTED_ORIGINS``, this setting does not allow you to
-distinguish between domains that are trusted to *read* resources by CORS and
-domains that are trusted to *change* resources by avoiding CSRF protection.
-
-With this feature enabled you should also add
-``corsheaders.middleware.CorsPostCsrfMiddleware`` after
-``django.middleware.csrf.CsrfViewMiddleware`` in your ``MIDDLEWARE_CLASSES`` to
-undo the ``Referer`` replacement:
-
-.. code-block:: python
-
-    MIDDLEWARE_CLASSES = [
-        ...,
-        "corsheaders.middleware.CorsMiddleware",
-        ...,
-        "django.middleware.csrf.CsrfViewMiddleware",
-        "corsheaders.middleware.CorsPostCsrfMiddleware",
-        ...,
+        "https://read-and-write.example.com",
     ]
 
 Signals
 -------
 
 If you have a use case that requires more than just the above configuration,
 you can attach code to check if a given request should be allowed. For example,
 this can be used to read the list of origins you allow from a model. Attach any
 number of handlers to the ``check_request_enabled``
-`Django signal <https://docs.djangoproject.com/en/3.0/ref/signals/>`_, which
+`Django signal <https://docs.djangoproject.com/en/stable/ref/signals/>`_, which
 provides the ``request`` argument (use ``**kwargs`` in your handler to protect
 against any future arguments being added). If any handler attached to the
 signal returns a truthy value, the request will be allowed.
 
 For example you might define a handler like this:
 
 .. code-block:: python
@@ -405,21 +390,21 @@
     # myapp/handlers.py
     from corsheaders.signals import check_request_enabled
 
     from myapp.models import MySite
 
 
     def cors_allow_mysites(sender, request, **kwargs):
-        return MySite.objects.filter(host=request.host).exists()
+        return MySite.objects.filter(host=request.headers["origin"]).exists()
 
 
     check_request_enabled.connect(cors_allow_mysites)
 
 Then connect it at app ready time using a `Django AppConfig
-<https://docs.djangoproject.com/en/3.0/ref/applications/>`_:
+<https://docs.djangoproject.com/en/stable/ref/applications/>`_:
 
 .. code-block:: python
 
     # myapp/__init__.py
 
     default_app_config = "myapp.apps.MyAppConfig"
 
@@ -454,9 +439,7 @@
 
 
     def cors_allow_api_to_everyone(sender, request, **kwargs):
         return request.path.startswith("/api/")
 
 
     check_request_enabled.connect(cors_allow_api_to_everyone)
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-cors-headers-3.9.0/src/django_cors_headers.egg-info/SOURCES.txt` & `django_cors_headers-4.0.0/src/django_cors_headers.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-HISTORY.rst
+CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
-setup.py
 src/corsheaders/__init__.py
 src/corsheaders/apps.py
 src/corsheaders/checks.py
 src/corsheaders/conf.py
 src/corsheaders/defaults.py
 src/corsheaders/middleware.py
 src/corsheaders/py.typed
 src/corsheaders/signals.py
 src/django_cors_headers.egg-info/PKG-INFO
 src/django_cors_headers.egg-info/SOURCES.txt
 src/django_cors_headers.egg-info/dependency_links.txt
 src/django_cors_headers.egg-info/not-zip-safe
 src/django_cors_headers.egg-info/requires.txt
-src/django_cors_headers.egg-info/top_level.txt
+src/django_cors_headers.egg-info/top_level.txt
+tests/test_checks.py
+tests/test_conf.py
+tests/test_middleware.py
```

