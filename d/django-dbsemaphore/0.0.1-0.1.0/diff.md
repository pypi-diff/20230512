# Comparing `tmp/django-dbsemaphore-0.0.1.tar.gz` & `tmp/django-dbsemaphore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dbsemaphore-0.0.1.tar", last modified: Tue Aug 30 20:34:36 2022, max compression
+gzip compressed data, was "django-dbsemaphore-0.1.0.tar", last modified: Fri May 12 11:02:36 2023, max compression
```

## Comparing `django-dbsemaphore-0.0.1.tar` & `django-dbsemaphore-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.742703 django-dbsemaphore-0.0.1/
--rw-r-----   0 boer      (1000) boer      (1000)     7652 2022-08-30 18:41:01.000000 django-dbsemaphore-0.0.1/LICENSE.txt
--rw-r-----   0 boer      (1000) boer      (1000)       16 2022-08-30 18:23:34.000000 django-dbsemaphore-0.0.1/MANIFEST.in
--rw-r-----   0 boer      (1000) boer      (1000)     4681 2022-08-30 20:34:36.742703 django-dbsemaphore-0.0.1/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)     3708 2022-08-30 20:24:07.000000 django-dbsemaphore-0.0.1/README.md
--rw-r-----   0 boer      (1000) boer      (1000)        6 2022-08-30 20:29:54.000000 django-dbsemaphore-0.0.1/VERSION
--rw-r-----   0 boer      (1000) boer      (1000)     1351 2022-08-30 20:34:36.743703 django-dbsemaphore-0.0.1/setup.cfg
--rwxr-x---   0 boer      (1000) boer      (1000)       61 2022-08-30 18:23:00.000000 django-dbsemaphore-0.0.1/setup.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.738703 django-dbsemaphore-0.0.1/src/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.740703 django-dbsemaphore-0.0.1/src/dbsemaphore/
--rw-r-----   0 boer      (1000) boer      (1000)       53 2022-08-25 20:11:46.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/__init__.py
--rw-r-----   0 boer      (1000) boer      (1000)      252 2022-08-30 18:36:56.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/admin.py
--rw-r-----   0 boer      (1000) boer      (1000)      154 2022-08-25 19:48:21.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/apps.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.738703 django-dbsemaphore-0.0.1/src/dbsemaphore/management/
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.741703 django-dbsemaphore-0.0.1/src/dbsemaphore/management/commands/
--rw-r-----   0 boer      (1000) boer      (1000)     1237 2022-08-30 17:26:38.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/management/commands/dbsemaphore-test-acquire.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.741703 django-dbsemaphore-0.0.1/src/dbsemaphore/migrations/
--rw-r-----   0 boer      (1000) boer      (1000)      648 2022-08-30 18:14:24.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/migrations/0001_initial.py
--rw-r-----   0 boer      (1000) boer      (1000)        0 2022-08-25 19:48:21.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/migrations/__init__.py
--rw-r-----   0 boer      (1000) boer      (1000)      367 2022-08-30 18:30:38.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/models.py
--rw-r-----   0 boer      (1000) boer      (1000)     2236 2022-08-30 20:24:31.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/semaphore.py
--rw-r-----   0 boer      (1000) boer      (1000)     1344 2022-08-30 18:37:41.000000 django-dbsemaphore-0.0.1/src/dbsemaphore/tests.py
-drwxr-x---   0 boer      (1000) boer      (1000)        0 2022-08-30 20:34:36.742703 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/
--rw-r-----   0 boer      (1000) boer      (1000)     4681 2022-08-30 20:34:36.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/PKG-INFO
--rw-r-----   0 boer      (1000) boer      (1000)      633 2022-08-30 20:34:36.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/SOURCES.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2022-08-30 20:34:36.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/dependency_links.txt
--rw-r-----   0 boer      (1000) boer      (1000)       14 2022-08-30 20:34:36.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/requires.txt
--rw-r-----   0 boer      (1000) boer      (1000)       12 2022-08-30 20:34:36.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/top_level.txt
--rw-r-----   0 boer      (1000) boer      (1000)        1 2022-08-30 18:48:06.000000 django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/zip-safe
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.609585 django-dbsemaphore-0.1.0/
+-rw-r-----   0 boer      (1000) boer      (1000)     7652 2022-08-30 18:41:01.000000 django-dbsemaphore-0.1.0/LICENSE.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       16 2022-08-30 18:23:34.000000 django-dbsemaphore-0.1.0/MANIFEST.in
+-rw-r-----   0 boer      (1000) boer      (1000)     5398 2023-05-12 11:02:36.609585 django-dbsemaphore-0.1.0/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)     4425 2023-05-12 10:56:18.000000 django-dbsemaphore-0.1.0/README.md
+-rw-r-----   0 boer      (1000) boer      (1000)        6 2023-05-12 10:37:45.000000 django-dbsemaphore-0.1.0/VERSION
+-rw-r-----   0 boer      (1000) boer      (1000)     1352 2023-05-12 11:02:36.610585 django-dbsemaphore-0.1.0/setup.cfg
+-rwxr-x---   0 boer      (1000) boer      (1000)       61 2022-08-30 18:23:00.000000 django-dbsemaphore-0.1.0/setup.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.598584 django-dbsemaphore-0.1.0/src/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.603584 django-dbsemaphore-0.1.0/src/dbsemaphore/
+-rw-r-----   0 boer      (1000) boer      (1000)       53 2022-08-25 20:11:46.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/__init__.py
+-rw-r-----   0 boer      (1000) boer      (1000)      252 2022-08-30 18:36:56.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/admin.py
+-rw-r-----   0 boer      (1000) boer      (1000)      154 2022-08-25 19:48:21.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/apps.py
+-rw-r-----   0 boer      (1000) boer      (1000)     1325 2023-05-12 10:35:29.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/contextmanager.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.598584 django-dbsemaphore-0.1.0/src/dbsemaphore/management/
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.604585 django-dbsemaphore-0.1.0/src/dbsemaphore/management/commands/
+-rw-r-----   0 boer      (1000) boer      (1000)     1237 2022-08-30 17:26:38.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/management/commands/dbsemaphore-test-acquire.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.605584 django-dbsemaphore-0.1.0/src/dbsemaphore/migrations/
+-rw-r-----   0 boer      (1000) boer      (1000)      648 2022-08-30 18:14:24.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/migrations/0001_initial.py
+-rw-r-----   0 boer      (1000) boer      (1000)        0 2022-08-25 19:48:21.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/migrations/__init__.py
+-rw-r-----   0 boer      (1000) boer      (1000)      367 2022-08-30 18:30:38.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/models.py
+-rw-r-----   0 boer      (1000) boer      (1000)     2236 2022-08-30 20:24:31.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/semaphore.py
+-rw-r-----   0 boer      (1000) boer      (1000)     1344 2022-08-30 18:37:41.000000 django-dbsemaphore-0.1.0/src/dbsemaphore/tests.py
+drwxr-x---   0 boer      (1000) boer      (1000)        0 2023-05-12 11:02:36.609585 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/
+-rw-r-----   0 boer      (1000) boer      (1000)     5398 2023-05-12 11:02:36.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/PKG-INFO
+-rw-r-----   0 boer      (1000) boer      (1000)      667 2023-05-12 11:02:36.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/SOURCES.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2023-05-12 11:02:36.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/dependency_links.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       14 2023-05-12 11:02:36.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/requires.txt
+-rw-r-----   0 boer      (1000) boer      (1000)       12 2023-05-12 11:02:36.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/top_level.txt
+-rw-r-----   0 boer      (1000) boer      (1000)        1 2022-08-30 18:48:06.000000 django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/zip-safe
```

### Comparing `django-dbsemaphore-0.0.1/LICENSE.txt` & `django-dbsemaphore-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-dbsemaphore-0.0.1/PKG-INFO` & `django-dbsemaphore-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dbsemaphore
-Version: 0.0.1
+Version: 0.1.0
 Summary: django-dbsemaphore — multi-ticket semaphores implemented on top of DB row locks
 Home-page: https://hub.sr.ht/~nullenenenen/django-dbsemaphore/
 Author: nullenenenen
 Author-email: nullenenenen@gavagai.eu
 License: LGPL-3.0+
 Project-URL: Documentation, https://git.sr.ht/~nullenenenen/django-dbsemaphore/tree/master/item/README.md
 Project-URL: Source, https://git.sr.ht/~nullenenenen/django-dbsemaphore/
