# Comparing `tmp/djangoldp_application-1.0.9.tar.gz` & `tmp/djangoldp_application-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_application-1.0.9.tar", last modified: Tue May  2 16:51:50 2023, max compression
+gzip compressed data, was "dist/djangoldp_application-1.1.0.tar", last modified: Fri May 12 14:15:26 2023, max compression
```

## Comparing `djangoldp_application-1.0.9.tar` & `djangoldp_application-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/
--rw-r--r--   0 root         (0) root         (0)      300 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1108 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-02 16:51:49.000000 djangoldp_application-1.0.9/djangoldp_application.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application/
--rw-rw-rw-   0 root         (0) root         (0)    10807 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/views.py
--rw-rw-rw-   0 root         (0) root         (0)    18785 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5338 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-02 16:51:47.000000 djangoldp_application-1.0.9/djangoldp_application/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 16:51:50.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0009_applicationgraphics.py
--rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0010_auto_20230331_0921.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0003_application_api_url.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0005_auto_20230331_0850.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0007_auto_20230331_0857.py
--rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0008_applicationnpm.py
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0004_auto_20230328_1657.py
--rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0002_deployment.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-02 16:51:31.000000 djangoldp_application-1.0.9/djangoldp_application/migrations/0006_applicationservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1076 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application/
+-rw-rw-rw-   0 root         (0) root         (0)    11964 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    19301 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5406 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-12 14:15:23.000000 djangoldp_application-1.1.0/djangoldp_application/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 14:15:26.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0009_applicationgraphics.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0014_auto_20230512_1613.py
+-rw-rw-rw-   0 root         (0) root         (0)    22281 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0011_auto_20230512_1555.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0010_auto_20230331_0921.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0013_auto_20230512_1608.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0012_auto_20230512_1556.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0003_application_api_url.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0005_auto_20230331_0850.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0007_auto_20230331_0857.py
+-rw-rw-rw-   0 root         (0) root         (0)     2157 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0008_applicationnpm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0004_auto_20230328_1657.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0002_deployment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-05-12 14:15:08.000000 djangoldp_application-1.1.0/djangoldp_application/migrations/0006_applicationservice.py
```

### Comparing `djangoldp_application-1.0.9/README.md` & `djangoldp_application-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/setup.cfg` & `djangoldp_application-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application.egg-info/SOURCES.txt` & `djangoldp_application-1.1.0/djangoldp_application.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,8 +19,12 @@
 djangoldp_application/migrations/0004_auto_20230328_1657.py
 djangoldp_application/migrations/0005_auto_20230331_0850.py
 djangoldp_application/migrations/0006_applicationservice.py
 djangoldp_application/migrations/0007_auto_20230331_0857.py
 djangoldp_application/migrations/0008_applicationnpm.py
 djangoldp_application/migrations/0009_applicationgraphics.py
 djangoldp_application/migrations/0010_auto_20230331_0921.py
+djangoldp_application/migrations/0011_auto_20230512_1555.py
+djangoldp_application/migrations/0012_auto_20230512_1556.py
+djangoldp_application/migrations/0013_auto_20230512_1608.py
+djangoldp_application/migrations/0014_auto_20230512_1613.py
 djangoldp_application/migrations/__init__.py
```

### Comparing `djangoldp_application-1.0.9/djangoldp_application/views.py` & `djangoldp_application-1.1.0/djangoldp_application/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from .models import Application, Federation
+from django.conf import settings
+from django.core.mail import send_mail
 from django.http import JsonResponse
+from django.utils.translation import ugettext_lazy as _
+from djangoldp_component.models import Component, Package
 from rest_framework import serializers, viewsets
 from rest_framework_yaml.parsers import YAMLParser
 from rest_framework_yaml.renderers import YAMLRenderer
-from .models import Application, Federation
-from djangoldp_component.models import Component, Package
-from django.conf import settings
 
 
+EMAIL_FROM = (getattr(settings, 'DEFAULT_FROM_EMAIL', False) or getattr(settings, 'EMAIL_HOST_USER', False))
 ANSIBLE_SERVERS = set({"127.0.0.1"})
 
 
 if hasattr(settings, "ANSIBLE_SERVERS"):
     ANSIBLE_SERVERS = ANSIBLE_SERVERS.union(getattr(settings, "ANSIBLE_SERVERS"))
 
 
