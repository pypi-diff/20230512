# Comparing `tmp/django-healthpoint-0.4.1.tar.gz` & `tmp/django-healthpoint-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-healthpoint-0.4.1.tar", last modified: Wed Sep  9 11:30:31 2020, max compression
+gzip compressed data, was "django-healthpoint-0.5.0.tar", last modified: Fri May 12 18:14:21 2023, max compression
```

## Comparing `django-healthpoint-0.4.1.tar` & `django-healthpoint-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 pennersr  (1001) pennersr  (1001)        0 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      111 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/AUTHORS
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     1072 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/LICENSE
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)       99 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/MANIFEST.in
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     4217 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/PKG-INFO
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     2640 2020-01-04 10:59:07.000000 django-healthpoint-0.4.1/README.rst
-drwxrwxr-x   0 pennersr  (1001) pennersr  (1001)        0 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     4217 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/PKG-INFO
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      558 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/SOURCES.txt
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)        1 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/dependency_links.txt
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)        1 2019-11-14 13:33:39.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/not-zip-safe
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)       13 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/requires.txt
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)       12 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/django_healthpoint.egg-info/top_level.txt
-drwxrwxr-x   0 pennersr  (1001) pennersr  (1001)        0 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/healthpoint/
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      505 2020-09-09 11:28:11.000000 django-healthpoint-0.4.1/healthpoint/__init__.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      759 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/decorators.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      443 2020-09-09 11:16:52.000000 django-healthpoint-0.4.1/healthpoint/registry.py
-drwxrwxr-x   0 pennersr  (1001) pennersr  (1001)        0 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/healthpoint/tests/
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)        0 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/tests/__init__.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      200 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/tests/health.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      405 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/tests/settings.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     1253 2019-11-14 14:51:50.000000 django-healthpoint-0.4.1/healthpoint/tests/test_views.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      106 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/tests/urls.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)      147 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/healthpoint/urls.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     1792 2020-09-09 11:20:25.000000 django-healthpoint-0.4.1/healthpoint/views.py
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)       38 2020-09-09 11:30:31.000000 django-healthpoint-0.4.1/setup.cfg
--rw-rw-r--   0 pennersr  (1001) pennersr  (1001)     2186 2019-11-14 13:31:59.000000 django-healthpoint-0.4.1/setup.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/
+-rw-rw-r--   0 pennersr  (1000) users      (100)      158 2020-10-13 18:13:04.000000 django-healthpoint-0.5.0/AUTHORS
+-rw-rw-r--   0 pennersr  (1000) users      (100)     1072 2019-11-14 13:31:59.000000 django-healthpoint-0.5.0/LICENSE
+-rw-rw-r--   0 pennersr  (1000) users      (100)       99 2019-11-14 13:31:59.000000 django-healthpoint-0.5.0/MANIFEST.in
+-rw-r--r--   0 pennersr  (1000) users      (100)     3767 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/PKG-INFO
+-rw-rw-r--   0 pennersr  (1000) users      (100)     2799 2023-05-12 18:00:00.000000 django-healthpoint-0.5.0/README.rst
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/django_healthpoint.egg-info/
+-rw-rw-r--   0 pennersr  (1000) users      (100)     3767 2023-05-12 18:14:21.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/PKG-INFO
+-rw-rw-r--   0 pennersr  (1000) users      (100)      568 2023-05-12 18:14:21.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/SOURCES.txt
+-rw-rw-r--   0 pennersr  (1000) users      (100)        1 2023-05-12 18:14:21.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/dependency_links.txt
+-rw-rw-r--   0 pennersr  (1000) users      (100)        1 2019-11-14 13:33:39.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/not-zip-safe
+-rw-rw-r--   0 pennersr  (1000) users      (100)       12 2023-05-12 18:14:21.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/requires.txt
+-rw-rw-r--   0 pennersr  (1000) users      (100)       12 2023-05-12 18:14:21.000000 django-healthpoint-0.5.0/django_healthpoint.egg-info/top_level.txt
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/healthpoint/
+-rw-rw-r--   0 pennersr  (1000) users      (100)      514 2023-05-12 18:13:37.000000 django-healthpoint-0.5.0/healthpoint/__init__.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)      775 2020-10-13 18:11:49.000000 django-healthpoint-0.5.0/healthpoint/decorators.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)      442 2023-05-12 18:07:33.000000 django-healthpoint-0.5.0/healthpoint/registry.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/healthpoint/tests/
+-rw-rw-r--   0 pennersr  (1000) users      (100)        0 2019-11-14 13:31:59.000000 django-healthpoint-0.5.0/healthpoint/tests/__init__.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)      200 2020-10-13 18:11:49.000000 django-healthpoint-0.5.0/healthpoint/tests/health.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)      377 2021-09-09 16:46:51.000000 django-healthpoint-0.5.0/healthpoint/tests/settings.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)     2500 2023-05-12 18:07:33.000000 django-healthpoint-0.5.0/healthpoint/tests/test_views.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      108 2023-05-12 18:07:33.000000 django-healthpoint-0.5.0/healthpoint/tests/urls.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      143 2023-05-12 18:07:33.000000 django-healthpoint-0.5.0/healthpoint/urls.py
+-rw-rw-r--   0 pennersr  (1000) users      (100)     2544 2023-05-12 18:07:33.000000 django-healthpoint-0.5.0/healthpoint/views.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      110 2023-05-12 18:14:21.868588 django-healthpoint-0.5.0/setup.cfg
+-rw-r--r--   0 pennersr  (1000) users      (100)     2237 2023-05-12 18:07:36.000000 django-healthpoint-0.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-healthpoint-0.4.1/LICENSE` & `django-healthpoint-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-healthpoint-0.4.1/PKG-INFO` & `django-healthpoint-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-healthpoint
-Version: 0.4.1
+Version: 0.5.0
 Summary: Easily create an endpoint for health checks
 Home-page: http://github.com/pennersr/django-healthpoint
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
-License: UNKNOWN
-Description: ==============================
-        Welcome to django-healthpoint!
-        ==============================
-        
-        .. image:: https://badge.fury.io/py/django-healthpoint.png
-           :target: http://badge.fury.io/py/django-healthpoint
-        
-        .. image:: https://travis-ci.org/pennersr/django-healthpoint.png
-           :target: http://travis-ci.org/pennersr/django-healthpoint
-        
-        .. image:: https://img.shields.io/pypi/v/django-healthpoint.svg
-           :target: https://pypi.python.org/pypi/django-healthpoint
-        
-        .. image:: https://coveralls.io/repos/pennersr/django-healthpoint/badge.png?branch=master
-           :alt: Coverage Status
-           :target: https://coveralls.io/r/pennersr/django-healthpoint
-        
-        .. image:: https://pennersr.github.io/img/bitcoin-badge.svg
-           :target: https://blockchain.info/address/1AJXuBMPHkaDCNX2rwAy34bGgs7hmrePEr
-        
-        .. image:: https://pennersr.github.io/img/emacs-badge.svg
-           :target: https://www.gnu.org/software/emacs/
-        
-        Framework for adding an endpoint for health checks to your project.
-        
-        Source code
-          http://github.com/pennersr/django-healthpoint
-        
-        
-        Quickstart
-        ==========
-        
-        Install the app::
-        
-            # settings.py
-            INSTALLED_APPS = [
-                ...
-                'healthpoint'
-            ]
-        
-            # If specified, this user is able to see the details for each
-            # individual check in the endpoint.
-            HEALTHPOINT_BASICAUTH_USERNAME = 'john'
-            HEALTHPOINT_BASICAUTH_PASSWORD = 'doe'
-        
-            # urls.py
-            urlpatterns = [
-                ...
-                url(r'^', include('healthpoint.urls')),
-            ]
-        
-        Add a module named ``health.py`` to any of your apps. For example::
-        
-            from datetime import timedelta
-        
-            from django.contrib.auth.models import User
-            from django.utils import timezone
-        
-            from healthpoint.decorators import health_check
-        
-        
-            @health_check
-            def user_signup():
-                last_user = User.objects.last()
-                time_since_last_signup = timezone.now() - last_user.date_joined
-                # Return True/False, throw an exception, or return a tuple with a
-                # detail message.
-                return (
-                    time_since_last_signup <= timedelta(days=1),
-                    "last signup was: {}".format(last_user.date_joined))
-        
-        
-        The health checks can be accessed via the ``/health/`` endpoint:
-        
-        - It executes all health checks, and reports status 200 if all checks succeed, status 500 otherwise.
-        
-        - If a staff user is logged in, the endpoint reports the result for each individual check::
-        
-            {
-             "success": {},
-             "error": {
-               "myproject.myapp.health.user_signup": "Last signup was: 2017-10-29 08:45:51"
-             }
-            }
-        
-        - To provide more detail on the result, the ``@health_check`` can return a tuple ``(success:bool, detail:str)``. The detail message will be listed in the result.
-        
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+==============================
+Welcome to django-healthpoint!
+==============================
+
+.. image:: https://badge.fury.io/py/django-healthpoint.png
+   :target: http://badge.fury.io/py/django-healthpoint
+
+.. image:: https://github.com/pennersr/django-healthpoint/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pennersr/django-healthpoint/actions
+
+.. image:: https://img.shields.io/pypi/v/django-healthpoint.svg
+   :target: https://pypi.python.org/pypi/django-healthpoint
+
+.. image:: https://coveralls.io/repos/pennersr/django-healthpoint/badge.png?branch=master
+   :alt: Coverage Status
+   :target: https://coveralls.io/r/pennersr/django-healthpoint
+
+.. image:: https://pennersr.github.io/img/bitcoin-badge.svg
+   :target: https://blockchain.info/address/1AJXuBMPHkaDCNX2rwAy34bGgs7hmrePEr
+
+.. image:: https://pennersr.github.io/img/emacs-badge.svg
+   :target: https://www.gnu.org/software/emacs/
+
+Framework for adding an endpoint for health checks to your project.
+
+Source code
+  http://github.com/pennersr/django-healthpoint
+
+
+Quickstart
+==========
+
+Install the app::
+
+    # settings.py
+    INSTALLED_APPS = [
+        ...
+        'healthpoint'
+    ]
+
+    # If specified, this user is able to see the details for each
+    # individual check in the endpoint.
+    HEALTHPOINT_BASICAUTH_USERNAME = 'john'
+    HEALTHPOINT_BASICAUTH_PASSWORD = 'doe'
+
+    # If set to True authentication is required for executing the
+    # health checks.
+    HEALTHPOINT_AUTH_REQUIRED = True
+
+    # urls.py
+    urlpatterns = [
+        ...
+        url(r'^', include('healthpoint.urls')),
+    ]
+
+Add a module named ``health.py`` to any of your apps. For example::
+
+    from datetime import timedelta
+
+    from django.contrib.auth.models import User
+    from django.utils import timezone
+
+    from healthpoint.decorators import health_check
+
+
+    @health_check
+    def user_signup():
+        last_user = User.objects.last()
+        time_since_last_signup = timezone.now() - last_user.date_joined
+        # Return True/False, throw an exception, or return a tuple with a
+        # detail message.
+        return (
+            time_since_last_signup <= timedelta(days=1),
+            "last signup was: {}".format(last_user.date_joined))
+
+
+The health checks can be accessed via the ``/health/`` endpoint:
+
+- It executes all health checks, and reports status 200 if all checks succeed, status 500 otherwise.
+
+- If a staff user is logged in, the endpoint reports the result for each individual check::
+
+    {
+     "success": {},
+     "error": {
+       "myproject.myapp.health.user_signup": "Last signup was: 2017-10-29 08:45:51"
+     }
+    }
+
+- To provide more detail on the result, the ``@health_check`` can return a tuple ``(success:bool, detail:str)``. The detail message will be listed in the result.
```

### Comparing `django-healthpoint-0.4.1/README.rst` & `django-healthpoint-0.5.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ==============================
 Welcome to django-healthpoint!
 ==============================
 
 .. image:: https://badge.fury.io/py/django-healthpoint.png
    :target: http://badge.fury.io/py/django-healthpoint
 
