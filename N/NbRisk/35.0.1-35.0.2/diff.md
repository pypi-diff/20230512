# Comparing `tmp/NbRisk-35.0.1.tar.gz` & `tmp/NbRisk-35.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-35.0.1.tar", last modified: Thu May 11 23:04:26 2023, max compression
+gzip compressed data, was "NbRisk-35.0.2.tar", last modified: Fri May 12 20:04:09 2023, max compression
```

## Comparing `NbRisk-35.0.1.tar` & `NbRisk-35.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:26.039620 NbRisk-35.0.1/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.0.1/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.0.1/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.943619 NbRisk-35.0.1/NbRisk.egg-info/
--rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-11 23:04:25.000000 NbRisk-35.0.1/NbRisk.egg-info/top_level.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-11 23:04:26.035620 NbRisk-35.0.1/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2698 2023-05-11 21:21:40.000000 NbRisk-35.0.1/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.967619 NbRisk-35.0.1/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.0.1/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.0.1/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.975619 NbRisk-35.0.1/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.0.1/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-10 14:35:17.000000 NbRisk-35.0.1/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.0.1/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.0.1/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.0.1/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.0.1/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.0.1/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.0.1/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-10 14:35:17.000000 NbRisk-35.0.1/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.983619 NbRisk-35.0.1/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.0.1/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.0.1/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.0.1/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.0.1/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8511 2023-05-10 12:47:27.000000 NbRisk-35.0.1/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.0.1/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.1/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3428 2023-05-10 13:24:07.000000 NbRisk-35.0.1/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-35.0.1/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:25.931619 NbRisk-35.0.1/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-11 23:04:26.015620 NbRisk-35.0.1/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-11 22:46:19.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-11 22:46:32.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-11 22:46:26.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-11 22:33:43.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-11 22:34:00.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-11 21:46:58.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-11 21:46:54.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_search.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     4982 2023-05-11 23:00:59.000000 NbRisk-35.0.1/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-11 22:48:14.000000 NbRisk-35.0.1/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    10228 2023-05-11 22:45:54.000000 NbRisk-35.0.1/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-11 23:04:26.039620 NbRisk-35.0.1/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.0.1/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.170702 NbRisk-35.0.2/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.0.2/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.0.2/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.126701 NbRisk-35.0.2/NbRisk.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-12 20:04:09.000000 NbRisk-35.0.2/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1526 2023-05-12 20:04:09.000000 NbRisk-35.0.2/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-05-12 20:04:09.000000 NbRisk-35.0.2/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2023-05-12 20:04:09.000000 NbRisk-35.0.2/NbRisk.egg-info/top_level.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3127 2023-05-12 20:04:09.170702 NbRisk-35.0.2/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2698 2023-05-12 19:59:37.000000 NbRisk-35.0.2/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.150702 NbRisk-35.0.2/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      662 2023-04-02 19:37:23.000000 NbRisk-35.0.2/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.0.2/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.150702 NbRisk-35.0.2/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.2/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.0.2/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.0.2/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.0.2/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.0.2/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.0.2/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.0.2/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1633 2023-04-21 01:17:07.000000 NbRisk-35.0.2/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4997 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.2/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.154702 NbRisk-35.0.2/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.0.2/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.0.2/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.0.2/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.0.2/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.0.2/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8497 2023-05-12 20:00:26.000000 NbRisk-35.0.2/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.0.2/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.0.2/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2023-05-12 20:01:49.000000 NbRisk-35.0.2/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      770 2023-04-02 19:37:24.000000 NbRisk-35.0.2/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.110701 NbRisk-35.0.2/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-05-12 20:04:09.170702 NbRisk-35.0.2/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability_search.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4982 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2023-05-12 20:02:05.000000 NbRisk-35.0.2/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10228 2023-05-12 19:59:37.000000 NbRisk-35.0.2/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2023-05-12 20:04:09.174702 NbRisk-35.0.2/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.0.2/setup.py
```

### Comparing `NbRisk-35.0.1/LICENSE` & `NbRisk-35.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/NbRisk.egg-info/PKG-INFO` & `NbRisk-35.0.2/NbRisk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.0.1
+Version: 35.0.2
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.0.1/NbRisk.egg-info/SOURCES.txt` & `NbRisk-35.0.2/NbRisk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/PKG-INFO` & `NbRisk-35.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.0.1
+Version: 35.0.2
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.0.1/README.md` & `NbRisk-35.0.2/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/__init__.py` & `NbRisk-35.0.2/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/api/nested_serializers.py` & `NbRisk-35.0.2/nb_risk/api/nested_serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/api/serializers.py` & `NbRisk-35.0.2/nb_risk/api/serializers.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/api/views.py` & `NbRisk-35.0.2/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/choices.py` & `NbRisk-35.0.2/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/columns.py` & `NbRisk-35.0.2/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/cve.py` & `NbRisk-35.0.2/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/filters.py` & `NbRisk-35.0.2/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/forms.py` & `NbRisk-35.0.2/nb_risk/forms.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/migrations/0001_initial.py` & `NbRisk-35.0.2/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `NbRisk-35.0.2/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/migrations/0003_control.py` & `NbRisk-35.0.2/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/models.py` & `NbRisk-35.0.2/nb_risk/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
         "Integrity Impact (I)", max_length=100, blank=True
     )
     cvssavailabilityImpact = models.CharField(
         "Availability Impact (A)", max_length=100, blank=True
     )
     cvssbaseScore = models.FloatField("Base Score", max_length=100, blank=True)
 
-    @property
     def affected_assets(self):
         return self.vulnerability_assignments.count()
 
     def __str__(self):
         return self.name
 
     def get_absolute_url(self):
```

