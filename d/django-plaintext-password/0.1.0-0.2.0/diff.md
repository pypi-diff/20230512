# Comparing `tmp/django-plaintext-password-0.1.0.tar.gz` & `tmp/django-plaintext-password-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-plaintext-password-0.1.0.tar", last modified: Fri Dec 11 21:24:19 2020, max compression
+gzip compressed data, was "django-plaintext-password-0.2.0.tar", last modified: Fri May 12 15:31:48 2023, max compression
```

## Comparing `django-plaintext-password-0.1.0.tar` & `django-plaintext-password-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 21:24:19.199153 django-plaintext-password-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (116)     3564 2020-12-11 21:24:19.199153 django-plaintext-password-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-11 21:24:08.000000 django-plaintext-password-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 21:24:19.199153 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3564 2020-12-11 21:24:18.000000 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      360 2020-12-11 21:24:19.000000 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-11 21:24:18.000000 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-12-11 21:24:18.000000 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2020-12-11 21:24:18.000000 django-plaintext-password-0.1.0/django_plaintext_password.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-11 21:24:19.199153 django-plaintext-password-0.1.0/plaintext_password/
--rw-r--r--   0 runner    (1001) docker     (116)     1153 2020-12-11 21:24:08.000000 django-plaintext-password-0.1.0/plaintext_password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      383 2020-12-11 21:24:08.000000 django-plaintext-password-0.1.0/plaintext_password/checks.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-11 21:24:08.000000 django-plaintext-password-0.1.0/plaintext_password/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)      434 2020-12-11 21:24:19.199153 django-plaintext-password-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1294 2020-12-11 21:24:08.000000 django-plaintext-password-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:48.016740 django-plaintext-password-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-12 15:31:48.016740 django-plaintext-password-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:48.016740 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-05-12 15:31:47.000000 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 15:31:47.000000 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:31:47.000000 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 15:31:47.000000 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-12 15:31:47.000000 django-plaintext-password-0.2.0/django_plaintext_password.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:48.016740 django-plaintext-password-0.2.0/plaintext_password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/plaintext_password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/plaintext_password/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/plaintext_password/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-12 15:31:48.016740 django-plaintext-password-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-12 15:31:32.000000 django-plaintext-password-0.2.0/setup.py
```

### Comparing `django-plaintext-password-0.1.0/PKG-INFO` & `django-plaintext-password-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 Metadata-Version: 2.1
 Name: django-plaintext-password
-Version: 0.1.0
+Version: 0.2.0
 Summary: https://github.com/RealOrangeOne/django-plaintext-password
 Home-page: https://github.com/RealOrangeOne/django-plaintext-password
 Author: Jake Howard
 License: BSD