-.. image:: https://travis-ci.org/pennersr/django-healthpoint.png
-   :target: http://travis-ci.org/pennersr/django-healthpoint
+.. image:: https://github.com/pennersr/django-healthpoint/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pennersr/django-healthpoint/actions
 
 .. image:: https://img.shields.io/pypi/v/django-healthpoint.svg
    :target: https://pypi.python.org/pypi/django-healthpoint
 
 .. image:: https://coveralls.io/repos/pennersr/django-healthpoint/badge.png?branch=master
    :alt: Coverage Status
    :target: https://coveralls.io/r/pennersr/django-healthpoint
@@ -39,14 +39,18 @@
     ]
 
     # If specified, this user is able to see the details for each
     # individual check in the endpoint.
     HEALTHPOINT_BASICAUTH_USERNAME = 'john'
     HEALTHPOINT_BASICAUTH_PASSWORD = 'doe'
 
+    # If set to True authentication is required for executing the
+    # health checks.
+    HEALTHPOINT_AUTH_REQUIRED = True
+
     # urls.py
     urlpatterns = [
         ...
         url(r'^', include('healthpoint.urls')),
     ]
 
 Add a module named ``health.py`` to any of your apps. For example::
```

### Comparing `django-healthpoint-0.4.1/django_healthpoint.egg-info/PKG-INFO` & `django-healthpoint-0.5.0/django_healthpoint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,114 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-healthpoint
-Version: 0.4.1
+Version: 0.5.0
 Summary: Easily create an endpoint for health checks
 Home-page: http://github.com/pennersr/django-healthpoint
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
-License: UNKNOWN
-Description: ==============================
-        Welcome to django-healthpoint!
-        ==============================
-        
-        .. image:: https://badge.fury.io/py/django-healthpoint.png
-           :target: http://badge.fury.io/py/django-healthpoint
-        
-        .. image:: https://travis-ci.org/pennersr/django-healthpoint.png
-           :target: http://travis-ci.org/pennersr/django-healthpoint
-        
-        .. image:: https://img.shields.io/pypi/v/django-healthpoint.svg
-           :target: https://pypi.python.org/pypi/django-healthpoint
-        
-        .. image:: https://coveralls.io/repos/pennersr/django-healthpoint/badge.png?branch=master
-           :alt: Coverage Status
-           :target: https://coveralls.io/r/pennersr/django-healthpoint
-        
-        .. image:: https://pennersr.github.io/img/bitcoin-badge.svg
-           :target: https://blockchain.info/address/1AJXuBMPHkaDCNX2rwAy34bGgs7hmrePEr
-        
-        .. image:: https://pennersr.github.io/img/emacs-badge.svg
-           :target: https://www.gnu.org/software/emacs/
-        
-        Framework for adding an endpoint for health checks to your project.
-        
-        Source code
-          http://github.com/pennersr/django-healthpoint
-        
-        
-        Quickstart
-        ==========
-        
-        Install the app::
-        
-            # settings.py
-            INSTALLED_APPS = [
-                ...
-                'healthpoint'
-            ]
-        
-            # If specified, this user is able to see the details for each
-            # individual check in the endpoint.
-            HEALTHPOINT_BASICAUTH_USERNAME = 'john'
-            HEALTHPOINT_BASICAUTH_PASSWORD = 'doe'
-        
-            # urls.py
-            urlpatterns = [
-                ...
-                url(r'^', include('healthpoint.urls')),
-            ]
-        
-        Add a module named ``health.py`` to any of your apps. For example::
-        
-            from datetime import timedelta
-        
-            from django.contrib.auth.models import User
-            from django.utils import timezone
-        
-            from healthpoint.decorators import health_check
-        
-        
-            @health_check
-            def user_signup():
-                last_user = User.objects.last()
-                time_since_last_signup = timezone.now() - last_user.date_joined
-                # Return True/False, throw an exception, or return a tuple with a
-                # detail message.
-                return (
-                    time_since_last_signup <= timedelta(days=1),
-                    "last signup was: {}".format(last_user.date_joined))
-        
-        
-        The health checks can be accessed via the ``/health/`` endpoint:
-        
-        - It executes all health checks, and reports status 200 if all checks succeed, status 500 otherwise.
-        
-        - If a staff user is logged in, the endpoint reports the result for each individual check::
-        
-            {
-             "success": {},
-             "error": {
-               "myproject.myapp.health.user_signup": "Last signup was: 2017-10-29 08:45:51"
-             }
-            }
-        
-        - To provide more detail on the result, the ``@health_check`` can return a tuple ``(success:bool, detail:str)``. The detail message will be listed in the result.
-        
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+==============================
+Welcome to django-healthpoint!
+==============================
+
+.. image:: https://badge.fury.io/py/django-healthpoint.png
+   :target: http://badge.fury.io/py/django-healthpoint
+
+.. image:: https://github.com/pennersr/django-healthpoint/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/pennersr/django-healthpoint/actions
+
+.. image:: https://img.shields.io/pypi/v/django-healthpoint.svg
+   :target: https://pypi.python.org/pypi/django-healthpoint
+
+.. image:: https://coveralls.io/repos/pennersr/django-healthpoint/badge.png?branch=master
+   :alt: Coverage Status
+   :target: https://coveralls.io/r/pennersr/django-healthpoint
+
+.. image:: https://pennersr.github.io/img/bitcoin-badge.svg
+   :target: https://blockchain.info/address/1AJXuBMPHkaDCNX2rwAy34bGgs7hmrePEr
+
+.. image:: https://pennersr.github.io/img/emacs-badge.svg
+   :target: https://www.gnu.org/software/emacs/
+
+Framework for adding an endpoint for health checks to your project.
+
+Source code
+  http://github.com/pennersr/django-healthpoint
+
+
+Quickstart
+==========
+
+Install the app::
+
+    # settings.py
+    INSTALLED_APPS = [
+        ...
+        'healthpoint'
+    ]
+
+    # If specified, this user is able to see the details for each
+    # individual check in the endpoint.
+    HEALTHPOINT_BASICAUTH_USERNAME = 'john'
+    HEALTHPOINT_BASICAUTH_PASSWORD = 'doe'
+
+    # If set to True authentication is required for executing the
+    # health checks.
+    HEALTHPOINT_AUTH_REQUIRED = True
+
+    # urls.py
+    urlpatterns = [
+        ...
+        url(r'^', include('healthpoint.urls')),
+    ]
+
+Add a module named ``health.py`` to any of your apps. For example::
+
+    from datetime import timedelta
+
+    from django.contrib.auth.models import User
+    from django.utils import timezone
+
+    from healthpoint.decorators import health_check
+
+
+    @health_check
+    def user_signup():
+        last_user = User.objects.last()
+        time_since_last_signup = timezone.now() - last_user.date_joined
+        # Return True/False, throw an exception, or return a tuple with a
+        # detail message.
+        return (
+            time_since_last_signup <= timedelta(days=1),
+            "last signup was: {}".format(last_user.date_joined))
+
+
+The health checks can be accessed via the ``/health/`` endpoint:
+
+- It executes all health checks, and reports status 200 if all checks succeed, status 500 otherwise.
+
+- If a staff user is logged in, the endpoint reports the result for each individual check::
+
+    {
+     "success": {},
+     "error": {
+       "myproject.myapp.health.user_signup": "Last signup was: 2017-10-29 08:45:51"
+     }
+    }
+
+- To provide more detail on the result, the ``@health_check`` can return a tuple ``(success:bool, detail:str)``. The detail message will be listed in the result.
```

### Comparing `django-healthpoint-0.4.1/django_healthpoint.egg-info/SOURCES.txt` & `django-healthpoint-0.5.0/django_healthpoint.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 django_healthpoint.egg-info/PKG-INFO
 django_healthpoint.egg-info/SOURCES.txt
 django_healthpoint.egg-info/dependency_links.txt
 django_healthpoint.egg-info/not-zip-safe
 django_healthpoint.egg-info/requires.txt
 django_healthpoint.egg-info/top_level.txt