@@ -126,87 +129,75 @@
                 )
 
         for applicationComponent in application["components"]:
             component = Component.objects.get(id=applicationComponent.obj.component_id)
             insertComponent = {
                 "type": component.name,
                 "route": format(component.preferred_route),
-                "parameters": [],
+                "parameters": {},
                 "extensions": [],
             }
             if component.auto_import:
                 insertComponent["experimental"] = ["routing"]
             keys = []
             for parameter in applicationComponent.obj.parameters.all():
                 if parameter.key == "route":
                     insertComponent["route"] = format(parameter.value)
                 else:
-                    i = {}
-                    i[parameter.key] = format(parameter.value)
-                    insertComponent["parameters"].append(i)
+                    insertComponent["parameters"][parameter.key] = format(parameter.value)
                 keys.append(parameter.key)
             for parameter in component.parameters.all():
                 if not parameter.key in keys:
                     if parameter.key == "route":
                         insertComponent["route"] = format(parameter.default)
                     else:
-                        i = {}
-                        i[parameter.key] = format(parameter.default)
-                        insertComponent["parameters"].append(i)
+                        insertComponent["parameters"][parameter.key] = format(parameter.default)
             for extensionComponent in applicationComponent.obj.extensions.all():
                 extension = Component.objects.get(id=extensionComponent.component_id)
                 componentExtension = {
                     "type": extension.name,
                     "route": format(component.preferred_route),
-                    "parameters": [],
+                    "parameters": {},
                 }
                 if extension.auto_import:
                     componentExtension["experimental"] = ["routing"]
                 keys = []
                 for parameter in extensionComponent.parameters.all():
                     if parameter.key == "route":
                         componentExtension["route"] = format(parameter.value)
                     else:
-                        i = {}
-                        i[parameter.key] = format(parameter.value)
-                        componentExtension["parameters"].append(i)
+                        componentExtension["parameters"][parameter.key] = format(parameter.value)
                     keys.append(parameter.key)
                 for parameter in extension.parameters.all():
                     if not parameter.key in keys:
                         if parameter.key == "route":
                             componentExtension["route"] = format(parameter.default)
                         else:
-                            i = {}
-                            i[parameter.key] = format(parameter.default)
-                            componentExtension["parameters"].append(i)
+                            componentExtension["parameters"][parameter.key] = format(parameter.default)
                 insertComponent["extensions"].append(componentExtension)
             serialized["apps"]["hosts"][application["slug"]]["components"].append(
                 insertComponent
             )
 
         insertDependencies = []
         for applicationPackage in application["packages"]:
             package = Package.objects.get(id=applicationPackage.obj.package_id)
             insertDependency = {
                 "distribution": package.distribution,
                 "module": package.module,
-                "parameters": [],
+                "parameters": {},
             }
             keys = []
             for parameter in applicationPackage.obj.parameters.all():
                 if not parameter.key in keys:
-                    i = {}
-                    i[parameter.key] = format(parameter.value)
-                    insertDependency["parameters"].append(i)
+                    insertDependency["parameters"][parameter.key] = format(parameter.value)
                     keys.append(parameter.key)
             for parameter in package.parameters.all():
                 if not parameter.key in keys:
-                    i = {}
-                    i[parameter.key] = format(parameter.default)
-                    insertDependency["parameters"].append(i)
+                    insertDependency["parameters"][parameter.key] = format(parameter.default)
             insertDependencies.append(insertDependency)
         serialized["apps"]["hosts"][application["slug"]][
             "packages"
         ] = insertDependencies
 
         return serialized
 
@@ -242,27 +233,59 @@
     queryset = Application.objects.all()
     serializer_class = ApplicationDetailSerializer
     lookup_field = "slug"
     parser_classes = (YAMLParser,)
     renderer_classes = (YAMLRenderer,)
 
 
