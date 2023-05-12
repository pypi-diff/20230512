# Comparing `tmp/bpkio_cli-1.0.1.tar.gz` & `tmp/bpkio_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_cli-1.0.1.tar", max compression
+gzip compressed data, was "bpkio_cli-1.1.0.tar", max compression
```

## Comparing `bpkio_cli-1.0.1.tar` & `bpkio_cli-1.1.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-12 18:00:34.356420 bpkio_cli-1.0.1/bpkio_cli/__init__.py
--rw-r--r--   0        0        0     3338 2023-04-29 21:08:44.550102 bpkio_cli-1.0.1/bpkio_cli/__main__.py
--rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.0.1/bpkio_cli/click_mods/__init__.py
--rw-r--r--   0        0        0     4511 2023-04-29 21:09:43.731932 bpkio_cli-1.0.1/bpkio_cli/click_mods/group_rest_resource.py
--rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.0.1/bpkio_cli/click_mods/option_eat_all.py
--rw-r--r--   0        0        0      564 2023-04-29 21:08:44.551140 bpkio_cli-1.0.1/bpkio_cli/commands/__init__.py
--rw-r--r--   0        0        0     4510 2023-04-30 21:27:53.430919 bpkio_cli-1.0.1/bpkio_cli/commands/configure.py
--rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.0.1/bpkio_cli/commands/consumption.py
--rw-r--r--   0        0        0      762 2023-04-26 12:03:04.836639 bpkio_cli-1.0.1/bpkio_cli/commands/hello.py
--rw-r--r--   0        0        0      983 2023-04-26 12:03:04.836946 bpkio_cli-1.0.1/bpkio_cli/commands/memory.py
--rw-r--r--   0        0        0     3134 2023-04-26 12:03:04.837256 bpkio_cli-1.0.1/bpkio_cli/commands/package.py
--rw-r--r--   0        0        0     6769 2023-05-12 07:40:03.089081 bpkio_cli-1.0.1/bpkio_cli/commands/profiles.py
--rw-r--r--   0        0        0     3186 2023-05-01 07:55:57.224646 bpkio_cli-1.0.1/bpkio_cli/commands/services.py
--rw-r--r--   0        0        0     5419 2023-04-29 21:54:24.509681 bpkio_cli-1.0.1/bpkio_cli/commands/sources.py
--rw-r--r--   0        0        0    16043 2023-05-12 07:37:34.389621 bpkio_cli-1.0.1/bpkio_cli/commands/template_crud.py
--rw-r--r--   0        0        0     7223 2023-05-12 07:39:22.268209 bpkio_cli-1.0.1/bpkio_cli/commands/template_crud_slots.py
--rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.0.1/bpkio_cli/commands/tenants.py
--rw-r--r--   0        0        0     5348 2023-05-12 07:40:30.476002 bpkio_cli-1.0.1/bpkio_cli/commands/url.py
--rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.0.1/bpkio_cli/commands/users.py
--rw-r--r--   0        0        0     1043 2023-04-30 21:10:36.024729 bpkio_cli-1.0.1/bpkio_cli/core/app_settings.py
--rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.0.1/bpkio_cli/core/exceptions.py
--rw-r--r--   0        0        0     2128 2023-04-30 21:09:27.517510 bpkio_cli-1.0.1/bpkio_cli/core/initialize.py
--rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.0.1/bpkio_cli/core/logger.py
--rw-r--r--   0        0        0     8665 2023-05-04 10:16:16.190924 bpkio_cli-1.0.1/bpkio_cli/core/packager.py
--rw-r--r--   0        0        0     5741 2023-04-29 21:14:44.072132 bpkio_cli-1.0.1/bpkio_cli/core/resource_recorder.py
--rw-r--r--   0        0        0     2207 2023-04-26 12:03:04.840592 bpkio_cli-1.0.1/bpkio_cli/core/resources_context.py
--rw-r--r--   0        0        0     4860 2023-05-12 07:34:46.029061 bpkio_cli-1.0.1/bpkio_cli/core/response_handler.py
--rw-r--r--   0        0        0      545 2023-05-12 07:26:04.407684 bpkio_cli-1.0.1/bpkio_cli/options/__init__.py
--rw-r--r--   0        0        0      304 2023-04-27 14:26:01.184020 bpkio_cli-1.0.1/bpkio_cli/options/admin.py
--rw-r--r--   0        0        0      355 2023-04-27 14:26:01.184412 bpkio_cli-1.0.1/bpkio_cli/options/json.py
--rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.0.1/bpkio_cli/options/list.py
--rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.0.1/bpkio_cli/options/poll.py
--rw-r--r--   0        0        0      568 2023-05-02 19:55:34.650018 bpkio_cli-1.0.1/bpkio_cli/options/read.py
--rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.0.1/bpkio_cli/options/search.py
--rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.0.1/bpkio_cli/options/table.py
--rw-r--r--   0        0        0      777 2023-05-04 11:31:15.973002 bpkio_cli-1.0.1/bpkio_cli/options/urls.py
--rw-r--r--   0        0        0      289 2023-05-12 07:26:12.169733 bpkio_cli-1.0.1/bpkio_cli/utils/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.0.1/bpkio_cli/utils/arrays.py
--rw-r--r--   0        0        0     3319 2023-04-29 21:32:02.053678 bpkio_cli-1.0.1/bpkio_cli/utils/config_provider.py
--rw-r--r--   0        0        0     1202 2023-04-28 08:03:11.236380 bpkio_cli-1.0.1/bpkio_cli/utils/datetimes.py
--rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.0.1/bpkio_cli/utils/json.py
--rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.0.1/bpkio_cli/utils/profile_maker.py
--rw-r--r--   0        0        0     4658 2023-05-04 20:28:53.083959 bpkio_cli-1.0.1/bpkio_cli/utils/url_builders.py
--rw-r--r--   0        0        0      583 2023-04-09 19:02:06.960542 bpkio_cli-1.0.1/bpkio_cli/utils/urls.py
--rw-r--r--   0        0        0      611 2023-04-21 22:26:37.261644 bpkio_cli-1.0.1/bpkio_cli/writers/breadcrumbs.py
--rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.0.1/bpkio_cli/writers/colorizer.py
--rw-r--r--   0        0        0     4128 2023-05-02 20:54:33.828754 bpkio_cli-1.0.1/bpkio_cli/writers/content_display.py
--rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.0.1/bpkio_cli/writers/diff.py
--rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.0.1/bpkio_cli/writers/formatter.py
--rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.0.1/bpkio_cli/writers/hls_formatter.py
--rw-r--r--   0        0        0     1583 2023-04-29 21:08:44.553756 bpkio_cli-1.0.1/bpkio_cli/writers/players.py
--rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.0.1/bpkio_cli/writers/tables.py
--rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.0.1/bpkio_cli/writers/xml_formatter.py
--rw-r--r--   0        0        0     1188 2023-05-12 18:05:34.104089 bpkio_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 bpkio_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-28 20:04:37.409875 bpkio_cli-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-12 21:49:06.044277 bpkio_cli-1.1.0/bpkio_cli/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-29 21:08:44.550102 bpkio_cli-1.1.0/bpkio_cli/__main__.py
+-rw-r--r--   0        0        0       91 2023-04-29 21:05:12.410693 bpkio_cli-1.1.0/bpkio_cli/click_mods/__init__.py
+-rw-r--r--   0        0        0     4511 2023-04-29 21:09:43.731932 bpkio_cli-1.1.0/bpkio_cli/click_mods/group_rest_resource.py
+-rw-r--r--   0        0        0     1747 2023-03-23 13:12:03.515867 bpkio_cli-1.1.0/bpkio_cli/click_mods/option_eat_all.py
+-rw-r--r--   0        0        0      564 2023-04-29 21:08:44.551140 bpkio_cli-1.1.0/bpkio_cli/commands/__init__.py
+-rw-r--r--   0        0        0     4634 2023-05-12 21:43:26.529478 bpkio_cli-1.1.0/bpkio_cli/commands/configure.py
+-rw-r--r--   0        0        0     1758 2023-04-28 08:13:42.029805 bpkio_cli-1.1.0/bpkio_cli/commands/consumption.py
+-rw-r--r--   0        0        0      762 2023-04-26 12:03:04.836639 bpkio_cli-1.1.0/bpkio_cli/commands/hello.py
+-rw-r--r--   0        0        0      983 2023-04-26 12:03:04.836946 bpkio_cli-1.1.0/bpkio_cli/commands/memory.py
+-rw-r--r--   0        0        0     3134 2023-04-26 12:03:04.837256 bpkio_cli-1.1.0/bpkio_cli/commands/package.py
+-rw-r--r--   0        0        0     6852 2023-05-12 19:43:30.439010 bpkio_cli-1.1.0/bpkio_cli/commands/profiles.py
+-rw-r--r--   0        0        0     3401 2023-05-12 20:34:15.984115 bpkio_cli-1.1.0/bpkio_cli/commands/services.py
+-rw-r--r--   0        0        0     3740 2023-05-12 21:34:14.672836 bpkio_cli-1.1.0/bpkio_cli/commands/services_create.py
+-rw-r--r--   0        0        0     5419 2023-04-29 21:54:24.509681 bpkio_cli-1.1.0/bpkio_cli/commands/sources.py
+-rw-r--r--   0        0        0    16787 2023-05-12 19:58:32.261329 bpkio_cli-1.1.0/bpkio_cli/commands/template_crud.py
+-rw-r--r--   0        0        0     7223 2023-05-12 07:39:22.268209 bpkio_cli-1.1.0/bpkio_cli/commands/template_crud_slots.py
+-rw-r--r--   0        0        0      332 2023-04-28 08:33:05.100937 bpkio_cli-1.1.0/bpkio_cli/commands/tenants.py
+-rw-r--r--   0        0        0     5348 2023-05-12 07:40:30.476002 bpkio_cli-1.1.0/bpkio_cli/commands/url.py
+-rw-r--r--   0        0        0      359 2023-04-28 08:33:22.939414 bpkio_cli-1.1.0/bpkio_cli/commands/users.py
+-rw-r--r--   0        0        0     1043 2023-04-30 21:10:36.024729 bpkio_cli-1.1.0/bpkio_cli/core/app_settings.py
+-rw-r--r--   0        0        0      135 2023-04-20 16:43:38.934392 bpkio_cli-1.1.0/bpkio_cli/core/exceptions.py
+-rw-r--r--   0        0        0     2128 2023-04-30 21:09:27.517510 bpkio_cli-1.1.0/bpkio_cli/core/initialize.py
+-rw-r--r--   0        0        0     1718 2023-04-07 16:07:08.180945 bpkio_cli-1.1.0/bpkio_cli/core/logger.py
+-rw-r--r--   0        0        0     8665 2023-05-04 10:16:16.190924 bpkio_cli-1.1.0/bpkio_cli/core/packager.py
+-rw-r--r--   0        0        0     5741 2023-04-29 21:14:44.072132 bpkio_cli-1.1.0/bpkio_cli/core/resource_recorder.py
+-rw-r--r--   0        0        0     2207 2023-04-26 12:03:04.840592 bpkio_cli-1.1.0/bpkio_cli/core/resources_context.py
+-rw-r--r--   0        0        0     5142 2023-05-12 18:56:36.153732 bpkio_cli-1.1.0/bpkio_cli/core/response_handler.py
+-rw-r--r--   0        0        0      545 2023-05-12 07:26:04.407684 bpkio_cli-1.1.0/bpkio_cli/options/__init__.py
+-rw-r--r--   0        0        0      304 2023-04-27 14:26:01.184020 bpkio_cli-1.1.0/bpkio_cli/options/admin.py
+-rw-r--r--   0        0        0      355 2023-05-12 19:07:07.722647 bpkio_cli-1.1.0/bpkio_cli/options/json.py
+-rw-r--r--   0        0        0      958 2023-05-12 07:26:58.744571 bpkio_cli-1.1.0/bpkio_cli/options/list.py
+-rw-r--r--   0        0        0      933 2023-04-27 14:26:01.185185 bpkio_cli-1.1.0/bpkio_cli/options/poll.py
+-rw-r--r--   0        0        0      568 2023-05-02 19:55:34.650018 bpkio_cli-1.1.0/bpkio_cli/options/read.py
+-rw-r--r--   0        0        0     1183 2023-04-27 14:26:01.185667 bpkio_cli-1.1.0/bpkio_cli/options/search.py
+-rw-r--r--   0        0        0      445 2023-05-04 18:13:29.662132 bpkio_cli-1.1.0/bpkio_cli/options/table.py
+-rw-r--r--   0        0        0      777 2023-05-04 11:31:15.973002 bpkio_cli-1.1.0/bpkio_cli/options/urls.py
+-rw-r--r--   0        0        0      289 2023-05-12 07:26:12.169733 bpkio_cli-1.1.0/bpkio_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-12 07:34:26.643986 bpkio_cli-1.1.0/bpkio_cli/utils/arrays.py
+-rw-r--r--   0        0        0     3398 2023-05-12 19:50:24.682253 bpkio_cli-1.1.0/bpkio_cli/utils/config_provider.py
+-rw-r--r--   0        0        0     1202 2023-04-28 08:03:11.236380 bpkio_cli-1.1.0/bpkio_cli/utils/datetimes.py
+-rw-r--r--   0        0        0      136 2023-04-14 20:15:18.159888 bpkio_cli-1.1.0/bpkio_cli/utils/json.py
+-rw-r--r--   0        0        0      567 2023-04-29 21:58:38.435162 bpkio_cli-1.1.0/bpkio_cli/utils/profile_maker.py
+-rw-r--r--   0        0        0     4658 2023-05-12 19:12:42.208834 bpkio_cli-1.1.0/bpkio_cli/utils/url_builders.py
+-rw-r--r--   0        0        0      583 2023-04-09 19:02:06.960542 bpkio_cli-1.1.0/bpkio_cli/utils/urls.py
+-rw-r--r--   0        0        0      611 2023-04-21 22:26:37.261644 bpkio_cli-1.1.0/bpkio_cli/writers/breadcrumbs.py
+-rw-r--r--   0        0        0     1404 2023-05-02 20:19:18.033992 bpkio_cli-1.1.0/bpkio_cli/writers/colorizer.py
+-rw-r--r--   0        0        0     4128 2023-05-02 20:54:33.828754 bpkio_cli-1.1.0/bpkio_cli/writers/content_display.py
+-rw-r--r--   0        0        0      840 2023-04-26 12:03:04.848088 bpkio_cli-1.1.0/bpkio_cli/writers/diff.py
+-rw-r--r--   0        0        0      152 2023-04-26 12:03:04.848777 bpkio_cli-1.1.0/bpkio_cli/writers/formatter.py
+-rw-r--r--   0        0        0     4533 2023-05-09 10:21:54.315733 bpkio_cli-1.1.0/bpkio_cli/writers/hls_formatter.py
+-rw-r--r--   0        0        0      715 2023-05-12 19:01:29.004428 bpkio_cli-1.1.0/bpkio_cli/writers/json_formatter.py
+-rw-r--r--   0        0        0     1583 2023-04-29 21:08:44.553756 bpkio_cli-1.1.0/bpkio_cli/writers/players.py
+-rw-r--r--   0        0        0     1865 2023-05-12 07:26:12.170387 bpkio_cli-1.1.0/bpkio_cli/writers/tables.py
+-rw-r--r--   0        0        0     5205 2023-04-26 12:03:04.849885 bpkio_cli-1.1.0/bpkio_cli/writers/xml_formatter.py
+-rw-r--r--   0        0        0     1209 2023-05-12 21:55:00.912742 bpkio_cli-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 bpkio_cli-1.1.0/PKG-INFO
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/__main__.py` & `bpkio_cli-1.1.0/bpkio_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/click_mods/group_rest_resource.py` & `bpkio_cli-1.1.0/bpkio_cli/click_mods/group_rest_resource.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/click_mods/option_eat_all.py` & `bpkio_cli-1.1.0/bpkio_cli/click_mods/option_eat_all.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/__init__.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/configure.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 @tenants.command(help="Switch the tenant used for subsequent invocations")
 @click.argument("tenant", required=False)
 @click.pass_context
 def switch(ctx, tenant):
     if not tenant:
         cp = TenantProfileProvider()
         tenant_list = cp.list_tenants()