@@ -40,36 +40,37 @@
 Locked files (or locked byte ranges) disappear when a process crashes; its file descriptors are gone thus so are its locks.
 That's a great property. However, file locks are not multi-ticket. The file (or byterange therein) is either locked or not.
 The OS file locking APIs are good to implement *mutexes* with, but not *semaphores* — except, trivially, a 1-ticket semaphore — which is a mutex ;-).
 
 # Quirks
 - In contrast to Posix/SysV semaphores and `lockf`-based approaches, with django-dbsemaphore you can't block until a ticket becomes available.
 - From within the same transaction you can acquire tickets you already have over and over. In fact, it's currently impossible to get new tickets of a semaphore on a transaction that already has a ticket of that same semaphore. Typically, you won't need multiple tickets of the same semaphore in the same transaction, but a future version of this software might make it possible. In the meantime, consider using multiple semaphores for your multistage semaphore needs.
-- They work within transactions. You'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. There's no other way to return a ticket.
+- At the base level, they work within transactions. If you want to use `dbsemaphore.semaphore.acquire()`, you'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. However, there is a context manager (`dbsemaphore.contextmanager.semaphore_ticket()`) that abstracts all of that away for you and makes it easy to use a ticket from anywhere in your code. See below.
 
 # Compatibility
 Currently this is tested on PostgreSQL 14 and Django 3.2.
 - It currently doesn't work on SQLite due to the way in which tables are locked in `semaphore.make()`
 - MySQL, Oracle: Untested.
 - (neat) Patches welcome!
 
 # Installing
 1. `pip install django-dbsemaphore`
 2. add 'dbsemaphore' to your Django's `settings.INSTALLED_APPS`.
 3. run `./manage.py migrate dbsemaphore` or some variation of such
 
 # How to use it
 