-def mark_as_done(request, slug):
+def mark_as_doing(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
         for deploy in application.deployments.filter(status="Todo"):
+            deploy.status = "Doing"
+            deploy.save()
+        return JsonResponse({"status": "success"}, status=200)
+    else:
+        return JsonResponse({"status": "invalid request"}, status=400)
+
+def mark_as_done(request, slug):
+    if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
+        application = Application.objects.get(slug=slug)
+        for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Done"
             deploy.save()
+            if deploy.requester:
+                message = _("Woah! Deployment done!")
+                send_mail(
+                    _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
+                    message,
+                    EMAIL_FROM,
+                    [deploy.requester.email],
+                    fail_silently=True,
+                    html_message=message
+                )
+
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
 
 
 def mark_as_failed(request, slug):
     if request.method == "GET" and get_client_ip(request) in ANSIBLE_SERVERS:
         application = Application.objects.get(slug=slug)
-        for deploy in application.deployments.filter(status="Todo"):
+        for deploy in application.deployments.filter(status="Doing"):
             deploy.status = "Failed"
             deploy.save()
+            if deploy.requester:
+                message = _("Woah! Deployment failed!")
+                send_mail(
+                    _('Déploiement de ') + application.application_title + " (https://{})".format(application.client_url),
+                    message,
+                    EMAIL_FROM,
+                    [deploy.requester.email],
+                    fail_silently=True,
+                    html_message=message
+                )
+
         return JsonResponse({"status": "success"}, status=200)
     else:
         return JsonResponse({"status": "invalid request"}, status=400)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `djangoldp_application-1.0.9/djangoldp_application/models.py` & `djangoldp_application-1.1.0/djangoldp_application/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-import uuid
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.db.models.signals import pre_save, post_save
 from django.dispatch import receiver
 from django.utils.text import slugify
 from django.utils.translation import ugettext_lazy as _
+from djangoldp_component.models import Component, Package
 from djangoldp.models import Model
 from rest_framework.exceptions import ValidationError
-
-from djangoldp_component.models import Component, Package
+import uuid
 
 
 class Application(Model):
     repository = models.CharField(max_length=255, blank=True, null=True)
     friendly_name = models.CharField(max_length=255, blank=True, null=True)
     short_description = models.CharField(max_length=255, blank=True, null=True)
     creator = models.ForeignKey(
         get_user_model(),
         related_name="applications",
         on_delete=models.SET_NULL,
         null=True,
         blank=True,
     )
-    api_url = models.CharField(max_length=255, blank=True, null=True)
-    client_url = models.CharField(max_length=255, blank=True, null=True)
-    # May move appliation_* to graphics model?
+    api_url = models.CharField(
+        max_length=255, blank=True, null=True, help_text='Without "http(s)://"'
+    )
+    client_url = models.CharField(
+        max_length=255, blank=True, null=True, help_text='Without "http(s)://"'
+    )
+    # May move appliation_* to graphics?
     application_title = models.CharField(max_length=255, blank=True, null=True)
     application_logo = models.CharField(max_length=255, blank=True, null=True)
     slug = models.SlugField(unique=True, blank=True, null=True)
 
     @property
     def deploy(self):
         return self.deployments.filter(status="Todo").count() > 0
@@ -76,28 +79,37 @@
         superuser_perms = ["view"]
         verbose_name = _("application")
         verbose_name_plural = _("applications")
 
 
 STATUS_CHOICES = [
     ("Todo", _("Todo")),
+    ("Doing", _("Doing")),
     ("Done", _("Done")),
     ("Failed", _("Failed")),
 ]
 
 
 class Deployment(Model):
     application = models.ForeignKey(
         Application,
         on_delete=models.CASCADE,
         related_name="deployments",
         null=True,
         blank=True,
     )
-    date = models.DateTimeField(auto_now_add=True)
+    requester = models.ForeignKey(
+        get_user_model(),
+        related_name="deployments",
+        on_delete=models.SET_NULL,
+        null=True,
+        blank=True,
+    )
+    date = models.DateTimeField(auto_now_add=True, verbose_name="Request date")
+    resolutionDate = models.DateTimeField(auto_now=True, verbose_name="Resolution date")
     status = models.CharField(
         max_length=8, choices=STATUS_CHOICES, default="Todo", null=True, blank=True
     )
 
     def __str__(self):
         try:
             return "{} - {} ({})".format(
@@ -107,26 +119,29 @@
             return self.urlid
 
     class Meta(Model.Meta):
         anonymous_perms = ["view"]
         authenticated_perms = ["inherit", "add"]
         container_path = "/deployments/"
         depth = 0
-        ordering = ["application__urlid", "date"]
-        owner_field = "application__creator"
+        auto_author = "requester"
+        owner_field = "requester"
         owner_perms = ["inherit", "change", "delete"]
+        ordering = ["application__urlid", "date"]
         rdf_context = {
             "application": "sib:application",
             "date": "sib:deploymentDate",
+            "resolutionDate": "sib:deploymentDate",
             "status": "sib:deploymentStatus",
         }
         rdf_type = "sib:federation"
         serializer_fields = [
             "@id",
             "date",
+            "resolutionDate",
             "status",
         ]
         superuser_perms = ["view"]
         verbose_name = _("deployment")
         verbose_name_plural = _("deployments")
```

### Comparing `djangoldp_application-1.0.9/djangoldp_application/admin.py` & `djangoldp_application-1.1.0/djangoldp_application/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,18 +141,18 @@
         "base_component__application__friendly_name",
         "base_component__application__short_description",
     ]
     ordering = ["base_component__application__slug", "component__slug"]
 
 
 class DeploymentAdmin(DjangoLDPAdmin):