### Comparing `NbRisk-35.0.1/nb_risk/navigation.py` & `NbRisk-35.0.2/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/tables.py` & `NbRisk-35.0.2/nb_risk/tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import django_tables2 as tables
+from django_tables2.utils import Accessor
 
-from netbox.tables import NetBoxTable, ChoiceFieldColumn, columns
+from netbox.tables import NetBoxTable, columns
+from django.db.models import Count
 
 from . import models
 from . import columns as riskColumns
 
 # ThreatSource Tables
 
 
@@ -31,19 +33,33 @@
 
 # Vulnerability Tables
 
 
 class VulnerabilityTable(NetBoxTable):
 
     name = tables.Column(linkify=True)
-    affected_assets = tables.Column(verbose_name="Affected Assets")
+    affected = columns.LinkedCountColumn(
+        verbose_name="Affected Assets",
+        accessor=Accessor("affected_assets"),
+        viewname='plugins:nb_risk:vulnerabilityassignment_list',
+        url_params={
+            'vulnerability': 'name',
+        },
+    )
+
+    def order_affected(self, queryset, is_descending):
+        if is_descending:
+            queryset = queryset.annotate(affected_assets=Count('vulnerability_assignments')).order_by('-affected_assets')
+        else:
+            queryset = queryset.annotate(affected_assets=Count('vulnerability_assignments')).order_by('affected_assets')
+        return (queryset, True)
 
     class Meta(NetBoxTable.Meta):
         model = models.Vulnerability
-        fields = ["name", "cve", "description", "affected_assets", "cvssbaseScore"]
+        fields = ["name", "cve", "description", "affected", "cvssbaseScore"]
 
 
 # VulnerabilityAssignment Tables
 
 
 class VulnerabilityAssignmentTable(NetBoxTable):
```

### Comparing `NbRisk-35.0.1/nb_risk/template_content.py` & `NbRisk-35.0.2/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/control.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/control.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/risk.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/threatevent.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/threatsource.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/templates/nb_risk/vulnerability_search.html` & `NbRisk-35.0.2/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/urls.py` & `NbRisk-35.0.2/nb_risk/urls.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/nb_risk/views.py` & `NbRisk-35.0.2/nb_risk/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.0.1/setup.py` & `NbRisk-35.0.2/setup.py`

 * *Files identical despite different names*