-Run the Django test, or read `test.py`, or have a look at the below:
+Have a look at the below examples, run the Django test, or read `test.py`.
+
+
+## Semaphore management
 
 ```python
 from dbsemaphore import semaphore as sem
 
-# Semaphore management
-
 # Creates a semaphore called 'test' with 3 tickets
 >>> sem.make('test', 3)
 
 # Increases the number of tickets of semaphore 'test' to 4.
 # Blocks on concurrent calls of `make`.
 # If 'test' doesn't exist, it will be created (with 4 tickets).
 >>> sem.make('test', 4)
@@ -81,21 +82,39 @@
 
 # Returns a dictionary of available semaphores, with their ticket counts.
 >>> sem.list()
 {'test', 2}
 
 # Destroys the semaphore. Blocks until all its tickets have been returned.
 >>> sem.destroy('test')
+```
+
+## Acquiring tickets; what we're here for!
 
+### With the contextmanager
 
-# Acquiring tickets; what we're here for!
+```python
+from dbsemaphore.contextmanager import semaphore_ticket
 
+# We use the semaphore named 'test' that we have created above.
+with semaphore_ticket('test') as theticket:
+    if theticket is None:
+        print("Boo! No ticket was available!")
+    else:
+        do_the_ticketed_thing()
+```
+
+### Using the lower-level API
+
+```python
 from django.db import transaction
+from dbsemaphore import semaphore as sem
 
 @transaction.atomic
 def do_something_potentially_from_many_processes_or_threads_but_not_too_many_at_the_same_time():
+    # We use the semaphore named 'test' that we have created above.
     if ticket := sem.acquire('test'):
         do_that_something()
 
 # When the transaction terminates, the ticket is returned to the semaphore.
 # In fact, there isn't any API function to explicitly return a ticket...
 ```
