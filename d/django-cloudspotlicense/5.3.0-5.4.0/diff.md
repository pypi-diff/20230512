# Comparing `tmp/django-cloudspotlicense-5.3.0.tar.gz` & `tmp/django-cloudspotlicense-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-cloudspotlicense-5.3.0.tar", last modified: Mon Mar 27 15:19:38 2023, max compression
+gzip compressed data, was "dist\django-cloudspotlicense-5.4.0.tar", last modified: Fri May 12 07:06:26 2023, max compression
```

## Comparing `django-cloudspotlicense-5.3.0.tar` & `django-cloudspotlicense-5.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/
--rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/admin.py
--rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/apps.py
--rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/context_processors.py
--rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/
--rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
--rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/__init__.py
--rw-rw-rw-   0        0        0     2695 2022-12-09 13:18:17.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/mixins.py
--rw-rw-rw-   0        0        0     1450 2022-10-17 09:58:57.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/models.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templates/auth/
--rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templates/auth/login.html
--rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templates/auth/select_company.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templatetags/
--rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templatetags/license_tags.py
--rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/templatetags/__init__.py
--rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/tests.py
--rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/urls.py
--rw-rw-rw-   0        0        0      270 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/utils.py
--rw-rw-rw-   0        0        0    13431 2023-03-27 15:17:49.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/views.py
--rw-rw-rw-   0        0        0       69 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     8123 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1114 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       24 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-5.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-5.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8123 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7259 2023-03-08 12:16:04.000000 django-cloudspotlicense-5.3.0/README.md
--rw-rw-rw-   0        0        0       86 2023-03-27 15:19:38.000000 django-cloudspotlicense-5.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2023-03-27 15:18:37.000000 django-cloudspotlicense-5.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/
+-rw-rw-rw-   0        0        0       66 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/admin.py
+-rw-rw-rw-   0        0        0      183 2022-10-05 10:03:35.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/apps.py
+-rw-rw-rw-   0        0        0      246 2022-10-19 14:26:18.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/context_processors.py
+-rw-rw-rw-   0        0        0      905 2022-10-05 12:22:39.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/
+-rw-rw-rw-   0        0        0     3881 2022-10-05 11:36:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      452 2022-10-17 09:58:41.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0002_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0      505 2022-10-17 09:59:00.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0003_alter_cloudspotcompany_users.py
+-rw-rw-rw-   0        0        0        0 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2695 2022-12-09 13:18:17.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/mixins.py
+-rw-rw-rw-   0        0        0     1515 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/models.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/
+-rw-rw-rw-   0        0        0      634 2022-10-05 10:05:52.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/login.html
+-rw-rw-rw-   0        0        0      496 2022-10-17 09:51:34.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/select_company.html
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/
+-rw-rw-rw-   0        0        0      377 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/license_tags.py
+-rw-rw-rw-   0        0        0        0 2022-12-09 12:36:09.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/templatetags/__init__.py
+-rw-rw-rw-   0        0        0       63 2022-10-05 08:35:57.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/tests.py
+-rw-rw-rw-   0        0        0     1019 2023-03-08 12:37:58.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/urls.py
+-rw-rw-rw-   0        0        0      270 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/utils.py
+-rw-rw-rw-   0        0        0    14417 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/views.py
+-rw-rw-rw-   0        0        0       69 2023-03-13 08:55:48.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     8123 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1114 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       24 2023-05-12 07:06:25.000000 django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2021-04-16 13:14:04.000000 django-cloudspotlicense-5.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       93 2022-10-05 14:15:21.000000 django-cloudspotlicense-5.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8123 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7259 2023-03-08 12:16:04.000000 django-cloudspotlicense-5.4.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-12 07:06:26.000000 django-cloudspotlicense-5.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2023-05-12 07:05:12.000000 django-cloudspotlicense-5.4.0/setup.py
```

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/helpers.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/helpers.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/migrations/0001_initial.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/mixins.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/mixins.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/models.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,13 +26,14 @@
         self.content_type = ct
         super().save(*args)
         
 class CloudspotUser(AbstractUser):
     id  = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     license_token = models.CharField(max_length=100, null=True, blank=True)
     company = models.ForeignKey('CloudspotCompany', on_delete=models.SET_NULL, null=True, blank=True)
+    pin = models.CharField(max_length=6, null=True, blank=True)
 
 class CloudspotCompany(models.Model):
     id  = models.UUIDField(primary_key=True, editable=False)
     name = models.CharField(max_length=100, null=True, blank=True)
     
     users = models.ManyToManyField('CloudspotUser', related_name="available_companies")
```

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/templates/auth/login.html` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/templates/auth/login.html`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/urls.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/urls.py`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense/views.py` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,21 @@
         if not company: return HttpResponseBadRequest('Company with ID {0} could not be found.'.format(company_id))
         if company not in user.available_companies.all(): return HttpResponseBadRequest('User is not in requested company.')
         
         # User is a valid user and has a valid company
         # Use the returned auth token to get all the permissions for the specified company
         api = CloudspotLicense_API(settings.CLOUDSPOT_LICENSE_APP, token=auth_token)
         