```

### Comparing `django-healthpoint-0.4.1/healthpoint/decorators.py` & `django-healthpoint-0.5.0/healthpoint/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from functools import wraps
 
 from healthpoint.registry import register_health_check
 
 
 def health_check(f):
-
     @wraps(f)
     def wrapper(*args, **kwargs):
         try:
             result = f(*args, **kwargs)
             if isinstance(result, bool):
-                success, detail = result, 'OK' if result else 'ERROR'
+                success, detail = result, "OK" if result else "ERROR"
             elif isinstance(result, tuple) and len(result) == 2:
                 success, detail = result
             else:
                 raise ValueError(
-                    'Your @health_check must return'
-                    ' a `bool`, or a tuple of (`bool`, `detail`)')
+                    "Your @health_check must return"
+                    " a `bool`, or a tuple of (`bool`, `detail`)"
+                )
         except Exception as e:
             success, detail = False, str(e)
         return success, detail
 
     register_health_check(wrapper)
     return wrapper
```

### Comparing `django-healthpoint-0.4.1/setup.py` & `django-healthpoint-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 #!/usr/bin/env python
 from __future__ import unicode_literals
+
 import codecs
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 from setuptools.command.test import test as TestCommand
 
 import healthpoint
 
 
 class DjangoTests(TestCommand):