```

### Comparing `django-dbsemaphore-0.0.1/README.md` & `django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: django-dbsemaphore
+Version: 0.1.0
+Summary: django-dbsemaphore — multi-ticket semaphores implemented on top of DB row locks
+Home-page: https://hub.sr.ht/~nullenenenen/django-dbsemaphore/
+Author: nullenenenen
+Author-email: nullenenenen@gavagai.eu
+License: LGPL-3.0+
+Project-URL: Documentation, https://git.sr.ht/~nullenenenen/django-dbsemaphore/tree/master/item/README.md
+Project-URL: Source, https://git.sr.ht/~nullenenenen/django-dbsemaphore/
+Keywords: Django semaphore
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Classifier: Topic :: Database
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Django-DBSemaphore
 
 This gives you multi-ticket DB-defined semaphores implemented on top of DB row locks.
 
 # Alternatives
 
 The orthodox alternatives are:
@@ -17,36 +40,37 @@
 Locked files (or locked byte ranges) disappear when a process crashes; its file descriptors are gone thus so are its locks.
 That's a great property. However, file locks are not multi-ticket. The file (or byterange therein) is either locked or not.
 The OS file locking APIs are good to implement *mutexes* with, but not *semaphores* — except, trivially, a 1-ticket semaphore — which is a mutex ;-).
 
 # Quirks
 - In contrast to Posix/SysV semaphores and `lockf`-based approaches, with django-dbsemaphore you can't block until a ticket becomes available.
 - From within the same transaction you can acquire tickets you already have over and over. In fact, it's currently impossible to get new tickets of a semaphore on a transaction that already has a ticket of that same semaphore. Typically, you won't need multiple tickets of the same semaphore in the same transaction, but a future version of this software might make it possible. In the meantime, consider using multiple semaphores for your multistage semaphore needs.
-- They work within transactions. You'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. There's no other way to return a ticket.
+- At the base level, they work within transactions. If you want to use `dbsemaphore.semaphore.acquire()`, you'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. However, there is a context manager (`dbsemaphore.contextmanager.semaphore_ticket()`) that abstracts all of that away for you and makes it easy to use a ticket from anywhere in your code. See below.
 
 # Compatibility
 Currently this is tested on PostgreSQL 14 and Django 3.2.
 - It currently doesn't work on SQLite due to the way in which tables are locked in `semaphore.make()`
 - MySQL, Oracle: Untested.
 - (neat) Patches welcome!
 
 # Installing
 1. `pip install django-dbsemaphore`
 2. add 'dbsemaphore' to your Django's `settings.INSTALLED_APPS`.
 3. run `./manage.py migrate dbsemaphore` or some variation of such
 
 # How to use it
 
-Run the Django test, or read `test.py`, or have a look at the below:
+Have a look at the below examples, run the Django test, or read `test.py`.
+
+
+## Semaphore management
 
 ```python
 from dbsemaphore import semaphore as sem
 
-# Semaphore management
-
 # Creates a semaphore called 'test' with 3 tickets
 >>> sem.make('test', 3)
 
 # Increases the number of tickets of semaphore 'test' to 4.
 # Blocks on concurrent calls of `make`.
 # If 'test' doesn't exist, it will be created (with 4 tickets).
 >>> sem.make('test', 4)
@@ -58,21 +82,39 @@
 
 # Returns a dictionary of available semaphores, with their ticket counts.
 >>> sem.list()
 {'test', 2}
 
 # Destroys the semaphore. Blocks until all its tickets have been returned.
 >>> sem.destroy('test')
+```
+
+## Acquiring tickets; what we're here for!
 