-    list_display = ("application", "date", "status")
+    list_display = ("application", "requester", "date", "status", "resolutionDate")
     exclude = ("urlid", "slug", "is_backlink", "allow_create_backlink")
-    search_fields = ["urlid", "application__slug", "application__friendly_name"]
-    ordering = ["application__slug", "date"]
+    search_fields = ["urlid", "application__slug", "requester__name", "application__friendly_name"]
+    ordering = ["application__slug", "date", "resolutionDate"]
 
 
 admin.site.register(Application, ApplicationAdmin)
 admin.site.register(Federation, EmptyAdmin)
 admin.site.register(ApplicationGraphics, EmptyAdmin)
 admin.site.register(ApplicationService, EmptyAdmin)
 admin.site.register(ApplicationNPM, EmptyAdmin)
```

### Comparing `djangoldp_application-1.0.9/djangoldp_application/djangoldp_urls.py` & `djangoldp_application-1.1.0/djangoldp_application/djangoldp_urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.urls import path
 from .views import (
     ApplicationViewSet,
     ApplicationDetailViewSet,
+    mark_as_doing,
     mark_as_done,
     mark_as_failed,
 )
 
 urlpatterns = [
     path(
         "ansible/inventory/",
@@ -14,14 +15,19 @@
     ),
     path(
         "ansible/<slug:slug>/",
         ApplicationDetailViewSet.as_view({"get": "retrieve"}, lookup_field="slug"),
         name="ansible_inventory_detail",
     ),
     path(
+        "ansible/<slug:slug>/doing/",
+        mark_as_doing,
+        name="ansible_inventory_mark_doing",
+    ),
+    path(
         "ansible/<slug:slug>/done/",
         mark_as_done,
         name="ansible_inventory_mark_done",
     ),
     path(
         "ansible/<slug:slug>/failed/",
         mark_as_failed,
```

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0009_applicationgraphics.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0009_applicationgraphics.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0001_initial.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0010_auto_20230331_0921.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0010_auto_20230331_0921.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0005_auto_20230331_0850.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0005_auto_20230331_0850.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0008_applicationnpm.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0008_applicationnpm.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0004_auto_20230328_1657.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0004_auto_20230328_1657.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0002_deployment.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0002_deployment.py`

 * *Files identical despite different names*

### Comparing `djangoldp_application-1.0.9/djangoldp_application/migrations/0006_applicationservice.py` & `djangoldp_application-1.1.0/djangoldp_application/migrations/0006_applicationservice.py`

 * *Files identical despite different names*