-        choices = [dict(value=t.label, name=f"{t.label} ({t.id})") for t in tenant_list]
+        tenant_list = sorted(tenant_list, key=lambda t: t.label)
+        choices = [dict(value=t.label, name=f"{t.label} ({t.id})  -  {t.fqdn}") for t in tenant_list]
 
         tenant = inquirer.fuzzy(message="Select a tenant", choices=choices).execute()
 
     # Write it to the .tenant file
     with open(".tenant", "w") as f:
         f.write(tenant)
 
@@ -148,8 +149,8 @@
         )
 
 
 # Command: EDIT
 @tenants.command(help="Edit the tenant credential file manually")
 def edit():
     cp = TenantProfileProvider()
-    click.launch(str(cp.inifile))
+    click.edit(filename=str(cp.inifile), editor=ConfigProvider().get("editor"))
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/consumption.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/hello.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/hello.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/memory.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/memory.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/package.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/package.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/profiles.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from bpkio_api.models import TranscodingProfile, TranscodingProfileIn
 from InquirerPy import inquirer
 
 import bpkio_cli.options as bic_options
 from bpkio_cli.click_mods import ApiResourceGroup
 from bpkio_cli.core.app_settings import AppContext
 from bpkio_cli.utils.arrays import order_by_dict_keys