+### With the contextmanager
 
-# Acquiring tickets; what we're here for!
+```python
+from dbsemaphore.contextmanager import semaphore_ticket
+
+# We use the semaphore named 'test' that we have created above.
+with semaphore_ticket('test') as theticket:
+    if theticket is None:
+        print("Boo! No ticket was available!")
+    else:
+        do_the_ticketed_thing()
+```
+
+### Using the lower-level API
 
+```python
 from django.db import transaction
+from dbsemaphore import semaphore as sem
 
 @transaction.atomic
 def do_something_potentially_from_many_processes_or_threads_but_not_too_many_at_the_same_time():
+    # We use the semaphore named 'test' that we have created above.
     if ticket := sem.acquire('test'):
         do_that_something()
 
 # When the transaction terminates, the ticket is returned to the semaphore.
 # In fact, there isn't any API function to explicitly return a ticket...
-```
+```
```

### Comparing `django-dbsemaphore-0.0.1/setup.cfg` & `django-dbsemaphore-0.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 author_email = nullenenenen@gavagai.eu
 description = django-dbsemaphore — multi-ticket semaphores implemented on top of DB row locks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://hub.sr.ht/~nullenenenen/django-dbsemaphore/
 keywords = Django semaphore
 license = LGPL-3.0+
-license_file = LICENSE.txt
+license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 3 - Alpha
 	Framework :: Django
 	Intended Audience :: Developers
 	License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 	Operating System :: OS Independent
 	Topic :: Software Development
```

### Comparing `django-dbsemaphore-0.0.1/src/dbsemaphore/management/commands/dbsemaphore-test-acquire.py` & `django-dbsemaphore-0.1.0/src/dbsemaphore/management/commands/dbsemaphore-test-acquire.py`

 * *Files identical despite different names*

### Comparing `django-dbsemaphore-0.0.1/src/dbsemaphore/migrations/0001_initial.py` & `django-dbsemaphore-0.1.0/src/dbsemaphore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dbsemaphore-0.0.1/src/dbsemaphore/semaphore.py` & `django-dbsemaphore-0.1.0/src/dbsemaphore/semaphore.py`

 * *Files identical despite different names*

### Comparing `django-dbsemaphore-0.0.1/src/dbsemaphore/tests.py` & `django-dbsemaphore-0.1.0/src/dbsemaphore/tests.py`

 * *Files identical despite different names*

### Comparing `django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/PKG-INFO` & `django-dbsemaphore-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: django-dbsemaphore
-Version: 0.0.1
-Summary: django-dbsemaphore — multi-ticket semaphores implemented on top of DB row locks
-Home-page: https://hub.sr.ht/~nullenenenen/django-dbsemaphore/
-Author: nullenenenen
-Author-email: nullenenenen@gavagai.eu
-License: LGPL-3.0+
-Project-URL: Documentation, https://git.sr.ht/~nullenenenen/django-dbsemaphore/tree/master/item/README.md
-Project-URL: Source, https://git.sr.ht/~nullenenenen/django-dbsemaphore/
-Keywords: Django semaphore
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Classifier: Topic :: Database
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Django-DBSemaphore
 
 This gives you multi-ticket DB-defined semaphores implemented on top of DB row locks.
 
 # Alternatives
 
 The orthodox alternatives are:
@@ -40,36 +17,37 @@
 Locked files (or locked byte ranges) disappear when a process crashes; its file descriptors are gone thus so are its locks.
 That's a great property. However, file locks are not multi-ticket. The file (or byterange therein) is either locked or not.
 The OS file locking APIs are good to implement *mutexes* with, but not *semaphores* — except, trivially, a 1-ticket semaphore — which is a mutex ;-).
 
 # Quirks
 - In contrast to Posix/SysV semaphores and `lockf`-based approaches, with django-dbsemaphore you can't block until a ticket becomes available.
 - From within the same transaction you can acquire tickets you already have over and over. In fact, it's currently impossible to get new tickets of a semaphore on a transaction that already has a ticket of that same semaphore. Typically, you won't need multiple tickets of the same semaphore in the same transaction, but a future version of this software might make it possible. In the meantime, consider using multiple semaphores for your multistage semaphore needs.