-
     def finalize_options(self):
         TestCommand.finalize_options(self)
         self.test_args = []
         self.test_suite = True
 
     def run_tests(self):
         from django.core import management
-        DSM = 'DJANGO_SETTINGS_MODULE'
+
+        DSM = "DJANGO_SETTINGS_MODULE"
         if DSM not in os.environ:
-            os.environ[DSM] = 'healthpoint.tests.settings'
+            os.environ[DSM] = "healthpoint.tests.settings"
         management.execute_from_command_line()
 
 
 def read_files(*filenames):
     """
     Output the contents of one or more files to a single concatenated string.
     """
     output = []
     for filename in filenames:
-        f = codecs.open(filename, encoding='utf-8')
+        f = codecs.open(filename, encoding="utf-8")
         try:
             output.append(f.read())
         finally:
             f.close()
-    return '\n\n'.join(output)
+    return "\n\n".join(output)
 
 
 # Dynamically calculate the version based on healthpoint.VERSION.
 version = healthpoint.__version__
 
 setup(
-    name='django-healthpoint',
+    name="django-healthpoint",
     version=version,
-    url='http://github.com/pennersr/django-healthpoint',
-    description='Easily create an endpoint for health checks',
-    long_description=read_files('README.rst'),
-    author='Raymond Penners',
-    author_email='raymond.penners@intenct.nl',
-    platforms=['any'],
+    url="http://github.com/pennersr/django-healthpoint",
+    description="Easily create an endpoint for health checks",
+    long_description=read_files("README.rst"),
+    author="Raymond Penners",
+    author_email="raymond.penners@intenct.nl",
+    platforms=["any"],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=[
-        'django>=1.10'
-    ],
-    cmdclass={'test': DjangoTests},
+    install_requires=["django>=3.2"],
+    cmdclass={"test": DjangoTests},
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Web Environment',
-        'Framework :: Django',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Software Development :: Libraries :: Application Frameworks',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     zip_safe=False,
 )
```