+from bpkio_cli.utils.config_provider import ConfigProvider
 from bpkio_cli.utils.json import is_json
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.tables import display_table
 
 default_fields = ["id", "name", "num_layers"]
 
 
@@ -210,15 +211,15 @@
 @click.pass_obj
 def update(obj: AppContext, tenant: int):
     id = obj.resources.last()
     profile = obj.api.transcoding_profiles.retrieve(id, tenantId=tenant)
     profile.tenantId = tenant
     payload = j.dumps(j.loads(profile.json()), indent=2)
 
-    updated_resource_json = click.edit(payload, editor="nano")
+    updated_resource_json = click.edit(payload, editor=ConfigProvider().get("editor"))
 
     obj.api.transcoding_profiles.update(id, j.loads(updated_resource_json))
 
     click.secho(f"Resource {id} updated", fg="green")
 
 
 # --- DELETE Command
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/services.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/services.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import click
 import cloup
 from bpkio_api.models import (
     AdInsertionService,
     ContentReplacementService,
     ContentReplacementSlot,
     ServiceSparse,
     VirtualChannelService,
     VirtualChannelSlot,
 )
+from bpkio_cli.commands.services_create import create_ad_insertion_service_command
 
 from bpkio_cli.commands.template_crud import create_resource_group
 from bpkio_cli.commands.template_crud_slots import create_child_resource_group