-- They work within transactions. You'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. There's no other way to return a ticket.
+- At the base level, they work within transactions. If you want to use `dbsemaphore.semaphore.acquire()`, you'll need to structure your ticket acquisitions around DB transactions, and close those transactions (rollback or commit) to return the tickets. However, there is a context manager (`dbsemaphore.contextmanager.semaphore_ticket()`) that abstracts all of that away for you and makes it easy to use a ticket from anywhere in your code. See below.
 
 # Compatibility
 Currently this is tested on PostgreSQL 14 and Django 3.2.
 - It currently doesn't work on SQLite due to the way in which tables are locked in `semaphore.make()`
 - MySQL, Oracle: Untested.
 - (neat) Patches welcome!
 
 # Installing
 1. `pip install django-dbsemaphore`
 2. add 'dbsemaphore' to your Django's `settings.INSTALLED_APPS`.
 3. run `./manage.py migrate dbsemaphore` or some variation of such
 
 # How to use it
 
-Run the Django test, or read `test.py`, or have a look at the below:
+Have a look at the below examples, run the Django test, or read `test.py`.
+
+
+## Semaphore management
 
 ```python
 from dbsemaphore import semaphore as sem
 
-# Semaphore management
-
 # Creates a semaphore called 'test' with 3 tickets
 >>> sem.make('test', 3)
 
 # Increases the number of tickets of semaphore 'test' to 4.
 # Blocks on concurrent calls of `make`.
 # If 'test' doesn't exist, it will be created (with 4 tickets).
 >>> sem.make('test', 4)
@@ -81,21 +59,39 @@
 
 # Returns a dictionary of available semaphores, with their ticket counts.
 >>> sem.list()
 {'test', 2}
 
 # Destroys the semaphore. Blocks until all its tickets have been returned.
 >>> sem.destroy('test')
+```
+
+## Acquiring tickets; what we're here for!
 
+### With the contextmanager
 
-# Acquiring tickets; what we're here for!
+```python
+from dbsemaphore.contextmanager import semaphore_ticket
 
+# We use the semaphore named 'test' that we have created above.
+with semaphore_ticket('test') as theticket:
+    if theticket is None:
+        print("Boo! No ticket was available!")
+    else:
+        do_the_ticketed_thing()
+```
+
+### Using the lower-level API
+
+```python
 from django.db import transaction
+from dbsemaphore import semaphore as sem
 
 @transaction.atomic
 def do_something_potentially_from_many_processes_or_threads_but_not_too_many_at_the_same_time():
+    # We use the semaphore named 'test' that we have created above.
     if ticket := sem.acquire('test'):
         do_that_something()
 
 # When the transaction terminates, the ticket is returned to the semaphore.
 # In fact, there isn't any API function to explicitly return a ticket...
-```
+```
```

### Comparing `django-dbsemaphore-0.0.1/src/django_dbsemaphore.egg-info/SOURCES.txt` & `django-dbsemaphore-0.1.0/src/django_dbsemaphore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 VERSION
 setup.cfg
 setup.py
 src/dbsemaphore/__init__.py
 src/dbsemaphore/admin.py
 src/dbsemaphore/apps.py
+src/dbsemaphore/contextmanager.py
 src/dbsemaphore/models.py
 src/dbsemaphore/semaphore.py
 src/dbsemaphore/tests.py
 src/dbsemaphore/management/commands/dbsemaphore-test-acquire.py
 src/dbsemaphore/migrations/0001_initial.py
 src/dbsemaphore/migrations/__init__.py
 src/django_dbsemaphore.egg-info/PKG-INFO
```