+        # Set the company for impersonation
+        # TODO: Change the company only for the impersonation, so that the user can still use their own chosen company while being impersonated
         user.company = company
+        
+        # Update the license token so we don't get a mismatch between the license server and the application
+        user.license_token = auth_token
+        
         user.save()
         
         try:
             permissions = api.get_company_permissions(company_id)
         except Exception as e:
             return HttpResponseBadRequest('Could not retrieve permissions for user. Error: {0}'.format(e))
         
@@ -281,8 +287,21 @@
                 return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : 'No user matched the current_email.' }}, status=HTTPStatus.NOT_FOUND)
             
             user.username = change_to_email
             user.email = change_to_email
             user.save()
             
             return JsonResponse({ 'status' : ResponseStatus.OBJECT_UPDATED })
-            
+        elif event == 'user.pin.updated':
+            user_username = data['user_username']
+            pin = data['pin']
+            if pin == '': pin = None
+            
+            try:
+                user = UserModel.objects.get(username=user_username)
+            except UserModel.DoesNotExist:
+                return JsonResponse({ 'status' : ResponseStatus.NOT_FOUND, 'error' : { 'message' : 'No user matched the user_username.' }}, status=HTTPStatus.NOT_FOUND)
+            
+            user.pin = pin
+            user.save()
+            
+            return JsonResponse({ 'status' : ResponseStatus.OBJECT_UPDATED })
```

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/PKG-INFO` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 5.3.0
+Version: 5.4.0
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.3.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-5.3.0/django_cloudspotlicense.egg-info/SOURCES.txt` & `django-cloudspotlicense-5.4.0/django_cloudspotlicense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/LICENSE.txt` & `django-cloudspotlicense-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/PKG-INFO` & `django-cloudspotlicense-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-cloudspotlicense
-Version: 5.3.0
+Version: 5.4.0
 Summary: Django package to integrate the authentication of the Cloudspot License Server in other django applications
 Home-page: https://github.com/Ecosy-EU/django-cloudspotlicense
 Author: Alexander Schillemans
 Author-email: alexander.schillemans@lhs.global
 License: GPL-3.0-or-later
-Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.3.0.tar.gz
+Download-URL: https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz
 Keywords: cloudspot,django
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `django-cloudspotlicense-5.3.0/README.md` & `django-cloudspotlicense-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-cloudspotlicense-5.3.0/setup.py` & `django-cloudspotlicense-5.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'django-cloudspotlicense',         
   packages=['django_cloudspotlicense', 'django_cloudspotlicense.migrations', 'django_cloudspotlicense.templatetags'],
   include_package_data=True,
-  version = '5.3.0',
+  version = '5.4.0',
   license='GPL-3.0-or-later',
   description = 'Django package to integrate the authentication of the Cloudspot License Server in other django applications',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Alexander Schillemans',
   author_email = 'alexander.schillemans@lhs.global',
   url = 'https://github.com/Ecosy-EU/django-cloudspotlicense',
-  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.3.0.tar.gz',
+  download_url = 'https://github.com/Ecosy-EU/django-cloudspotlicense/archive/refs/tags/5.4.0.tar.gz',
   keywords = ['cloudspot', 'django'],
   install_requires=[
           'requests',
           'cloudspot-license-api',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