+from bpkio_cli.core.app_settings import AppContext
 
 default_fields = ["id", "name", "type", "serviceId", "format"]
 
 
 def add_services_section(cli):
     root_endpoint = "services"
     root: cloup.Group = create_resource_group(
@@ -54,14 +57,15 @@
         create_resource_group(
             "ad-insertion",
             resource_class=AdInsertionService,
             endpoint_path=[root_endpoint, "ad_insertion"],
             aliases=["dai", "ssai"],
             default_fields=["id", "name", "type", "sub_type", "serviceId", "format"],
             with_content_commands=["all"],
+            extra_commands=[create_ad_insertion_service_command()]
         ),
         create_resource_group(
             "virtual-channel",
             resource_class=VirtualChannelService,
             endpoint_path=[root_endpoint, "virtual_channel"],
             aliases=["vc"],
             default_fields=default_fields,
@@ -90,7 +94,8 @@
     return create_child_resource_group(
         "slot",
         resource_class=resource_class,
         endpoint_path=parent_path + ["slots"],
         aliases=["slots"],
         default_fields=default_fields,
     )
+
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/sources.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/template_crud.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/template_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import json as j
 import re
 from typing import List
 from urllib.parse import quote_plus
 
 import click
 import cloup
 from bpkio_api.models import ServiceIn, SourceIn
 
 import bpkio_cli.options as bic_options
 from bpkio_cli.click_mods.group_rest_resource import ApiResourceGroup
 from bpkio_cli.commands.package import package_resources
 from bpkio_cli.core.app_settings import AppContext
 from bpkio_cli.core.exceptions import BroadpeakIoCliError
 from bpkio_cli.core.resources_context import ResourcesContext, UnknownResourceError
+from bpkio_cli.utils.config_provider import ConfigProvider
 from bpkio_cli.utils.profile_maker import make_transcoding_profile
 from bpkio_cli.utils.url_builders import get_service_handler, get_source_handler
 from bpkio_cli.writers.breadcrumbs import display_resource_info
 from bpkio_cli.writers.content_display import display_content
 from bpkio_cli.writers.players import StreamPlayer
 from bpkio_cli.writers.tables import display_table
 
@@ -206,15 +208,34 @@
         resource = retrieve_resource()
 
         endpoint = get_api_endpoint()
         endpoint.delete(resource.id)
 
         click.secho(f"Resource {resource.id} deleted", fg="green")
 
-    sections.append(cloup.Section("CRUD commands", [list, get, json, search, delete]))
+    # --- UPDATE Command
+    @cloup.command(aliases=["put"], help=f"Update a {resource_title}")
+    @click.pass_context
+    def update(ctx):
+        resource = retrieve_resource()
+        payload = j.dumps(j.loads(resource.json()), indent=2)
+
+        updated_resource_json = click.edit(
+            payload, editor=ConfigProvider().get("editor")
+        )
+
+        endpoint = get_api_endpoint()
+        # TODO - try to parse into the resource class (otherwise can only work with specific resource sub-types)
+        endpoint.update(resource.id, j.loads(updated_resource_json))
+
+        click.secho(f"Resource {resource.id} updated", fg="green")
+
+    sections.append(
+        cloup.Section("CRUD commands", [list, get, json, search, delete, update])
+    )
 
     # === CONTENT Commands ===
 
     content_section = cloup.Section("Content commands", [])
 
     if any(x in with_content_commands for x in ["all", "url"]):
         # --- URL Command
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/template_crud_slots.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/template_crud_slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/commands/url.py` & `bpkio_cli-1.1.0/bpkio_cli/commands/url.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/app_settings.py` & `bpkio_cli-1.1.0/bpkio_cli/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/initialize.py` & `bpkio_cli-1.1.0/bpkio_cli/core/initialize.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/logger.py` & `bpkio_cli-1.1.0/bpkio_cli/core/logger.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/packager.py` & `bpkio_cli-1.1.0/bpkio_cli/core/packager.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/resource_recorder.py` & `bpkio_cli-1.1.0/bpkio_cli/core/resource_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/resources_context.py` & `bpkio_cli-1.1.0/bpkio_cli/core/resources_context.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/core/response_handler.py` & `bpkio_cli-1.1.0/bpkio_cli/core/response_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import click
 import tabulate
 from bpkio_api.models import BaseResource
 from pydantic import BaseModel
 
 from bpkio_cli.core.resource_recorder import ResourceRecorder
 from bpkio_cli.utils.arrays import pluck_and_cast_properties, sort_objects
+from bpkio_cli.writers.json_formatter import JSONFormatter
 from bpkio_cli.writers.tables import display_table
 
 tabulate.PRESERVE_WHITESPACE = True
 
 
 class ResponseHandler:
     def __init__(self, cache: Optional[ResourceRecorder] = None) -> None:
@@ -57,15 +58,16 @@
         if self.cache:
             self.cache.record(resources)
 
         if json:
             if isinstance(resources[0], BaseModel):
                 resources = [j.loads(r.json(exclude_none=True)) for r in resources]
 
-            print(j.dumps(resources, indent=2))
+            colored_json = JSONFormatter().format(resources)
+            click.echo(colored_json)
             return
 
         # Extract the select_fields
         if select_fields:
             select_fields = " ".join(select_fields)  # type: ignore
             select_fields = re.findall(r"\w[\w\.]*", select_fields)  # type: ignore
 
@@ -80,19 +82,24 @@
         json: Optional[bool] = False,
     ):
         # Record the resource
         if self.cache and hasattr(resource, "id"):
             self.cache.record(resource)
 
         if json and isinstance(resource, BaseModel):
-            print(j.dumps(j.loads(resource.json(exclude_none=False)), indent=2))
+            data = j.loads(resource.json(exclude_none=False))
+            colored_json = JSONFormatter().format(data)
+            click.echo(colored_json)
+
             return resource
 
         elif not isinstance(resource, BaseResource):
-            print(j.dumps(resource, indent=2))
+            data = j.dumps(resource, indent=2)
+            colored_json = JSONFormatter().format(data)
+            click.echo(colored_json)
 
         else:
             rows = []
 
             # Identifier
             header = "{} {}".format(
                 click.style(resource.__class__.__name__, fg="white", dim=True),
@@ -134,9 +141,9 @@
                     lines.append(" ".join(elements))
                 rows.append("\n".join(lines))
 
             display_table(rows)
 
     @staticmethod
     def treat_simple_list(data: list):
-        print(tabulate.tabulate(data, headers="keys"))
+        click.echo(tabulate.tabulate(data, headers="keys"))
         return
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/__init__.py` & `bpkio_cli-1.1.0/bpkio_cli/options/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/list.py` & `bpkio_cli-1.1.0/bpkio_cli/options/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/poll.py` & `bpkio_cli-1.1.0/bpkio_cli/options/poll.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/read.py` & `bpkio_cli-1.1.0/bpkio_cli/options/read.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/search.py` & `bpkio_cli-1.1.0/bpkio_cli/options/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/options/urls.py` & `bpkio_cli-1.1.0/bpkio_cli/options/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/arrays.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/config_provider.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/config_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
     def __init__(self, config_path="~/.bpkio/cli.cfg"):
         self.config_path = os.path.expanduser(config_path)
         self.config = configparser.ConfigParser()
         self.initialize()
 
     def initialize(self):
         default_values = {
-            "settings": {"player": "browser"},
+            "settings": {"player": "browser", "editor": "vim"},
+            "pygments": {"style": "monokai", "linenos": "0"},
             "players": {
                 "browser": "{url}",
                 "demo": "https://theoplayer.ridgeline.fr/?url1={url}&title1={name}&autoplay=true",
                 "hls": "https://hlsjs.video-dev.org/demo/?src={url}",
                 "dash": "https://reference.dashif.org/dash.js/nightly/samples/dash-if-reference-player/index.html?mpd={url}",
             },
         }
```

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/datetimes.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/datetimes.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/profile_maker.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/profile_maker.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/url_builders.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/url_builders.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/utils/urls.py` & `bpkio_cli-1.1.0/bpkio_cli/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/breadcrumbs.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/colorizer.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/colorizer.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/content_display.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/content_display.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/diff.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/diff.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/hls_formatter.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/hls_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/players.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/players.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/tables.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/tables.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/bpkio_cli/writers/xml_formatter.py` & `bpkio_cli-1.1.0/bpkio_cli/writers/xml_formatter.py`

 * *Files identical despite different names*

### Comparing `bpkio_cli-1.0.1/pyproject.toml` & `bpkio_cli-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "bpkio-cli"
-version = "1.0.1"
+version = "1.1.0"
 description = "A command line interface to the broadpeak.io APIs, with additional helpers"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_cli" }]
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 vcs = "git"
 style = "semver"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py", "*/__version__.py", "*/_version.py"]
 
 [tool.poetry.dependencies]
 # bpkio-python-sdk = { path = "../bpkio-python-sdk", develop = true }
-bpkio-python-sdk = "1.0.0"
+bpkio-python-sdk = "^1.0.1"
 python = "^3.10"
 click = "^8.1.3"
 colorama = "^0.4.6"
 # inquirerpy = { git = "https://github.com/kazhala/InquirerPy" }
 inquirerpy = "^0.3.4"
 tabulate = "^0.9.0"
 arrow = "^1.2.3"
 dateparser = "^1.1.8"
 setuptools = "^67.6.1"
 cloup = "^2.0.0.post1"
 diskcache = "^5.4.0"
+pygments = "^2.15.1"
 
 [tool.poetry.scripts]
 bic = "bpkio_cli.__main__:safe_entry_point"
 bic-debug = "bpkio_cli.__main__:debug_entry_point"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
```

### Comparing `bpkio_cli-1.0.1/PKG-INFO` & `bpkio_cli-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bpkio-cli
-Version: 1.0.1
+Version: 1.1.0
 Summary: A command line interface to the broadpeak.io APIs, with additional helpers
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: bpkio-python-sdk (==1.0.0)
+Requires-Dist: bpkio-python-sdk (>=1.0.1,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
 Requires-Dist: diskcache (>=5.4.0,<6.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
+Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: setuptools (>=67.6.1,<68.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

