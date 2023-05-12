# Comparing `tmp/django-cloudspotlicense-5.4.0.tar.gz` & `tmp/django-cloudspotlicense-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-cloudspotlicense-5.4.0.tar", last modified: Fri May 12 07:06:26 2023, max compression
+gzip compressed data, was "dist\django-cloudspotlicense-5.4.1.tar", last modified: Fri May 12 09:25:16 2023, max compression
```

## Comparing `django-cloudspotlicense-5.4.0.tar` & `django-cloudspotlicense-5.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/
--rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/admin.py
--rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/apps.py
--rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/context_processors.py
--rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/
--rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/__init__.py
--rw-rw-rw-   0        0        0     2695 2022-12-09 13:18:17.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/mixins.py
--rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/models.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/
--rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/login.html
--rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/select_company.html
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/
--rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/license_tags.py
--rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/tests.py
--rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/urls.py
--rw-rw-rw-   0        0        0      270 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/utils.py
--rw-rw-rw-   0        0        0    14417 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/views.py
--rw-rw-rw-   0        0        0       69 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8123 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1114 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-5.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-5.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8123 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     7259 2023-03-08 12:16:04.000000 django-cloudspotlicense-5.4.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/
+-rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/admin.py
+-rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/apps.py
+-rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/context_processors.py
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/
+-rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2695 2022-12-09 13:18:17.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/mixins.py
+-rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/models.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templates/
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templates/auth/
+-rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templates/auth/login.html
+-rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templates/auth/select_company.html
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templatetags/
+-rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templatetags/license_tags.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/templatetags/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/tests.py
+-rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/urls.py
+-rw-rw-rw-   0        0        0      270 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/utils.py
+-rw-rw-rw-   0        0        0    14493 2023-05-12 09:25:10.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/views.py
+-rw-rw-rw-   0        0        0       69 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8123 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1114 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-5.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-5.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8123 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7259 2023-03-08 12:16:04.000000 django-cloudspotlicense-5.4.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 09:25:16.000000 django-cloudspotlicense-5.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-05-12 09:25:10.000000 django-cloudspotlicense-5.4.1/setup.py
```

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/helpers.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/helpers.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0001_initial.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/mixins.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/mixins.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/models.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/models.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/login.html` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/urls.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/urls.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense/views.py` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,25 +68,27 @@
         try:
             
             # Update the user with the new information
             user = UserModel.objects.get(username=username)
             user.first_name = api.user.first_name
             user.last_name = api.user.last_name
             user.license_token = api.token
+            user.pin = api.user.pin
             user.is_active = True
             user.save()
             
         except ObjectDoesNotExist:
             
             # We don't know the user, so we create them
             # Push it to the database
             user = UserModel.objects.create_user(username=username, email=username, password=password, **{
                 'first_name' : api.user.first_name,
                 'last_name' : api.user.last_name,
                 'license_token' : api.token,
+                'pin' : api.user.pin,
             })
             
             user.save()
             
         # Now that we know the user, we clear all the previously linked companies and reassign them to the companies that are included in the response
         user.available_companies.clear()
         for company_id in returned_companies: user.available_companies.add(company_id)
```

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/PKG-INFO` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 5.4.0
+Version: 5.4.1
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.1.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/SOURCES.txt` & `django-cloudspotlicense-5.4.1/django_cloudspotlicense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/LICENSE.txt` & `django-cloudspotlicense-5.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/PKG-INFO` & `django-cloudspotlicense-5.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 5.4.0
+Version: 5.4.1
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.1.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-5.4.0/README.md` & `django-cloudspotlicense-5.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.4.0/setup.py` & `django-cloudspotlicense-5.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'django-cloudspotlicense',         
   packages=['django_cloudspotlicense', 'django_cloudspotlicense.migrations', 'django_cloudspotlicense.templatetags'],
   include_package_data=True,
-  version = '5.4.0',
+  version = '5.4.1',
   license='GPL-3.0-or-later',
   description = 'Django package to integrate the authentication of the Cloudspot License Server in other django applications',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/django-cloudspotlicense',
-  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.1.tar.gz',
   keywords = ['cloudspot', 'django'],
   install_requires=[
           'requests',
           'cloudspot-license-api',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