-Description: # django-plaintext-password
-        
-        ![CI](https://github.com/RealOrangeOne/django-plaintext-password/workflows/CI/badge.svg)
-        
-        A Django password hasher to store passwords in plaintext.
-        
-        ## _"Should I use this in production?"_
-        
-        Oh definitely not. Storing passwords in plaintext is a very *very* bad thing. Django's defaults are incredibly secure and should be used unless you have a good reason not to.
-        
-        For more on why using this in production is a terrible idea, check out [How to store passwords](https://theorangeone.net/posts/how-to-store-passwords/).
-        
-        When running deployment checks, this will throw a "CRITICAL" error if in use.
-        
-        ## Installation and usage
-        
-        ```
-        pip install django-plaintext-password
-        ```
-        
-        Then add `plaintext_password.PlaintextPasswordHasher` to [`PASSWORD_HASHERS`](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-PASSWORD_HASHERS) in `settings.py`. To ensure it's used by default, make it the first or only item.
-        
-        ## How does it work?
-        
-        By default, Django will store the password `password123` in a format similar to:
-        
-        ```
-        pbkdf2_sha256$216000$gd57n4OWJrXh$Xs/TqhwJICOxsLONGlKXorjuWccooiuJmJOUaxbwcOQ=
-        ```
-        
-        This is good for security as the password has been both salted and hashed before being saved into the database, making it almost impossible to retrieve the original password. This library however, stores the password as-is:
-        
-        ```
-        plaintext$$password123
-        ```
-        
-        This makes searching by password possible, as well as comparing users passwords and allowing you to email users their passwords if they forget them - neat!
-        
-        In addition to storing the values directly in the database for easy retrieval, the comparison is done simply with `==`, rather than using [`secrets.compare_digest`](https://docs.python.org/3/library/secrets.html#secrets.compare_digest).
-        
-        ## Why?
-        
-        Well, why not?
-        
-        Although in all seriousness, If as part of your tests you're creating a large number of users, or just a couple users but you've got a lot of tests, you can get quite a performance improvement by simplifying the password hasher.
-        
-        Unfortunately due to a limitation (and feature) with Django, it's not possible to store just the value directly, it must be prefixed with the algorithm.
-        
 Keywords: django password plaintext
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-plaintext-password
+
+![CI](https://github.com/RealOrangeOne/django-plaintext-password/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plaintext-password.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plaintext-password.svg)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-plaintext-password.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plaintext-password.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plaintext-password.svg)
+
+
+A Django password hasher to store passwords in plaintext.
+
+## _"Should I use this in production?"_
+
+Oh definitely not. Storing passwords in plaintext is a very *very* bad thing. Django's defaults are incredibly secure and should be used unless you have a good reason not to.
+
+For more on why using this in production is a terrible idea, check out [How to store passwords](https://theorangeone.net/posts/how-to-store-passwords/).
+
+When running deployment checks, this will throw a "CRITICAL" error if in use.
+
+## Installation and usage
+
+```
+pip install django-plaintext-password
+```
+
+Then add `plaintext_password.PlaintextPasswordHasher` to [`PASSWORD_HASHERS`](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-PASSWORD_HASHERS) in `settings.py`. To ensure it's used by default, make it the first or only item.
+
+## How does it work?
+
+By default, Django will store the password `password123` in a format similar to:
+
+```
+pbkdf2_sha256$216000$gd57n4OWJrXh$Xs/TqhwJICOxsLONGlKXorjuWccooiuJmJOUaxbwcOQ=
+```
+
+This is good for security as the password has been both salted and hashed before being saved into the database, making it almost impossible to retrieve the original password. This library however, stores the password as-is:
+
+```
+plaintext$$password123
+```
+
+This makes searching by password possible, as well as comparing users passwords and allowing you to email users their passwords if they forget them - neat!
+
+In addition to storing the values directly in the database for easy retrieval, the comparison is done simply with `==`, rather than using [`secrets.compare_digest`](https://docs.python.org/3/library/secrets.html#secrets.compare_digest).
+
+## Why?
+
+Well, why not?
+
+Although in all seriousness, If as part of your tests you're creating a large number of users, or just a couple users but you've got a lot of tests, you can get quite a performance improvement by simplifying the password hasher.
+
+Unfortunately due to a limitation (and feature) with Django, it's not possible to store just the value directly, it must be prefixed with the algorithm.
```

### Comparing `django-plaintext-password-0.1.0/README.md` & `django-plaintext-password-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 # django-plaintext-password
 
 ![CI](https://github.com/RealOrangeOne/django-plaintext-password/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plaintext-password.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plaintext-password.svg)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-plaintext-password.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plaintext-password.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plaintext-password.svg)
+
 
 A Django password hasher to store passwords in plaintext.
 
 ## _"Should I use this in production?"_
 
 Oh definitely not. Storing passwords in plaintext is a very *very* bad thing. Django's defaults are incredibly secure and should be used unless you have a good reason not to.
```

### Comparing `django-plaintext-password-0.1.0/django_plaintext_password.egg-info/PKG-INFO` & `django-plaintext-password-0.2.0/django_plaintext_password.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 Metadata-Version: 2.1
 Name: django-plaintext-password
-Version: 0.1.0
+Version: 0.2.0
 Summary: https://github.com/RealOrangeOne/django-plaintext-password
 Home-page: https://github.com/RealOrangeOne/django-plaintext-password
 Author: Jake Howard
 License: BSD
-Description: # django-plaintext-password
-        
-        ![CI](https://github.com/RealOrangeOne/django-plaintext-password/workflows/CI/badge.svg)
-        
-        A Django password hasher to store passwords in plaintext.
-        
-        ## _"Should I use this in production?"_
-        
-        Oh definitely not. Storing passwords in plaintext is a very *very* bad thing. Django's defaults are incredibly secure and should be used unless you have a good reason not to.
-        
-        For more on why using this in production is a terrible idea, check out [How to store passwords](https://theorangeone.net/posts/how-to-store-passwords/).
-        
-        When running deployment checks, this will throw a "CRITICAL" error if in use.
-        
-        ## Installation and usage
-        
-        ```
-        pip install django-plaintext-password
-        ```
-        
-        Then add `plaintext_password.PlaintextPasswordHasher` to [`PASSWORD_HASHERS`](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-PASSWORD_HASHERS) in `settings.py`. To ensure it's used by default, make it the first or only item.
-        
-        ## How does it work?
-        
-        By default, Django will store the password `password123` in a format similar to:
-        
-        ```
-        pbkdf2_sha256$216000$gd57n4OWJrXh$Xs/TqhwJICOxsLONGlKXorjuWccooiuJmJOUaxbwcOQ=
-        ```
-        
-        This is good for security as the password has been both salted and hashed before being saved into the database, making it almost impossible to retrieve the original password. This library however, stores the password as-is:
-        
-        ```
-        plaintext$$password123
-        ```
-        
-        This makes searching by password possible, as well as comparing users passwords and allowing you to email users their passwords if they forget them - neat!
-        
-        In addition to storing the values directly in the database for easy retrieval, the comparison is done simply with `==`, rather than using [`secrets.compare_digest`](https://docs.python.org/3/library/secrets.html#secrets.compare_digest).
-        
-        ## Why?
-        
-        Well, why not?
-        
-        Although in all seriousness, If as part of your tests you're creating a large number of users, or just a couple users but you've got a lot of tests, you can get quite a performance improvement by simplifying the password hasher.
-        
-        Unfortunately due to a limitation (and feature) with Django, it's not possible to store just the value directly, it must be prefixed with the algorithm.
-        
 Keywords: django password plaintext
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# django-plaintext-password
+
+![CI](https://github.com/RealOrangeOne/django-plaintext-password/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plaintext-password.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plaintext-password.svg)
+![PyPI - Wheel](https://img.shields.io/pypi/wheel/django-plaintext-password.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plaintext-password.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plaintext-password.svg)
+
+
+A Django password hasher to store passwords in plaintext.
+
+## _"Should I use this in production?"_
+
+Oh definitely not. Storing passwords in plaintext is a very *very* bad thing. Django's defaults are incredibly secure and should be used unless you have a good reason not to.
+
+For more on why using this in production is a terrible idea, check out [How to store passwords](https://theorangeone.net/posts/how-to-store-passwords/).
+
+When running deployment checks, this will throw a "CRITICAL" error if in use.
+
+## Installation and usage
+
+```
+pip install django-plaintext-password
+```
+
+Then add `plaintext_password.PlaintextPasswordHasher` to [`PASSWORD_HASHERS`](https://docs.djangoproject.com/en/dev/ref/settings/#std:setting-PASSWORD_HASHERS) in `settings.py`. To ensure it's used by default, make it the first or only item.
+
+## How does it work?
+
+By default, Django will store the password `password123` in a format similar to:
+
+```
+pbkdf2_sha256$216000$gd57n4OWJrXh$Xs/TqhwJICOxsLONGlKXorjuWccooiuJmJOUaxbwcOQ=
+```
+
+This is good for security as the password has been both salted and hashed before being saved into the database, making it almost impossible to retrieve the original password. This library however, stores the password as-is:
+
+```
+plaintext$$password123
+```
+
+This makes searching by password possible, as well as comparing users passwords and allowing you to email users their passwords if they forget them - neat!
+
+In addition to storing the values directly in the database for easy retrieval, the comparison is done simply with `==`, rather than using [`secrets.compare_digest`](https://docs.python.org/3/library/secrets.html#secrets.compare_digest).
+
+## Why?
+
+Well, why not?
+
+Although in all seriousness, If as part of your tests you're creating a large number of users, or just a couple users but you've got a lot of tests, you can get quite a performance improvement by simplifying the password hasher.
+
+Unfortunately due to a limitation (and feature) with Django, it's not possible to store just the value directly, it must be prefixed with the algorithm.
```

### Comparing `django-plaintext-password-0.1.0/plaintext_password/__init__.py` & `django-plaintext-password-0.2.0/plaintext_password/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         decoded = self.decode(encoded)
         return {
             _("algorithm"): decoded["algorithm"],
             _("hash"): mask_hash(decoded["hash"], show=3),
         }
 
     def encode(self, password: str, salt: str):
-        assert salt == ""
         return f"{self.algorithm}$${password}"
 
     def verify(self, password: str, encoded: str) -> bool:
         """
         Constant-time comparison? What's that?
         """
         return encoded == self.encode(password, "")
```

### Comparing `django-plaintext-password-0.1.0/setup.py` & `django-plaintext-password-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="django-plaintext-password",
-    version="0.1.0",
+    version="0.2.0",
     url="https://github.com/RealOrangeOne/django-plaintext-password",
     author="Jake Howard",
     description="https://github.com/RealOrangeOne/django-plaintext-password",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="BSD",
     packages=find_packages(include=["plaintext_password*"]),
     package_data={"plaintext_password": ["py.typed"]},
-    install_requires=["Django>=2.2"],
-    python_requires=">=3.6",
+    install_requires=["Django>=3.2"],
+    python_requires=">=3.8",
     keywords="django password plaintext",
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
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
 )
```

